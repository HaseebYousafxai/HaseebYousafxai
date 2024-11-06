<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Haseeb Ahmad - Portfolio</title>
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

        /* Projects Section */
        .projects-section {
            padding: 100px 0;
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .project-item {
            background: #112240;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .project-item:hover {
            transform: translateY(-10px);
        }

        .project-image {
            width: 100%;
            height: 200px;
            position: relative;
            overflow: hidden;
        }

        .project-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .project-item:hover .project-image img {
            transform: scale(1.1);
        }

        .project-content {
            padding: 20px;
        }

        .project-title {
            color: #64ffda;
            font-size: 20px;
            margin-bottom: 10px;
        }

        .project-description {
            color: #8892b0;
            font-size: 16px;
            margin-bottom: 15px;
        }

        .project-tech-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 15px;
        }

        .project-tech-item {
            background: rgba(100, 255, 218, 0.1);
            color: #64ffda;
            padding: 5px 10px;
            border-radius: 4px;
            font-size: 14px;
        }

        .project-links {
            display: flex;
            gap: 15px;
        }

        .project-link {
            color: #64ffda;
            text-decoration: none;
            font-size: 14px;
            transition: color 0.3s;
        }

        .project-link:hover {
            color: #ccd6f6;
        }

        .placeholder-image {
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, #112240, #233554);
            display: flex;
            align-items: center;
            justify-content: center;
            color: #64ffda;
            font-size: 24px;
        }

        /* Work Experience Section */
        .work-experience {
            padding: 100px 0;
        }

        .section-title {
            color: #ccd6f6;
            font-size: 32px;
            margin-bottom: 40px;
        }

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

        /* Skills Section */
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

        /* Contact Section */
        .contact {
            text-align: center;
            padding: 100px 0;
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
            <a href="#" class="logo">HA.</a>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#projects">Projects</a>
                <a href="#experience">Experience</a>
                <a href="#skills">Skills</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>

    <section class="hero">
        <div class="container hero-content">
            <p class="hero-title"><strong>Hi, my name is</strong></p>
            <h1 class="hero-name">Haseeb Ahmad.</h1>
            <h2 class="hero-description">Data Scientist & Machine Learning Engineer.</h2>
            <p class="hero-text">
                I am a motivated Data Analyst and Data Scientist with expertise in Python, Pandas, and
                Power BI. My experience includes data cleaning, manipulation, and creating interactive
                dashboards for data-driven decision-making.
            </p>
            <a href="#projects" class="button">Check out my work!</a>
        </div>
    </section>

    <section id="projects" class="projects-section">
        <div class="container">
            <h2 class="section-title">Featured Projects</h2>
            <div class="project-grid">
                <!-- Car Price Prediction Project -->
                <div class="project-item">
                    <div class="project-image">
                        <div class="placeholder-image">
                            🚗 Car Price Prediction
                        </div>
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">Car Price Prediction</h3>
                        <p class="project-description">
                            A machine learning model to predict car prices based on various features using regression techniques.
                        </p>
                        <div class="project-tech-list">
                            <span class="project-tech-item">Python</span>
                            <span class="project-tech-item">Scikit-learn</span>
                            <span class="project-tech-item">Pandas</span>
                            <span class="project-tech-item">NumPy</span>
                        </div>
                        <div class="project-links">
                            <a href="https://github.com/HaseebYousafxai/Oasis-Infobyte-tasks/blob/main/carpriceprediction.ipynb" class="project-link" target="_blank">View Source Code →</a>
                        </div>
                    </div>
                </div>

                <!-- Credit Card Fraud Detection -->
                <div class="project-item">
                    <div class="project-image">
                        <div class="placeholder-image">
                            💳 Fraud Detection
                        </div>
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">Credit Card Fraud Detection</h3>
                        <p class="project-description">
                            An advanced machine learning system to detect fraudulent credit card transactions.
                        </p>
                        <div class="project-tech-list">
                            <span class="project-tech-item">Python</span>
                            <span class="project-tech-item">TensorFlow</span>
                            <span class="project-tech-item">Scikit-learn</span>
                            <span class="project-tech-item">Pandas</span>
                        </div>
                        <div class="project-links">
                            <a href="https://github.com/HaseebYousafxai/Pinnacle_Tasks/blob/main/creditcardfraudnotebook.ipynb" class="project-link" target="_blank">View Source Code →</a>
                        </div>
                    </div>
                </div>

                <!-- University Analysis Dashboard -->
                <div class="project-item">
                    <div class="project-image">
                        <div class="placeholder-image">
                            📊 University Analysis
                        </div>
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">University Analysis Dashboard</h3>
                        <p class="project-description">
                            Interactive Power BI dashboard analyzing university data and metrics.
                        </p>
                        <div class="project-tech-list">
                            <span class="project-tech-item">Power BI</span>
                            <span class="project-tech-item">DAX</span>
                            <span class="project-tech-item">Data Modeling</span>
                        </div>
                        <div class="project-links">
                            <a href="YOUR_POWERBI_DASHBOARD_LINK" class="project-link" target="_blank">View Dashboard →</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="experience" class="work-experience">
        <div class="container">
            <h2 class="section-title">Work Experience</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3 class="project-title">Limited Structures</h3>
                    <p class="project-description">
                        Data Scientist (Nov 2024 - Present)<br>
                        • Conducted Exploratory Data Analysis (EDA)<br>
                        • Trained and integrated machine learning models<br>
                        • Collaborated with cross-functional teams
                    </p>
                    <div class="project-tech">
                        <span>Python</span>
                        <span>Machine Learning</span>
                        <span>EDA</span>
                    </div>
                </div>

                <div class="project-card">
                    <h3 class="project-title">Oasis Infobyte</h3>
                    <p class="project-description">
                        Data Scientist (Oct 2024 - Nov 2024)<br>
                        • Conducted data analysis and model development<br>
                        • Applied machine learning techniques<br>
                        • Enhanced solution effectiveness
                    </p>
                    <div class="project-tech">
                        <span>Data Analysis</span>
                        <span>Machine Learning</span>
                        <span>Python</span>
                    </div>
                </div>

                <div class="project-card">
                    <h3 class="project-title">Pinnacle Full Stack</h3>
                    <p class="project-description">
                        Data Scientist (Sept 2024 - Oct 2024)<br>
                        • Leveraged machine learning algorithms<br>
                        • Extracted insights from complex datasets<br>
                        • Enhanced product offerings
                    </p>
                    <div class="project-tech">
                        <span>Data Analysis</span>
                        <span>Machine Learning</span>
                        <span>Python</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="skills">
        <div class="container">
            <h2 class="section-title">Skills & Technologies</h2>
            <div class="skills-container">
                <div class="skill-card">Python</div>
                <div class="skill-card">Data Analysis</div>
                <div class="skill-card">Data Science</div>
                <div class="skill-card">Machine Learning Models Integration</div>
                <div class="skill-card">Design Interface For Machine Learning Models</div>
                <div class="skill-card">Data Reporting</div>
                <div class="skill-card">Data dashboards</div>
                <div class="skill-card">Problem Solving Decision Making</div>
                <div class="skill-card">AI Base Web Apps</div>
                <div class="skill-card">Project Management</div>
                <div class="skill-card">Buisiness Analysis</div>
                <div class="skill-card">Power BI</div>
                <div class="skill-card">Data Mining</div>
                <div class="skill-card">Machine Learning</div>
                <div class="skill-card">Data Visualization</div>
                <div class="skill-card">MS Excel</div>
                <div class="skill-card">SQL</div>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <p class="contact-title">What's Next?</p>
            <h2 class="contact-heading">Get In Touch</h2>
            <p class="contact-text">
                Currently looking for new opportunities. Whether you have a question or
                just want to say hi, I'll try my best to get back to you!
            </p>
            <a href="mailto:haseebyousafxai81@gmail.com" class="button">Say Hello</a>
        </div>
    </section>
</body>
</html>
