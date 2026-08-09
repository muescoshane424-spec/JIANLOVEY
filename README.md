```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>For My Spider-Man 🕷️❤️</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      font-family: "Arial", sans-serif;
      background:
        radial-gradient(circle at center, #3b0000 0%, #120000 55%, #050505 100%);
      color: white;
    }

    /* Spider-Man web background */
    .web {
      position: absolute;
      width: 700px;
      height: 700px;
      border-radius: 50%;
      opacity: 0.18;
      background:
        repeating-radial-gradient(
          circle,
          transparent 0 45px,
          #ffffff 46px 48px
        );
      animation: spin 30s linear infinite;
    }

    .web::before,
    .web::after {
      content: "";
      position: absolute;
      inset: 0;
      border-radius: 50%;
      background:
        repeating-conic-gradient(
          from 0deg,
          transparent 0deg 14deg,
          white 15deg 16deg
        );
    }

    @keyframes spin {
      from {
        transform: rotate(0deg);
      }
      to {
        transform: rotate(360deg);
      }
    }

    /* Floating hearts */
    .heart {
      position: absolute;
      bottom: -50px;
      font-size: 25px;
      animation: float 7s linear infinite;
      opacity: 0.8;
    }

    .heart:nth-child(1) {
      left: 10%;
      animation-delay: 0s;
    }

    .heart:nth-child(2) {
      left: 25%;
      animation-delay: 2s;
    }

    .heart:nth-child(3) {
      left: 70%;
      animation-delay: 1s;
    }

    .heart:nth-child(4) {
      left: 85%;
      animation-delay: 3s;
    }

    @keyframes float {
      0% {
        transform: translateY(0) scale(0.8);
        opacity: 0;
      }

      20% {
        opacity: 0.9;
      }

      100% {
        transform: translateY(-110vh) scale(1.4) rotate(20deg);
        opacity: 0;
      }
    }

    /* Main card */
    .card {
      position: relative;
      z-index: 10;
      width: min(90%, 520px);
      padding: 45px 30px;
      text-align: center;
      border-radius: 30px;
      background: rgba(15, 15, 15, 0.88);
      border: 2px solid #e50914;
      box-shadow:
        0 0 20px rgba(229, 9, 20, 0.5),
        0 0 60px rgba(229, 9, 20, 0.2);
      backdrop-filter: blur(10px);
      animation: appear 1.2s ease;
    }

    @keyframes appear {
      from {
        opacity: 0;
        transform: scale(0.8) translateY(30px);
      }

      to {
        opacity: 1;
        transform: scale(1) translateY(0);
      }
    }

    .spiderman {
      font-size: 75px;
      margin-bottom: 10px;
      animation: bounce 2s ease-in-out infinite;
      filter: drop-shadow(0 0 12px #e50914);
    }

    @keyframes bounce {
      0%, 100% {
        transform: translateY(0);
      }

      50% {
        transform: translateY(-10px);
      }
    }

    h1 {
      margin: 5px 0 15px;
      color: #ff2b36;
      font-size: 32px;
      text-shadow: 0 0 12px rgba(255, 30, 40, 0.7);
    }

    p {
      font-size: 19px;
      line-height: 1.7;
      margin: 15px 0;
    }

    .special {
      color: #ffb3b8;
      font-size: 16px;
      font-style: italic;
      margin-top: 20px;
    }

    .question {
      font-size: 24px;
      font-weight: bold;
      margin-top: 25px;
      color: white;
    }

    /* Buttons */
    .buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
      margin-top: 30px;
    }

    button {
      border: none;
      padding: 14px 24px;
      border-radius: 30px;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      transition: 0.25s ease;
    }

    .yes {
      background: #e50914;
      color: white;
      box-shadow: 0 0 15px rgba(229, 9, 20, 0.6);
    }

    .yes:hover {
      transform: scale(1.08);
      background: #ff1f2b;
      box-shadow: 0 0 25px rgba(255, 30, 40, 0.9);
    }

    .maybe {
      background: white;
      color: #111;
    }

    .maybe:hover {
      transform: scale(1.05);
    }

    #response {
      margin-top: 25px;
      min-height: 30px;
      font-size: 18px;
      font-weight: bold;
      color: #ff6972;
    }

    .signature {
      margin-top: 25px;
      font-size: 14px;
      color: #aaa;
    }

    /* Mobile */
    @media (max-width: 600px) {
      .card {
        padding: 35px 22px;
      }

      .spiderman {
        font-size: 60px;
      }

      h1 {
        font-size: 27px;
      }

      p {
        font-size: 17px;
      }

      .question {
        font-size: 21px;
      }
    }
  </style>
</head>

<body>

  <!-- Spider-Man style web -->
  <div class="web"></div>

  <!-- Floating hearts -->
  <div class="heart">❤️</div>
  <div class="heart">🕷️</div>
  <div class="heart">❤️</div>
  <div class="heart">🕸️</div>

  <!-- Main message -->
  <div class="card">

    <div class="spiderman">🕷️</div>

    <h1>Hey, My Spider-Man ❤️</h1>

    <p>
      You may not have spider-sense... 👀
      <br>
      but somehow, you managed to crawl
      <strong>straight into my heart.</strong> 🥹❤️
    </p>

    <p>
      So I have a very important mission for you... 🕸️
    </p>

    <div class="question">
      Will you watch Spider-Man with me? 🕷️🎬❤️
    </div>

    <p class="special">
      Just you and me, a good movie,
      lots of laughs, and a little bit of
      superhero magic. 🥰
      <br><br>
      Because honestly...
      <strong>watching Spider-Man with you
      would make it extra special. ❤️</strong>
    </p>

    <div class="buttons">
      <button class="yes" onclick="sayYes()">
        Yes, my Spider-Man! 🕷️❤️
      </button>

      <button class="maybe" onclick="sayMaybe()">
        I'll think about it... 🥺
      </button>
    </div>

    <div id="response"></div>

    <div class="signature">
      🕸️ Made especially for you 🕸️
    </div>

  </div>

  <script>
    function sayYes() {
      document.getElementById("response").innerHTML =
        "YAYYY! 🥹🕷️❤️ Our Spider-Man movie date is officially ON! 🎬🍿";

      createHearts();

      setTimeout(() => {
        alert("You said YES! 🕷️❤️🍿");
      }, 300);
    }

    function sayMaybe() {
      document.getElementById("response").innerHTML =
        "I'll wait for you, Spider-Man... 🥺🕸️❤️";
    }

    function createHearts() {
      for (let i = 0; i < 20; i++) {
        const heart = document.createElement("div");

        heart.innerHTML = Math.random() > 0.5 ? "❤️" : "🕷️";

        heart.style.position = "fixed";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.bottom = "-30px";
        heart.style.fontSize = (20 + Math.random() * 25) + "px";
        heart.style.zIndex = "100";
        heart.style.pointerEvents = "none";

        document.body.appendChild(heart);

        const animation = heart.animate(
          [
            {
              transform: "translateY(0) rotate(0deg)",
              opacity: 1
            },
            {
              transform:
                `translateY(-110vh) rotate(${Math.random() * 360}deg)`,
              opacity: 0
            }
          ],
          {
            duration: 3000 + Math.random() * 2500,
            easing: "ease-out"
          }
        );

        animation.onfinish = () => heart.remove();
      }
    }
  </script>

</body>
</html>
```
