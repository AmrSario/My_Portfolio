<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Amr Mohamed - Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-color: #f8f9fa;
      --text-color: #222;
      --section-bg: #ffffff;
      --accent-color: #0077cc;
      --header-bg: linear-gradient(to right, #6dd5ed, #2193b0);
      --footer-color: #888;
      --btn-bg: linear-gradient(to right, #25D366, #128C7E);
    }

    body.dark-mode {
      --bg-color: #121212;
      --text-color: #e4e4e4;
      --section-bg: #1e1e1e;
      --accent-color: #66b2ff;
      --header-bg: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      --footer-color: #aaa;
      --btn-bg: linear-gradient(to right, #128C7E, #075E54);
    }

    * {
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: var(--bg-color);
      color: var(--text-color);
      line-height: 1.6;
      overflow-x: hidden;
      transition: background 0.4s, color 0.4s;
    }

    header {
      background: var(--header-bg);
      padding: 80px 20px 50px;
      text-align: center;
      color: #fff;
      animation: fadeInDown 1.5s ease-in-out;
      position: relative;
    }

    header h1 {
      margin: 0;
      font-size: 3em;
      letter-spacing: 1px;
      animation: slideInLeft 1s ease-out;
    }

    header p {
      font-size: 1.2em;
      margin-top: 12px;
      animation: slideInRight 1s ease-out;
    }

    #mode-toggle {
      position: absolute;
      top: 20px;
      right: 20px;
      background: none;
      border: 2px solid #fff;
      border-radius: 30px;
      color: #fff;
      font-size: 1em;
      padding: 6px 14px;
      cursor: pointer;
      transition: background 0.3s, color 0.3s;
    }

    #mode-toggle:hover {
      background: rgba(255, 255, 255, 0.15);
    }

    section {
      max-width: 1000px;
      margin: 50px auto;
      background: var(--section-bg);
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease, background 0.4s;
      animation: fadeUp 1.2s ease-in-out;
    }

    section:hover {
      transform: translateY(-6px);
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.15);
    }

    h2 {
      color: var(--accent-color);
      border-left: 5px solid var(--accent-color);
      padding-left: 12px;
      margin-bottom: 20px;
      font-size: 1.8em;
      animation: bounceIn 1.4s;
    }

    ul {
      padding-left: 20px;
    }

    ul li {
      margin-bottom: 10px;
      position: relative;
      padding-left: 15px;
      animation: fadeInLeft 1s;
    }

    ul li::before {
      content: "✔";
      position: absolute;
      left: 0;
      color: #00aa66;
    }

    .contact {
      font-size: 1.1em;
      margin-top: 20px;
    }

    .whatsapp-btn {
      display: inline-block;
      background: var(--btn-bg);
      color: white;
      padding: 14px 24px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.05em;
      margin-top: 20px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.2);
      transition: all 0.3s ease;
      animation: pulse 2s infinite;
    }

    .whatsapp-btn:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 20px rgba(0,0,0,0.25);
    }

    footer {
      text-align: center;
      margin: 60px 0 30px;
      color: var(--footer-color);
      font-size: 0.95em;
      animation: fadeIn 2s;
    }

    @keyframes fadeInDown {
      from {opacity: 0; transform: translateY(-30px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @keyframes fadeUp {
      from {opacity: 0; transform: translateY(40px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @keyframes slideInLeft {
      from {opacity: 0; transform: translateX(-50px);}
      to {opacity: 1; transform: translateX(0);}
    }

    @keyframes slideInRight {
      from {opacity: 0; transform: translateX(50px);}
      to {opacity: 1; transform: translateX(0);}
    }

    @keyframes bounceIn {
      0% {transform: scale(0.5); opacity: 0;}
      60% {transform: scale(1.2); opacity: 1;}
      100% {transform: scale(1);}
    }

    @keyframes fadeInLeft {
      from {opacity: 0; transform: translateX(-20px);}
      to {opacity: 1; transform: translateX(0);}
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }

    @keyframes pulse {
      0%, 100% {transform: scale(1);}
      50% {transform: scale(1.05);}
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2em;
      }

      section {
        padding: 25px;
        margin: 30px 15px;
      }

      .whatsapp-btn {
        font-size: 0.95em;
        padding: 10px 18px;
      }
    }
  </style>
</head>
<body>
  <header>
    <button id="mode-toggle">🌙</button>
    <h1>Amr Mohamed Shaaban</h1>
    <p>High School Student from Egypt | Graphic Designer & Translator</p>
  </header>

  <section>
    <h2>About Me</h2>
    <p>I’m a dedicated high school student from Egypt, passionate about graphic design and languages. I create all kinds of static graphic designs with top quality and creativity. Please note that I do not offer motion graphics or video editing services. In addition, I work as a full professional translator with high accuracy and attention to detail.</p>
  </section>

  <section>
    <h2>Design Software I Use</h2>
    <ul>
      <li>Adobe Photoshop</li>
      <li>Adobe Illustrator</li>
      <li>Adobe After Effects</li>
      <li>AI-based Design Tools</li>
    </ul>
  </section>

  <section>
    <h2>Contact</h2>
    <p class="contact">You can reach me directly on WhatsApp:</p>
    <a href="https://wa.me/201159455350" class="whatsapp-btn" target="_blank">📞 01159455350 (Available on WhatsApp)</a>
    <p class="contact">Email: m.t.m.lead2013@gmail.com</p>
  </section>

  <footer>
    <p>Designed with passion by Amr Mohamed</p>
  </footer>

  <script>
    const toggle = document.getElementById('mode-toggle');
    toggle.addEventListener('click', () => {
      document.body.classList.toggle('dark-mode');
      toggle.textContent = document.body.classList.contains('dark-mode') ? '🌞' : '🌙';
    });
  </script>
</body>
</html>
