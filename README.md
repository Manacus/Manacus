<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Fundación Manacus </title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background: #fff;
      color: #232323;
      line-height: 1.6;
    }
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 32px 16px;
    }
    .logo-header {
      display: flex;
      align-items: center;
      gap: 2em;
      margin-top: 2.5em;
      margin-bottom: 2.7em;
    }
    .logo-title-group {
      flex-grow: 1;
    }
    .logo-title {
      color: #19306c;
      font-size: 5em;
      font-weight: bold;
      letter-spacing: -2.2px;
      margin-bottom: 0.1em;
      margin-top: 0;
      line-height: 1.05;
    }
    .logo-subtitle {
      color: #222;
      font-size: 1em;
      letter-spacing: 0.25em;
      margin-top: 0.7em;
      margin-bottom: 0;
      font-weight: lighter;
    }
    .logo-img-placeholder {
      width: 130px;
      height: 110px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #f4f4f4;
      border: 2px dashed #19306c77;
      border-radius: 13px;
      color: #aaa;
      font-size: 1em;
      margin-left: 0.5em;
      margin-right: 0.7em;
      text-align: center;
      box-sizing: border-box;
    }
    @media (max-width: 650px) {
      .logo-header { flex-direction: column; align-items: flex-start; gap: 1em; }
      .logo-img-placeholder { width: 100px; height: 70px; font-size: 0.82em; }
      .logo-title { font-size: 1.6em; }
    }
    h1, h2, h3 {
      color: #19306c;
      font-weight: bold;
      letter-spacing: -2px;
    }
    h1 {
      font-size: 2.4em;
      margin-bottom: 0.25em;
      margin-top: 0.7em;
    }
    h2 {
      font-size: 2.1em;
      margin-top: 2.8em;
      margin-bottom: 1.5em;
      letter-spacing: -1.5px;
    }
    h3 {
      font-size: 1.18em;
      letter-spacing: -1px;
      color: #19306c;
      margin-bottom: 0.2em;
    }
    .objetivo {
      font-style: italic;
      color: #333;
      margin-bottom: 1.5em;
      font-size: 1.16em;
    }
    .desc {
      margin-bottom: 2.5em;
    }
    .footer {
      border-top: 1px solid #bbb;
      margin-top: 2em;
      padding-top: 0.7em;
      font-size: 0.98em;
      color: #666;
      display: flex;
      justify-content: space-between;
    }
    .commit-section {
      background: #f8fafd;
      padding: 2.2em 1em 2em 1em;
      border-radius: 10px;
      margin-top: 2.2em;
    }
    .commit-title {
      color: #fdbe5d;
      font-weight: bold;
      font-size: 1.38em;
      letter-spacing: -1px;
      margin-bottom: 0.2em;
      display: inline-block;
    }
    .commit-subtitle {
      color: #19306c;
      font-weight: bold;
      font-size: 1.32em;
      display: inline-block;
      margin-left: 0.5em;
      margin-bottom: 1.1em;
    }
    .commit-list {
      margin: 0;
      padding: 0;
      list-style: none;
    }
    .commit-item {
      display: flex;
      align-items: flex-start;
      margin-bottom: 1.4em;
    }
    .commit-number {
      background: #19306c;
      color: #fff;
      font-weight: bold;
      font-size: 1.15em;
      width: 2em;
      height: 2em;
      border-radius: 0.3em;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 1em;
      flex-shrink: 0;
    }
    .commit-number.orange {
      background: #fdbe5d;
      color: #19306c;
    }
    .commit-content {
      flex: 1;
    }
    .commit-content strong {
      color: #19306c;
    }
    .servicios-section {
      margin-top: 3em;
    }
    .servicios-title {
      color: #19306c;
      font-size: 2.1em;
      font-weight: bold;
      margin-bottom: 1.5em;
      margin-top: 0;
      letter-spacing: -1.5px;
    }
    .servicio-block {
      margin-bottom: 2.2em;
      background: #f9f9f9;
      border-radius: 10px;
      padding: 1.2em 1.2em 1.2em 4.2em;
      position: relative;
      box-shadow: 0 1px 6px rgba(32,46,80,0.03);
      border-left: 10px solid #fdbe5d;
    }
    .servicio-icon {
      position: absolute;
      left: 1em;
      top: 1.3em;
      font-size: 1.8em;
    }
    .servicio-title {
      color: #19306c;
      font-size: 1.1em;
      font-weight: bold;
      margin-bottom: 0.6em;
      background: #fdbe5d30;
      display: inline-block;
      padding: 2px 10px;
      border-radius: 4px;
    }
    .servicio-title.gray {
      background: #e8ecef;
      color: #19306c;
    }
    .servicio-title.blue {
      background: #eaf4fa;
      color: #19306c;
    }
    .servicio-title.yellow {
      background: #fff7e1;
      color: #19306c;
    }
    .servicio-list {
      margin-top: 0.3em;
      margin-bottom: 0;
      padding-left: 1.2em;
    }
    .servicio-list li {
      margin-bottom: 0.4em;
      font-size: 1em;
    }
    .equipo-section {
      margin-top: 3.2em;
      margin-bottom: 2.5em;
    }
    .equipo-title {
      color: #19306c;
      font-size: 2em;
      font-weight: bold;
      margin-bottom: 1.3em;
      letter-spacing: -1.5px;
      margin-top: 0;
    }
    .miembro-block {
      background: #f8fafd;
      border-radius: 10px;
      margin-bottom: 1.7em;
      padding: 2em 1.3em 1.6em 1.3em;
      box-shadow: 0 1px 6px rgba(32,46,80,0.02);
      border-left: 8px solid #19306c;
    }
    .miembro-nombre {
      color: #19306c;
      font-size: 1.18em;
      font-weight: bold;
      margin-bottom: 0.08em;
      letter-spacing: -1px;
      text-transform: uppercase;
    }
    .miembro-cargo {
      color: #4475bb;
      font-size: 1em;
      font-weight: bold;
      margin-bottom: 0.65em;
      letter-spacing: -0.5px;
      text-transform: uppercase;
    }
    .miembro-desc {
      margin-bottom: 1.2em;
      font-size: 1em;
      color: #333;
    }
    .miembro-contacto {
      display: flex;
      align-items: center;
      gap: 1.7em;
      margin-top: 0.7em;
    }
    .miembro-contacto-item {
      display: flex;
      align-items: center;
      font-size: 0.98em;
      color: #19306c;
      background: #e8ecef;
      padding: 0.35em 0.95em;
      border-radius: 16px;
      margin-right: 0.5em;
      gap: 0.7em;
      text-decoration: none;
      transition: background 0.2s;
    }
    .miembro-contacto-item:hover {
      background: #fdbe5d55;
    }
    .miembro-contacto-icon {
      font-size: 1.12em;
      margin-right: 0.35em;
    }
    .elegir-section {
      margin-top: 3.2em;
      background: #f4f6fa;
      border-radius: 12px;
      padding: 0 0 2.2em 0;
      overflow: hidden;
      box-shadow: 0 1px 10px rgba(32,46,80,0.06);
    }
    .elegir-img-container {
      width: 100%;
      background: #19306c;
      display: flex;
      align-items: flex-end;
      justify-content: flex-start;
      position: relative;
      height: 260px;
    }
    .elegir-img {
      display: block;
      width: 82%;
      max-width: 480px;
      margin-left: 4.5%;
      margin-top: 2.7em;
      border-radius: 0 0 0 0;
      box-shadow: 0 2px 14px rgba(32,46,80,0.07);
      z-index: 2;
      position: relative;
    }
    .elegir-bar {
      position: absolute;
      right: 0;
      top: 70%;
      width: 60px;
      height: 50px;
      background: #fdbe5d;
      z-index: 1;
      border-radius: 0 0 0 18px;
    }
    .elegir-content {
      padding: 2.5em 2.2em 0.5em 2.2em;
    }
    .elegir-title {
      color: #19306c;
      font-size: 2em;
      font-weight: bold;
      margin-bottom: 1.05em;
      margin-top: 0.1em;
      letter-spacing: -1.5px;
    }
    .elegir-list {
      font-size: 1.07em;
      margin-bottom: 1.8em;
      margin-top: 0.8em;
      margin-left: 0;
      padding-left: 0;
      list-style: none;
    }
    .elegir-list li {
      margin-bottom: 0.65em;
    }
    .elegir-list strong,
    .elegir-list b {
      color: #19306c;
    }
    .elegir-contact {
      margin-top: 1.3em;
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 1.4em;
      font-size: 1em;
    }
    .elegir-contact-label {
      color: #19306c;
      font-weight: bold;
      margin-right: 0.7em;
    }
    .elegir-contact-link {
      color: #19306c;
      text-decoration: none;
      background: #fff;
      padding: 0.3em 1em;
      border-radius: 15px;
      display: flex;
      align-items: center;
      gap: 0.4em;
      font-size: 0.98em;
      border: 1px solid #e8ecef;
      margin-right: 0.5em;
      transition: background 0.2s;
    }
    .elegir-contact-link:hover {
      background: #fdbe5d44;
    }
    .elegir-contact-icon {
      margin-right: 0.3em;
      font-size: 1.15em;
    }
    .elegir-footer {
      border-top: 1px solid #bbb;
      margin-top: 2em;
      padding-top: 0.7em;
      font-size: 0.98em;
      color: #666;
      display: flex;
      justify-content: space-between;
    }
    @media (max-width: 500px) {
      .logo-header { flex-direction: column; align-items: flex-start; gap: 1em; }
      .logo-img-placeholder { width: 90px; height: 50px; font-size: 0.7em; }
      .logo-title { font-size: 1em; }
      h1 { font-size: 1.4em; }
      .container { padding: 12px 4px; }
      .commit-section { padding: 1em 0.4em; }
      .servicios-title, .equipo-title, .elegir-title { font-size: 1.25em; }
      .servicio-block, .miembro-block { padding: 1em 0.5em; }
      .servicio-icon { font-size: 1.1em; left: 0.5em; }
      .elegir-img-container { height: 110px; }
      .elegir-img { width: 90%; max-width: 300px; }
      .elegir-content { padding: 1.2em 0.6em 0.6em 0.6em; }
      .elegir-contact { gap: 0.7em; font-size: 0.93em; }
    }
  </style>
