<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Página Genérica</title>
</head>
<body>
  <h1>Bienvenido a la página genérica</h1>
  <button id="btnSaludo">Haz clic aquí</button>
  <p id="mensaje"></p>

  <script>
    document.getElementById('btnSaludo').addEventListener('click', function() {
      document.getElementById('mensaje').textContent = '¡Hola! Gracias por visitar esta página.';
    });
  </script>
</body>
</html>
