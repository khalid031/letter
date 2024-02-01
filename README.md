<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Love Gift Card | @helpme_coder</title>
  <style>
    body {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      background: repeating-linear-gradient(45deg, #fce0d4, #fce0d4 10px, #f8bbd0 10px, #f8bbd0 20px); /* Ice cream color gradient */
    }

    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
    }

    .envelope {
      background-color: #ffee58; /* Envelope color */
      width: 220px;
      height: 160px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 10px;
      position: relative;
      overflow: hidden;
      cursor: pointer;
      transition: transform 0.5s ease-in-out;
    }

    .envelope:hover {
      transform: translateY(-30px);
    }

    .flap {
      position: absolute;
      top: 0;
      left: 50%;
      width: 0;
      height: 0;
      border-left: 35px solid transparent;
      border-right: 35px solid transparent;
      border-bottom: 35px solid #ffee58; /* Envelope color */
      transform: translateX(-50%);
      transition: transform 0.5s ease-in-out;
    }

    .envelope:hover .flap {
      transform: translateY(30px);
    }

    .envelope-text {
      font-size: 18px;
      font-weight: bold;
      color: #721c24; /* Text color */
    }

    .card {
      position: absolute;
      width: 200px;
      height: 120px;
      background-color: #ffccd4; /* Card background color */
      border-radius: 10px;
      padding: 15px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
      overflow: hidden;
      transition: transform 0.5s ease-in-out;
      display: flex;
      flex-wrap: wrap;
      align-content: space-between;
    }

    .envelope:hover .card {
      transform: translateY(-100%);
    }

    .subject {
      font-size: 16px;
      text-align: center;
      color: #721c24; /* Text color */
      font-style: italic;
    }

    .apology {
      font-size: 12px;
      text-align: center;
      color: #721c24; /* Text color */
      flex: 0 0 100%;
      margin-top: 8px;
    }

    .ice-cream {
      font-size: 16px;
      animation: iceCreamExplosion 0.8s ease-in-out;
    }

    @keyframes iceCreamExplosion {
      0% {
        transform: translateY(0) rotate(0);
      }
      25% {
        transform: translateY(-25px) rotate(45deg);
      }
      50% {
        transform: translateY(0) rotate(90deg);
      }
      75% {
        transform: translateY(-25px) rotate(135deg);
      }
      100% {
        transform: translateY(0) rotate(180deg);
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="envelope">
      <div class="flap"></div>
      <div class="envelope-text">From Khalid to Rumie</div>
      <div class="card">
        <div class="subject">Sorry</div>
        <div class="ice-cream">🍦</div>
        <div class="ice-cream">🍦</div>
        <div class="ice-cream">🍦</div>
        <div class="ice-cream">🍦</div>
        <div class="ice-cream">🍦</div>
        <div class="ice-cream">🍦</div>
      </div>
    </div>
  </div>
</body>
</html>
