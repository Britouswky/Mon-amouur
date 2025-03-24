<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Un campo de tulipanes para Ana</title>
  <style>
    body {
      background: linear-gradient(#cce7e8, #ffffff);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      font-family: 'Courier New', monospace;
    }
    h1 {
      color: #4b4b4b;
      margin-bottom: 20px;
    }
    .tulipanes {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }
    .tulipan {
      width: 30px;
      height: 80px;
      background: linear-gradient(white, #e0e0e0);
      border-radius: 50% 50% 0 0;
      position: relative;
    }
    .tulipan::before {
      content: "";
      position: absolute;
      bottom: 0;
      left: 50%;
      width: 4px;
      height: 40px;
      background: green;
      transform: translateX(-50%);
    }
    p {
      margin-top: 30px;
      max-width: 600px;
      text-align: center;
      color: #333;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #4b4b4b;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #333;
    }
    .mensaje-sorpresa {
      margin-top: 20px;
      max-width: 600px;
      text-align: center;
      color: #4b4b4b;
      display: none;
      font-style: italic;
    }
  </style>
</head>
<body>

  <h1>Para ti, Ana</h1>

  <div class="tulipanes">
    <!-- Tulipanes -->
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
    <div class="tulipan"></div>
  </div>

  <p>Un campo de tulipanes blancos, tan puros como lo que siento por ti.<br>
  Tres meses juntos, y apenas estamos comenzando a florecer. Feliz aniversario, mi Ana.</p>

  <button onclick="mostrarMensaje()">Haz clic para ver cuánto te amo</button>

  <div class="mensaje-sorpresa" id="mensaje">
    Cada tulipán aquí es un te amo, pero mi amor por ti no cabe en un campo, ni en mil.<br>
    Gracias por estos tres meses, por tu risa, por tu mirada... eres mi milagro favorito.
  </div>

  <script>
    function mostrarMensaje() {
      const mensaje = document.getElementById('mensaje');
      mensaje.style.display = 'block';
    }
  </script>

</body>
</html>
