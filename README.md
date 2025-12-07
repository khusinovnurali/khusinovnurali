<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Nurali Khusinov | Fullstack Developer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700&family=Inter:wght@400;600;700&display=swap');

    :root {
      --bg: #0d1117;
      --text: #c9d1d9;
      --accent: #58a6ff;
      --card: #161b22;
      --border: #30363d;
      --green: #238636;
      --purple: #8b46ff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'Inter', sans-serif;
      line-height: 1.6;
      padding: 40px 20px;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background-image: 
        radial-gradient(circle at 10% 20%, rgba(88, 166, 255, 0.15) 0%, transparent 20%),
        radial-gradient(circle at 90% 80%, rgba(139, 70, 255, 0.15) 0%, transparent 20%);
    }

    .container {
      max-width: 800px;
      width: 100%;
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 48px 40px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.4);
      position: relative;
      overflow: hidden;
    }

    .container::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; height: 4px;
      background: linear-gradient(90deg, #58a6ff, #8b46ff, #238636);
      border-radius: 16px 16px 0 0;
    }

    h1 {
      font-family: 'JetBrains Mono', monospace;
      font-size: 3rem;
      font-weight: 700;
      background: linear-gradient(90deg, #58a6ff, #8b46ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-align: center;
      margin-bottom: 8px;
    }

    .subtitle {
      text-align: center;
      font-size: 1.3rem;
      color: #8b949e;
      margin-bottom: 48px;
    }

    .section {
      margin-bottom: 48px;
    }

    .section h2 {
      font-family: 'JetBrains Mono', monospace;
      font-size: 1.5rem;
      margin-bottom: 20px;
      color: var(--accent);
      position: relative;
      padding-left: 20px;
    }

    .section h2::before {
      content: '';
      position: absolute;
      left: 0;
      top: 50%;
      transform: translateY(-50%);
      width: 6px;
      height: 24px;
      background: var(--accent);
      border-radius: 3px;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 16px;
    }

    .skill {
      background: rgba(88, 166, 255, 0.1);
      border: 1px solid var(--border);
      padding: 14px 16px;
      border-radius: 12px;
      text-align: center;
      font-weight: 600;
      transition: all 0.3s ease;
      cursor: default;
    }

    .skill:hover {
      transform: translateY(-6px);
      background: rgba(88, 166, 255, 0.2);
      border-color: var(--accent);
      box-shadow: 0 10px 20px rgba(88, 166, 255, 0.15);
    }

    .contact {
      display: flex;
      justify-content: center;
      gap: 24px;
      flex-wrap: wrap;
      margin-top: 40px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 14px 28px;
      background: rgba(88, 166, 255, 0.1);
      color: var(--text);
      text-decoration: none;
      border-radius: 12px;
      font-weight: 600;
      transition: all 0.4s ease;
      border: 1px solid var(--border);
    }

    .btn i { font-size: 1.4rem; }
    .btn:hover {
      background: var(--accent);
      color: white;
      transform: translateY(-4px);
      box-shadow: 0 10px 25px rgba(88, 166, 255, 0.3);
      border-color: var(--accent);
    }

    .telegram:hover { background: #229ED9; }
    .linkedin:hover { background: #0A66C2; }
    .gmail:hover { background: #EA4335; }

    @media (max-width: 600px) {
      h1 { font-size: 2.4rem; }
      .container { padding: 32px 24px; }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Nurali Khusinov</h1>
      <p class="subtitle">Fullstack Developer</p>
    </header>

    <section class="section">
      <h2>Technologies</h2>
      <div class="skills-grid">
        <!-- Backend -->
        <div class="skill">Python</div>
        <div class="skill">Flask</div>
        <div class="skill">Django</div>
        <div class="skill">C</div>
        <div class="skill">C++</div>
        
        <!-- Frontend -->
        <div class="skill">HTML5</div>
        <div class="skill">CSS3</div>
        <div class="skill">JavaScript</div>
        <div class="skill">Bootstrap</div>
        <div class="skill">Jinja2</div>
        
        <!-- DB & Tools -->
        <div class="skill">PostgreSQL</div>
        <div class="skill">MySQL</div>
        <div class="skill">SQLite</div>
        <div class="skill">Redis</div>
        <div class="skill">Docker</div>
        <div class="skill">Linux</div>
        <div class="skill">Git</div>
        <div class="skill">GitHub</div>
      </div>
    </section>

    <div class="contact">
      <a href="https://t.me/khusinov7" class="btn telegram" target="_blank">
        <i class="fab fa-telegram-plane"></i> Telegram
      </a>
      <a href="https://www.linkedin.com/in/nurali-khusinov" class="btn linkedin" target="_blank">
        <i class="fab fa-linkedin"></i> LinkedIn
      </a>
      <a href="mailto:xnurali2197@gmail.com" class="btn gmail">
        <i class="fas fa-envelope"></i> Gmail
      </a>
    </div>
  </div>
</body>
</html>
