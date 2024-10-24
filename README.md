<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Themed Social Links Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Header Section with Google Search -->
  <header>
    <div class="logo">
      <h1>My Website</h1>
    </div>
    <div class="search-bar">
      <form action="https://www.google.com/search" method="get" target="_blank">
        <input type="text" name="q" placeholder="Search Google...">
        <button type="submit">Search</button>
      </form>
    </div>
  </header>

  <!-- Social Media Links -->
  <section class="social-links">
    <h2>Follow Us on Social Media</h2>
    <div class="links">
      <a href="https://www.facebook.com" target="_blank">Facebook</a>
      <a href="https://www.youtube.com" target="_blank">YouTube</a>
      <a href="https://www.tiktok.com" target="_blank">TikTok</a>
      <a href="https://www.twitter.com" target="_blank">Twitter</a>
    </div>
  </section>

  <!-- Footer Section -->
  <footer>
    <p>&copy; 2024 My Website. All rights reserved.</p>
  </footer>
</body>
</html>



/* General Styling */
body {
  margin: 0;
  font-family: 'Arial', sans-serif;
  background-color: #121212; /* Dark background */
  color: #ffffff; /* White text */
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: #1f1f1f;
  border-bottom: 2px solid #000; /* Black border */
}

header .logo {
  font-size: 24px;
  font-weight: bold;
}

header .search-bar form {
  display: flex;
  align-items: center;
}

header .search-bar input {
  padding: 8px;
  border-radius: 4px;
  border: none;
  outline: none;
  width: 200px;
}

header .search-bar button {
  padding: 8px 12px;
  margin-left: 8px;
  background-color: #4caf50;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

header .search-bar button:hover {
  background-color: #45a049;
}

.social-links {
  text-align: center;
  margin: 50px 0;
}

.social-links h2 {
  font-size: 28px;
}

.social-links .links a {
  margin: 15px;
  padding: 12px 25px;
  border: 2px solid #000; /* Black border for logo style */
  border-radius: 8px;
  background-color: #282828;
  color: #ffffff;
  text-decoration: none;
  font-size: 18px;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.social-links .links a:hover {
  background-color: #4caf50; /* Green highlight on hover */
  color: white;
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #1f1f1f;
  border-top: 2px solid #000; /* Black border */
}

