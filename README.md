<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Will You Marry Me?</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #ffe6f0;
      overflow: hidden;
      font-family: 'Segoe UI', sans-serif;
    }

    .container {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      color: #ff1493;
    }

    h1 {
      font-size: 3rem;
      white-space: nowrap;
      border-right: 3px solid;
      width: 0;
      overflow: hidden;
      animation: typing 4s steps(40, end) forwards, blink 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    .btn {
      margin-top: 30px;
      padding: 15px 30px;
      background-color: #ff69b4;
      color: white;
      border: none;
      border-radius: 30px;
      font-size: 1.2rem;
      cursor: pointer;
      transition: 0.3s ease;
      box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);
    }

    .btn:hover {
      background-color: #ff1493;
      transform: scale(1.05);
    }

    /* Hearts animation */
    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: float 10s linear infinite;
    }

    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        bottom: -10%;
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        bottom: 110%;
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h3>I LOVE YOU❤</h3></h3>
    <h1>Will You  BE MINE NANDHUU ?</h1>
    <button class="btn" onclick="alert('She said YES! 💍')">Yes ❤️</button>
   
     <h2>NO</h2> 
     
     
  </div>

  <!-- Animated hearts -->
  <script>
    for (let i = 0; i < 40; i++) {
      let heart = document.createElement("div");
      heart.classList.add("heart");
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = 5 + Math.random() * 5 + "s";
      heart.style.opacity = Math.random();
      document.body.appendChild(heart);
    }
  </script>
</body>
</html>
