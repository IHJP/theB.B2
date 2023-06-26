<!DOCTYPE html>
<html>
<head>
  <title>TheL.B</title>
  <style>
    /* Reset some default styles */
    body, h1, h2, p, ul, li {
      margin: 0;
      padding: 0;
    }
    
    /* Global styles */
    body {
      font-family: Arial, sans-serif;
      color: #fff; /* Text color set to white */
      overflow: hidden; /* Prevent scrolling due to background */
    }
    
    /* Header styles */
    header {
      background-color: #333;
      padding: 20px;
      text-align: center;
    }
    
    h1 {
      color: #fff;
      font-size: 28px;
      margin-bottom: 10px;
    }
    
    nav ul {
      list-style: none;
    }
    
    nav ul li {
      display: inline-block;
      margin-right: 10px;
    }
    
    nav ul li a {
      color: #fff;
      text-decoration: none;
    }
    
    /* Main content styles */
    main {
      padding: 20px;
    }
    
    h2 {
      font-size: 24px;
      margin-bottom: 10px;
    }
    
    p {
      margin-bottom: 10px;
    }
    
    /* Footer styles */
    footer {
      background-color: #333;
      padding: 20px;
      text-align: center;
      color: #fff;
      font-size: 14px;
    }
    
    footer a {
      color: #fff;
      text-decoration: none;
    }
    
    /* Center the text */
    .welcome-text {
      text-align: center;
      margin-bottom: 10px;
    }
    
    /* Set the background image */
    body {
      background: radial-gradient(ellipse at center, #232526 0%, #414345 100%);
    }
    
    /* Overlay for stars */
    .stars {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: -1;
    }
    
    /* Individual star */
    .star {
      position: absolute;
      background-color: #fff;
      border-radius: 50%;
      opacity: 0.5;
    }
    
    /* Animate stars */
    @keyframes twinkling {
      0% {
        opacity: 0.5;
      }
      50% {
        opacity: 1;
      }
      100% {
        opacity: 0.5;
      }
    }
    
    /* Apply animation to stars */
    .star.animated {
      animation: twinkling 3s infinite;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to my First Website!</h1>
    <div class="welcome-text">
      <p>.</p>
    </div>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">My Media</a></li>
        <li><a href="#">Other</a></li>
      </ul>
    </nav>
  </header>
  
  <main>
    <h1.5>Web Developer, programmer, and other...
   </h1.5>
    <p><h2> So this is my first web i make in four days! Well, i'm The B.B and that's meand the legend baka my cool fake name - BAKA. ;) .</h2>

    </p>
    
    <h4>.</h4>
    <p>
      Special thanks to TheEpicMs he who taught me a lot of things

      .</p>
    
    <h2>Who is me ?</h2>
    <p>I am just an ambitious person or a person with crazy ideas.</p>
  </main>
  
  <footer>
    <p>.</p>
    <p>:) <a href="https://www.instagram.com/90s_piro/" target="_blank">Follow me on Instagram</a></p>
  </footer>
  
  <!-- Overlay for stars -->
  <div class="stars">
    <!-- Generate multiple stars using JavaScript -->
  </div>
   
  <script>
    // Generate stars
    function generateStars() {
      const starsContainer = document.querySelector('.stars');
      const numStars = 100; // Adjust the number of stars as needed
      
      for (let i = 0; i < numStars; i++) {
        const star = document.createElement('div');
        star.className = 'star animated';
        star.style.top = Math.random() * 100 + '%';
        star.style.left = Math.random() * 100 + '%';
        star.style.width = Math.random() * 2 + 'px';
        star.style.height = star.style.width;
        starsContainer.appendChild(star);
      }
    }
    
    // Generate stars when the page loads
    window.addEventListener('load', generateStars);
  </script>
</body>
</html>
