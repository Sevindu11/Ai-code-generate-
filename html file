<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nexus - Digital Innovation Hub</title>
    <link rel="stylesheet" href="style.css">
    
</head>
<body>
    <!-- Animated background particles -->
    <div class="particles" id="particles"></div>

    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <div class="logo">ST Photo Editor </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
       
        <div class="hero-content">
            <h1>Welcome to the Future</h1>
              <h1>UI/UX DESIGNER </h1>
            <p>Experience cutting-edge digital innovation with stunning visuals and seamless interactions that push the boundaries of web design.</p>
            <a href="#features" class="cta-button">Explore Now</a>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="features-grid">
            <div class="feature-card fade-in">
                <div class="feature-icon">🚀</div>
                <h3>Lightning Fast</h3>
                <p>Optimized performance with cutting-edge technology ensuring blazing fast load times and smooth interactions.</p>
            </div>
            <div class="feature-card fade-in">
                <div class="feature-icon">🎨</div>
                <h3>Stunning Design</h3>
                <p>Modern, responsive design with beautiful animations and visual effects that captivate your audience.</p>
            </div>
            <div class="feature-card fade-in">
                <div class="feature-icon">⚡</div>
                <h3>Dynamic Effects</h3>
                <p>Interactive elements and smooth animations that create an engaging and memorable user experience.</p>
            </div>
             <div class="feature-card fade-in">
                <div class="feature-icon">⚡</div>
                <h3>Dynamic Effects</h3>
                <p>Interactive elements and smooth animations that create an engaging and memorable user experience.</p>
            </div>
        </div>
    </section>

    <!-- Card section-->
    <section>
        <div class="card">
            <div class="card-info">
                <p class="title">Magic Card</p>
            </div>
        </div>

    </section>


    <script>
        // Create floating particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;

            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDelay = Math.random() * 20 + 's';
                particle.style.animationDuration = (Math.random() * 10 + 10) + 's';
                particlesContainer.appendChild(particle);
            }
        }

        // Scroll animations
        function handleScrollAnimations() {
            const elements = document.querySelectorAll('.fade-in');
            elements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('visible');
                }
            });
        }

        // Smooth scrolling for navigation links
        function smoothScroll() {
            const links = document.querySelectorAll('a[href^="#"]');
            links.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                });
            });
        }

        // Navigation background on scroll
        function handleNavScroll() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.style.background = 'rgba(0, 0, 0, 0.3)';
            } else {
                nav.style.background = 'rgba(0, 0, 0, 0.1)';
            }
        }

        // Initialize everything
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            smoothScroll();
            handleScrollAnimations();
        });

        // Event listeners
        window.addEventListener('scroll', function() {
            handleScrollAnimations();
            handleNavScroll();
        });

        // Add hover effects to hero elements
        const heroContent = document.querySelector('.hero-content');
        heroContent.addEventListener('mousemove', function(e) {
            const rect = heroContent.getBoundingClientRect();
            const x = e.clientX - rect.left;
            const y = e.clientY - rect.top;
            
            const moveX = (x / rect.width - 0.5) * 20;
            const moveY = (y / rect.height - 0.5) * 20;
            
            heroContent.style.transform = `translate(${moveX}px, ${moveY}px)`;
        });

        heroContent.addEventListener('mouseleave', function() {
            heroContent.style.transform = 'translate(0, 0)';
        });
    </script>
</body>
</html>
