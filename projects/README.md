<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Proyectos | Fundación Manacus</title>
  <style>
    /* utilidades responsivas compartidas */
    body { font-family: 'Arial', sans-serif; background: #f9f9f9; color: #232323; margin: 0; padding: 0; }
    .page-container { max-width: 1100px; margin: 0 auto; padding: 36px 20px; background: #fff; border-radius: 12px; box-shadow: 0 1px 10px rgba(32,46,80,0.06); }
    .container { max-width: 900px; margin: 0 auto; padding: 32px 16px; background: #fff; border-radius: 12px; box-shadow: 0 1px 10px rgba(32,46,80,0.06); }
    img.responsive{ max-width:100%; height:auto; display:block; }
    .banner-proyecto {
      width: 100%;
      height: 240px;
      border-radius: 10px;
      box-shadow: 0 4px 18px rgba(0,0,0,0.12);
      margin-bottom: 1.2em;
      overflow: hidden;
      position: relative;
      /* eliminar fondo gris: la imagen ahora ocupa todo el área */
      background: none;
    }
    /* imagen ocupa todo el banner y se alinea a la derecha */
    .banner-proyecto img.banner-img {
      position: absolute;
      right: 0;
      top: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: right center;
      filter: brightness(0.93) saturate(0.95);
      z-index: 0;
      transition: transform 0.3s ease;
    }
    /* máscara para suavizar la transición desde la izquierda hacia la imagen:
       gradiente de opacidad (de blanco -> transparente) colocado encima de la imagen */
    .banner-proyecto::before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      bottom: 0;
      width: 55%;
      /* degradado que va de blanco opaco a transparente para que la imagen se desvanezca hacia la izquierda */
      background: linear-gradient(to right, rgba(255,255,255,0.95), rgba(255,255,255,0.0));
      pointer-events: none;
      z-index: 1;
    }
    .banner-proyecto .banner-overlay {
      position:absolute; left:32px; bottom:20px; background:rgba(0,0,0,0.45); color:#fff; padding:14px 18px; border-radius:8px; max-width:60%; box-shadow:0 6px 18px rgba(0,0,0,0.28); z-index:2;
    }
    .banner-proyecto .banner-overlay h2{ margin:0 0 6px 0; font-size:1.4em; }
    .banner-proyecto .banner-overlay p{ margin:0; font-size:1em; }
  @media (max-width: 900px) { .banner-proyecto{ height:180px } .banner-proyecto .banner-overlay{ left:16px; bottom:14px; max-width:68%; padding:12px } }
  @media (max-width: 480px) { .banner-proyecto{ height:120px } .banner-proyecto .banner-overlay{ left:10px; right:10px; bottom:10px; max-width:none; padding:8px } .banner-proyecto .banner-overlay h2{ font-size:1.05em } }
  /* contenedor adaptativo para móviles y tablets */
  @media (max-width: 980px){ .page-container{ padding:24px 14px } }
  @media (max-width: 650px){ .page-container{ padding:18px 12px; border-radius:8px } }
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
  <div class="banner-proyecto" role="img" aria-label="Banner proyectos">
    <img src="src\Banner extended.jpeg" alt="Banner proyectos" class="banner-img">
    <div class="banner-overlay">
      <h2>Proyectos</h2>
      <p>Iniciativas locales que integran tecnología, ciencia y comunidad para proteger la biodiversidad.</p>
    </div>
  </div>
    <div class="proyecto-block">
      <div class="proyecto-title">Puerto Triunfo <a href="puertoTriunfo/" target="_blank">- visitar</a> </div>
      <div class="proyecto-desc">La vereda Nápoles, poblada por familias que recibieron las tierras tras la incautación y redistribución de la antigua Hacienda Nápoles, limita con un gran parque de atracciones y lagos con hipopótamos; allí varias familias impulsan proyectos de restauración forestal para proteger aves, monos, ardillas y otros animales. En 2025 Manacus, junto a la antropóloga Alejandra Osejo trabajó con las familias instalando sensores de monitoreo acústico en dos iniciativas locales: un cultivo agroforestal de cacao liderado por la familia de “Chocolate Napol's” y un santuario de abejas llamado “Vibsionary Rescuin the Planet”</div>
    </div>
    <a href="../" class="back-btn">← Volver a la página anterior</a>
  </div>
</body>
</html>
