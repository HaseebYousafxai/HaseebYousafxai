<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #0a192f;
            color: #8892b0;
            line-height: 1.6;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        /* Navigation */
        nav {
            background-color: rgba(10, 25, 47, 0.95);
            position: fixed;
            width: 100%;
            z-index: 100;
            padding: 20px 0;
        }
        .nav-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            color: #64ffda;
            font-size: 24px;
            font-weight: bold;
            text-decoration: none;
        }
        .nav-links {
            display: flex;
            gap: 30px;
        }
        .nav-links a {
            color: #ccd6f6;
            text-decoration: none;
            font-size: 16px;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: #64ffda;
        }
        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 80px;
        }
        .hero-content {
            max-width: 1000px;
        }
        .hero-title {
            color: #64ffda;
            font-size: 16px;
            margin-bottom: 20px;
        }
        .hero-name {
            color: #ccd6f6;
            font-size: 80px;
            font-weight: bold;
            margin-bottom: 20px;
        }
        .hero-description {
            font-size: 60px;
            color: #8892b0;
            margin-bottom: 30px;
        }
        .hero-text {
            max-width: 540px;
            margin-bottom: 50px;
        }
        /* Sections */
        section {
            padding: 100px 0;
        }
        .section-title {
            color: #ccd6f6;
            font-size: 32px;
            margin-bottom: 40px;
        }
        /* Projects */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        .project-card {
            background-color: #112240;
            padding: 30px;
            border-radius: 4px;
            transition: transform 0.3s;
        }
        .project-card:hover {
            transform: translateY(-5px);
        }
        .project-title {
            color: #ccd6f6;
            font-size: 24px;
            margin-bottom: 15px;
        }
        .project-description {
            margin-bottom: 20px;
        }
        .project-tech {
            display: flex;
            gap: 15px;
            font-size: 14px;
            color: #64ffda;
        }
        /* Skills */
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .skill-card {
            background-color: #112240;
            padding: 15px 25px;
            border-radius: 4px;
            color: #64ffda;
        }
        /* Contact */
        .contact {
            text-align: center;
        }
        .contact-title {
            color: #64ffda;
            font-size: 16px;
            margin-bottom: 20px;
        }
        .contact-heading {
            color: #ccd6f6;
            font-size: 60px;
            margin-bottom: 20px;
        }
        .contact-text {
            max-width: 600px;
            margin: 0 auto 30px;
        }
     .button {
            display: inline-block;
            background-color: transparent;
            color: #64ffda;
            border: 1px solid #64ffda;
            padding: 15px 30px;
            border-radius: 4px;
            text-decoration: none;
            transition: all 0.3s;
        }
        .button:hover {
            background-color: rgba(100, 255, 218, 0.1);
        }
        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-name {
                font-size: 40px;
            }
            .hero-description {
                font-size: 30px;
            }
            .nav-links {
                display: none;
            }
            .section-title {
                font-size: 24px;
            }
            .contact-heading {
                font-size: 40px;
            }
        }
    </style>
</head>
<body>
    <nav>
        <div class="container nav-content">
            <a href="#" class="logo">JD.</a>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#projects">Projects</a>
                <a href="#skills">Skills</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>
    <section class="hero">
        <div class="container hero-content">
            <p class="hero-title">Hi, my name is</p>
            <h1 class="hero-name">John Doe.</h1>
            <h2 class="hero-description">I build things for the web.</h2>
            <p class="hero-text">
                I'm a software engineer specializing in building exceptional digital experiences.
                Currently, I'm focused on building accessible, human-centered products.
            </p>
            <a href="#projects" class="button">Check out my work!</a>
        </div>
    </section>
    <section id="projects">
        <div class="container">
            <h2 class="section-title">Some Things I've Built</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3 class="project-title">Project One</h3>
                    <p class="project-description">
                        A web app for visualizing personalized Spotify data. View your
                        top artists, top tracks, recently played tracks, and detailed audio
                        information about each track.
                    </p>
                    <div class="project-tech">
                        <span>React</span>
                        <span>Node.js</span>
                        <span>Express</span>
                    </div>
                </div>
                <div class="project-card">
                    <h3 class="project-title">Project Two</h3>
                    <p class="project-description">
                        A minimal, dark blue theme for VS Code, Sublime Text, Atom, iTerm,
                        and more. Available on Visual Studio Marketplace.
                    </p>
                    <div class="project-tech">
                        <span>VS Code</span>
                        <span>Sublime Text</span>
                        <span>Atom</span>
                    </div>
                </div>
                <div class="project-card">
                    <h3 class="project-title">Project Three</h3>
                    <p class="project-description">
                        A nicer look at your GitHub profile and repo stats. Includes data
                        visualizations of your top languages, starred repositories, and sort
                        through your top repos by number of stars, forks, and size.
                    </p>
                    <div class="project-tech">
                        <span>Next.js</span>
                        <span>Chart.js</span>
                        <span>GitHub API</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="skills">
        <div class="container">
            <h2 class="section-title">Skills & Technologies</h2>
            <div class="skills-container">
                <div class="skill-card">Data Analysis</div>
                <div class="skill-card">Machine Learning</div>
                <div class="skill-card">Python</div>
                <div class="skill-card">Power BI Dashboards</div>
                <div class="skill-card">Data Science</div>
                <div class="skill-card">Machine Learning Models Integration</div>
                <div class="skill-card">Data Reporting</div>
                <div class="skill-card">Data Visualization</div>
            </div>
        </div>
    </section>
    <section id="contact" class="contact">
        <div class="container">
            <p class="contact-title">What's Next?</p>
            <h2 class="contact-heading">Get In Touch</h2>
            <p class="contact-text">
                I'm currently looking for new opportunities. Whether you have a question or
                just want to say hi, I'll try my best to get back to you!
            </p>
            <a href="mailto:haseebyousafxai81@gmail.com" class="button">Say Hello</a>
        </div>
    </section>
</body>
</html>
