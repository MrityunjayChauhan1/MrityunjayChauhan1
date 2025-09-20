<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mrityunjay Chauhan - Java Full Stack Developer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #0a192f 0%, #172a45 100%);
            color: #e6f1ff;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            text-align: center;
            padding: 60px 0 30px;
            position: relative;
            overflow: hidden;
        }
        
        .gif-container {
            margin: 0 auto 30px;
            width: 300px;
            height: 200px;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 247, 255, 0.2);
            transition: transform 0.5s;
            position: relative;
        }
        
        .gif-container:hover {
            transform: scale(1.05);
        }
        
        .gif-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            background: linear-gradient(90deg, #00FFAA 0%, #00D4FF 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .typing-text {
            font-family: 'Fira Code', monospace;
            font-size: 1.8rem;
            margin: 20px 0;
            min-height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .typing-text span {
            display: inline-block;
            overflow: hidden;
            border-right: 3px solid #00FFAA;
            white-space: nowrap;
            animation: typing 4s steps(30, end) infinite, blink 0.8s infinite;
        }
        
        @keyframes typing {
            0% { width: 0; }
            50% { width: 100%; }
            90% { width: 100%; }
            100% { width: 0; }
        }
        
        @keyframes blink {
            from, to { border-color: transparent; }
            50% { border-color: #00FFAA; }
        }
        
        .divider {
            height: 3px;
            background: linear-gradient(90deg, transparent, #00FFAA, transparent);
            margin: 40px auto;
            width: 80%;
            border-radius: 50%;
        }
        
        .section-title {
            text-align: center;
            font-size: 2rem;
            margin: 40px 0 30px;
            color: #00FFAA;
            position: relative;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, transparent, #00FFAA, transparent);
            border-radius: 50%;
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
        }
        
        .skill-card {
            background: rgba(27, 31, 59, 0.8);
            border-radius: 15px;
            padding: 20px;
            width: 280px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .skill-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 255, 170, 0.2);
        }
        
        .skill-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #00D4FF;
        }
        
        .skill-icons {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin-top: 15px;
        }
        
        .skill-icon {
            font-size: 2.5rem;
            transition: transform 0.3s;
            display: flex;
            justify-content: center;
            align-items: center;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: rgba(0, 212, 255, 0.1);
        }
        
        .skill-icon:hover {
            transform: scale(1.2);
        }
        
        .skill-icon i {
            background: linear-gradient(135deg, #00FFAA 0%, #00D4FF 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stats-container {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 40px 0;
            flex-wrap: wrap;
        }
        
        .stat-item {
            text-align: center;
            background: rgba(27, 31, 59, 0.8);
            padding: 20px;
            border-radius: 15px;
            width: 280px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s;
        }
        
        .stat-item:hover {
            transform: scale(1.05);
        }
        
        .snake-container {
            margin: 40px auto;
            width: 100%;
            max-width: 800px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 255, 170, 0.2);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
        }
        
        .social-link {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(135deg, #00FFAA 0%, #00D4FF 100%);
            color: #0a192f;
            font-size: 1.5rem;
            text-decoration: none;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .social-link:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 255, 170, 0.4);
        }
        
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 40px;
            background: rgba(10, 25, 47, 0.8);
            border-top: 1px solid rgba(0, 255, 170, 0.2);
        }
        
        .particles-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            .typing-text {
                font-size: 1.4rem;
            }
            
            .skill-card, .stat-item {
                width: 100%;
                max-width: 320px;
            }
            
            .stats-container {
                gap: 15px;
            }
        }
    </style>
