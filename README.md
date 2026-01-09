<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Krystel Gwen Ordiales</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f0ff;
      color: #2c2c2c;
    }

    header {
      background: linear-gradient(rgba(88, 24, 124, 0.7), rgba(88, 24, 124, 0.7)),
      
      color: white;
      text-align: center;
      padding: 80px 20px;
    }

    header h1 {
      font-size: 3em;
      margin: 0;
      text-shadow: 2px 2px 6px black;
    }

    header p {
      font-size: 1.2em;
      margin-top: 10px;
    }

    nav {
      display: flex;
      justify-content: center;
      background: #4a148c;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 15px 20px;
      transition: 0.3s;
    }

    nav a:hover {
      background: #9c27b0;
    }

    section {
      padding: 50px 20px;
      text-align: center;
    }

    h2 {
      color: #6a1b9a;
    }

    .skills-bar {
      background: #d1c4e9;
      border-radius: 25px;
      margin: 10px auto;
      width: 60%;
      height: 25px;
      overflow: hidden;
    }

    .skills-fill {
      background: linear-gradient(to right, #8e24aa, #ba68c8);
      height: 100%;
      width: 0;
      text-align: right;
      padding-right: 10px;
      color: white;
      line-height: 25px;
      transition: width 2s ease;
      font-size: 0.9em;
    }

    footer {
      background: #4a148c;
      color: white;
      text-align: center;
      padding: 15px;
    }

    a {
      color: #6a1b9a;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header id="home">
    <h1>Krystel Gwen Ordiales</h1>
    <p>Dreamer • Creator • Aspiring Web Adventurer</p>
  </header>

  <!-- Navigation -->
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About Me</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <p>
      Hi! I’m <strong>Krystel Gwen Ordiales</strong>, a passionate dreamer who loves creativity,
      learning new things, and exploring the world of web development.
  <!-- Skills Section -->
  <section id="skills">
    <h2>My Skills</h2>
    <p>Here are some of my strengths</p>

    <div class="skills-bar">
      <div class="skills-fill" data-skill="90%">HTML & CSS</div>
    </div>

    <div class="skills-bar">
      <div class="skills-fill" data-skill="80%">JavaScript</div>
    </div>

    <div class="skills-bar">
      <div class="skills-fill" data-skill="85%">Creativity</div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <p>Email: <a href="mailto:penarandajohnroland@gmail.com">penarandajohnroland@gmail.com</a></p>
    <p>“Let’s create something amazing together.”</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Made with 💜 Purple Energy</p>
  </footer>

  <script>
    // Animate skill bars on scroll
    window.addEventListener("scroll", function () {
      let skills = document.querySelectorAll(".skills-fill");
      skills.forEach(skill => {
        let rect = skill.getBoundingClientRect();
        if (rect.top < window.innerHeight) {
          skill.style.width = skill.getAttribute("data-skill");
        }
      });
    });
  </script>

</body>
</html>
