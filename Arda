<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rayyona, beni seviyor musun?</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff0f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }
    h1 {
      font-size: 2.5rem;
      color: #d63384;
    }
    .buttons {
      margin-top: 30px;
    }
    button {
      padding: 15px 25px;
      font-size: 1.2rem;
      margin: 10px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.3s ease;
    }
    #yesBtn {
      background-color: #28a745;
      color: white;
    }
    #noBtn {
      background-color: #dc3545;
      color: white;
      position: relative;
    }
    #message {
      margin-top: 40px;
      font-size: 1.5rem;
      color: #d63384;
      display: none;
    }
  </style>
</head>
<body>
  <h1>Rayyona, beni seviyor musun? 💖</h1>
  <div class="buttons">
    <button id="yesBtn">Evet ❤️</button>
    <button id="noBtn">Hayır 😢</button>
  </div>
  <div id="message">Ben de seni çok seviyorum Rayyona! 💕</div>

  <script>
    const yesBtn = document.getElementById('yesBtn');
    const noBtn = document.getElementById('noBtn');
    const message = document.getElementById('message');

    yesBtn.addEventListener('click', () => {
      message.style.display = 'block';
      document.body.style.backgroundColor = '#fff7fb';
      yesBtn.style.display = 'none';
      noBtn.style.display = 'none';
      confetti();
    });

    noBtn.addEventListener('mouseover', () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 100);
      noBtn.style.position = 'absolute';
      noBtn.style.left = `${x}px`;
      noBtn.style.top = `${y}px`;
    });

    function confetti() {
      for (let i = 0; i < 100; i++) {
        const confetto = document.createElement('div');
        confetto.style.position = 'fixed';
        confetto.style.width = '10px';
        confetto.style.height = '10px';
        confetto.style.background = `hsl(${Math.random() * 360}, 70%, 60%)`;
        confetto.style.top = '-10px';
        confetto.style.left = `${Math.random() * window.innerWidth}px`;
        confetto.style.animation = 'fall 3s ease-out forwards';
        confetto.style.zIndex = 9999;
        document.body.appendChild(confetto);
        setTimeout(() => confetto.remove(), 3000);
      }
    }

    const style = document.createElement('style');
    style.innerHTML = `@keyframes fall { to { transform: translateY(100vh) rotate(360deg); opacity: 0; } }`;
    document.head.appendChild(style);
  </script>
</body>
</html>
