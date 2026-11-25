<index.html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Golu Kumar Kewat | Software Developer</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navbar -->
    <header>
        <nav class="navbar">
            <div class="logo">Golu<span>.dev</span></div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="about">
        <div class="hero-content">
            <p class="greeting">Hi, I'm</p>
            <h1>Golu Kumar Kewat</h1>
            <h2>Software Developer</h2>
            <p class="bio">
                Passionate about building clean, functional, and user-friendly web applications. 
                Currently focusing on modern web technologies and solving real-world problems through code.
            </p>
            <div class="hero-buttons">
                <a href="#projects" class="btn primary">View My Work</a>
                <a href="https://github.com/golukumarkewat21" target="_blank" class="btn secondary">GitHub Profile</a>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section class="section" id="skills">
        <h2 class="section-title">Technical Skills</h2>
        <div class="skills-grid">
            <div class="skill-card">HTML5 & CSS3</div>
            <div class="skill-card">JavaScript (ES6+)</div>
            <div class="skill-card">React.js</div>
            <div class="skill-card">Node.js</div>
            <div class="skill-card">Git & GitHub</div>
            <div class="skill-card">Responsive Design</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="section" id="projects">
        <h2 class="section-title">Featured Projects</h2>
        <div class="projects-grid">
            
            <div class="project-card">
                <h3>Expense Tracker App</h3>
                <p>A web application to track daily income and expenses with local storage support and category filters.</p>
                <div class="tags">
                    <span>HTML</span><span>CSS</span><span>JavaScript</span>
                </div>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank">GitHub Code →</a>
                </div>
            </div>

            <div class="project-card">
                <h3>Weather Forecast App</h3>
                <p>Real-time weather dashboard fetching live temperature, humidity, and wind data using OpenWeather API.</p>
                <div class="tags">
                    <span>JavaScript</span><span>REST API</span><span>CSS</span>
                </div>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank">GitHub Code →</a>
                </div>
            </div>

            <div class="project-card">
                <h3>Task Management System</h3>
                <p>Clean productivity tool allowing users to add, edit, prioritize, and complete daily tasks effortlessly.</p>
                <div class="tags">
                    <span>React</span><span>Tailwind CSS</span>
                </div>
                <div class="project-links">
                    <a href="https://github.com/golukumarkewat21" target="_blank">GitHub Code →</a>
                </div>
            </div>

        </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact" id="contact">
        <h2 class="section-title">Get In Touch</h2>
        <p>Interested in collaborating or hiring? Feel free to reach out!</p>
        <a href="mailto:your.email@example.com" class="btn primary">Say Hello</a>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2026 Golu Kumar Kewat. Built with HTML & CSS.</p>
    </footer>

</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    scroll-behavior: smooth;
}

body {
    background-color: #0f172a;
    color: #f8fafc;
    line-height: 1.6;
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.2rem 8%;
    background-color: #1e293b;
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    color: #fff;
}

.logo span {
    color: #38bdf8;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 1.5rem;
}

.nav-links a {
    color: #cbd5e1;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: #38bdf8;
}

/* Hero Section */
.hero {
    min-height: 85vh;
    display: flex;
    align-items: center;
    padding: 0 8%;
}

.greeting {
    color: #38bdf8;
    font-size: 1.1rem;
    font-weight: 600;
}

.hero h1 {
    font-size: 3.2rem;
    margin: 0.3rem 0;
}

.hero h2 {
    font-size: 1.8rem;
    color: #94a3b8;
    margin-bottom: 1rem;
}

.bio {
    max-width: 600px;
    color: #cbd5e1;
    margin-bottom: 2rem;
}

.hero-buttons {
    display: flex;
    gap: 1rem;
}

.btn {
    padding: 0.75rem 1.5rem;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 600;
    transition: 0.3s;
}

.primary {
    background-color: #38bdf8;
    color: #0f172a;
}

.primary:hover {
    background-color: #0284c7;
    color: #fff;
}

.secondary {
    border: 1px solid #38bdf8;
    color: #38bdf8;
}

.secondary:hover {
    background-color: rgba(56, 189, 248, 0.1);
}

/* Sections */
.section {
    padding: 4rem 8%;
}

.section-title {
    font-size: 2rem;
    margin-bottom: 2rem;
    border-left: 4px solid #38bdf8;
    padding-left: 0.8rem;
}

/* Skills */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1rem;
}

.skill-card {
    background-color: #1e293b;
    padding: 1.2rem;
    text-align: center;
    border-radius: 8px;
    font-weight: 600;
    border: 1px solid #334155;
}

/* Projects */
.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.5rem;
}

.project-card {
    background-color: #1e293b;
    padding: 1.5rem;
    border-radius: 10px;
    border: 1px solid #334155;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.project-card h3 {
    color: #38bdf8;
    margin-bottom: 0.5rem;
}

.project-card p {
    color: #cbd5e1;
    font-size: 0.95rem;
    margin-bottom: 1rem;
}

.tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
}

.tags span {
    background-color: #0f172a;
    color: #38bdf8;
    padding: 0.25rem 0.6rem;
    border-radius: 4px;
    font-size: 0.8rem;
}

.project-links a {
    color: #fff;
    text-decoration: none;
    font-weight: 600;
    font-size: 0.9rem;
}

.project-links a:hover {
    color: #38bdf8;
}

/* Contact & Footer */
.contact {
    text-align: center;
}

.contact .section-title {
    border: none;
    padding: 0;
}

.contact p {
    color: #cbd5e1;
    margin-bottom: 1.5rem;
}

footer {
    text-align: center;
    padding: 1.5rem;
    background-color: #1e293b;
    color: #94a3b8;
    font-size: 0.9rem;
}

/* Mobile Responsive */
@media (max-width: 600px) {
    .hero h1 { font-size: 2.2rem; }
    .nav-links { display: none; }
}
