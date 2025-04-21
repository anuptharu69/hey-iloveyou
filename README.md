
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>I Love You Anisha</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: radial-gradient(#ffe6f0, #ffc0cb);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      overflow: hidden;
      color: #d6336c;
    }

    h1 {
      font-size: 3em;
      margin: 20px 0 10px;
      text-shadow: 2px 2px #fff;
    }

    p {
      font-size: 1.2em;
      margin: 10px;
    }

    .heart3d {
      width: 150px;
      height: 150px;
      position: relative;
      transform-style: preserve-3d;
      animation: spin 10s linear infinite;
    }

    .heart3d::before,
    .heart3d::after {
      content: "❤️";
      font-size: 150px;
      position: absolute;
      top: 0;
      left: 0;
      transform: translateZ(0);
    }

    .heart3d::after {
      transform: rotateY(180deg);
    }

    @keyframes spin {
      from { transform: rotateY(0deg); }
      to { transform: rotateY(360deg); }
    }

    .couple-img {
      width: 300px;
      height: auto;
      border-radius: 15px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.2);
      margin-top: 30px;
    }

    .floating-hearts {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      overflow: hidden;
    }

    .floating-hearts span {
      position: absolute;
      color: #ff69b4;
      animation: float 6s linear infinite;
      font-size: 24px;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) scale(0.5);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-10vh) scale(1.2);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="heart3d"></div>
  <h1>I Love You Anisha</h1>
  <p>You’re the light of my life 🌟</p>
  <img class="couple-img" src="https://i.pinimg.com/originals/8a/90/87/8a9087ebf3e82c1e1968dc8442ee47b5.jpg" alt="Couple Image">
  
  <div class="floating-hearts">
    <!-- Floating hearts -->
    <span style="left: 10%;">💖</span>
    <span style="left: 30%;">💘</span>
    <span style="left: 50%;">💝</span>
    <span style="left: 70%;">💞</span>
    <span style="left: 90%;">💓</span>
  </div>
</body>
</html>
