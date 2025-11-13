## Hi there 👋


**Harshmishra9935/Harshmishra9935** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Animated Ball</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: radial-gradient(circle at center, #0f2027, #203a43, #2c5364);
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      font-family: sans-serif;
      color: white;
    }

    .ball {
      width: 100px;
      height: 100px;
      background: linear-gradient(135deg, #00c6ff, #0072ff);
      border-radius: 50%;
      box-shadow: 0 0 20px rgba(0, 114, 255, 0.8);
      position: absolute;
      animation: bounce 3s ease-in-out infinite;
      transition: transform 0.3s, box-shadow 0.3s;
      cursor: pointer;
    }

    @keyframes bounce {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-200px);
      }
    }

    .ball.clicked {
      transform: scale(1.3);
      box-shadow: 0 0 40px rgba(255, 255, 255, 1);
      background: linear-gradient(135deg, #ff9966, #ff5e62);
      animation: spin 1s linear infinite;
    }

    @keyframes spin {
      from { transform: rotate(0deg) scale(1.3); }
      to { transform: rotate(360deg) scale(1.3); }
    }

    h1 {
      position: absolute;
      bottom: 20px;
      text-align: center;
      width: 100%;
      font-size: 1.5em;
      letter-spacing: 1px;
    }
  </style>
</head>
<body>
  <div class="ball" id="ball"></div>
  <h1>Click the ball!</h1>

  <script>
    const ball = document.getElementById('ball');

    ball.addEventListener('click', () => {
      ball.classList.toggle('clicked');
    });
  </script>
</body>
</html>



 

