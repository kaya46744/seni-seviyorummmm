<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Seni Seviyorum Sen Beni Seviyor Musun?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #fff0f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    h1 {
      color: #e91e63;
    }

    .buttons {
      margin-top: 20px;
    }

    button {
      padding: 10px 20px;
      margin: 10px;
      font-size: 18px;
      cursor: pointer;
      border: none;
      border-radius: 5px;
      transition: 0.3s;
    }

    .yes {
      background-color: #4caf50;
      color: white;
    }

    .no {
      background-color: #f44336;
      color: white;
    }

    .heart {
      font-size: 50px;
      animation: heartbeat 1s infinite;
      color: red;
      display: none;
    }

    @keyframes heartbeat {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.4);
      }
    }

    .sad-emoji {
      font-size: 60px;
      display: none;
    }
  </style>
</head>
<body>
  <h1>Seni seviyorummmm 💖</h1>
  <p>Sen de beni seviyor musun?</p>

  <div class="buttons">
    <button class="yes" onclick="showLove()">Evet</button>
    <button class="no" onclick="showSad()">Hayır</button>
  </div>

  <div id="result">
    <div id="heart" class="heart">❤️</div>
    <div id="sad" class="sad-emoji">😢</div>
  </div>

  <script>
    function showLove() {
      document.getElementById("heart").style.display = "block";
      document.getElementById("sad").style.display = "none";
    }

    function showSad() {
      document.getElementById("sad").style.display = "block";
      document.getElementById("heart").style.display = "none";
    }
  </script>
</body>
</html>
