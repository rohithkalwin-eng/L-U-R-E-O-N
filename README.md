<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>L U R E O N</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #000011, #001122);
            color: #fff;
            overflow-x: hidden;
        }
        header {
            background: rgba(0, 0, 0, 0.8);
            padding: 1rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 10;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #00aaff;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 1rem;
            margin-right: 25px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
        }
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background-image: url('https://via.placeholder.com/1920x1080/000011/ffffff?text=Space+Background'); /* Replace with real space image */
            background-size: cover;
            position: relative;
        }
        .hero h1 {
            font-size: 3rem;
            margin: 0;
        }
        .hero p {
            font-size: 1.2rem;
            margin: 1rem 0;
        }
        .btn {
            background: #00aaff;
            color: #000;
            padding: 0.5rem 1rem;
            text-decoration: none;
            border-radius: 5px;
        }
        section {
            padding: 4rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .service {
            background: rgba(255, 255, 255, 0.1);
            padding: 1rem;
            border-radius: 10px;
        }
        footer {
            background: rgba(0, 0, 0, 0.8);
            text-align: center;
            padding: 1rem;
        }
        /* Starfield animation */
        #stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        .star {
            position: absolute;
            background: #fff;
            border-radius: 50%;
            animation: twinkle 2s infinite;
        }
        @keyframes twinkle {
            0%, 100% { opacity: 0; }
            50% { opacity: 1; }
        @-webkit-keyframes twinkle {
            0% { opacity: 0.2; }
            100% { opacity: 1; }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">L U R E O N</div>
            <ul>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section class="hero">
        <div id="stars"></div>
        <div>
            <h1>Defending the Future of Space</h1>
            <p>Strategic consulting for space operations, defense, and innovation—powered by Deloitte expertise.</p>
            <a href="#contact" class="btn">Launch Inquiry</a>
        </div>
    </section>
    
    <section id="services">
        <h2>Our Services</h2>
        <div class="services">
            <div class="service">
                <h3>Space Strategy Advisory</h3>
                <p>Develop mission-critical plans for satellite deployment and orbital defense.</p>
            </div>
            <div class="service">
                <h3>Cybersecurity in Space</h3>
                <p>Protect digital assets in high-stakes environments with advanced threat analysis.</p>
            </div>
            <div class="service">
                <h3>Defense Innovation</h3>
                <p>Integrate AI and emerging tech for next-gen military applications.</p>
            </div>
        </div>
    </section>
    
    <section id="about">
        <h2>About Us</h2>
        <p>Combining Deloitte's global consulting prowess with Space Force's operational excellence, we deliver unparalleled insights for space and defense challenges.</p>
    </section>
    
    <section id="contact">
        <h2>Contact</h2>
        <form>
            <input type="text" placeholder="Name" required><br>
            <input type="email" placeholder="Email" required><br>
            <textarea placeholder="Message"></textarea><br>
            <button type="submit" class="btn">Send</button>
        </form>
    </section>
    
    <footer>
        <p>&copy; 2025 L U R E O N. All rights reserved.</p>
    </footer>
    
    <script>
        // Simple starfield generator
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 100; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = Math.random() * 100 + '%';
            star.style.top = Math.random() * 100 + '%';
            star.style.width = star.style.height = Math.random() * 3 + 'px';
            star.style.animationDelay = Math.random() * 2 + 's';
            starsContainer.appendChild(star);
        }
    </script>
</body>
</html>
