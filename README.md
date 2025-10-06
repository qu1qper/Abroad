# Abroad
Code for write ur resume to university 

 HTML(index.html)
<!doctype html>
<html lang="ru">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Жума Am — Portfolio</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
<header class="header">
  <div class="container">
    <h1 class="brand">Жума <span>Am</span></h1>
    <nav class="nav">
      <a href="#about">Обо мне</a>
      <a href="#projects">Проекты</a>
      <a href="#contact">Контакты</a>
    </nav>
    <button class="burger" id="burger" aria-label="menu">☰</button>
  </div>
</header>

<section class="hero">
  <div class="container hero-inner">
    <div class="left">
      <h2>Привет — я <span class="accent">разработчик</span> и спортсмен</h2>
      <p class="lead">Я создаю проекты: боты, визуализаторы и умные веб-приложения. IELTS 7.5. Бокс — моя дисциплина.</p>
      <div class="cta">
        <a href="#projects" class="btn">Мои проекты</a>
        <a href="#contact" class="btn ghost">Связаться</a>
      </div>
      <div class="skills">
        <span>Python</span><span>JavaScript</span><span>Flask</span><span>aiogram</span><span>SQL</span>
      </div>
    </div>
    <div class="right card">
      <div class="avatar-wrap">
        <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?w=800&q=60" alt="avatar" class="avatar" />
      </div>
      <div class="stats">
        <div><strong>14</strong><span>лет</span></div>
        <div><strong>IELTS</strong><span>7.5</span></div>
        <div><strong>Box</strong><span>ежедневно</span></div>
      </div>
    </div>
  </div>
</section>

<main class="container main">
  <section id="projects" class="projects">
    <h3>Ключевые проекты</h3>
    <div class="grid">
      <article class="proj card">
        <h4>MathBase</h4>
        <p>Полнофункциональный сайт формул — LaTeX + поиск + Flask API + SQLite.</p>
        <a class="link" href="../mathbase">Код</a>
      </article>

      <article class="proj card">
        <h4>Snake Bot</h4>
        <p>Интерактивная змейка прямо в Telegram (inline-кнопки).</p>
        <a class="link" href="../tg-snake">Код</a>
      </article>

      <article class="proj card">
        <h4>Algo Visualizer</h4>
        <p>Визуализатор сортировок с canvas и шагами анимации.</p>
        <a class="link" href="../alg-visual">Демо</a>
      </article>
    </div>
  </section>

  <section id="about" class="about card">
    <h3>Обо мне</h3>
    <p>Учусь, кодю и тренируюсь. Люблю решать алгоритмические задачи и делать проекты, которые помогают людям учиться быстрее.</p>
  </section>

  <section id="contact" class="contact card">
    <h3>Контакты</h3>
    <p>Email: <a href="mailto:you@example.com">you@example.com</a></p>
    <p>GitHub: <a href="https://github.com/yourname">github.com/yourname</a></p>
  </section>
</main>

<footer class="footer">© <span id="year"></span> Жума Am</footer>

<script src="script.js"></script>
</body>
</html>

CSS (style.css)

:root{
  --bg:#081022; --card:#0d1726; --accent:#6ee7b7; --muted:#9fb0bf;
  font-family:Inter,system-ui,Arial; color-scheme: dark;
}
*{box-sizing:border-box}
body{margin:0;background:linear-gradient(180deg,#021124 0%,#07142a 100%); color:#eaf6f1; -webkit-font-smoothing:antialiased}
.container{max-width:1100px;margin:0 auto;padding:28px}
.header{position:sticky;top:0;z-index:20;backdrop-filter:blur(6px);padding:10px 0}
.brand{display:inline;font-weight:800}
.brand span{color:var(--accent)}
.nav{float:right}
.nav a{color:var(--muted);margin-left:20px;text-decoration:none}
.burger{display:none;background:transparent;border:0;color:var(--muted);font-size:22px}
.hero{padding:48px 0}
.hero-inner{display:flex;gap:24px;align-items:center}
.left{flex:1}
.lead{color:var(--muted);max-width:60ch}
.accent{color:var(--accent)}
.
