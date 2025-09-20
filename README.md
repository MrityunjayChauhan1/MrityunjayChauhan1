<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mrityunjay Chauhan - Portfolio</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #0d1117;
            color: #c9d1d9;
            margin: 0;
            padding: 20px;
            line-height: 1.6;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        .header {
            text-align: center;
            margin-bottom: 30px;
        }
        .typing-animation {
            font-family: 'Fira Code', monospace;
            font-size: 28px;
            margin-bottom: 20px;
        }
        .gif-container {
            text-align: center;
            margin: 30px 0;
        }
        .section {
            margin: 40px 0;
            padding: 20px;
            border-radius: 10px;
            background: linear-gradient(135deg, #161b22, #0d1117);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .section-title {
            text-align: center;
            margin-bottom: 20px;
            color: #58a6ff;
            font-size: 24px;
        }
        .skills-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            padding: 15px;
        }
        .skill-badge {
            padding: 10px 15px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            gap: 8px;
            font-weight: 600;
        }
        .stats-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }
        .stat-box {
            background: #161b22;
            border-radius: 10px;
            padding: 15px;
            min-width: 250px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }
        .social-btn {
            padding: 12px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: transform 0.3s;
        }
        .social-btn:hover {
            transform: translateY(-3px);
        }
        .divider {
            height: 3px;
            background: linear-gradient(90deg, #ff6ec4, #7873f5, #00c6ff, #f7971e);
            border-radius: 3px;
            margin: 30px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Typing Animation -->
        <div class="header">
            <div class="typing-animation">
                Hi, I'm Mrityunjay Chauhan 👋<br>
                Java Full Stack Developer 💻<br>
                MCA Student 🎓<br>
                UI & Backend Specialist 🚀
            </div>
        </div>

        <!-- Developer GIF -->
        <div class="gif-container">
            <img src="https://i.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.webp" width="500" alt="Developer Animation">
        </div>

        <div class="divider"></div>

        <!-- UI / Frontend -->
        <div class="section">
            <h2 class="section-title">🎨 UI / Frontend</h2>
            <div class="skills-container">
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">React</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">JavaScript</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">HTML</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">CSS</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">Bootstrap</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff6ec4, #7873f5);">Tailwind</div>
            </div>
        </div>

        <div class="divider"></div>

        <!-- Backend -->
        <div class="section">
            <h2 class="section-title">🖥️ Backend</h2>
            <div class="skills-container">
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff9966, #ff5e62);">Java</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff9966, #ff5e62);">Spring</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #ff9966, #ff5e62);">Maven</div>
            </div>
        </div>

        <div class="divider"></div>

        <!-- Databases -->
        <div class="section">
            <h2 class="section-title">🗄️ Databases</h2>
            <div class="skills-container">
                <div class="skill-badge" style="background: linear-gradient(135deg, #00c6ff, #0072ff);">MySQL</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #00c6ff, #0072ff);">Oracle</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #00c6ff, #0072ff);">MongoDB</div>
            </div>
        </div>

        <div class="divider"></div>

        <!-- Tools & Others -->
        <div class="section">
            <h2 class="section-title">⚙️ Tools & Others</h2>
            <div class="skills-container">
                <div class="skill-badge" style="background: linear-gradient(135deg, #f7971e, #ffd200);">Git</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #f7971e, #ffd200);">GitHub</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #f7971e, #ffd200);">VS Code</div>
                <div class="skill-badge" style="background: linear-gradient(135deg, #f7971e, #ffd200);">Postman</div>
            </div>
        </div>

        <div class="divider"></div>

        <!-- GitHub Stats -->
        <h2 class="section-title">📊 GitHub Stats</h2>
        <div class="stats-container">
            <div class="stat-box">
                <img src="https://github-readme-stats.vercel.app/api?username=MrityunjayChauhan1&show_icons=true&theme=dark&hide_border=true" alt="GitHub Stats">
            </div>
            <div class="stat-box">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=MrityunjayChauhan1&theme=dark&hide_border=true" alt="GitHub Streak">
            </div>
        </div>

        <div class="divider"></div>

        <!-- Connect With Me -->
        <h2 class="section-title">🌐 Connect With Me</h2>
        <div class="social-links">
            <a href="https://www.linkedin.com/in/mrityunjay-chauhan-" class="social-btn" style="background-color: #0A66C2; color: white;">
                LinkedIn
            </a>
            <a href="mailto:msdchauhan1@gmail.com" class="social-btn" style="background-color: #EA4335; color: white;">
                Gmail
            </a>
        </div>
    </div>
</body>
</html>
