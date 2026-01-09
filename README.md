<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title></title>
  <style>
    body {
      margin: 0;
      font-family: 'Treasure Map Deadhand', Arial, sans-serif;
      background: #fdf6e3;
      color: #222;
    }
    header {
      background: url('https://uploads.onecompiler.io/43yhwbaut/449pwykxy/1000016742.jpg') no-repeat center/cover;
      color: white;
      text-align: center;
      padding: 80px 20px;
    }
    header h1 {
      font-size: 3em;
      text-shadow: 2px 2px 6px black;
    }
    nav {
      display: flex;
      justify-content: center;
      background: #222;
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
      background: #f39c12;
    }
    section {
      padding: 50px 20px;
      text-align: center;
    }
    .skills-bar {
      background: #ddd;
      border-radius: 25px;
      margin: 10px auto;
      width: 60%;
      height: 25px;
      overflow: hidden;
    }
    .skills-fill {
      background: linear-gradient(to right, #f39c12, #e67e22);
      height: 100%;
      width: 0;
      text-align: right;
      padding-right: 10px;
      color: white;
      line-height: 25px;
      transition: width 2s ease;
    }
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header id="home">
    <h1></h1>
    <p></p>
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
    <p>Hi! I’m Krystel Gwen Ordiales, a passionate dreamer just like Luffy. I love coding, creativity, and setting sail towards new adventures in web development!</p>
    <img src="https://uploads.onecompiler.io/43yhwbaut/449pwykxy/1000016761.jpg" alt="Profile" width="200">
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <h2>My Haki</h2>
    <p>Here are some of my powers</p>
    <div class="skills-bar"><div class="skills-fill" data-skill="100%">Advance Conquerors Haki</div></div>
    <div class="skills-bar"><div class="skills-fill" data-skill="100%">Advance Armament Haki</div></div>
    <div class="skills-bar"><div class="skills-fill" data-skill="100%">Advance Observation Haki</div></div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <p>Email: <a href="mailto:penarandajohnroland@gmail.com">penarandajohnroland@gmail.com</a></p>
    <p>“Let’s set sail on a new adventure together!”</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Made with ☠️ One Piece Spirit</p>
  </footer>

  <script>
    // Animate skill bars on scroll
    window.addEventListener("scroll", function(){
      let skills = document.querySelectorAll(".skills-fill");
      skills.forEach(skill => {
        let rect = skill.getBoundingClientRect();
        if(rect.top < window.innerHeight){
          skill.style.width = skill.getAttribute("data-skill");
        }
      });
    });
  </script>

</body>
</html>
