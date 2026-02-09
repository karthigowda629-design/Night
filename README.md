# Night 

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Pookieeee 🎀</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Poppins', 'Segoe UI', sans-serif;
      background: radial-gradient(circle at top, #1b1f3b, #0f1225, #090b1a);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      color: #f5f5f5;
    }

    .container {
      background: rgba(20, 24, 55, 0.92);
      width: 92%;
      max-width: 420px;
      padding: 38px 28px;
      border-radius: 26px;
      text-align: center;
      box-shadow: 0 30px 70px rgba(0,0,0,0.6);
      animation: popIn 1.4s ease;
      position: relative;
      backdrop-filter: blur(6px);
    }

    h1 {
      color: #ff9ecb;
      margin-bottom: 6px;
      font-size: 26px;
    }

    .subtitle {
      color: #b8b8d9;
      font-size: 14px;
      margin-bottom: 18px;
    }

    .heart {
      font-size: 50px;
      animation: heartbeat 1.3s infinite;
      margin: 16px 0 20px;
      filter: drop-shadow(0 0 12px rgba(255,158,203,0.7));
    }

    p {
      color: #e6e6ff;
      font-size: 15.5px;
      line-height: 1.75;
      margin: 12px 0;
    }

    .soft {
      font-style: italic;
      color: #cfcff5;
      margin-top: 16px;
    }

    .buttons {
      margin-top: 28px;
      display: flex;
      flex-direction: column;
      gap: 14px;
    }

    button {
      padding: 14px 24px;
      border: none;
      border-radius: 999px;
      font-size: 15px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .btn-main {
      background: linear-gradient(135deg, #ff7abf, #ff4f9a);
      color: #fff;
      box-shadow: 0 12px 24px rgba(255,79,154,0.45);
    }

    .btn-main:hover {
      transform: translateY(-2px) scale(1.04);
    }

    .btn-wa {
      background: #25D366;
      color: #fff;
      box-shadow: 0 12px 24px rgba(37,211,102,0.45);
    }

    .btn-wa:hover {
      transform: translateY(-2px) scale(1.04);
    }

    .from {
      margin-top: 20px;
      font-weight: 600;
      color: #ff9ecb;
    }

    .floating {
      position: absolute;
      inset: 0;
      pointer-events: none;
      overflow: hidden;
    }

    .star {
      position: absolute;
      bottom: -40px;
      font-size: 18px;
      animation: floatUp linear infinite;
      opacity: 0.9;
      filter: drop-shadow(0 0 6px rgba(255,255,255,0.6));
    }

    @keyframes popIn {
      from { opacity: 0; transform: scale(0.88) translateY(30px); }
      to { opacity: 1; transform: scale(1) translateY(0); }
    }

    @keyframes heartbeat {
      0%,100% { transform: scale(1); }
      50% { transform: scale(1.28); }
    }

    @keyframes floatUp {
      from { transform: translateY(0); opacity: 0; }
      15% { opacity: 1; }
      to { transform: translateY(-110vh); opacity: 0; }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Hey Pookieeee 🎀</h1>
    <div class="subtitle">It’s quiet… so I’m saying this softly</div>

    <div class="heart">💖</div>

    <p>
      Nights make everything feel heavier.
      And honestly… I hate knowing I’m the reason your heart feels distant.
    </p>

    <p>
      I never meant to hurt you.
      I just want to fix what I broke — slowly, properly, with care.
    </p>

    <p class="soft">
      If you can’t forgive me yet, that’s okay.
      Just don’t disappear on me. 🌙
    </p>

    <div class="buttons">
      <button class="btn-main" onclick="gentleMsg()">Tap if you feel me 💗</button>

      <a href="https://wa.me/?text=Hey%20Karthiiii…%20I%20saw%20your%20page" target="_blank" style="text-decoration:none;">
        <button class="btn-wa">Message Karthiiii 💬</button>
      </a>
    </div>

    <div class="from">— Karthiiii 🌙</div>
  </div>

  <div class="floating" id="floating"></div>

  <script>
    function gentleMsg() {
      alert("Thank you for being here 💗\nI’m not going anywhere.");
    }

    const stars = ['✨','⭐','🌙','💫'];
    const floating = document.getElementById('floating');

    function createStar() {
      const span = document.createElement('span');
      span.className = 'star';
      span.innerText = stars[Math.floor(Math.random() * stars.length)];
      span.style.left = Math.random() * 100 + 'vw';
      span.style.animationDuration = (7 + Math.random() * 6) + 's';
      floating.appendChild(span);
      setTimeout(() => span.remove(), 13000);
    }

    setInterval(createStar, 700);

    const audio = new Audio('https://cdn.pixabay.com/download/audio/2022/10/03/audio_8b7c7c0d2b.mp3?filename=gentle-piano-ambient-114998.mp3');
    audio.loop = true;
    audio.volume = 0.12;
    audio.play().catch(()=>{});
  </script>
</body>
</html>
