<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="google-site-verification" content="StWd0B-r52YYfce-ykcJZfxL-oWb9af7AhZ-_x0YrIo" />
  <title>Fundación Manacus</title>
  <style>
  @media (max-width: 650px) {
      .header-manacus {
        padding: 0.3em 0 0.3em 0;
      }
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
    }
    /* Paleta inspirada en tonos marinos y acentos cálidos */
    :root{
      --manacus-primary: #0f355f; /* deep navy */
      --manacus-accent: #ffd166; /* warm yellow */
      --manacus-muted: #f4f8fb; /* very light */
    }
    .header-manacus {
      width: 100%;
      background: linear-gradient(90deg,var(--manacus-primary), #153a68);
      color: #fff;
      box-shadow: 0 2px 18px rgba(11,32,56,0.12);
      padding: 0.6em 0 0.6em 0;
      position: sticky;
      top: 0;
      z-index: 110;
      border-bottom: 1px solid rgba(255,255,255,0.04);
    }
    .header-content {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 2em;
      padding: 0 2em;
    }
    .header-logo {
      display: flex;
      align-items: center;
      gap: 1em;
    }
    .header-logo img {
      height: 48px;
      width: auto;
      display: block;
      filter: brightness(1.1);
    }
    .header-nav {
      display: flex;
      gap: 0.6em;
      flex-wrap: wrap;
      align-items: center;
    }
    .header-nav a {
      background: transparent;
      color: #fff;
      padding: 0.45em 0.9em;
      border-radius: 8px;
      font-weight: 700;
      text-decoration: none;
      font-size: 0.98em;
      border: 1px solid transparent;
      transition: background 0.18s, transform 0.18s;
    }
    .header-nav a:hover {
      background: rgba(255,209,102,0.12);
      transform: translateY(-2px);
    }
    .footer-rec{
      color: var(--manacus-primary);
      font-weight: bold;
      letter-spacing: -2px;
      font-size: 1.8em;
      margin-top: 0em;
      margin-bottom: 0em;
      letter-spacing: -1.5px;
      text-align:right;
    }
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background: #fff;
      color: #232323;
      line-height: 1.6;
    }
    h2 {
      color: #19306c;
      font-weight: bold;
      letter-spacing: -2px;
      font-size: 1.8em;
      margin-top: 1.5em;
      margin-bottom: 0.5em;
      letter-spacing: -1.5px;
    }
    .texto-inicio{
      color: #19306c;
      font-weight: bold;
      font-size: 1.4em;
      margin-top: 0em;
      margin-bottom: 0em;
      text-align:center;
    }
    /* Hero / banner full-bleed */
    .hero-fullwidth{
      width: 100vw;
      margin-left: calc(50% - 50vw);
      background: linear-gradient(90deg, rgba(15,53,95,0.95), rgba(21,58,104,0.7));
      color: #fff;
      padding: 3.2em 0;
      position: relative;
      overflow: hidden;
    }
    .hero-content{
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 2em;
      display: flex;
      gap: 2em;
      align-items: center;
      justify-content: space-between;
    }
    .hero-text{ flex: 1 1 48%; }
    .hero-text h1{ font-size:2.1em;margin:0 0 0.6em;color:var(--manacus-accent); }
    .hero-text p{ color: #f1f6fb; font-size:1.02em; margin-bottom:1em }
    .hero-cta{ display:inline-block;background:var(--manacus-accent);color:var(--manacus-primary);padding:0.6em 1.1em;border-radius:8px;font-weight:700;text-decoration:none }
    .hero-image{ flex: 0 0 48%; position:relative; display:flex; justify-content:flex-end }
    .hero-image img{ width: 56%; height:auto; max-height:320px; object-fit:cover; border-radius:10px; box-shadow:0 18px 45px rgba(2,10,30,0.45); transform:translateX(6%);} 
    /* Select Your Service style */
    .services-section{ max-width:1200px;margin:2.2em auto;padding:0 2em; }
    .services-header{ text-align:left;margin-bottom:1em }
    .service-grid{ display:grid; grid-template-columns: repeat(4,1fr); gap:1.15em }
      .service-card{ background:linear-gradient(180deg, #ffffff, #fbfdff); border-radius:12px; padding:1.1em; box-shadow:0 6px 22px rgba(11,32,56,0.06); border:1px solid rgba(15,53,95,0.06); transition: transform 0.22s ease, box-shadow 0.22s ease }
      .service-card:hover{ transform: translateY(-8px); box-shadow:0 22px 48px rgba(11,32,56,0.12) }
      .service-card .ic{ font-size:2.15em; margin-bottom:0.6em }
      .service-card h3{ margin:0 0 0.5em;color:var(--manacus-primary) }
      .service-card p{ margin:0;color:#4b5568 }
    @media (max-width: 1200px){ .service-grid{ grid-template-columns: repeat(3,1fr) } }
    @media (max-width: 980px){ .service-grid{ grid-template-columns: repeat(2,1fr) } .hero-image img{ width:68% } }
    @media (max-width: 650px){
        .hero-content{ flex-direction:column; gap:1.2em }
        .hero-image{ order: 2; width:100%; justify-content:center }
        .hero-image img{ width:86%; transform:none }
        .service-grid{ grid-template-columns: 1fr }
      }
  </style>
</head>
<body>
  <header class="header-manacus">
    <div class="header-content">
      <div class="header-logo">
        <img src="src/logo_cortado.png" alt="Logo Fundación Manacus" style="background:rgba(32,46,80,0.06);" >
      </div>
      <nav class="header-nav">
        <!-- <a href="services/">Investigación</a> -->
        <a href="projects/">Proyectos</a>
        <a href="tecnologia/">Tecnología</a>
        <a href="quienes/">¿Quiénes somos?</a>
        <a href="contacto/">Contacto</a>
        <a href="asocanainstrucciones/">Asocaña</a>
      </nav>
    </div>
  </header>
  <!-- CONTENIDO PRINCIPAL SIGUIENTE -->
  <div class="seccion-destacada" style="background:#f8fafd;border-radius:12px;padding:1.2em 1em;margin-bottom:0.5em;box-shadow:0 1px 10px rgba(32,46,80,0.06);max-width:1000px;margin-left:auto;margin-right:auto;">
    <div style="width:100%;display:flex;justify-content:center;align-items:center;margin-top:0.5em;margin-bottom:0.5em;">
      <img src="src/logo_cortado.png" alt="Logo Fundación Manacus" style="max-width:660px;width:100%;height:auto;display:block;background:#f8fafd">
    </div>
    <p class="texto-inicio">Promovemos la preservación y protección del medio ambiente | Fomentamos una perspectiva territorial y de derechos, reconociendo la diversidad cultural y social | Impulsamos nuevas tecnologías para la gestión sostenible de la biodiversidad.</p>
    <br><br>
    Consulta la documentación de la fundación en el siguiente
    <a href="https://drive.google.com/drive/folders/1CbhU2uk9KZeAq2XAYW3GV9nvNxB_VJUJ?usp=drive_link">ENLACE</a>
    <br>
    Queremos conocer tu opinión, deja tus comentarios
    <a href="https://forms.gle/BLGUCDMGW3Qd51Xg9">AQUÍ</a>
    <br>
    <!-- SELECT YOUR SERVICE (cards) -->
    <h2>Servicios</h2>
    <section class="services-section">
      <div class="service-grid">
        <div class="service-card">
          <div class="ic">🎤</div>
          <h3>Monitoreo acústico</h3>
          <p>Instalación de estaciones y procesamiento automático de detecciones.</p>
        </div>
        <div class="service-card">
          <div class="ic">📊</div>
          <h3>Análisis de datos</h3>
          <p>Modelos y dashboards para interpretación y toma de decisiones.</p>
        </div>
        <div class="service-card">
          <div class="ic">🤝</div>
          <h3>Capacitación</h3>
          <p>Talleres y formación para comunidades y técnicos locales.</p>
        </div>
        <div class="service-card">
          <div class="ic">📡</div>
          <h3>Desarrollo de tecnología</h3>
          <p>Diseño y desarrollo de soluciones a medida: sensores, firmware y plataformas para análisis acústico.</p>
        </div>
      </div>
    </section>
    <h2>Estamos comprometidos con:</h2>
        <ul>
          <li><strong style="color:#19306c;">Preservar</strong> la biodiversidad mediante el uso de tecnologías avanzadas.</li>
          <li><strong style="color:#19306c;">Fortalecer</strong> la toma de decisiones con datos acústicos precisos y análisis automatizados.</li>
          <li><strong style="color:#19306c;">Empoderar</strong> a comunidades, instituciones y empresas con capacidades técnicas en bioacústica.</li>
          <li><strong style="color:#19306c;">Innovar</strong> en metodologías de monitoreo para la conservación basada en evidencia.</li>
        </ul>
    <h2>Contamos con</h2>
      <ul>
        <li><strong style="color:#19306c;">Expertos</strong> en ecoacústica con experiencia en múltiples ecosistemas.</li>
        <li><strong style="color:#19306c;">Tecnología</strong> de punta para análisis eficiente de grandes volúmenes de datos.</li>
        <li><strong style="color:#19306c;">Enfoque interdisciplinario</strong> (ecología, acústica, ciencia de datos).</li>
        <li><strong style="color:#19306c;">Compromiso</strong> con la conservación y las comunidades locales.</li>
        <li><b style="color:#19306c;">Aliados estratégicos</b><br>
            Biodiversity Analytics S.A.S.<br>
            Instituto Humboldt</li>
      </ul>   
      <p class="footer-rec">Parte de la Red Ecoacústica Colombiana
        <img src="src/logo_REC.png" alt="Logo REC" style="max-width:80px;width:auto;height:auto;vertical-align:middle;display:inline-block;background:#f8fafd;margin-left:0.7em;"></p>
  </div>
  <footer style="width:100%;background:#f8fafd;color:#19306c;text-align:center;padding:1.2em 0;font-size:1.08em;margin-top:2em;box-shadow:0 -1px 8px #19306c22;">
  contacto@manacus.co | Cali, Valle del Cauca, Colombia | NIT: 9 0 1 9 5 6 7 5 3 | © 2025 Manacus
  </footer>
</body>
</html>



  






