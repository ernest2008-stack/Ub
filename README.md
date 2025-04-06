<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UB Football Academy | Elite Training</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* CSS Styles */
        :root {
            --primary: #0056b3;
            --secondary: #ff6b00;
            --dark: #1a1a1a;
            --light: #f8f9fa;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Logo Styles */
        .header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            color: var(--white);
            text-decoration: none;
            font-family: 'Arial Black', sans-serif;
        }

        .logo-main {
            font-size: 2rem;
            font-weight: 900;
            letter-spacing: 1px;
            text-transform: uppercase;
            line-height: 1;
        }

        .logo-year {
            font-size: 1rem;
            font-weight: 400;
            margin-top: 4px;
            letter-spacing: 2px;
        }

        /* Navigation */
        .nav-list {
            display: flex;
            list-style: none;
        }

        .nav-list li {
            margin-left: 2rem;
        }

        .nav-list a {
            color: var(--white);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-list a:hover {
            color: var(--secondary);
        }

        .cta-button {
            background-color: var(--secondary);
            padding: 0.5rem 1.5rem;
            border-radius: 5px;
            font-weight: 600;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: url('https://images.unsplash.com/photo-1574629810360-7efbbe195018') center/cover;
            display: flex;
            align-items: center;
            text-align: center;
            color: var(--white);
            margin-top: 80px;
            position: relative;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
        }

        .hero-content {
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        .btn-primary {
            background-color: var(--secondary);
            color: var(--white);
            padding: 1rem 2.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s;
        }

        .btn-primary:hover {
            background-color: #e05d00;
            transform: translateY(-3px);
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: var(--white);
            padding: 3rem 0;
            text-align: center;
        }

        .footer-logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 1.5rem;
            font-family: 'Arial Black', sans-serif;
        }

        .footer-logo span:first-child {
            font-size: 1.8rem;
            font-weight: 900;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-list {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="container header-container">
            <a href="#" class="logo">
                <span class="logo-main">UB ACADEMY</span>
                <span class="logo-year">2023</span>
            </a>
            
            <nav class="nav">
                <ul class="nav-list">
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#programs">Programs</a></li>
                    <li><a href="#coaches">Coaches</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact" class="cta-button">Join Now</a></li>
                </ul>
                <div class="hamburger">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </nav>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Welcome to UB Football Academy</h1>
                <p>Join us to enhance your football skills and achieve your dreams</p>
                <a href="#programs" class="btn-primary">Explore Programs</a>
            </div>
        </section>

        <section id="about" class="container section">
            <h2>About Us</h2>
            <p>UB Football Academy is dedicated to developing football talent through professional coaching and modern training methodologies.</p>
        </section>

        <section id="programs" class="container section">
            <h2>Our Programs</h2>
            <div class="programs-grid">
                <div class="program-card">
                    <h3>Beginner Training</h3>
                    <p>Fundamental skills development for new players</p>
                </div>
                <div class="program-card">
                    <h3>Advanced Techniques</h3>
                    <p>High-level training for competitive players</p>
                </div>
                <div class="program-card">
                    <h3>Team Strategy</h3>
                    <p>Tactical development for teams</p>
                </div>
            </div>
        </section>

        <section id="contact" class="container section">
            <h2>Contact Us</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <button type="submit" class="btn-primary">Submit</button>
            </form>
        </section>
    </main>

    <footer>
        <div class="container">
            <div class="footer-logo">
                <span>UB ACADEMY</span>
                <span>2023</span>
            </div>
            <p>&copy; 2023 UB Football Academy. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const hamburger = document.querySelector('.hamburger');
        const navList = document.querySelector('.nav-list');
        
        hamburger.addEventListener('click', () => {
            navList.classList.toggle('active');
            hamburger.classList.toggle('active');
        });
    </script>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UB Football Academy | Elite Training</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* CSS Styles */
        :root {
            --primary: #0056b3;
            --secondary: #ff6b00;
            --dark: #1a1a1a;
            --light: #f8f9fa;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Logo Styles */
        .header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            color: var(--white);
            text-decoration: none;
            font-family: 'Arial Black', sans-serif;
        }

        .logo-main {
            font-size: 2rem;
            font-weight: 900;
            letter-spacing: 1px;
            text-transform: uppercase;
            line-height: 1;
        }

        .logo-year {
            font-size: 1rem;
            font-weight: 400;
            margin-top: 4px;
            letter-spacing: 2px;
        }

        /* Navigation */
        .nav-list {
            display: flex;
            list-style: none;
        }

        .nav-list li {
            margin-left: 2rem;
        }

        .nav-list a {
            color: var(--white);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-list a:hover {
            color: var(--secondary);
        }

        .cta-button {
            background-color: var(--secondary);
            padding: 0.5rem 1.5rem;
            border-radius: 5px;
            font-weight: 600;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: url('https://images.unsplash.com/photo-1574629810360-7efbbe195018') center/cover;
            display: flex;
            align-items: center;
            text-align: center;
            color: var(--white);
            margin-top: 80px;
            position: relative;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
        }

        .hero-content {
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        .btn-primary {
            background-color: var(--secondary);
            color: var(--white);
            padding: 1rem 2.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s;
        }

        .btn-primary:hover {
            background-color: #e05d00;
            transform: translateY(-3px);
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: var(--white);
            padding: 3rem 0;
            text-align: center;
        }

        .footer-logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 1.5rem;
            font-family: 'Arial Black', sans-serif;
        }

        .footer-logo span:first-child {
            font-size: 1.8rem;
            font-weight: 900;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-list {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="container header-container">
            <a href="#" class="logo">
                <span class="logo-main">UB ACADEMY</span>
                <span class="logo-year">2023</span>
            </a>
            
            <nav class="nav">
                <ul class="nav-list">
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#programs">Programs</a></li>
                    <li><a href="#coaches">Coaches</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact" class="cta-button">Join Now</a></li>
                </ul>
                <div class="hamburger">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </nav>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Welcome to UB Football Academy</h1>
                <p>Join us to enhance your football skills and achieve your dreams</p>
                <a href="#programs" class="btn-primary">Explore Programs</a>
            </div>
        </section>

        <section id="about" class="container section">
            <h2>About Us</h2>
            <p>UB Football Academy is dedicated to developing football talent through professional coaching and modern training methodologies.</p>
        </section>

        <section id="programs" class="container section">
            <h2>Our Programs</h2>
            <div class="programs-grid">
                <div class="program-card">
                    <h3>Beginner Training</h3>
                    <p>Fundamental skills development for new players</p>
                </div>
                <div class="program-card">
                    <h3>Advanced Techniques</h3>
                    <p>High-level training for competitive players</p>
                </div>
                <div class="program-card">
                    <h3>Team Strategy</h3>
                    <p>Tactical development for teams</p>
                </div>
            </div>
        </section>

        <section id="contact" class="container section">
            <h2>Contact Us</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <button type="submit" class="btn-primary">Submit</button>
            </form>
        </section>
    </main>

    <footer>
        <div class="container">
            <div class="footer-logo">
                <span>UB ACADEMY</span>
                <span>2023</span>
            </div>
            <p>&copy; 2023 UB Football Academy. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const hamburger = document.querySelector('.hamburger');
        const navList = document.querySelector('.nav-list');
        
        hamburger.addEventListener('click', () => {
            navLinost.classList.toggle('active');
            hamburger.classList.toggle('active');
        });
    </script>
</body>
</html>
