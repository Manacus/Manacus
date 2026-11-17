<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="google-site-verification" content="StWd0B-r52YYfce-ykcJZfxL-oWb9af7AhZ-_x0YrIo" />
  <title>Fundación Manacus</title>
  <style>
  @import url('https://fonts.googleapis.com/css2?family=Manrope:wght@400;600;700;800&display=swap');

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
    :root{
      --manacus-primary: #1f5e3b;
      --manacus-secondary: #2f7a52;
      --manacus-accent: #9ed58c;
      --manacus-text: #1f3d2b;
      --manacus-muted: #eef7f1;
      --manacus-white: #ffffff;
    }
    *, *::before, *::after {
      box-sizing: border-box;
    }
    img, svg, video {
      max-width: 100%;
      height: auto;
    }
    .header-manacus {
      width: 100%;
      background: linear-gradient(90deg,var(--manacus-primary), #2b6f49);
      color: #fff;
      box-shadow: 0 8px 28px rgba(7, 27, 45, 0.18);
      padding: 0.6em 0 0.6em 0;
      position: sticky;
      top: 0;
      z-index: 110;
      border-bottom: 1px solid rgba(255,255,255,0.1);
      backdrop-filter: blur(8px);
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
      height: 52px;
      width: auto;
      display: block;
      filter: brightness(1.05);
    }
    .header-nav {
      display: flex;
      gap: 0.6em;
      flex-wrap: wrap;
      align-items: center;
    }
    .header-nav a {
      background: linear-gradient(90deg, #9ed58c, #b7e7a8);
      color: var(--manacus-primary);
      padding: 0.55em 1em;
      border-radius: 999px;
      font-weight: 800;
      text-decoration: none;
      font-size: 0.98em;
      border: 1px solid rgba(255,255,255,0.15);
      transition: transform 0.18s, box-shadow 0.18s;
      box-shadow: 0 4px 14px rgba(9, 31, 50, 0.22);
    }
    .header-nav a:hover {
      box-shadow: 0 8px 18px rgba(9, 31, 50, 0.34);
      transform: translateY(-2px);
    }
    .footer-rec{
      color: var(--manacus-primary);
      font-weight: 700;
      font-size: 1.35em;
      margin-top: 0;
      margin-bottom: 0;
      text-align: center;
    }
    body {
      font-family: 'Manrope', sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(180deg, #f7fcf8 0%, #ffffff 40%);
      color: var(--manacus-text);
      line-height: 1.6;
      overflow-x: hidden;
    }

    .seccion-destacada {
      background: rgba(255,255,255,0.9);
      border-radius: 22px;
      padding: 1.8em 1.5em 1.9em;
      margin: 1.2em auto 0.5em;
      width: min(1000px, calc(100% - 24px));
      box-shadow: 0 12px 35px rgba(13, 44, 72, 0.1);
      border: 1px solid rgba(47, 122, 82, 0.16);
    }

    .hero-callout {
      margin: 1.4em auto 1.6em;
      max-width: 860px;
      padding: clamp(1.2rem, 3vw, 2rem) clamp(1rem, 3.2vw, 2.2rem);
      background: linear-gradient(120deg, var(--manacus-primary), var(--manacus-secondary));
      border-radius: 18px;
      text-align: center;
      box-shadow: 0 12px 30px rgba(12, 43, 70, 0.24);
      position: relative;
      overflow: hidden;
    }

    .hero-callout::before {
      content: "";
      position: absolute;
      inset: -40% auto auto -15%;
      width: 280px;
      height: 280px;
      background: radial-gradient(circle, rgba(158,213,140,0.26), transparent 66%);
      pointer-events: none;
    }

    .hero-eyebrow {
      margin: 0;
      color: #e2f4e7;
      font-size: 0.86em;
      font-weight: 700;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    .hero-title {
      margin: 0.35em 0 0.45em;
      color: #f3fbf5;
      font-size: clamp(1.28rem, 3.1vw, 2rem);
      line-height: 1.2;
      font-weight: 800;
      text-wrap: balance;
    }

    .hero-link {
      display: inline-block;
      padding: 0.75em 1.2em;
      border-radius: 10px;
      background: var(--manacus-accent);
      color: var(--manacus-primary);
      text-decoration: none;
      font-weight: 800;
      box-shadow: 0 8px 18px rgba(10, 25, 40, 0.24);
      transition: transform 0.18s ease, box-shadow 0.18s ease;
      position: relative;
      z-index: 1;
      min-width: 220px;
      text-align: center;
    }

    .hero-link:hover {
      transform: translateY(-2px);
      box-shadow: 0 12px 24px rgba(10, 25, 40, 0.3);
    }

    .hero-links {
      display: flex;
      gap: 0.9em;
      justify-content: center;
      flex-wrap: wrap;
      position: relative;
      z-index: 1;
    }

    .brand-wrap {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 0.5em;
      margin-bottom: 0.5em;
    }

    .brand-logo {
      max-width: 660px;
      width: 100%;
      height: auto;
      display: block;
      background: transparent;
    }

    .rec-logo {
      max-width: 80px;
      width: auto;
      height: auto;
      vertical-align: middle;
      display: inline-block;
      background: #f8fafd;
      margin-left: 0.7em;
    }

    .footer-main {
      width: 100%;
      background: linear-gradient(90deg, #f4faf6, #edf6f0);
      color: var(--manacus-primary);
      text-align: center;
      padding: 1.2em 0;
      font-size: 1.02em;
      margin-top: 2em;
      box-shadow: 0 -1px 8px rgba(25,48,108,0.12);
      border-top: 1px solid rgba(22, 62, 95, 0.12);
      overflow-wrap: anywhere;
    }

    @media (max-width: 900px) {
      .header-content { padding: 0 1rem; }
      .seccion-destacada { border-radius: 16px; }
      .hero-link { min-width: 180px; }
    }

    @media (max-width: 650px){
      .header-content {
        flex-direction: column;
        align-items: stretch;
        gap: 0.7em;
      }
      .header-nav {
        flex-direction: column;
        align-items: stretch;
      }
      .header-nav a {
        width: 100%;
        text-align: center;
      }
      .seccion-destacada {
        width: calc(100% - 12px);
        padding: 0.95rem 0.75rem 1.1rem;
        margin-top: 0.7rem;
      }
      .hero-link { width: calc(100% - 0.8em); box-sizing: border-box; }
      .hero-links { width: 100%; }
      .hero-callout { margin: 1rem auto 1.1rem; border-radius: 14px; }
      .footer-rec { font-size: 1.08em; line-height: 1.45; }
      .rec-logo { margin-left: 0.45em; max-width: 70px; }
      .footer-main {
        padding: 1rem 0.7rem;
        font-size: 0.95em;
      }
    }
  </style>
</head>
<body>
  <header class="header-manacus">
    <div class="header-content">
      <nav class="header-nav">
        <!-- <a href="services/">Investigación</a> -->
        <a href="https://www.manacus.site/" target="_blank" rel="noopener">Visita nuestra página principal</a>
      </nav>
    </div>
  </header>
  <!-- CONTENIDO PRINCIPAL SIGUIENTE -->
  <div class="seccion-destacada">
    <div class="brand-wrap">
      <img src="src/MANACUS_BN_SIN_FONDO.png" alt="Logo Fundación Manacus" class="brand-logo">
    </div>
    <div class="hero-callout">
      <p class="hero-eyebrow">Fundación Manacus</p>
      <h1 class="hero-title">Conservación basada en evidencia, tecnología y territorio</h1>
      <div class="hero-links">
        <a class="hero-link" href="https://www.manacus.site/" target="_blank" rel="noopener">Visita nuestra página principal</a>
        <a class="hero-link" href="projects/puertoTriunfo/">Proyecto Puerto Triunfo</a>
      </div>
    </div>
      <p class="footer-rec">Parte de la Red Ecoacústica Colombiana
        <img src="src/logo_REC.png" alt="Logo REC" class="rec-logo"></p>
  </div>
  <footer class="footer-main">
  contacto@manacus.co | Cali, Valle del Cauca, Colombia | NIT: 901956753 | © 2025 Manacus
  </footer>
</body>
</html>



  






