<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Nature Punk - Página Genérica</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Montserrat', Arial, sans-serif;
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1500&q=80') no-repeat center center fixed;
      background-size: cover;
      color: #e0e0e0;
      min-height: 100vh;
    }
    .overlay {
      background: rgba(0, 0, 0, 0.85);
      min-height: 400vh;
      width: 100%;
      position: absolute;
      top: 0;
      left: 0;
      z-index: 0;
    }
    .main-content {
      position: relative;
      z-index: 1;
      max-width: 900px;
      margin: 0 auto;
      padding: 48px 24px;
    }
    nav {
      display: flex;
      justify-content: center;
      background: rgba(0,0,0,0.95);
      padding: 1.2em 0;
      border-bottom: 2px solid #7be87b;
      position: relative;
      z-index: 2;
    }
    nav a {
      color: #7be87b;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.15em;
      margin: 0 1.5em;
      transition: color 0.2s;
    }
    nav a:hover {
      color: #fff;
    }
    h1 {
      font-size: 2.5em;
      font-weight: 700;
      color: #7be87b;
      margin-bottom: 0.5em;
      text-shadow: 0 2px 8px #00000099;
    }
    section {
      background: rgba(0,0,0,0.85);
      border-radius: 14px;
      box-shadow: 0 1px 10px #00000044;
      padding: 2em;
      margin-bottom: 2em;
    }
    h2 {
      color: #7be87b;
      font-size: 1.5em;
      margin-bottom: 1em;
    }
    p {
      font-size: 1.13em;
      color: #e0e0e0;
    }
    .buttons{
      display:inline-block; padding:1em 2em; background:#222; color:#7be87b; border-radius:10px; font-size:1.08em; font-weight:bold; text-decoration:none; box-shadow:0 1px 8px #00000022; transition:background 0.2s; 
    }
    @media (max-width: 600px) {
      .main-content { padding: 24px 6px; }
      nav a { font-size: 1em; margin: 0 0.7em; }
      section { padding: 1em; }
    }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <nav>
    <a href="#inicio">GRILLA</a>
    <a href="#sobre">Firmware</a>
    <a href="#galeria">GrillApp</a>
    <a href="#contacto">Contacto</a>
  </nav>
  <div class="main-content">
    <section id="inicio">
      <h1>GRILLA</h1>
      <p>Sensores acústicos pasivos diseñados para estudiar la biodiversidad a partir de la grabación de sonidos ambientales.</p>
      <div style="margin-top:2em; display:flex; gap:2em; flex-wrap:wrap;">
        <a href="#manual" class="buttons">Manual de operación</a>
        <a href="#ficha" class="buttons">Ficha técnica</a>
      </div>
    </section>
    <section id="sobre">
      <h2>Firmware</h2>
      <p>Esta sección puede contener información sobre el propósito de la página, el equipo o la misión del proyecto.</p>
    </section>
    <section id="galeria">
      <h2>GrillApp</h2>
      <p>Aquí puedes mostrar imágenes, proyectos o cualquier contenido visual relevante.</p>
    </section>
    <section id="contacto">
      <h2>Contacto</h2>
      <p>Incluye aquí información de contacto, redes sociales o un formulario para mensajes.</p>
    </section>
  </div>
</body>
</html>
