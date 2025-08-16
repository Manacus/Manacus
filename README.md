<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Fundación Manacus</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f5f6fa;
      color: #232323;
      line-height: 1.6;
    }
    .header-manacus {
      width: 100%;
      background: #fff;
      box-shadow: 0 2px 12px rgba(32,46,80,0.07);
      padding: 0.5em 0 0.5em 0;
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 1px solid #e0e0e0;
    }
    .header-manacus nav a {
      background: none;
      color: #19306c;
      padding: 0.6em 1.3em;
      border-radius: 6px;
      font-weight: 600;
      text-decoration: none;
      font-size: 1em;
      box-shadow: none;
      transition: background 0.2s, color 0.2s;
      border: none;
    }
    .header-manacus nav a:hover {
      background: #eaf0fa;
      color: #232323;
    }
    h2 {
      color: #19306c;
      font-weight: bold;
      font-size: 1.8em;
      margin-top: 1.5em;
      margin-bottom: 0.5em;
      letter-spacing: -1px;
    }
    .seccion-destacada {
      background: #fff;
      border-radius: 12px;
      padding: 1.2em 1em;
      margin-bottom: 0.5em;
      box-shadow: 0 1px 10px rgba(32,46,80,0.06);
      max-width: 1000px;
      margin-left: auto;
      margin-right: auto;
      border: 1px solid #e0e0e0;
    }
    .seccion-destacada strong, .seccion-destacada b {
      color: #19306c;
    }
    .seccion-destacada a {
      color: #19306c;
      font-weight: 600;
      text-decoration: underline;
      transition: color 0.2s;
    }
    .seccion-destacada a:hover {
      color: #232323;
      background: #eaf0fa;
      border-radius: 4px;
      text-decoration: none;
    }
    ul {
      padding-left: 1.2em;
    }
    li {
      margin-bottom: 0.7em;
    }
    footer {
      width: 100%;
      background: #fff;
      color: #19306c;
      text-align: center;
      padding: 1.2em 0;
      font-size: 1.08em;
      margin-top: 2em;
      box-shadow: 0 -1px 8px #e0e0e0;
      border-top: 1px solid #e0e0e0;
    }
    @media (max-width: 650px) {
      .header-manacus > div {
        flex-direction: column !important;
        align-items: stretch !important;
        gap: 0.7em !important;
      }
      .header-manacus nav {
        flex-direction: column;
        gap: 0.7em;
        align-items: stretch;
      }
      .header-manacus a {
        font-size: 0.98em;
        padding: 0.5em 1em;
        width: 100%;
        box-sizing: border-box;
        text-align: left;
      }
      .seccion-destacada {
        padding: 1em 0.3em;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="header-manacus">
      <div style="max-width:1000px;margin-right:auto;display:flex;align-items:center;justify-content:flex-end;gap:1em;">
        <nav style="display:flex;gap:1em;flex-wrap:wrap;">
          <a href="services/">Servicios</a>
          <a href="projects/">Proyectos</a>
          <a href="tecnologia/">Tecnología</a>
          <a href="quienes/">¿Quiénes somos?</a>
          <a href="contacto/">Contacto</a>
        </nav>
      </div>
    </header>
  </div>
  <div class="seccion-destacada">
    <div style="width:100%;display:flex;justify-content:center;align-items:center;margin-top:0.5em;margin-bottom:0.5em;">
      <img src="src/logo_cortado.png" alt="Logo Fundación Manacus" style="max-width:660px;width:100%;height:auto;display:block;background:#fff">
    </div>
    <h2>NUESTRO OBJETIVO</h2>
    <strong>Promover la preservación y protección del medio ambiente, desde una perspectiva territorial y de derechos, que reconozca la diversidad cultural y social para el ordenamiento, uso y manejo adecuado de los recursos naturales renovables y no renovables; impulsando la implementación de nuevas tecnologías para el monitoreo, conservación y gestión sostenible de la biodiversidad.</strong>
    <br><br>
    Consulta la documentación de la fundación en el siguiente
    <a href="https://drive.google.com/drive/folders/1CbhU2uk9KZeAq2XAYW3GV9nvNxB_VJUJ?usp=drive_link">ENLACE</a>
    <br>
    Queremos conocer tu opinión, deja tus comentarios
    <a href="https://forms.gle/BLGUCDMGW3Qd51Xg9">AQUÍ</a>
    <br>
    <h2>Estamos comprometidos con:</h2>
    <ul>
      <li><strong>Preservar</strong> la biodiversidad mediante el uso de tecnologías avanzadas.</li>
      <li><strong>Fortalecer</strong> la toma de decisiones con datos acústicos precisos y análisis automatizados.</li>
      <li><strong>Empoderar</strong> a comunidades, instituciones y empresas con capacidades técnicas en bioacústica.</li>
      <li><strong>Innovar</strong> en metodologías de monitoreo para la conservación basada en evidencia.</li>
    </ul>
    <h2>Contamos con</h2>
    <ul>
      <li><strong>Expertos</strong> en ecoacústica con experiencia en múltiples ecosistemas.</li>
      <li><strong>Tecnología</strong> de punta para análisis eficiente de grandes volúmenes de datos.</li>
      <li><strong>Enfoque interdisciplinario</strong> (ecología, acústica, ciencia de datos).</li>
      <li><strong>Compromiso</strong> con la conservación y las comunidades locales.</li>
      <li><b>Aliados estratégicos</b><br>
        Biodiversity Analytics S.A.S.<br>
        Red Ecoacústica Colombiana (REC)<br>
        Instituto Humboldt</li>
    </ul>
  </div>
  <footer>
    Hacemos parte de la REC
  </footer>
</body>
</html>