</head>

<body>
  <div class="container">
    <!-- TÍTULO PRINCIPAL CON LOGOTIPO Y SUBTÍTULO -->
    <div class="logo-header">
      <div class="logo-title-group">
        <div class="logo-title">FUNDACIÓN<br>MANACUS</div>
      </div>
      <!-- Espacio reservado para imagen de logotipo/ave -->
      <div class="logo-img-placeholder">
        Aquí va la imagen/logo<br>de la Fundación
      </div>
    </div>
    <!-- CONTENIDO PRINCIPAL SIGUIENTE -->
    <h1>Nuestro objetivo</h1>
    <div class="objetivo">
      Se ha constitutido la Fundación Manacus para promover la preservación y protección del medio ambiente, desde una perspectiva territorial y de derechos, que reconozca la diversidad cultural y social para el ordenamiento, uso y manejo adecuado de los recursos naturales renovables y no renovables; impulsando la implementación de nuevas tecnologías para el monitoreo, conservación y gestión sostenible de la biodiversidad. 
       <div>
       <strong> Conoce más sobre la fundación</strong>  
       <a href="https://drive.google.com/drive/folders/1CbhU2uk9KZeAq2XAYW3GV9nvNxB_VJUJ?usp=drive_link">aquí</a>
       </div>
    </div>
    <div class="desc">
      Esperamos fomentar, gestionar y ejecutar acciones de protección y conservación ambiental, mediante el uso de herramientas tecnológicas como sensores remotos, inteligencia artificial, y otras innovaciones para el monitoreo y manejo de ecosistemas.
    </div>
    <div class="commit-section">
      <span class="commit-title">ESTAMOS</span>
      <span class="commit-subtitle">COMPROMETIDOS CON</span>
      <ul class="commit-list">
        <li class="commit-item">
          <span class="commit-number orange">1</span>
          <div class="commit-content">
            <strong>Preservar</strong> la biodiversidad mediante el uso de tecnologías avanzadas.
          </div>
        </li>
        <li class="commit-item">
          <span class="commit-number">2</span>
          <div class="commit-content">
            <strong>Fortalecer</strong> la toma de decisiones con datos acústicos precisos y análisis automatizados.
          </div>
        </li>
        <li class="commit-item">
          <span class="commit-number">3</span>
          <div class="commit-content">
            <strong>Empoderar</strong> a comunidades, instituciones y empresas con capacidades técnicas en bioacústica
          </div>
        </li>
        <li class="commit-item">
          <span class="commit-number">4</span>
          <div class="commit-content">
            <strong>Innovar</strong> en metodologías de monitoreo para la conservación basada en evidencia
          </div>
        </li>
      </ul>
    </div>
    <div class="servicios-section">
      <h2 class="servicios-title">Nuestros servicios</h2>
      <div class="servicio-block">
        <span class="servicio-icon" aria-label="Gestión">🔬</span>
        <div class="servicio-title">Gestión y ejecución de proyectos de investigación</div>
        <ul class="servicio-list">
          <li>Diseño e implementación de proyectos de investigación con monitoreo acústico pasivo (MAP).</li>
          <li>Líneas base acústicas para Estudios de Impacto Ambiental (EIA).</li>
          <li>Evaluación de biodiversidad mediante grabaciones autónomas y análisis de paisajes sonoros.</li>
          <li>Estudios de indicadores acústicos para evaluar la integridad ecológica.</li>
          <li>Monitoreo de especies de interés (murciélagos, aves, anfibios).</li>
        </ul>
      </div>
      <div class="servicio-block">
        <span class="servicio-icon" aria-label="Asesoría">🛠️</span>
        <div class="servicio-title gray">Asesoría técnica en implementación de monitoreo acústico pasivo</div>
        <ul class="servicio-list">
          <li>Selección, configuración e instalación de equipos.</li>
          <li>Diseño de muestreo para monitoreo a largo plazo.</li>
          <li>Protocolos de muestreo adaptados a ecosistemas prioritarios.</li>
          <li>Integración con otras tecnologías de sensoreamiento remoto [próximamente].</li>
        </ul>
      </div>
      <div class="servicio-block">
        <span class="servicio-icon" aria-label="Datos">📊</span>
        <div class="servicio-title blue">Análisis de datos provenientes de monitoreo acústico pasivo</div>
        <ul class="servicio-list">
          <li>Procesamiento de grabaciones con machine learning y algoritmos de detección automática.</li>
          <li>Comparación de tipos de coberturas mediante huellas acústicas.</li>
          <li>Mapeo de distribución espacial y temporal de vocalizaciones con Sistemas de Información Geográfica (SIG).</li>
        </ul>
      </div>
      <div class="servicio-block">
        <span class="servicio-icon" aria-label="Capacitación">🎓</span>
        <div class="servicio-title yellow">Capacitación y Transferencia Tecnológica</div>
        <ul class="servicio-list">
          <li>Talleres en monitoreo acústico pasivo y grabación acústica enfocado en espectro audible y ultrasonido.</li>
          <li>Charlas en análisis de datos ecoacústicos.</li>
          <li>Apoyo en diseño de estudios aplicados a la conservación.</li>
          <li>Desarrollo de guías metodológicas y manuales técnicos.</li>
        </ul>
      </div>
    </div>
    <div class="equipo-section">
      <h2 class="equipo-title">Equipo de trabajo</h2>
      <div class="miembro-block">
        <div class="miembro-nombre">HOOVER PANTOJA-SÁNCHEZ</div>
        <div class="miembro-cargo">INVESTIGADOR ASOCIADO</div>
        <div class="miembro-desc">
          Ph.D. en Ingeniería Electrónica con formación como Bioingeniero. Cuenta con más de 8 años de experiencia en investigación científica básica y aplicada, enfocada en el desarrollo de nuevas tecnologías y proyectos de bioacústica. A lo largo de su carrera, ha ocupado roles como investigador postdoctoral asociado en la Universidad de Purdue (Indiana, EE.UU) y Curador de la Colección de Sonidos Ambientales del Instituto Humboldt. Su principal interés es el desarrollo de tecnología para la investigación y el monitoreo de biodiversidad a partir de estrategias bioacústicas.
        </div>
        <div class="miembro-contacto">
          <a class="miembro-contacto-item" href="mailto:h.esteban.ps@gmail.com"><span class="miembro-contacto-icon">✉️</span> h.esteban.ps@gmail.com</a>
          <span class="miembro-contacto-item"><span class="miembro-contacto-icon">📱</span> +57 3182738651</span>
        </div>
      </div>
      <div class="miembro-block">
        <div class="miembro-nombre">ANGELA MARÍA MENDOZA-HENAO</div>
        <div class="miembro-cargo">INVESTIGADORA ASOCIADA</div>
        <div class="miembro-desc">
          Bióloga con Maestría y Doctorado en Ciencias Biológicas.<br>
          Investigadora con experiencia en el diseño, gestión y ejecución de proyectos de investigación en ecología, evolución, caracterización y monitoreo a la evaluación de la biodiversidad. Especial énfasis en análisis acústicos, incluyendo detección automática de especies con aplicación en ecosistemas agrícolas y áreas prioritarias de conservación. Experiencia en docencia universitaria de manera presencial y remota. Amplia trayectoria en sesiones de análisis de sonidos, así como en socialización de resultados científicos y educativos. Sus líneas de interés comprenden el desarrollo de indicadores acústicos para evaluar los bases de biodiversidad e implementación de indicadores acústicos en diferentes escenarios a nivel nacional. Ha participado en la curaduría y manejo de colecciones sonoras. Suele integrar el uso de herramientas estadísticas avanzadas y enfoques metodológicos simuladores para la investigación y la gestión de la biodiversidad.
        </div>
        <div class="miembro-contacto">
          <a class="miembro-contacto-item" href="mailto:am.mendozah@gmail.com"><span class="miembro-contacto-icon">✉️</span> am.mendozah@gmail.com</a>
          <span class="miembro-contacto-item"><span class="miembro-contacto-icon">📱</span> +57 3155777881</span>
        </div>
      </div>
      <h2 class="equipo-title" style="margin-top:2.5em;">Equipo de trabajo</h2>
      <div class="miembro-block">
        <div class="miembro-nombre">ANGELA MARIA BARONA-CORTTÉS</div>
        <div class="miembro-cargo">ADMINISTRATIVA</div>
        <div class="miembro-desc">
          Contadora con más de 31 años de experiencia en el área contable y financiera. Cuenta con experiencia en elaboración y análisis de estados financieros, balances, análisis de cartera, elaboración de declaraciones tributarias e impuestos, declaraciones de renta, control interno, presupuestos y flujo de caja. Énfasis en administración de fondos especiales de proyectos financiados por entidades nacionales e internacionales. Clubes Deportivos, entre otros.
        </div>
        <div class="miembro-contacto">
          <a class="miembro-contacto-item" href="mailto:am.barona.cortes@gmail.com"><span class="miembro-contacto-icon">✉️</span> am.barona.cortes@gmail.com</a>
          <span class="miembro-contacto-item"><span class="miembro-contacto-icon">📱</span> +57 3158542217</span>
        </div>
      </div>
    </div>
    <div class="elegir-section">
      <div class="elegir-img-container">
        <img class="elegir-img" src="/workspaces/Manacus/ManacusBosqueWebPage.jpg" alt="Paisaje natural con aves y árboles">
        <div class="elegir-bar"></div>
      </div>
      <div class="elegir-content">
        <div class="elegir-title">¿Porqué elegirnos?</div>
        <ul class="elegir-list">
          <li><strong>Expertos</strong> en ecoacústica con experiencia en múltiples ecosistemas.</li>
          <li><strong>Tecnología</strong> de punta para análisis eficiente de grandes volúmenes de datos.</li>
          <li><strong>Enfoque interdisciplinario</strong> (ecología, acústica, ciencia de datos)</li>
          <li><strong>Compromiso</strong> con la conservación y las comunidades locales.</li>
          <li><b>Aliados estratégicos</b><br>
              Red Ecoacústica Colombiana (REC)<br>
              Instituto Humboldt
          </li>
        </ul>
        <div class="elegir-contact">
          <span class="elegir-contact-label">Contáctanos</span>
          <a class="elegir-contact-link" href="mailto:h.esteban.ps@gmail.com"><span class="elegir-contact-icon">✉️</span> h.esteban.ps@gmail.com</a>
          <a class="elegir-contact-link" href="mailto:am.mendozah@gmail.com"><span class="elegir-contact-icon">✉️</span> am.mendozah@gmail.com</a>
          <span class="elegir-contact-link"><span class="elegir-contact-icon">📞</span> +57 3182738651</span>
          <span class="elegir-contact-link"><span class="elegir-contact-icon">📞</span> +57 3155777881</span>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
