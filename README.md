# PRODIGY_WD_01
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Navigation Menu</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    #navbar {
      position: fixed;
      top: 0;
      width: 100%;
      background-color: rgba(0, 0, 255, 0.5); /* Initial background color */
      transition: background-color 0.3s ease;
    }

    #navbar ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      text-align: center;
    }

    #navbar li {
      display: inline-block;
      margin-right: 20px;
    }

    #navbar a {
      display: block;
      padding: 10px 20px;
      color: white;
      text-decoration: none;
    }

    #navbar a:hover {
      background-color: rgba(0, 0, 255, 0.7); /* Background color on hover */
    }
  </style>
</head>
<body>
  <nav id="navbar">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <div id="content">
    <!-- Your page content goes here -->
    <div style="height: 2000px;">Scroll down to see the effect</div>
  </div>

  <script>
    window.addEventListener('scroll', function() {
      var navbar = document.getElementById('navbar');
      if (window.scrollY > 50) {
        navbar.style.backgroundColor = 'rgba(0, 0, 255, 0.8)'; // Change background color when scrolled
      } else {
        navbar.style.backgroundColor = 'rgba(0, 0, 255, 0.5)'; // Revert to initial background color
      }
    });
  </script>
</body>
</html>
