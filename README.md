<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ritesh Swain | Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <nav>
            <div class="logo">Ritesh Swain</div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Hi, I'm <span>Ritesh Swain</span></h1>
            <p>Electrical Engineer | Aspiring Full-Stack Developer</p>
            <a href="#contact" class="btn">Get in Touch</a>
        </div>
    </section>

    <section id="about" class="section">
        <h2>About Me</h2>
        <p>I'm a final-year electrical engineering student with experience in power distribution, robotics, and software development.</p>
    </section>

    <section id="experience" class="section">
        <h2>Experience</h2>
        <div class="exp-item">
            <h3>Graduate Engineer Trainee (GET) - JSW Steel</h3>
            <p>Preparing for an upcoming opportunity.</p>
        </div>
        <div class="exp-item">
            <h3>Electrical Intern - Rourkela Steel Plant (SAIL)</h3>
            <p>Worked on power distribution in industrial settings.</p>
        </div>
        <div class="exp-item">
            <h3>Intern - Railway Carriage Repair Workshop</h3>
            <p>Experience in train power car maintenance.</p>
        </div>
    </section>

    <section id="projects" class="section">
        <h2>Projects</h2>
        <div class="project">
            <h3>Robotics Society Leadership</h3>
            <p>Mentored students in IoT, circuit design, and robotics.</p>
        </div>
    </section>

    <section id="contact" class="section">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:your.email@example.com">your.email@example.com</a></p>
        <p>GitHub: <a href="https://github.com/Swainritesh" target="_blank">Swainritesh</a></p>
        <p>LinkedIn: <a href="https://linkedin.com/in/your-profile" target="_blank">Your Profile</a></p>
    </section>

    <footer>
        <p>&copy; 2025 Ritesh Swain. All rights reserved.</p>
    </footer>
</body>
</html>
,
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background-color: #000;
    color: #fff;
}

header {
    position: fixed;
    width: 100%;
    background: rgba(0, 0, 0, 0.8);
    padding: 10px 0;
    text-align: center;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    text-decoration: none;
    color: #fff;
    transition: 0.3s;
}

.nav-links a:hover {
    color: #bbb;
}

.hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: linear-gradient(to bottom, #000, #222);
}

.hero h1 span {
    color: #ffcc00;
}

.btn {
    background: #ffcc00;
    color: #000;
    padding: 10px 20px;
    text-decoration: none;
    display: inline-block;
    margin-top: 20px;
}

.section {
    padding: 50px 20px;
    text-align: center;
}

footer {
    text-align: center;
    padding: 10px;
    background: #111;
}
,
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener("click", function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute("href")).scrollIntoView({
            behavior: "smooth"
        });
    });
});
