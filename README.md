index.html
<head>
    <title>Golu Kumar Kewat | Software Developer</title>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* CSS Variables for Easy Customization */
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --text-primary: #f8fafc;
            --text-secondary: #94a3b8;
            --accent-color: #38bdf8;
            --accent-hover: #0284c7;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            line-height: 1.6;
        }

        /* Navbar */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(15, 23, 42, 0.9);
            backdrop-filter: blur(10px);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--accent-color);
            text-decoration: none;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            color: var(--text-primary);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent-color);
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 6rem 5% 2rem;
        }

        .hero h3 {
            color: var(--accent-color);
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            max-width: 600px;
            color: var(--text-secondary);
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        .btn-group {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
            justify-content: center;
        }

        .btn {
            padding: 0.8rem 1.8rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
        }

        .btn-primary {
            background-color: var(--accent-color);
            color: #0f172a;
        }

        .btn-primary:hover {
            background-color: var(--accent-hover);
            color: #fff;
        }

        .btn-outline {
            border: 2px solid var(--accent-color);
            color: var(--accent-color);
        }

        .btn-outline:hover {
            background-color: var(--accent-color);
            color: #0f172a;
        }

        /* Sections Common Styling */
        section {
            padding: 5rem 10%;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 60px;
            height: 4px;
            background: var(--accent-color);
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        /* About & Skills */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text p {
            color: var(--text-secondary);
            margin-bottom: 1rem;
        }

        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
        }

        .skill-tag {
            background: var(--card-bg);
            padding: 0.6rem 1.2rem;
            border-radius: 20px;
            border: 1px solid rgba(56, 189, 248, 0.3);
            font-size: 0.9rem;
            color: var(--accent-color);
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 12px;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .project-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
            border-color: var(--accent-color);
        }

        .project-card h3 {
            margin-bottom: 0.8rem;
            color: var(--text-primary);
        }

        .project-card p {
            color: var(--text-secondary);
            font-size: 0.95rem;
            margin-bottom: 1.5rem;
        }

        .project-links a {
            color: var(--accent-color);
            text-decoration: none;
            margin-right: 1rem;
            font-size: 0.9rem;
            font-weight: 600;
        }

        /* Contact & Socials */
        .contact-box {
            text-align: center;
            max-width: 600px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 3rem 2rem;
            border-radius: 12px;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .social-links a {
            color: var(--text-primary);
            font-size: 1.8rem;
            transition: color 0.3s, transform 0.3s;
        }

        .social-links a:hover {
            color: var(--accent-color);
            transform: scale(1.1);
        }

        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-secondary);
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 0.9rem;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            .hero h1 {
                font-size: 2.5rem;
            }
            .about-grid {
                grid-template-columns: 1fr;
            }
            section {
                padding: 4rem 5%;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <header>
        <a href="#" class="logo">Golu.dev</a>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h3>Hello, I'm</h3>
        <h1>Golu Kumar Kewat</h1>
        <p>A passionate Software Developer based in Bihar, India. I build clean, responsive web applications and digital solutions at <strong>@iconicsolutions</strong>.</p>
        <div class="btn-group">
            <a href="#projects" class="btn btn-primary">View My Work</a>
            <a href="#contact" class="btn btn-outline">Get In Touch</a>
        </div>
    </section>

    <!-- About & Skills Section -->
    <section id="about">
        <h2 class="section-title">About & Skills</h2>
        <div class="about-grid">
            <div class="about-text">
                <p>Main ek dedicated Software Developer hoon jo modern web technologies ke saath scalable aur user-friendly applications banane par focus karta hai.</p>
                <p>Naye tools seekhna, clean code likhna aur real-world problems ko technology ke zariye solve karna meri speciality hai.</p>
            </div>
            <div>
                <h3 style="margin-bottom: 1rem;">Tech Stack</h3>
                <div class="skills-container">
                    <span class="skill-tag">HTML5</span>
                    <span class="skill-tag">CSS3</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">Git & GitHub</span>
                    <span class="skill-tag">Responsive Design</span>
                    <span class="skill-tag">Web Development</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2 class="section-title">Featured Projects</h2>
        <div class="projects-grid">
            <!-- Project 1 -->
            <div class="project-card">
                <h3>Personal Portfolio Website</h3>
                <p>Ek modern aur mobile-friendly portfolio website jo HTML, CSS aur JavaScript ka upyog karke banayi gayi hai aur GitHub Pages par hosted hai.</p>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank"><i class="fab fa-github"></i> Source Code</a>
                </div>
            </div>

            <!-- Project 2 -->
            <div class="project-card">
                <h3>Iconic Solutions Web App</h3>
                <p>Business landing page aur service management interface jo clients ko smooth user experience pradan karta hai.</p>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank"><i class="fab fa-github"></i> Source Code</a>
                </div>
            </div>

            <!-- Project 3 -->
            <div class="project-card">
                <h3>Task Manager Tool</h3>
                <p>Daily productivity badhane ke liye ek simple aur fast To-Do aur task tracking web application.</p>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank"><i class="fab fa-github"></i> Source Code</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2 class="section-title">Contact Me</h2>
        <div class="contact-box">
            <p style="color: var(--text-secondary);">Kisi project par kaam karna chahte hain ya koi sawal hai? Mujhse seedha connect karein:</p>
            <div class="social-links">
                <a href="https://github.com/golukumarkewat21" target="_blank" title="GitHub"><i class="fab fa-github"></i></a>
                <a href="https://instagram.com" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
                <a href="mailto:contact@example.com" title="Email"><i class="fas fa-envelope"></i></a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; <span id="year"></span> Golu Kumar Kewat. Built with ❤️ and hosted on GitHub.</p>
    </footer>

    <!-- JavaScript -->
    <script>
        // Automatically update copyright year
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
