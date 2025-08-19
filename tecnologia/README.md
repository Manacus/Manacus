<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Tecnología | Fundación Manacus</title>
  <style>
    body { font-family: 'Arial', sans-serif; background: #f9f9f9; color: #232323; margin: 0; padding: 0; }
    .container { max-width: 900px; margin: 0 auto; padding: 32px 16px; background: #fff; border-radius: 12px; box-shadow: 0 1px 10px rgba(32,46,80,0.06); }
    .banner-tecno {
      width: 100%;
      height: 260px;
      border-radius: 10px;
      box-shadow: 0 4px 18px rgba(0,0,0,0.12);
      margin-bottom: 1.2em;
      overflow: hidden;
      position: relative;
      background: #222;
    }
    .banner-tecno .banner-img {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      transform-origin: center center;
    }
    .banner-tecno .banner-img.mirror {
      transform: scaleX(-1);
    }
    .banner-tecno .banner-overlay {
      position: absolute;
      left: 40px;
      bottom: 28px;
      background: rgba(0,0,0,0.45);
      color: #fff;
      padding: 18px 22px;
      border-radius: 8px;
      max-width: 58%;
      box-shadow: 0 6px 18px rgba(0,0,0,0.28);
    }
    .banner-tecno .banner-overlay h2 {
      margin: 0 0 6px 0;
      font-size: 1.6em;
      line-height: 1.1;
      color: #fff;
    }
    .banner-tecno .banner-overlay p {
      margin: 0;
      font-size: 1em;
      color: #f0f0f0;
      opacity: 0.95;
    }
    @media (max-width: 900px) {
  .banner-tecno { height: 200px; background-position: center center; }
  .banner-tecno .banner-overlay { left: 20px; bottom: 18px; max-width: 64%; padding: 14px 16px; }
    }
    @media (max-width: 480px) {
  .banner-tecno { height: 140px; background-position: center center; }
  .banner-tecno .banner-overlay { left: 12px; right: 12px; bottom: 12px; max-width: none; padding: 10px 12px; }
  .banner-tecno .banner-overlay h2 { font-size: 1.1em; }
  .banner-tecno .banner-overlay p { font-size: 0.95em; }
    }
    h1 { color: #19306c; font-size: 2.2em; font-weight: bold; margin-bottom: 1.2em; }
    .proyecto-block { background: #f9f9f9; border-radius: 10px; box-shadow: 0 1px 6px rgba(32,46,80,0.03); border-left: 10px solid #fdbe5d; padding: 2.2em 2em 2em 4.2em; margin-bottom: 2em; }
    .proyecto-title { color: #19306c; font-size: 1.3em; font-weight: bold; margin-bottom: 0.7em; letter-spacing: -1.5px; }
    .proyecto-desc { color: #232323; font-size: 1.13em; margin-bottom: 1.5em; font-weight: 500; }
    .proyecto-link { display:inline-block; padding:0.9em 2em; background:#19306c; color:#fff; border-radius:10px; font-size:1.08em; font-weight:bold; text-decoration:none; box-shadow:0 1px 8px #19306c22; transition:background 0.2s; }
    .proyecto-link:hover { background:#fdbe5d; color:#19306c; }
    .back-btn { display:flex; justify-content:center; margin-top:2.5em; padding:0.7em 1.6em; background:#19306c; color:#fff; border-radius:10px; font-weight:bold; text-decoration:none; font-size:1.08em; box-shadow:0 1px 6px #19306c22; transition:background 0.2s; }
    .back-btn:hover { background:#fdbe5d; color:#19306c; }
  </style>
</head>
<body>
  <div class="container">
  <div class="banner-tecno" role="img" aria-label="Banner tecnología">
    <img src="src/banner-tecno-01.png" alt="Banner tecnología" class="banner-img mirror">
    <div class="banner-overlay">
      <h2>Tecnología para monitoreo de fauna</h2>
      <p>Herramientas tecnológicas acústicas diseñadas para el estudio de la biodiversidad.</p>
    </div>
  </div>
    <div class="proyecto-block">
  <a href="Grillos/" class="proyecto-title">Grillos</a>
      <div class="proyecto-desc">Sensores acústicos pasivos para monitoreo de fauna</div>
    </div>
    <a href="../" class="back-btn">← Volver a la página anterior</a>
  </div>
</body>
</html>
