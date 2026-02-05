<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>🍋 Lemon Dance</title>
<style>
  body {
    background: #111;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .lemon {
    width: 150px;
    height: 200px;
    background: yellow;
    border-radius: 50% 50% 45% 45%;
    position: relative;
    animation: dance 0.4s infinite alternate;
  }

  .eye {
    width: 15px;
    height: 15px;
    background: black;
    border-radius: 50%;
    position: absolute;
    top: 50px;
  }

  .eye.left { left: 40px; }
  .eye.right { right: 40px; }

  .mouth {
    width: 40px;
    height: 20px;
    border-bottom: 4px solid black;
    border-radius: 0 0 50px 50px;
    position: absolute;
    bottom: 60px;
    left: 50%;
    transform: translateX(-50%);
  }

  @keyframes dance {
    0% { transform: rotate(-5deg) translateX(-10px); }
    100% { transform: rotate(5deg) translateX(10px); }
  }
</style>
</head>
<body>

<div class="lemon">
  <div class="eye left"></div>
  <div class="eye right"></div>
  <div class="mouth"></div>
</div>

</body>
</html>
