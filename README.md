<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ietheria - Contact Us</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --success-color: #27ae60;
            --error-color: #e74c3c;
            --border-radius: 8px;
            --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: #f9f9f9;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 1rem 0;
            box-shadow: var(--box-shadow);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: white;
            text-decoration: none;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }

        nav ul li a:hover {
            color: var(--secondary-color);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 4rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto;
        }

        /* Main Content */
        main {
            padding: 3rem 0;
        }

        .content-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        @media (max-width: 768px) {
            .content-grid {
                grid-template-columns: 1fr;
            }
        }

        .about-section h2,
        .contact-section h2 {
            margin-bottom: 1.5rem;
            color: var(--primary-color);
            border-bottom: 2px solid var(--secondary-color);
            padding-bottom: 0.5rem;
        }

        /* Contact Form */
        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
        }

        .form-group {
            margin-bottom: 1.5rem;
            position: relative;
        }

        .honeypot {
            position: absolute;
            left: -9999px;
        }

        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        input, textarea {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: var(--border-radius);
            font-family: inherit;
            font-size: 1rem;
            transition: var(--transition);
        }

        input:focus, textarea:focus {
            outline: none;
            border-color: var(--secondary-color);
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.2);
        }

        textarea {
            min-height: 150px;
            resize: vertical;
        }

        .required::after {
            content: " *";
            color: var(--error-color);
        }

        .btn {
            display: inline-block;
            background-color: var(--secondary-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: var(--border-radius);
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
        }

        .btn:hover {
            background-color: #2980b9;
            transform: translateY(-2px);
        }

        .btn:active {
            transform: translateY(0);
        }

        /* Messages */
        .message {
            padding: 1rem;
            border-radius: var(--border-radius);
            margin-bottom: 1.5rem;
            display: none;
        }

        .message.success {
            background-color: rgba(39, 174, 96, 0.1);
            border: 1px solid var(--success-color);
            color: var(--success-color);
        }

        .message.error {
            background-color: rgba(231, 76, 60, 0.1);
            border: 1px solid var(--error-color);
            color: var(--error-color);
        }

        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        .footer-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        @media (max-width: 768px) {
            .footer-content {
                flex-direction: column;
                gap: 1rem;
            }
        }

        .social-links a {
            color: white;
            margin-left: 1rem;
            font-size: 1.2rem;
            text-decoration: none;
        }

        .social-links a:hover {
            color: var(--secondary-color);
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="#" class="logo">Ietheria</a>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Welcome to Ietheria</h1>
            <p>We provide innovative solutions to help your business thrive in the digital age.</p>
        </div>
    </section>

    <main class="container">
        <div class="content-grid">
            <section class="about-section">
                <h2>About Ietheria</h2>
                <p>Ietheria is a forward-thinking company dedicated to delivering exceptional digital experiences and solutions. Our team of experts combines creativity with technical expertise to help businesses achieve their goals.</p>
                <p>We believe in building lasting relationships with our clients by understanding their unique needs and delivering tailored solutions that drive real results.</p>
                <h3>Our Values</h3>
                <ul>
                    <li>Innovation and Creativity</li>
                    <li>Quality and Excellence</li>
                    <li>Customer-Centric Approach</li>
                    <li>Integrity and Transparency</li>
                </ul>
            </section>

            <section class="contact-section">
                <h2>Get In Touch</h2>
                <p>Have a question or want to work with us? Fill out the form below and we'll get back to you as soon as possible.</p>
                
                <div class="contact-form">
                    <div id="message" class="message"></div>
                    
                    <form id="contactForm">
                        <!-- Honeypot fields to prevent spam -->
                        <div class="form-group honeypot">
                            <label for="username">Username</label>
                            <input type="text" id="username" name="username" autocomplete="off">
                        </div>
                        <div class="form-group honeypot">
                            <label for="password">Password</label>
                            <input type="password" id="password" name="password" autocomplete="off">
                        </div>
                        
                        <div class="form-group">
                            <label for="Name" class="required">Name</label>
                            <input type="text" id="Name" name="Name" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="Email" class="required">Email</label>
                            <input type="email" id="Email" name="Email" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="Message" class="required">Message</label>
                            <textarea id="Message" name="Message" required></textarea>
                        </div>
                        
                        <button type="submit" class="btn">Send Message</button>
                    </form>
                </div>
            </section>
        </div>
    </main>

    <footer>
        <div class="container footer-content">
            <p>&copy; 2023 Ietheria. All rights reserved.</p>
            <div class="social-links">
                <a href="#">Facebook</a>
                <a href="#">Twitter</a>
                <a href="#">LinkedIn</a>
                <a href="#">Instagram</a>
            </div>
        </div>
    </footer>

    <script>
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            
            // Show loading state
            const submitBtn = this.querySelector('button[type="submit"]');
            const originalText = submitBtn.textContent;
            submitBtn.textContent = 'Sending...';
            submitBtn.disabled = true;
            
            // Send the request to your Vercel function
            fetch('/api/contact', {  // Update this path to match your actual API endpoint
                method: 'POST',
                body: formData
            })
            .then(response => {
                if (!response.ok) {
                    throw new Error('Network response was not ok');
                }
                return response.json();
            })
            .then(data => {
                const messageEl = document.getElementById('message');
                
                if (data.ok) {
                    messageEl.textContent = 'Thank you! Your message has been sent successfully.';
                    messageEl.className = 'message success';
                    document.getElementById('contactForm').reset();
                } else {
                    throw new Error(data.error || 'Failed to send message');
                }
                
                messageEl.style.display = 'block';
            })
            .catch(error => {
                const messageEl = document.getElementById('message');
                messageEl.textContent = 'Sorry, there was an error sending your message. Please try again later.';
                messageEl.className = 'message error';
                messageEl.style.display = 'block';
                console.error('Error:', error);
            })
            .finally(() => {
                // Reset button state
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            });
        });
    </script>
</body>
</html># Ietheria
Ietheria repository
