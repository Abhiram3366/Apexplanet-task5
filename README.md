# Apexplanet-task5
web development
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Final Project - ApexPlanet</title>
  <link rel="stylesheet" href="task5.css">
</head>
<body>
  <!-- Header -->
  <header>
    <nav class="navbar">
      <h1 class="logo">ApexPlanet</h1>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <h2>Welcome to Final Project & Optimization</h2>
    <p>Build. Optimize. Deploy with performance and responsiveness.</p>
    <button onclick="showAlert()">Get Started</button>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Project</h2>
    <p>
      This project demonstrates how to integrate HTML, CSS, and JavaScript 
      to build a responsive, optimized, and cross-browser compatible web app.
    </p>
  </section>

  <!-- Services Section -->
  <section id="services" class="services">
    <h2>Our Features</h2>
    <div class="cards">
      <div class="card">
        <img src="https://via.placeholder.com/300" alt="Web App" loading="lazy">
        <h3>Full Web Application</h3>
        <p>Capstone project with integrated features and dynamic UI.</p>
      </div>
      <div class="card">
        <img src="https://via.placeholder.com/300" alt="Optimization" loading="lazy">
        <h3>Performance Optimization</h3>
        <p>Fast load times, lazy loading, and minimized assets.</p>
      </div>
      <div class="card">
        <img src="https://via.placeholder.com/300" alt="Responsive" loading="lazy">
        <h3>Cross-Browser & Mobile</h3>
        <p>Works smoothly on Chrome, Firefox, Safari, and mobile browsers.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 ApexPlanet Software Pvt Ltd | All Rights Reserved</p>
  </footer>

  <script src="task5.js"></script>
</body>
</html>



/* General Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Segoe UI", sans-serif;
  line-height: 1.6;
  color: #333;
  background: #f9f9f9;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 40px;
  background: #2b6777;
  color: #fff;
}

.navbar .logo {
  font-size: 22px;
  font-weight: bold;
}

.navbar .nav-links {
  list-style: none;
  display: flex;
}

.navbar .nav-links li {
  margin: 0 10px;
}

.navbar .nav-links a {
  text-decoration: none;
  color: #fff;
  transition: 0.3s;
}

.navbar .nav-links a:hover {
  color: #ffcc00;
}

/* Hero Section */
.hero {
  text-align: center;
  padding: 80px 20px;
  background: #52ab98;
  color: white;
}

.hero button {
  margin-top: 20px;
  padding: 10px 20px;
  border: none;
  background: #ffcc00;
  color: #333;
  font-size: 16px;
  border-radius: 5px;
  cursor: pointer;
}

.hero button:hover {
  background: #e6b800;
}

/* About */
.about, .services, .contact {
  padding: 60px 20px;
  text-align: center;
  background: #fff;
  margin: 20px auto;
  border-radius: 10px;
  width: 90%;
  max-width: 1000px;
}

/* Services Cards */
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.card {
  background: #f0f0f0;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 10px;
}

/* Contact Form */
.contact form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  width: 90%;
  max-width: 500px;
  margin: auto;
}

.contact input, .contact textarea {
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 6px;
}

.contact button {
  padding: 12px;
  background: #2b6777;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.contact button:hover {
  background: #1e4d59;
}

/* Footer */
footer {
  text-align: center;
  padding: 15px;
  background: #2b6777;
  color: white;
  margin-top: 20px;
}



// Show alert on button click
function showAlert() {
  alert("Welcome! Let's get started with the Final Project 🚀");
}

// Contact Form Submission (demo)
document.getElementById("contactForm").addEventListener("submit", function(e) {
  e.preventDefault();
  alert("Thank you for contacting us! We will reach out soon.");
});
