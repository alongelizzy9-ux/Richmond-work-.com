<script>
  




        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #34495e;
            --success: #27ae60;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background: var(--primary);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo-icon {
            font-size: 2rem;
            margin-right: 10px;
        }

        .logo h1 {
            font-size: 1.8rem;
            font-weight: 600;
        }

        .tagline {
            font-size: 0.9rem;
            opacity: 0.8;
            font-style: italic;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 25px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 8px 15px;
            border-radius: 4px;
        }

        nav ul li a:hover {
            background: var(--secondary);
            transform: translateY(-2px);
        }

        /* Hero Section */
        .hero {
            padding: 4rem 0;
            text-align: center;
            background: white;
            margin: 2rem 0;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .hero h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
            color: var(--dark);
        }

        .cta-button {
            display: inline-block;
            background: var(--secondary);
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(50, 50, 93, 0.11), 0 1px 3px rgba(0, 0, 0, 0.08);
        }

        .cta-button:hover {
            background: var(--primary);
            transform: translateY(-3px);
            box-shadow: 0 7px 14px rgba(50, 50, 93, 0.1), 0 3px 6px rgba(0, 0, 0, 0.08);
        }

        /* Section Styles */
        section {
            padding: 4rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: var(--primary);
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }

        .section-title h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--secondary);
            border-radius: 2px;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 3rem;
            align-items: center;
        }

        .profile-img {
            width: 100%;
            max-width: 300px;
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            border: 5px solid white;
        }

        .about-text h3 {
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .about-text p {
            margin-bottom: 1.5rem;
            color: var(--dark);
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 1.5rem;
        }

        .skill-tag {
            background: var(--light);
            color: var(--primary);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }

        .project-img {
            height: 200px;
            background: var(--light);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            color: var(--secondary);
        }

        .project-content {
            padding: 1.5rem;
        }

        .project-content h3 {
            font-size: 1.4rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .project-content p {
            color: var(--dark);
            margin-bottom: 1rem;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 1rem;
        }

        .tech-tag {
            background: rgba(52, 152, 219, 0.1);
            color: var(--secondary);
            padding: 4px 10px;
            border-radius: 4px;
            font-size: 0.8rem;
        }

        .project-links {
            display: flex;
            gap: 10px;
        }

        .project-link {
            text-decoration: none;
            color: var(--secondary);
            font-weight: 500;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            transition: all 0.3s ease;
        }

        .project-link:hover {
            color: var(--accent);
        }

        /* Learning Journey */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline::after {
            content: '';
            position: absolute;
            width: 6px;
            background: var(--secondary);
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -3px;
            border-radius: 3px;
        }

        .timeline-item {
            padding: 10px 40px;
            position: relative;
            background: inherit;
            width: 50%;
        }

        .timeline-item::after {
            content: '';
            position: absolute;
            width: 25px;
            height: 25px;
            right: -12px;
            background: white;
            border: 4px solid var(--secondary);
            top: 15px;
            border-radius: 50%;
            z-index: 1;
        }

        .left {
            left: 0;
        }

        .right {
            left: 50%;
        }

        .left::before {
            content: " ";
            height: 0;
            position: absolute;
            top: 22px;
            width: 0;
            z-index: 1;
            right: 30px;
            border: medium solid white;
            border-width: 10px 0 10px 10px;
            border-color: transparent transparent transparent white;
        }

        .right::before {
            content: " ";
            height: 0;
            position: absolute;
            top: 22px;
            width: 0;
            z-index: 1;
            left: 30px;
            border: medium solid white;
            border-width: 10px 10px 10px 0;
            border-color: transparent white transparent transparent;
        }

        .right::after {
            left: -12px;
        }

        .timeline-content {
            padding: 20px 30px;
            background: white;
            position: relative;
            border-radius: 6px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
        }

        .timeline-date {
            color: var(--secondary);
            font-weight: 600;
            margin-bottom: 5px;
        }

        /* Contact Section */
        .contact-content {
            max-width: 700px;
            margin: 0 auto;
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .contact-form {
            display: grid;
            gap: 1.5rem;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group label {
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--primary);
        }

        .form-group input,
        .form-group textarea {
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-family: inherit;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--secondary);
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.2);
        }

        .form-group textarea {
            min-height: 150px;
            resize: vertical;
        }

        .submit-btn {
            background: var(--secondary);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 6px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            justify-self: center;
        }

        .submit-btn:hover {
            background: var(--primary);
            transform: translateY(-2px);
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: white;
            padding: 3rem 0 2rem;
            text-align: center;
        }

        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .social-links {
            display: flex;
            gap: 20px;
            margin-bottom: 1.5rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            color: var(--secondary);
            transform: translateY(-3px);
        }

        .copyright {
            font-size: 0.9rem;
            opacity: 0.7;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                margin-top: 1rem;
            }

            nav ul li {
                margin: 0 10px;
            }

            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .timeline::after {
                left: 31px;
            }

            .timeline-item {
                width: 100%;
                padding-left: 70px;
                padding-right: 25px;
            }

            .timeline-item::before {
                left: 60px;
                border: medium solid white;
                border-width: 10px 10px 10px 0;
                border-color: transparent white transparent transparent;
            }

            .left::after, .right::after {
                left: 18px;
            }

            .right {
                left: 0%;
            }
        }
</script>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="">
    <title>Richmond's Dev Journey | Web Developer in Training</title>
    <link rel="stylesheet" href="style.css">

