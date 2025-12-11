# MannyBzz.github.io[dealershipIndex.html](https://github.com/user-attachments/files/24105090/dealershipIndex.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Elite Motors - Grand Opening</title>

  <!-- Inline CSS -->
  <style>
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      color: #222;
      background: url('background-texture.jpg') no-repeat center center fixed;
      background-size: cover;
      margin: 0;
      padding: 0;
      cursor: none; /* hides default cursor for custom effect */
    }

    /* Custom cursor circle */
    .cursor {
      width: 20px;
      height: 20px;
      border: 2px solid #0073e6;
      border-radius: 50%;
      position: fixed;
      transform: translate(-50%, -50%);
      pointer-events: none;
      transition: transform 0.15s ease-out, width 0.2s, height 0.2s;
      z-index: 9999;
    }

    .cursor.hover {
      width: 40px;
      height: 40px;
      border-color: #ff6600;
    }

    header {
      text-align: center;
      background-color: #003366;
      color: white;
      padding: 40px 0;
    }

    header img {
      width: 120px;
      height: auto;
      border-radius: 50%;
      transition: transform 0.3s;
    }

    header img:hover {
      transform: scale(1.1);
    }

    h1 {
      font-size: 2.5em;
      margin-top: 15px;
      color: #ffcc00;
    }

    .content {
      max-width: 900px;
      margin: 40px auto;
      background-color: rgba(255, 255, 255, 0.9);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
    }

    .intro {
      font-size: 1.2em;
      color: #003366;
      text-align: center;
    }

    .bio {
      margin-top: 20px;
      line-height: 1.6em;
      color: #444;
    }

    .photo {
      text-align: center;
      margin: 30px 0;
    }

    .photo img {
      width: 400px;
      border-radius: 12px;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .photo img:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px #888;
    }

    footer {
      background-color: #222;
      color: #fff;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }

    footer a {
      color: #66ccff;
      text-decoration: none;
      margin: 0 12px;
      transition: color 0.3s;
    }

    footer a:hover {
      color: #ff6600;
    }
  </style>
</head>

<body>
  <!-- Custom cursor -->
  <div class="cursor"></div>

  <!-- HEADER -->
  <header>
    <img src= "logo.jpeg" alt="Elite Motors Logo" />
    <h1>Elite Motors - Grand Opening</h1>
    <p>Where Innovation Meets the Road</p>
  </header>

  <!-- MAIN CONTENT -->
  <div class="content">
    <p class="intro">
      Welcome to <strong>Elite Motors</strong> — your destination for modern vehicles, trusted service, and unmatched customer care!
    </p>

    <p class="bio">
      Elite Motors is proud to announce the grand opening of our brand-new dealership in the heart of the city.
      We specialize in new and certified pre-owned vehicles from leading brands, offering a world-class showroom
      experience and top-tier customer support. Our mission is to make every driver’s dream car a reality with
      affordable financing, expert maintenance, and premium quality.
    </p>

    <div class="photo">
      <img src= "showroom.jpeg" alt="Elite Motors Showroom" />
      <p><em>Our state-of-the-art showroom, ready to serve you.</em></p>
    </div>

    <p style="text-align:center; color:#555; font-size:0.9em;">
      &copy; 2012 Elite Motors — All Rights Reserved
    </p>
  </div>

  <!-- FOOTER -->
  <footer>
    <a href="mailto:info@elitemotors.com">Contact Us</a> |
    <a href="https://www.google.com/maps" target="_blank">Find Us</a>
  </footer>

  <!-- Custom Cursor Script -->
  <script>
    const cursor = document.querySelector('.cursor');

    document.addEventListener('mousemove', e => {
      cursor.style.left = e.clientX + 'px';
      cursor.style.top = e.clientY + 'px';
    });

    document.querySelectorAll('a, img, button').forEach(el => {
      el.addEventListener('mouseenter', () => cursor.classList.add('hover'));
      el.addEventListener('mouseleave', () => cursor.classList.remove('hover'));
    });
  </script>
</body>
</html>
