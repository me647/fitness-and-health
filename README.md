# fitness-and-health
This website serves as a comprehensive guide for users interested in exploring fitness routines, gaining nutrition tips, and practicing mindfulness techniques to achieve a balanced lifestyle.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Health & Fitness</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    /* Custom Styling */
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f8f9fa;
    }
    h1, h2, h3 {
      font-weight: bold;
    }
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
    }

    .hero {
      background-color: #007bff;
      color: white;
      padding: 100px 0;
      text-align: center;
    }

    .hero h1 {
      font-size: 3rem;
    }

    .hero p {
      font-size: 1.2rem;
    }

    .about-section, .services, .contact-form {
      margin-top: 50px;
    }

    .card-body {
      background-color: #f1f1f1;
    }

    .scroll-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #007bff;
      color: white;
      border: none;
      padding: 10px;
      border-radius: 50%;
      font-size: 18px;
      cursor: pointer;
      display: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #343a40;
      color: white;
    }

    footer a {
      color: #ffffff;
      text-decoration: none;
    }

    /* Responsive styling for smaller devices */
    @media (max-width: 768px) {
      .hero {
        padding: 50px 0;
      }
      .card-body {
        padding: 20px;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Health & Fitness</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Home Page -->
  <section id="home" class="hero">
    <h1>Welcome to Health & Fitness</h1>
    <p>Your ultimate destination for a healthier, fitter lifestyle. Get fit, stay healthy, and transform your life today! We offer expert guidance, personalized plans, and the support you need to achieve your fitness goals. Whether you're looking to lose weight, build muscle, or improve overall health, we have the tools and resources to help you succeed.</p>
    <p>Join our community of fitness enthusiasts and start your journey today!</p>
  </section>

  <!-- About Page -->
  <section id="about" class="container about-section">
    <h2>About Us</h2>
    <p>At Health & Fitness, we believe that everyone deserves to live a healthy and active lifestyle. Our mission is to make fitness accessible to all, providing customized plans and expert advice tailored to your unique goals and needs. Whether you're new to fitness or a seasoned athlete, we are here to support your journey every step of the way.</p>

    <p>Our team of certified trainers, nutritionists, and coaches are dedicated to helping you unlock your full potential. We offer personalized workout plans, nutritional guidance, and online coaching to ensure you have everything you need to achieve your fitness goals. Our approach is built on science, motivation, and a passion for wellness.</p>

    <div class="row services">
      <div class="col-md-4">
        <div class="card">
          <img src="pexels-olly-864990.jpg" class="card-img-top" alt="Workout Plans">
          <div class="card-body">
            <h5 class="card-title">Workout Plans</h5>
            <p class="card-text">Custom workout plans tailored to your goals. Whether you're a beginner or advanced, we have the right plan for you.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="pexels-janetrangdoan-1171170.jpg" class="card-img-top" alt="Nutrition Advice">
          <div class="card-body">
            <h5 class="card-title">Nutrition Advice</h5>
            <p class="card-text">Get expert nutritional advice to fuel your body properly and achieve optimal results from your workouts.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="pexels-tirachard-kumtanom-112571-347134.jpg" class="card-img-top" alt="Online Coaching">
          <div class="card-body">
            <h5 class="card-title">Online Coaching</h5>
            <p class="card-text">Get personal coaching from certified fitness trainers to help you stay on track with your fitness journey.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Page -->
  <section id="contact" class="container contact-form">
    <h2>Contact Us</h2>
    <form id="contactForm">
      <div class="mb-3">
        <label for="name" class="form-label">Full Name</label>
        <input type="text" class="form-control" id="name" required>
      </div>
      <div class="mb-3">
        <label for="email" class="form-label">Email Address</label>
        <input type="email" class="form-control" id="email" required>
      </div>
      <div class="mb-3">
        <label for="message" class="form-label">Message</label>
        <textarea class="form-control" id="message" rows="3" required></textarea>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
  </section>

  <!-- Scroll-to-Top Button -->
  <button id="scrollBtn" class="scroll-btn" onclick="scrollToTop()">↑</button>

  <!-- Footer with GitHub Link -->
  <footer>
    <p>&copy; 2024 Health & Fitness | <a href="https://github.com" target="_blank">GitHub</a></p>
  </footer>

  <!-- JavaScript -->
  <script>
    // Scroll to Top Button Functionality
    window.onscroll = function() {
      let scrollBtn = document.getElementById("scrollBtn");
      if (document.body.scrollTop > 200 || document.documentElement.scrollTop > 200) {
        scrollBtn.style.display = "block";
      } else {
        scrollBtn.style.display = "none";
      }
    };

    function scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    // Contact Form Validation and Alert
    document.getElementById('contactForm').addEventListener('submit', function(event) {
      event.preventDefault();
      alert('Thank you for your message! We will get back to you shortly.');
    });
  </script>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
