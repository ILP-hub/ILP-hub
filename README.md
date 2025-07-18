<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ILP • Junior Web & Backend Dev</title>

  <!-- Шрифт -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">

  <style>
    /* ======= Базовые переменные ======= */
    :root{
      --primary: #8b5cf6;
      --bg: #1c1917;
      --text: #ffffff;
      --card-bg: rgba(255,255,255,0.05);
    }

    /* ======= Сброс / базовые стили ======= */
    *{ box-sizing:border-box; margin:0; padding:0; }
    body{
      font-family:'Inter',sans-serif;
      background:var(--bg);
      color:var(--text);
      display:flex;
      flex-direction:column;
      align-items:center;
      padding:2.5rem 1rem;
      animation:fadeIn 0.9s ease-out both;
    }
    a{ text-decoration:none; }
    img{ display:block; max-width:100%; }

    /* ======= Анимации ======= */
    @keyframes fadeIn{
      from{opacity:0; transform:translateY(20px);}
      to  {opacity:1; transform:translateY(0);}
    }
    @keyframes float{
      0%,100%{transform:translateY(0);}
      50%    {transform:translateY(-12px);}
    }
    @keyframes pop{
      0%  {transform:scale(0.6); opacity:0;}
      60% {transform:scale(1.05); opacity:1;}
      100%{transform:scale(1);   opacity:1;}
    }

    /* ======= Шапка ======= */
    header{
      text-align:center;
      margin-bottom:3rem;
    }
    header img{
      width:72px;
      animation:float 3.8s ease-in-out infinite;
    }
    header h1{
      margin-top:1rem;
      font-size:2.6rem;
      font-weight:800;
      line-height:1.2;
    }
    header h1 span{ color:var(--primary); }

    /* ======= Блоки ======= */
    section{
      width:100%;
      max-width:960px;
      margin-bottom:3rem;
      animation:pop 0.7s cubic-bezier(.5,1.7,.3,.9) both;
    }
    section h2{
      font-size:1.6rem;
      margin-bottom:1.2rem;
      text-align:center;
      color:var(--primary);
    }

    /* ======= Список “Обо мне” ======= */
    .about ul{
      list-style:none;
      display:flex;
      flex-direction:column;
      gap:.6rem;
      padding:0 1rem;
      text-align:center;
      font-size:1.05rem;
    }
    .about b{ color:var(--primary); }

    /* ======= Скиллы ======= */
    .skills-list{
      display:flex;
      flex-wrap:wrap;
      justify-content:center;
      gap:1.2rem;
    }
    .skills-list a{
      width:64px; height:64px;
      border-radius:14px;
      background:var(--card-bg);
      display:flex; align-items:center; justify-content:center;
      transition:transform .3s, box-shadow .3s;
    }
    .skills-list a:hover{
      transform:translateY(-6px) scale(1.05) rotate(3deg);
      box-shadow:0 8px 20px -4px var(--primary);
    }

    /* ======= Статистика GitHub ======= */
    .stats{
      display:flex;
      flex-wrap:wrap;
      gap:1.5rem;
      justify-content:center;
    }
    .stats img{
      height:185px;
      border-radius:14px;
      box-shadow:0 6px 18px rgba(0,0,0,.4);
      background:#000; /* на случай, если сервис вернёт прозрачность */
    }

    /* ======= Контакты ======= */
    .contacts{
      display:flex;
      flex-wrap:wrap;
      justify-content:center;
      gap:1rem;
    }
    .contacts a{
      padding:.55rem 1rem;
      background:var(--card-bg);
      border-radius:8px;
      font-weight:600;
      transition:background .25s, transform .25s;
    }
    .contacts a:hover{
      background:var(--primary);
      transform:translateY(-3px);
    }

    /* ======= Футер ======= */
    footer{
      text-align:center;
      font-size:.9rem;
      opacity:.7;
      margin-top:.5rem;
    }
    footer a{ color:var(--primary); }
  </style>