</head>
<body>
    <div class="particles-container" id="particles"></div>
    
    <div class="container">
        <header>
            <div class="gif-container">
                <img src="https://media.giphy.com/media/3o7TKy0F2Aj8N2YQJy/giphy.gif" alt="Night Coding Animation">
            </div>
            
            <h1>Mrityunjay Chauhan</h1>
            
            <div class="typing-text">
                <span id="typing"></span>
            </div>
        </header>
        
        <div class="divider"></div>
        
        <h2 class="section-title">🎨 UI / Frontend</h2>
        <div class="skills-container">
            <div class="skill-card">
                <h3>Frontend Technologies</h3>
                <div class="skill-icons">
                    <div class="skill-icon"><i class="fab fa-react"></i></div>
                    <div class="skill-icon"><i class="fab fa-js"></i></div>
                    <div class="skill-icon"><i class="fab fa-html5"></i></div>
                    <div class="skill-icon"><i class="fab fa-css3-alt"></i></div>
                    <div class="skill-icon"><i class="fab fa-bootstrap"></i></div>
                </div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">🖥️ Backend</h2>
        <div class="skills-container">
            <div class="skill-card">
                <h3>Backend Technologies</h3>
                <div class="skill-icons">
                    <div class="skill-icon"><i class="fab fa-java"></i></div>
                    <div class="skill-icon"><i class="fas fa-leaf"></i></div>
                    <div class="skill-icon"><i class="fas fa-cube"></i></div>
                </div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">🗄️ Databases</h2>
        <div class="skills-container">
            <div class="skill-card">
                <h3>Databases</h3>
                <div class="skill-icons">
                    <div class="skill-icon"><i class="fas fa-database"></i></div>
                    <div class="skill-icon"><i class="fas fa-server"></i></div>
                    <div class="skill-icon"><i class="fas fa-dharmachakra"></i></div>
                </div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">⚙️ Tools & Others</h2>
        <div class="skills-container">
            <div class="skill-card">
                <h3>Tools & Technologies</h3>
                <div class="skill-icons">
                    <div class="skill-icon"><i class="fab fa-git"></i></div>
                    <div class="skill-icon"><i class="fab fa-github"></i></div>
                    <div class="skill-icon"><i class="fas fa-code"></i></div>
                    <div class="skill-icon"><i class="fas fa-paper-plane"></i></div>
                </div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">📊 GitHub Stats</h2>
        <div class="stats-container">
            <div class="stat-item">
                <img src="https://github-readme-stats.vercel.app/api?username=MrityunjayChauhan1&show_icons=true&theme=dark&hide_border=true" alt="GitHub Stats">
            </div>
            <div class="stat-item">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=MrityunjayChauhan1&theme=dark&hide_border=true" alt="GitHub Streak">
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">🐍 Contribution Animation</h2>
        <div class="snake-container">
            <img src="https://raw.githubusercontent.com/MrityunjayChauhan1/MrityunjayChauhan1/output/github-contribution-grid-snake.svg" alt="Contribution Snake" style="width: 100%;">
        </div>
        
        <div class="divider"></div>
        
        <h2 class="section-title">🌐 Connect With Me</h2>
        <div class="social-links">
            <a href="https://www.linkedin.com/in/mrityunjay-chauhan-" class="social-link">
                <i class="fab fa-linkedin-in"></i>
            </a>
            <a href="mailto:msdchauhan1@gmail.com" class="social-link">
                <i class="far fa-envelope"></i>
            </a>
            <a href="https://github.com/MrityunjayChauhan1" class="social-link">
                <i class="fab fa-github"></i>
            </a>
        </div>
    </div>
    
    <footer>
        <p>© 2023 Mrityunjay Chauhan | Java Full Stack Developer</p>
    </footer>

    <script>
        // Typing animation
        const texts = [
            "Hi, I'm Mrityunjay Chauhan 👋",
            "Java Full Stack Developer 💻",
            "MCA Student 🎓",
            "UI & Backend Specialist 🚀"
        ];
        let textIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        let typingDelay = 100;
        let deletingDelay = 50;
        let pauseDelay = 1500;
        
        function type() {
            const currentText = texts[textIndex];
            const typingElement = document.getElementById('typing');
            
            if (isDeleting) {
                typingElement.textContent = currentText.substring(0, charIndex - 1);
                charIndex--;
                typingDelay = deletingDelay;
            } else {
                typingElement.textContent = currentText.substring(0, charIndex + 1);
                charIndex++;
                typingDelay = 100;
            }
            
            if (!isDeleting && charIndex === currentText.length) {
                typingDelay = pauseDelay;
                isDeleting = true;
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                textIndex = (textIndex + 1) % texts.length;
                typingDelay = 500;
            }
            
            setTimeout(type, typingDelay);
        }
        
        document.addEventListener('DOMContentLoaded', type);
        
        // Particle animation
        function initParticles() {
            const container = document.getElementById('particles');
            const canvasWidth = container.clientWidth;
            const canvasHeight = container.clientHeight;
            
            const scene = new THREE.Scene();
            const camera = new THREE.PerspectiveCamera(75, canvasWidth / canvasHeight, 0.1, 1000);
            const renderer = new THREE.WebGLRenderer({ alpha: true });
            renderer.setSize(canvasWidth, canvasHeight);
            container.appendChild(renderer.domElement);
            
            const particles = new THREE.BufferGeometry();
            const particleCount = 1000;
            
            const posArray = new Float32Array(particleCount * 3);
            const colorArray = new Float32Array(particleCount * 3);
            
            for (let i = 0; i < particleCount * 3; i++) {
                posArray[i] = (Math.random() - 0.5) * 10;
                colorArray[i] = Math.random();
            }
            
            particles.setAttribute('position', new THREE.BufferAttribute(posArray, 3));
            particles.setAttribute('color', new THREE.BufferAttribute(colorArray, 3));
            
            const particleMaterial = new THREE.PointsMaterial({
                size: 0.02,
                vertexColors: true,
                transparent: true,
                opacity: 0.6
            });
            
            const particleSystem = new THREE.Points(particles, particleMaterial);
            scene.add(particleSystem);
            
            camera.position.z = 2;
            
            function animate() {
                requestAnimationFrame(animate);
                
                particleSystem.rotation.x += 0.001;
                particleSystem.rotation.y += 0.001;
                
                renderer.render(scene, camera);
            }
            
            animate();
            
            window.addEventListener('resize', () => {
                const newWidth = container.clientWidth;
                const newHeight = container.clientHeight;
                camera.aspect = newWidth / newHeight;
                camera.updateProjectionMatrix();
                renderer.setSize(newWidth, newHeight);
            });
        }
        
        initParticles();
    </script>
</body>
</html>
