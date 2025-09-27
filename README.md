<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Personal Portfolio - Lilly</title>
  
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  
  <style>
    /* General */
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(to right, #ff7e5f, #feb47b);
      height: 100vh;
      display: flex;
      align-items: center;
      text-align: center;
      color: white;
    }

    /* Section Headings */
    section h2 {
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    /* Portfolio Cards */
    .card {
      border-radius: 12px;
      overflow: hidden;
      transition: transform 0.3s;
    }
    .card:hover {
      transform: scale(1.05);
    }

    /* Contact Form */
    form .form-control {
      border-radius: 8px;
      border: 2px solid #ccc;
    }
    form .btn {
      border-radius: 8px;
      font-weight: bold;
    }

    /* Footer */
    footer a {
      margin: 0 5px;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top">
    <div class="container">
      <a class="navbar-brand fw-bold text-warning" href="#">Lilly</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" 
              data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" 
              aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="#about">About Me</a></li>
          <li class="nav-item"><a class="nav-link" href="#portfolio">Portfolio</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero">
    <div class="container">
      <h1 class="display-3 fw-bold">Hi, I'm Lilly</h1>
      <p class="lead">Web Developer | Designer | Freelancer</p>
      <a href="#portfolio" class="btn btn-warning btn-lg mt-3">View My Work</a>
    </div>
  </header>

  <!-- About Me -->
  <section id="about" class="py-5 bg-light">
    <div class="container text-center">
      <h2 class="mb-4 text-primary">About Me</h2>
      <img src="https://via.placeholder.com/150" alt="Profile" class="rounded-circle mb-3" width="150">
      <p class="text-muted px-5">
        I am a passionate web developer and designer with a Bachelor’s Degree in Computer Science from Christ University. Over the years, I have built strong expertise in front-end development, responsive design, and UI/UX principles. I specialize in creating clean, modern, and user-friendly websites using HTML, CSS, JavaScript, Bootstrap, and jQuery, along with design tools such as Figma and Photoshop. My journey began with freelance projects, where I worked on personal portfolios and business landing pages, and it has grown into a career focused on building professional, interactive, and visually appealing web experiences. Outside of coding, I enjoy photography, traveling, and exploring creative ways to combine technology with design.
    
      </p>
    </div>
  </section>

  <!-- Portfolio Gallery -->
  <section id="portfolio" class="py-5">
    <div class="container">
      <h2 class="text-center mb-5 text-success">My Projects</h2>
      <div class="row g-4">
        <div class="col-md-6 col-lg-3">
          <div class="card shadow">
            <img src="https://source.unsplash.com/400x300/?web,design" class="card-img-top" alt="Project 1">
            <div class="card-body bg-warning text-dark">
              <h5 class="card-title">Online Resume Builder</h5>
              <p class="card-text">Developed a web-based tool where users can input personal details and instantly generate a formatted resume. Built with HTML, CSS, and JavaScript.</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="card shadow">
            <img src="https://source.unsplash.com/400x300/?graphic,design" class="card-img-top" alt="Project 2">
            <div class="card-body bg-primary text-white">
              <h5 class="card-title">Photography Portfolio Website</h5>
              <p class="card-text">Created a gallery-style website for a photographer, featuring categorized collections and a lightbox view for images.</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="card shadow">
            <img src="https://source.unsplash.com/400x300/?portfolio,website" class="card-img-top" alt="Project 3">
            <div class="card-body bg-success text-white">
              <h5 class="card-title">Task Manager App</h5>
              <p class="card-text">A simple to-do application where users can add, mark as complete, or delete daily tasks.</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3">
          <div class="card shadow">
            <img src="https://source.unsplash.com/400x300/?landing,page" class="card-img-top" alt="Project 4">
            <div class="card-body bg-danger text-white">
              <h5 class="card-title">E-Commerce Product Page</h5>
              <p class="card-text">Designed a responsive product showcase page with pricing, product images, and a call-to-action. Focused on clean UI and mobile-friendly layouts using Bootstrap.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Form -->
  <section id="contact" class="py-5 bg-light">
    <div class="container">
      <h2 class="text-center text-danger mb-5">Contact Me</h2>
      <div class="row justify-content-center">
        <div class="col-md-8">
          <form>
            <div class="mb-3">
              <label for="name" class="form-label fw-bold">Name</label>
              <input type="text" class="form-control" id="name" placeholder="Enter your name">
            </div>
            <div class="mb-3">
              <label for="email" class="form-label fw-bold">Email</label>
              <input type="email" class="form-control" id="email" placeholder="Enter your email">
            </div>
            <div class="mb-3">
              <label for="message" class="form-label fw-bold">Message</label>
              <textarea class="form-control" id="message" rows="5" placeholder="Your message"></textarea>
            </div>
            <button type="submit" class="btn btn-success btn-lg w-100">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white text-center py-3">
    <p class="mb-0">© 2025 Lilly | Connect with me on 
      <a href="#" class="text-warning text-decoration-none">LinkedIn</a>, 
      <a href="#" class="text-info text-decoration-none">Twitter</a>, 
      <a href="#" class="text-danger text-decoration-none">Instagram</a>
    </p>
  </footer>

  <!-- jQuery + Bootstrap Bundle -->
  <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

  <!-- Smooth Scrolling -->
  <script>
    $(document).ready(function(){
      $("a.nav-link").on('click', function(event) {
        if (this.hash !== "") {
          event.preventDefault();
          var hash = this.hash;
          $('html, body').animate({
            scrollTop: $(hash).offset().top
          }, 800);
        }
      });
    });
  </script>
</body>
</html>

