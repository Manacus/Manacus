
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Escuchar para convivir </title>
    <style>
        :root{
          --manacus-primary: #0f355f; /* deep navy */
          --manacus-accent: #ffd166; /* warm yellow */
          --manacus-muted: #f4f8fb; /* very light */
          --manacus-card-border: rgba(15,53,95,0.06);
        }
        html,body{height:100%;}
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--manacus-muted);
            color: #222;
            -webkit-font-smoothing:antialiased;
        }
        header{
            background: linear-gradient(90deg,var(--manacus-primary), #153a68);
            color: #fff;
            padding: 28px 12px;
            text-align: center;
            box-shadow: 0 2px 18px rgba(11,32,56,0.08);
        }
        header h1{ margin:0; color:var(--manacus-accent); font-size:1.5em; letter-spacing:-0.6px; }
        /* Contenedor principal con ancho limitado */
        .container{ max-width:1200px; margin:24px auto; padding:0 18px; display:grid; grid-template-columns: repeat(auto-fill,minmax(260px,1fr)); gap:20px; align-items:start; }
        /* Tarjetas con estilo coherente */
        .card{ background: linear-gradient(180deg,#ffffff,#fbfdff); border-radius:12px; padding-bottom:10px; overflow:hidden; text-align:center; box-shadow:0 10px 30px rgba(11,32,56,0.06); border:1px solid var(--manacus-card-border); }
        .card img{ width:100%; height:180px; object-fit:cover; display:block; border-bottom:1px solid #eef3fb; }
        .card h3{ margin:10px 12px; color:var(--manacus-primary); font-size:1.02em; }
        .card audio{ width:92%; margin:8px auto 14px; display:block; }
        /* Sección principal del reproductor/hero */
        .hero-audio{ grid-column: 1 / -1; display:flex; justify-content:center; padding:10px; }
        .hero-card{ width:100%; max-width:760px; border-radius:12px; overflow:hidden; }
        /* Texto introductorio */
        p.lead{ text-align:center; font-style:italic; margin:18px auto; max-width:1000px; color:#12314f; line-height:1.5; }
        /* Footer más ligero y coherente */
        footer{ grid-column:1 / -1; text-align:center; padding:20px; color:var(--manacus-primary); background:transparent; }
        footer a{ color:var(--manacus-primary); text-decoration:none; font-weight:600 }
        /* Responsive tweaks */
        @media (max-width:700px){
            header{ padding:18px 8px }
            header h1{ font-size:1.15em }
            .card img{ height:160px }
            p.lead{ padding:0 14px }
        }
    /* Reglas del header global (coherencia con la página principal) */
    .header-manacus { width: 100%; background: linear-gradient(90deg,var(--manacus-primary), #153a68); color: #fff; box-shadow: 0 2px 18px rgba(11,32,56,0.12); padding: 0.6em 0; position: sticky; top: 0; z-index: 110; border-bottom: 1px solid rgba(255,255,255,0.04); }
    .header-content { max-width: 1200px; margin: 0 auto; display: flex; align-items: center; justify-content: space-between; gap: 2em; padding: 0 2em; }
    .header-logo { display: flex; align-items: center; gap: 1em; }
    .header-logo img { height: 48px; width: auto; display: block; filter: brightness(1.1); }
    .header-nav { display: flex; gap: 0.6em; flex-wrap: wrap; align-items: center; }
    .header-nav a { background: transparent; color: #fff; padding: 0.45em 0.9em; border-radius: 8px; font-weight: 700; text-decoration: none; font-size: 0.98em; border: 1px solid transparent; transition: background 0.18s, transform 0.18s; }
    .header-nav a:hover { background: rgba(255,209,102,0.12); transform: translateY(-2px); }
    </style>
</head>
<body>
        <header class="header-manacus">
                <div class="header-content">
                    <div class="header-logo">
                        <img src="/workspaces/Manacus/src/logo_cortado.png" alt="Logo Fundación Manacus" style="background:rgba(32,46,80,0.06);">
                    </div>
                    <nav class="header-nav">
                        <!-- <a href="../services/">Investigación</a> -->
                        <a href="../projects/">Proyectos</a>
                        <a href="../tecnologia/">Tecnología</a>
                        <a href="../quienes/">¿Quiénes somos?</a>
                        <a href="../contacto/">Contacto</a>
                    </nav>
                </div>
        </header>
    <p class="lead">
        La vereda Nápoles está habitada por familias que recibieron sus tierras tras la incautación y redistribución de la antigua Hacienda Nápoles por parte del gobierno colombiano, después de la muerte de Pablo Escobar. Estos predios se ubican en la frontera de un gran parque de diversiones y cerca de lagos habitados por hipopótamos.
        En este lugar, algunas familias han desarrollado proyectos para el cuidado y la restauración del bosque, con el objetivo de proteger el hábitat de aves, monos, ardillas y otros animales que comparten el espacio con ellos.
        De febrero a junio de 2025, un grupo interdisciplinario de biólogos, antropólogos e ingenieros nos unimos a estas familias para ayudarlas a escuchar a los animales con los que conviven. Instalamos grabadoras de monitoreo acústico en dos iniciativas de conservación locales.
        La primera fue en un cultivo agroforestal de cacao, donde la familia detrás de "Chocolate Napol's" ha desarrollado estrategias sostenibles de producción. La segunda fue en un santuario de abejas, llamado "Vibsionary Rescuin the Planet", creado y custodiado por otra familia en un bosque que colinda con el parque de atracciones.
    </p>   
    <section class="hero-audio">
        <div class="hero-card card">
            <h3 style="text-align: center; padding-top:12px;">Escucha aquí el paisaje sonoro de la región</h3>
            <audio controls style="display: block; margin: 6px auto;">
                <source src="src/Puerto triunfo.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
    </section>
    <p class="lead">A continuación puedes escuchar los sonidos de algunas aves registradas por medio del Monitoreo acústico pasivo en 2025.</p>
    <div class="container">
        <!-- Foto 1 -->
        <div class="card">
            <img src="src/Ara ararauna_New.jpg" alt="Foto Ara ararauna">
            <h3><i>Ara ararauna</i></h3>
            <audio controls>
                <source src="src/Ara ararauna.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Crypturellus soui_New.jpeg.png" alt="Foto Crypturellus soui">
            <h3><i>Crypturellus soui</i></h3>
            <audio controls>
                <source src="src/Crypturellus soui.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Megascops choliba_New.png" alt="Foto Megascops choliba">
            <h3><i>Megascops choliba</i></h3>
            <audio controls>
                <source src="src/Megascops choliba.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Ortalis columbiana_New.jpeg.png" alt="Foto Ortalis columbiana">
            <h3><i>Ortalis columbiana</i></h3>
            <audio controls>
                <source src="src/Ortalis columbiana.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Galbula ruficauda_New.jpeg.png" alt="Foto Galbula ruficauda">
            <h3><i>Galbula ruficauda</i></h3>
            <audio controls>
                <source src="src/Galbula ruficauda.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Glaucis hirsutus_New.jpeg.png" alt="Foto Glaucis hirsutus">
            <h3><i>Glaucis hirsutus</i></h3>
            <audio controls>
                <source src="src/Glaucis hirsutus.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Hylophilus flavipes_New.jpg" alt="Foto Hylophilus flavipes">
            <h3><i>Hylophilus flavipes</i></h3>
            <audio controls>
                <source src="src/Hylophilus flavipes.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Lepidocolaptes souleyetii_New.jpg" alt="Foto Lepidocolaptes souleyetii">
            <h3><i>Lepidocolaptes souleyetii</i></h3>
            <audio controls>
                <source src="src/Lepidocolaptes souleyetii.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Stix virgata_new.jpg" alt="Foto Strix virgata">
            <h3><i>Strix virgata</i></h3>
            <audio controls>
                <source src="src/Strix virgata.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Dryocopus lineatus_New.jpg" alt="Foto Dryocopus lineatus">
            <h3><i>Dryocopus lineatus</i></h3>
            <audio controls>
                <source src="src/Dryocopus lineatus.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
        <div class="card">
            <img src="src/Mionectes oleagineus_New.jpg" alt="Foto Mionectes oleagineus">
            <h3><i>Mionectes oleagineus</i></h3>
            <audio controls>
                <source src="src/Mionectes oleagineus.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
    </div>
    <footer>
        <h3>Creditos:  </h3>
            <ul>Alejandra Osejo-Varona, Angela Mendoza-Henao, Hoover Pantoja</ul>
            <ul>Chocolate Napol’s: Diego Marín, Marcela Bernal, Daniel Marín</ul>
            <ul>Vibsionary Rescuin the planet: Johan, et al</ul>
            <h3>Agradecimientos </h3>
            <ul>Daniel David-Gutierrez</ul>
            <p>2025 Manacus. Todos los derechos reservados. | <a href="#">Política de Privacidad</a></p>
    </footer>
</body>
</html>
