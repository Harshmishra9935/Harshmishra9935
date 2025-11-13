## Hi there 👋


**Harshmishra9935/Harshmishra9935** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Animated Landing Page</title>
  <style>
    /* ===== Reset and Base Styles ===== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: #0f2027;
      background: linear-gradient(120deg, #203a43, #2c5364, #0f2027);
      color: #fff;
      overflow-x: hidden;
    }

    /* ===== Navigation Bar ===== */
    header {
      width: 100%;
      position: fixed;
      top: 0;
      left: 0;
      background: rgba(0, 0, 0, 0.4);
      backdrop-filter: blur(8px);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 80px;
      z-index: 1000;
      transition: 0.3s;
    }

    header.scrolled {
      background: rgba(0, 0, 0, 0.8);
      padding: 10px 60px;
    }

    .logo {
      font-size: 1.8em;
      font-weight: bold;
      letter-spacing: 2px;
      color: #00c6ff;
    }

    nav ul {
      display: flex;
      list-style: none;
    }

    nav ul li {
      margin-left: 40px;
    }

    nav ul li a {
      text-decoration: none;
      color: #fff;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #00c6ff;
    }

    /* ===== Hero Section ===== */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(135deg, #00c6ff33, #0072ff33);
      backdrop-filter: blur(2px);
      animation: fadeIn 1.5s ease forwards;
    }

    .hero h1 {
      font-size: 3.5em;
      margin-bottom: 10px;
      opacity: 0;
      transform: translateY(30px);
      animation: slideUp 1s ease forwards 0.5s;
    }

    .hero p {
      font-size: 1.3em;
      max-width: 600px;
      opacity: 0;
      transform: translateY(30px);
      animation: slideUp 1s ease forwards 1s;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes slideUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* ===== Sections ===== */
    section {
      padding: 100px 80px;
      opacity: 0;
      transform: translateY(60px);
      transition: all 1s ease;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .features {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      gap: 40px;
    }

    .feature-box {
      background: rgba(255,255,255,0.1);
      padding: 40px;
      border-radius: 10px;
      width: 300px;
      text-align: center;
      transition: transform 0.3s, background 0.3s;
    }

    .feature-box:hover {
      transform: translateY(-10px);
      background: rgba(255,255,255,0.2);
    }

    /* ===== Footer ===== */
    footer {
      text-align: center;
      padding: 40px;
      background: rgba(0, 0, 0, 0.6);
    }

  </style>
</head>
<body>
  <!-- ===== Navigation ===== -->
  <header id="header">
    <div class="logo">MyBrand</div>
    <nav>
      <ul>
        <li><a href="#hero">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- ===== Hero Section ===== -->
  <section class="hero" id="hero">
    <h1>Welcome to My Animated Site</h1>
    <p>Experience smooth animations and a modern, responsive design built with HTML, CSS, and JavaScript.</p>
  </section>

  <!-- ===== About Section ===== -->
  <section id="about">
    <h2>About Us</h2>
    <p>We build visually appealing and interactive websites using modern web technologies. Scroll animations, parallax effects, and responsive design — all in one package.</p>
  </section>

  <!-- ===== Services Section ===== -->
  <section id="services">
    <h2>Our Services</h2>
    <div class="features">
      <div class="feature-box">
        <h3>Web Design</h3>
        <p>Clean, elegant, and user-friendly designs to captivate your audience.</p>
      </div>
      <div class="feature-box">
        <h3>Animation</h3>
        <p>Bring life to your website with subtle yet powerful motion effects.</p>
      </div>
      <div class="feature-box">
        <h3>Development</h3>
        <p>High-performance code that ensures speed, security, and scalability.</p>
      </div>
    </div>
  </section>

  <!-- ===== Contact Section ===== -->
  <section id="contact">
    <h2>Contact Us</h2>
    <p>Ready to create something amazing? Let’s work together!</p>
  </section>

  <!-- ===== Footer ===== -->
  <footer>
    <p>&copy; 2025 MyBrand. All rights reserved.</p>
  </footer>

  <script>
    // Change navbar on scroll
    const header = document.getElementById('header');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) header.classList.add('scrolled');
      else header.classList.remove('scrolled');
    });

    // Reveal sections on scroll
    const sections = document.querySelectorAll('section');
    window.addEventListener('scroll', () => {
      sections.forEach(sec => {
        const top = sec.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) sec.classList.add('visible');
      });
    });
  </script>
</body>
</html>

