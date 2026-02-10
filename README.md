# San-valentin
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>San Valentín 💘</title>
  <style>
    body {
      background: linear-gradient(135deg, #ff5f9e, #ffc371);
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      color: white;
      text-align: center;
    }
    .card {
      background: rgba(255,255,255,0.15);
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,.3);
    }
    button {
      padding: 15px 25px;
      font-size: 18px;
      border: none;
      border-radius: 12px;
      margin: 10px;
      cursor: pointer;
    }
    #yes {
      background: #ff2e63;
      color: white;
    }
    #no {
      background: white;
      color: #ff2e63;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>💖 ¿Quieres ser mi San Valentín? 💖</h1>
    <button id="yes" onclick="acepto()">Sí 💘</button>
    <button id="no" onmouseover="mover()">No 😅</button>
  </div>

<script>
  function mover() {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 50);
    const no = document.getElementById("no");
    no.style.left = x + "px";
    no.style.top = y + "px";
  }

  function acepto() {
    document.body.innerHTML = "<h1>🥰 Sabía que dirías que sí 💖</h1><p>Prepárate para un San Valentín especial 😏</p>";
  }
</script>

</body>
</html>