</head>
<body>

  <!-- 👾 HEADER: приветствие -->
  <header>
    <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Alien%20Monster.png" alt="Alien Monster">
    <h1>Привет, я <span>ILP</span>!</h1>
    <p><i>Junior Web &amp; Backend Developer • Mid-level Mobile Developer</i></p>
  </header>

  <!-- 🌟 ОБО МНЕ -->
  <section class="about">
    <h2>🌟 Обо мне</h2>
    <ul>
      <li><b>🌐 Web Development:</b> Junior</li>
      <li><b>🖥️ Backend Development:</b> Junior</li>
      <li><b>📱 Mobile Development:</b> Mid-level</li>
      <li><b>🚀 Стек:</b> PHP, Python, JavaScript, Kotlin, Dart, Node.js, MySQL, MongoDB, Redis…</li>
    </ul>
  </section>

  <!-- 💻 SKILLS -->
  <section>
    <h2>💻 Skills</h2>
    <div class="skills-list">
      <!-- Первый ряд -->
      <a href="https://www.php.net/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/php-colored.svg"          alt="PHP"></a>
      <a href="https://www.python.org/"    target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg"       alt="Python"></a>
      <a href="https://developer.mozilla.org/ru/docs/Web/JavaScript" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/javascript-colored.svg" alt="JavaScript"></a>
      <a href="https://kotlinlang.org/"    target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/kotlin-colored.svg"       alt="Kotlin"></a>
      <a href="https://dart.dev/"          target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/dart-colored.svg"         alt="Dart"></a>
      <a href="https://git-scm.com/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/git-colored.svg"          alt="Git"></a>
      <a href="https://www.oracle.com/java/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/java-colored.svg"       alt="Java"></a>
      <a href="https://www.gnu.org/software/bash/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/gnubash.svg"     alt="Bash"></a>
      <a href="https://code.visualstudio.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/visualstudiocode.svg" alt="VS Code"></a>
      <a href="https://developer.mozilla.org/ru/docs/Web/HTML" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/html5-colored.svg" alt="HTML5"></a>

      <!-- Второй ряд -->
      <a href="https://reactjs.org/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/react-colored.svg"        alt="React"></a>
      <a href="https://vuejs.org/"         target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/vuejs-colored.svg"        alt="Vue.js"></a>
      <a href="https://jquery.com/"        target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/jquery-colored.svg"       alt="jQuery"></a>
      <a href="https://www.w3.org/TR/CSS/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/css3-colored.svg"         alt="CSS3"></a>
      <a href="https://tailwindcss.com/"   target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/tailwindcss-colored.svg"   alt="TailwindCSS"></a>
      <a href="https://webpack.js.org/"    target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/webpack-colored.svg"       alt="Webpack"></a>
      <a href="https://vitejs.dev/"        target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/vite-colored.svg"          alt="Vite"></a>
      <a href="https://nodejs.org/"        target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/nodejs-colored.svg"        alt="Node.js"></a>
      <a href="https://expressjs.com/"     target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/express-colored.svg"       alt="Express"></a>

      <!-- Третий ряд -->
      <a href="https://www.mongodb.com/"   target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/mongodb-colored.svg"       alt="MongoDB"></a>
      <a href="https://www.mysql.com/"     target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/mysql-colored.svg"         alt="MySQL"></a>
      <a href="https://firebase.google.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/firebase-colored.svg"    alt="Firebase"></a>
      <a href="https://supabase.io/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/supabase-colored.svg"       alt="Supabase"></a>
      <a href="https://www.figma.com/"     target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/figma-colored.svg"         alt="Figma"></a>
      <a href="https://wordpress.com/"     target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/wordpress-colored.svg"      alt="WordPress"></a>
      <a href="https://flutter.dev/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/flutter-colored.svg"        alt="Flutter"></a>
      <a href="https://laravel.com/"       target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/laravel-colored.svg"        alt="Laravel"></a>
      <a href="https://www.docker.com/"    target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/docker-colored.svg"         alt="Docker"></a>
    </div>
  </section>

  <!-- 📈 СТАТИСТИКА -->
  <section class="stats">
    <img src="https://github-readme-stats.vercel.app/api?username=ILP-hub&show_icons=true&count_private=true&title_color=a855f7&text_color=ffffff&icon_color=a855f7&bg_color=1c1917&hide_border=true" alt="GitHub Stats">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ILP-hub&langs_count=10&title_color=a855f7&text_color=ffffff&icon_color=a855f7&bg_color=1c1917&hide_border=true&custom_title=Top%20Languages" alt="Top Languages">
  </section>

  <!-- 📫 КОНТАКТЫ -->
  <section>
    <h2>📫 Со мной</h2>
    <div class="contacts">
      <a href="mailto:youremail@example.com">✉️ Email</a>
      <a href="https://www.linkedin.com/in/yourprofile" target="_blank">🔗 LinkedIn</a>
      <a href="https://t.me/yourtelegram"               target="_blank">📨 Telegram</a>
      <a href="https://github.com/ILP-hub"              target="_blank">🐙 GitHub</a>
    </div>
  </section>

  <!-- ======= ФУТЕР ======= -->
  <footer>
    Made with ❤️ by ILP • Last updated: <b>April&nbsp;23,&nbsp;2025</b>
  </footer>

</body>
</html>
