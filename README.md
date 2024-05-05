<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Art Gallery</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            overflow-x: hidden; /* Hide horizontal scrollbar */
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        h1, h2, h3 {
            color: #333;
        }
        /* Navigation Styles */
        nav {
            background-color: #333;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
        }
        nav ul {
            margin: 0;
            padding: 0;
            list-style-type: none;
            display: flex;
            justify-content: space-around;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            display: block;
            color: #fff;
            text-decoration: none;
            padding: 15px 20px;
            transition: background-color 0.3s ease;
        }
        nav ul li a:hover {
            background-color: #555;
        }
        /* Section Styles */
        section {
            padding: 50px 20px;
        }
        /* Icon Styles */
        .icon {
            display: block;
            margin: 20px auto;
            width: 100px; /* Adjust size as needed */
            height: auto;
        }
    </style>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <section id="home">
            <h1>Welcome to Our Art Gallery</h1>
            <img class="icon" src="placeholder.png" alt="Icon"> <!-- Replace 'placeholder.png' with your actual icon image -->
        </section>

        <section id="about">
            <h2>About Us</h2>
            <p>This is a brief description of our art gallery.</p>
        </section>

        <section id="services">
            <h2>Our Services</h2>
            <p>Here are the services we offer to our customers.</p>
        </section>

        <section id="contact">
            <h2>Contact Us</h2>
            <p>If you have any questions, feel free to contact us.</p>
        </section>
    </div>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
