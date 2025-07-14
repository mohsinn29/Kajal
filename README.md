<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Dearest Angel Kajal</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins&display=swap');

    body {
      margin: 0;
      padding: 0;
      background: radial-gradient(circle, #ffe4e1, #ffc0cb);
      font-family: 'Poppins', sans-serif;
      overflow-x: hidden;
    }

    .container {
      text-align: center;
      padding: 50px 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3em;
      color: #ff69b4;
      margin-bottom: 10px;
    }

    .quote {
      font-size: 1.5em;
      color: #d63384;
      margin: 30px auto;
      max-width: 700px;
      background: rgba(255, 255, 255, 0.5);
      padding: 20px;
      border-radius: 20px;
      box-shadow: 0 0 15px rgba(255, 192, 203, 0.7);
    }

    .sparkle {
      position: absolute;
      width: 5px;
      height: 5px;
      background: white;
      border-radius: 50%;
      opacity: 0;
      animation: sparkle 3s infinite;
    }

    @keyframes sparkle {
      0% {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateY(-100px) scale(0.5);
        opacity: 0;
      }
    }

    button {
      background-color: #ff69b4;
      border: none;
      padding: 15px 30px;
      color: white;
      font-size: 1em;
      font-family: 'Poppins', sans-serif;
      border-radius: 30px;
      cursor: pointer;
      margin-top: 20px;
      transition: transform 0.2s;
    }

    button:hover {
      transform: scale(1.1);
    }

    .proposal {
      font-size: 2em;
      color: #ff1493;
      margin-top: 50px;
      font-family: 'Great Vibes', cursive;
    }

    .final-proposal {
      font-size: 2.5em;
      color: #c2185b;
      font-family: 'Great Vibes', cursive;
      margin-top: 40px;
      padding: 30px;
      background: rgba(255, 240, 245, 0.7);
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(255, 105, 180, 0.6);
      display: none;
    }

    footer {
      margin-top: 60px;
      padding: 20px;
      background-color: #ffe4e1;
      font-size: 1em;
      color: #d63384;
      font-weight: bold;
      text-align: center;
      font-family: 'Great Vibes', cursive;
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>My Dearest Angel Kajal</h1>

    <div class="quote" id="quoteBox">
      "Your smile is the spark that lights up my entire world. Kajal, you're my fairy dream come true."
    </div>

    <button onclick="nextClick()" id="loveBtn">Click for Show Love 💖</button>

    <div id="proposal" class="proposal">
      Dizzy ♥ Kajal,<br>
      Will you be the fairy of my forever? 💍✨
    </div>

    <div id="finalProposal" class="final-proposal">
      From the moment I met you, Kajal, my world changed forever. You are not just a dream, you are my reality, my heart, my every heartbeat. 💖<br>
      Will you make my life magical by being with me forever? 🌹💍<br>
      Yours forever, Dizzy 💕
    </div>
  </div>

  <footer>
    Dizzy & Kajal
  </footer>

  <script>
    const quotes = [
      "You're the magic in my stars, Kajal. ✨",
      "Every moment with you is a fairytale, Kajal. 💫",
      "Your love is softer than the clouds and sweeter than a dream. ☁️",
      "When I look at you, I see the rest of my life. 💕",
      "Kajal, you're not just a name, you're my heartbeat. 💓",
      "Being with you is like dancing in a garden of love and light. 🌸"
    ];

    let clickCount = 0;

    function nextClick() {
      const box = document.getElementById("quoteBox");
      const btn = document.getElementById("loveBtn");

      if (clickCount < quotes.length) {
        box.textContent = quotes[clickCount];
        clickCount++;
        if (clickCount === quotes.length) {
          btn.textContent = "Final Love 💘";
        }
      } else {
        document.getElementById("finalProposal").style.display = "block";
        btn.style.display = "none";
      }
    }

    for (let i = 0; i < 60; i++) {
      const sparkle = document.createElement('div');
      sparkle.classList.add('sparkle');
      sparkle.style.left = `${Math.random() * 100}vw`;
      sparkle.style.top = `${Math.random() * 100}vh`;
      sparkle.style.animationDelay = `${Math.random() * 3}s`;
      document.body.appendChild(sparkle);
    }
  </script>
</body>

</html>

