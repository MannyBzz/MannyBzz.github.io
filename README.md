
[IndexBIS23.html](https://github.com/user-attachments/files/24106099/IndexBIS23.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BIS23 Portfolio - Emmanuel Sintim</title>

    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">

    <!-- CSS -->
    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            overflow-x: hidden;
            color: #fff;
            background: linear-gradient(-45deg, #1abc9c, #3498db, #9b59b6, #e74c3c);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
        }

        @keyframes gradientBG {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        /* Header */
        header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 20px 50px;
            background-color: rgba(0,0,0,0.5);
            position: sticky;
            top: 0;
            z-index: 10;
        }

        header img.logo {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            border: 2px solid #fff;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #fff;
            margin-left: 20px;
            display: inline-block;
        }

        header p {
            font-size: 1.1rem;
            color: #ecf0f1;
            margin-left: 10px;
        }

        /* Introduction Section */
        .intro {
            text-align: center;
            padding: 100px 20px;
        }

        .intro h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #fff;
            margin-bottom: 20px;
        }

        .intro p {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 0 auto;
            color: #f1c40f;
        }

        /* Bio Section */
        .bio {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            padding: 80px 20px;
            gap: 40px;
        }

        .bio img {
            width: 300px;
            height: auto;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
            transition: transform 0.3s ease;
        }

        .bio img:hover {
            transform: scale(1.1);
        }

        .bio-text {
            max-width: 500px;
        }

        .bio-text h3 {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: #f39c12;
            margin-bottom: 15px;
        }

        .bio-text p {
            font-size: 1.1rem;
            color: #ecf0f1;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 20px;
            background-color: rgba(0,0,0,0.6);
            color: #ecf0f1;
            margin-top: 50px;
        }

        footer a {
            color: #1abc9c;
            margin: 0 10px;
            text-decoration: none;
            transition: color 0.3s;
        }

        footer a:hover {
            color: #e74c3c;
        }

        /* Custom Cursor */
        .cursor {
            width: 20px;
            height: 20px;
            border: 2px solid #fff;
            border-radius: 50%;
            position: absolute;
            pointer-events: none;
            transform: translate(-50%, -50%);
            transition: transform 0.1s ease, background-color 0.2s ease;
            z-index: 1000;
        }

        /* Button style */
        .btn {
            display: inline-block;
            padding: 10px 25px;
            margin-top: 15px;
            background-color: #e67e22;
            color: #fff;
            font-weight: bold;
            border-radius: 8px;
            transition: all 0.3s ease;
            text-decoration: none;
        }

        .btn:hover {
            background-color: #d35400;
            transform: scale(1.05);
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="logo-section">
            <img src="esIAMGE.png" alt="Emmanuel Sintim Logo" class="logo">
        </div>
        <div>
            <h1>BIS23 Portfolio</h1>
            <p>Page for Midterm and Final project</p>
        </div>
    </header>

    <!-- Introduction -->
    <section class="intro">
        <h2>Welcome to My BIS23 Portfolio</h2>
        <p>This website showcases my work for the Midterm and Final project. Explore my bio, projects, and creative endeavors. All work presented here is part of my BIS23 journey.</p>
    </section>

    <!-- Bio Section -->
    <section class="bio">
        <!-- Replace 'your-picture.jpg' with your personal picture -->
        <img src="3583447E-9E49-42A5-AE0F-6AA316F13DFA.jpeg" alt="Emmanuel Sintim Picture">
        <div class="bio-text">
            <h3>About Me</h3>
            <p>Hello! I am Emmanuel Sintim, a passionate student exploring the world of technology, design, and web development. This section is dedicated to introducing myself and my projects for the BIS23 Midterm and Final. Feel free to explore and learn more about my work.</p>
            <a href="#projects" class="btn">View Projects</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2012 Emmanuel Sintim. All Rights Reserved.</p>
        <p>
            <a href="#">Home</a> | 
            <a href="#">Projects</a> | 
            <a href="#">Contact</a>
        </p>
    </footer>

    <!-- Custom Cursor -->
    <div class="cursor" id="cursor"></div>
    <script>
        const cursor = document.getElementById('cursor');

        document.addEventListener('mousemove', e => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
        });

        document.querySelectorAll('a, img, .btn').forEach(elem => {
            elem.addEventListener('mouseover', () => {
                cursor.style.transform = 'translate(-50%, -50%) scale(2.2)';
                cursor.style.backgroundColor = 'rgba(255,255,255,0.3)';
            });
            elem.addEventListener('mouseout', () => {
                cursor.style.transform = 'translate(-50%, -50%) scale(1)';
                cursor.style.backgroundColor = 'transparent';
            });
        });
    </script>

</body>
</html>