</head>
<body>
    <header>
        <div class="container header-content">
            <div class="logo">
                <div class="logo-icon">👨‍💻</div>
                <div>
                    <h1>Richmond's Dev Journey</h1>
                    <div class="tagline">12-year-old Web Developer in Training</div>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#journey">My Journey</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h2>Welcome to My Developer Portfolio</h2>
            <p>I'm Richmond, a 12-year-old passionate about learning web development. This is where I document my coding journey and share my projects as I grow my skills.</p>
            <a href="#projects" class="cta-button">View My Projects</a>
        </div>
    </section>

    <section id="about" class="container">
        <div class="section-title">
            <h2>About Me</h2>
        </div>
        <div class="about-content">
            <img src="https://via.placeholder.com/300" alt="Richmond's Photo" class="profile-img">
            <div class="about-text">
                <h3>Hi, I'm Richmond! 👋</h3>
                <p>I'm a 12-year-old student who discovered the amazing world of web development about 2 years ago. What started as curiosity has quickly become a passion!</p>
                <p>When I'm not coding or studying, I enjoy playing soccer, reading science fiction, and experimenting with robotics. I believe technology can solve real-world problems and I want to be part of that solution.</p>
                <p>My goal is to become a full-stack developer by the time I'm 16. I know it's ambitious, but I'm committed to learning something new every day!</p>
                <div class="skills">
                    <div class="skill-tag">HTML5</div>
                    <div class="skill-tag">CSS3</div>
                    <div class="skill-tag">JavaScript (Beginner)</div>
 
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="container">
        <div class="section-title">
            <h2>My Projects</h2>
        </div>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-img">📝</div>
                <div class="project-content">
                    <h3>Todo List App</h3>
                    <p>My first JavaScript project! A simple todo list application with local storage to save tasks.</p>
                    <div class="project-tech">
                        <span class="tech-tag">HTML</span>
                        <span class="tech-tag">CSS</span>
                        <span class="tech-tag">JavaScript</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">🔗 Live Demo</a>
                        <a href="#" class="project-link">💻 Code</a>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-img">🍝</div>
                <div class="project-content">
                    <h3>Restaurant websites</h3>
                    <p>Create a modern resturant website for restaurant business </p>
                    <div class="project-tech">
                        <span class="tech-tag">HTML</span>
                        <span class="tech-tag">CSS</span>
                        <span class="tech-tag">JavaScript</span>

                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">🔗 Live Demo</a>
                        <a href="#" class="project-link">💻 Code</a>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-img">🎮</div>
                <div class="project-content">
                    <h3>Memory Card Game</h3>
                    <p>A fun memory matching game built with JavaScript. Features timer and move counter.</p>
                    <div class="project-tech">
                        <span class="tech-tag">HTML</span>
                        <span class="tech-tag">CSS</span>
                        <span class="tech-tag">JavaScript</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">🔗 Live Demo</a>
                        <a href="#" class="project-link">💻 Code</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="journey" class="container">
        <div class="section-title">
            <h2>My Learning Journey</h2>
        </div>
        <div class="timeline">
            <div class="timeline-item left">
                <div class="timeline-content">
                    <div class="timeline-date">August 2023</div>
                    <h3>First HTML Page</h3>
                    <p>Created my first "DAN RICH" webpage. Learned basic HTML structure and tags.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <div class="timeline-date">October 2023</div>
                    <h3>CSS Styling</h3>
                    <p>Discovered the power of CSS. Made my first colorful, styled website about my favorite video games.</p>
                </div>
            </div>
            
            <div class="timeline-item left">
                <div class="timeline-content">
                    <div class="timeline-date">November 2023</div>
                    <h3>JavaScript Basics</h3>
                    <p>Started learning JavaScript. Built a simple calculator and understood variables and functions.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <div class="timeline-date">November 2023</div>
                    <h3>First Real Project</h3>
                    <p>Created my Website Learned about Html css and java script.</p>
                </div>
            </div>
            
            
 
            </div>
        </div>
    </section>

    <section id="contact" class="container">
        <div class="section-title">
            <h2>Get In Touch</h2>
        </div>
        <div class="contact-content">
            <p>Have a question or want to collaborate on a project? I'd love to hear from you!</p>
            <form class="contact-form" onsubmit="handleSubmit(event)">
                <div class="form-group">
                    <label for="name">Your Name</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email Address</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="message">Your Message</label>
                    <textarea id="message" name="message" required></textarea>
                </div>
                <button type="submit" class="submit-btn">Send Message</button>
            </form>
            <div id="form-message" style="margin-top: 1rem; text-align: center; display: none;"></div>
        </div>
    </section>

    <footer>
        <div class="container footer-content">
            <div class="social-links">
                <a href="#" title="GitHub">🐙</a>
                <a href="#" title="CodePen">🖊️</a>
                <a href="#" title="LinkedIn">👔</a>
            </div>
            <p class="copyright">&copy; 2023 Richmond's Dev Journey. All rights reserved.</p>
            <p class="copyright">Designed and coded with ❤️ by a 12-year-old developer</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Form submission handler
        function handleSubmit(event) {
            event.preventDefault();
            
            // Get form values
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;
            
            // Display success message
            const formMessage = document.getElementById('form-message');
            formMessage.innerHTML = `
                <div style="background: #d4edda; color: #155724; padding: 15px; border-radius: 6px; border-left: 4px solid #28a745;">
                    <strong>Thanks ${name}!</strong> I've received your message and will get back to you soon. 
                    Since I'm still learning, this form doesn't actually send emails yet, but I appreciate your message! 😊
                </div>
            `;
            formMessage.style.display = 'block';
            
            // Reset form
            document.getElementById('name').value = '';
            document.getElementById('email').value = '';
            document.getElementById('message').value = '';
            
            // Scroll to message
            formMessage.scrollIntoView({ behavior: 'smooth', block: 'center' });
        }

        // Add animation to project cards on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.project-card').forEach(card => {
            card.style.opacity = 0;
            card.style.transform = 'translateY(20px)';
            card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(card);
        });
    </script>
</body>
</html>
