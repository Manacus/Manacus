<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Grillos</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* utilidades responsivas compartidas */
    body {
      margin: 0;
      padding: 0;
      font-family: 'Montserrat', Arial, sans-serif;
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1500&q=80') no-repeat center center fixed;
      background-size: cover;
      color: #e0e0e0;
      min-height: 100vh;
    }
    .page-container { max-width:1100px; margin:0 auto; padding:36px 20px }
    img.responsive{ max-width:100%; height:auto; display:block }
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
    @media (max-width: 980px){ .page-container{ padding:24px 14px } }
    @media (max-width: 650px){ .page-container{ padding:18px 12px } nav{ padding:0.8em 0 } }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <nav>
  <a href="#inicio">Grillos</a>
  <a href="#sobre">Firmware</a>
  <a href="#galeria">GrillApp</a>
  <a href="#contacto">Adquiérelos</a>
  </nav>
  <div class="main-content">
    <section id="inicio">
      <div style="display:flex; flex-direction:row; align-items:center; justify-content:space-between; gap:2em;">
        <div style="flex:1;">
          <h1>GRILLOS</h1>
          <p>Sensores acústicos pasivos de bajo costo diseñados para estudiar la biodiversidad a partir de la grabación de sonidos ambientales.</p>
          <div style="margin-top:2em; display:flex; gap:2em; flex-wrap:wrap; justify-content:left;">
            <a href="https://docs.google.com/document/d/1kwLbPUh7tB_ICO8ptXz6Q2vYcHChcv4enA8AXWpYvIY/edit?usp=sharing" class="buttons">Manual de operación</a>
            <a href="#ficha" class="buttons">Ficha técnica</a>
          </div>
        </div>
        <div style="width:220px;min-height:120px;display:flex;align-items:center;justify-content:center;background:rgba(32,46,80,0.08);border-radius:12px;">
          <img src="src/GrabadoraWeb.png" alt="Grillos sensor" style="max-width:200px;width:100%;height:auto;display:block;background= rgba(0,0,0,0.95)">
        </div>
      </div>
    </section>
    <section id="sobre">
      <h2>Firmware</h2>
      <p>Programa de funcionamiento para los grillos. Descarga la version más reciente aquí: <a href="src/audio_recorder.uf2">v1.0.0</a></p>
      <div style="margin-top:2em; display:flex; gap:2em; flex-wrap:wrap; justify-content:left;">
            <a href="https://docs.google.com/document/d/1kwLbPUh7tB_ICO8ptXz6Q2vYcHChcv4enA8AXWpYvIY/edit?usp=sharing" class="buttons">Manual de instalación</a>
      </div>
    </section>
    <section id="galeria">
      <div style="display:flex; flex-direction:row; align-items:center; justify-content:space-between; gap:2em;">
        <div style="flex:1;">
          <h2>GrillApp</h2>
          <p>Aplicacion android para configuración de dispositivos. Descargala en la <a href="https://play.google.com/apps/internaltest/4701477267970862944">Playstore</a>.</p>
        </div>
      <div style="display:flex;">
          <img src="src/iconGrillApp.png" alt="Grillos sensor" style="max-width:100px;width:100%;height:auto;display:block;background=">
        </div>
      </div>
    </section>
    <section id="contacto">
      <h2>Adquiérelos o solicita soporte técnico</h2>
      <p>Contacta al equipo desarrollador para comprarlos o asistencia técnica escribiendo a los números de Whatsapp <a href="https://wa.me/573182738651" style="color:#7be87b;font-weight:bold;text-decoration:none;font-size:1.13em;" target="_blank">+573182738651</a> </p>
    </section>
    <section id="blog-comentarios" style="background:rgba(0,0,0,0.85);border-radius:14px;box-shadow:0 1px 10px #00000044;padding:2em;margin-bottom:2em;margin-top:2em;max-width:900px;margin-left:auto;margin-right:auto;">
      <h2 style="color:#7be87b;font-size:1.5em;margin-bottom:1em;">Blog de comentarios</h2>
      <p style="color:#e0e0e0;font-size:1.13em;">¿Tienes dudas, sugerencias o quieres compartir tu experiencia? Déjanos tu comentario en el siguiente formulario y lo abordaremos aquí:</p>
      <a href="https://docs.google.com/forms/d/e/1FAIpQLSf4NiZ8JfTC9KQMdadXNc920cEf2aMV2ISSf42PrF-RB2xQog/viewform?usp=sharing&ouid=109877167667955358409" target="_blank" style="display:inline-block;padding:1em 2em;background:#7be87b;color:#222;border-radius:10px;font-size:1.08em;font-weight:bold;text-decoration:none;box-shadow:0 1px 8px #00000022;transition:background 0.2s;">Dejar comentario</a>
      <div style="margin-top:2em;min-height:120px;border:2px dashed #7be87b;border-radius:10px;background:#181818;display:flex;align-items:center;justify-content:center;color:#bdbdbd;font-size:1.13em;">
        Espacio para entradas de blog
      </div>
    </section>
  </div>
</body>
</html>
