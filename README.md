 const express = require("express");
const mongoose = require("mongoose");
const jwt = require("jsonwebtoken");
const app = express();
const PORT = 3000;

app.use(express.json());

mongoose.connect("mongodb://localhost:27017/messaging-app", { useNewUrlParser: true, useUnifiedTopology: true });

// User schema
const userSchema = new mongoose.Schema({
    phone: { type: String, unique: true },
    password: String
});

const User = mongoose.model("User", userSchema);

// Register endpoint
app.post("/register", async (req, res) => {
    const { phone, password } = req.body;
    try {
        const user = new User({ phone, password });
        await user.save();
        res.status(201).send("User registered");
    } catch (error) {
        res.status(400).send("User already exists");
    }
});

// Login endpoint
app.post("/login", async (req, res) => {
    const { phone, password } = req.body;
    const user = await User.findOne({ phone, password });
    if (user) {
        const token = jwt.sign({ phone }, "SECRET_KEY");
        res.json({ token });
    } else {
        res.status(400).send("Invalid credentials");
    }
});

app.listen(PORT, () => {
    console.log(`Server running on http://localhost:${PORT}`);
});
