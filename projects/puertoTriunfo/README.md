
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Escuchar para convivir</title>
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
        .container{ max-width:1200px; margin:24px auto; padding:0 18px; display:grid; grid-template-columns: repeat(auto-fill,minmax(260px,1fr)); gap:20px; align-items:start; overflow:hidden; position:relative; }
        @media (max-width: 900px) {
            .container {
                grid-template-columns: repeat(auto-fill,minmax(220px,1fr));
                gap:14px;
                padding:0 8px;
            }
            .card img {
                height:140px;
            }
        }
        @media (max-width: 600px) {
            .container {
                grid-template-columns: 1fr;
                gap:10px;
                padding:0 4px;
            }
            .card {
                padding-bottom:6px;
                border-radius:8px;
            }
            .card img {
                height:100px;
                border-radius:8px 8px 0 0;
            }
        }
        /* Tarjetas con estilo coherente */
        .card{ background: linear-gradient(180deg,#ffffff,#fbfdff); border-radius:12px; padding-bottom:10px; overflow:hidden; text-align:center; box-shadow:0 10px 30px rgba(11,32,56,0.06); border:1px solid var(--manacus-card-border); }
        .card img{ width:100%; height:180px; object-fit:cover; display:block; border-bottom:1px solid #eef3fb; }
        .card h3{ margin:10px 12px; color:var(--manacus-primary); font-size:1.02em; }
        .card audio{ width:92%; margin:8px auto 14px; display:block; }
        /* Sección principal del reproductor/hero */
        .hero-audio{ grid-column: 1 / -1; display:flex; justify-content:center; padding:10px; }
        .hero-card{ width:100%; max-width:760px; border-radius:12px; overflow:hidden; }
        /* Texto introductorio */
        p.lead{ text-align:left; font-style:italic; margin:18px auto; max-width:1000px; color:#12314f; line-height:1.5; }
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
        /* Marco que alinea el contenido central */
        .page-frame{
            max-width:1100px;
            margin:18px auto;
            padding:22px;
            background: #ffffff;
            border-radius:12px;
            box-shadow: 0 12px 36px rgba(11,32,56,0.06);
            border:1px solid rgba(15,53,95,0.06);
            overflow:hidden;
            position:relative;
        }
        @media (max-width:700px){ .page-frame{ padding:14px; margin:12px; } }
    /* Reglas del header global (coherencia con la página principal) */
    .header-manacus { width: 100%; background: linear-gradient(90deg,var(--manacus-primary), #153a68); color: #fff; box-shadow: 0 2px 18px rgba(11,32,56,0.12); padding: 0.6em 0; position: sticky; top: 0; z-index: 110; border-bottom: 1px solid rgba(255,255,255,0.04); }
    .header-content { max-width: 1200px; margin: 0 auto; display: flex; align-items: center; justify-content: space-between; gap: 2em; padding: 0 2em; }
    .header-logo { display: flex; align-items: center; gap: 1em; }
    .header-logo img { height: 48px; width: auto; display: block; filter: brightness(1.1); }
    .header-nav { display: flex; gap: 0.6em; flex-wrap: wrap; align-items: center; }
    .header-nav a { background: transparent; color: #fff; padding: 0.45em 0.9em; border-radius: 8px; font-weight: 700; text-decoration: none; font-size: 0.98em; border: 1px solid transparent; transition: background 0.18s, transform 0.18s; }
    .header-nav a:hover { background: rgba(255,209,102,0.12); transform: translateY(-2px); }
        .services-section{ max-width:1200px;margin:2.2em auto;padding:0 2em; }
    .services-header{ text-align:left;margin-bottom:1em }
        .service-grid{ display:grid; grid-template-columns: repeat(2,1fr); gap:1.15em }
            .service-card{ background:linear-gradient(180deg, #ffffff, #fbfdff); border-radius:12px; padding:1.1em; box-shadow:0 6px 22px rgba(11,32,56,0.06); border:1px solid rgba(15,53,95,0.06); transition: transform 0.22s ease, box-shadow 0.22s ease }
            .service-card:hover{ transform: translateY(-8px); box-shadow:0 22px 48px rgba(11,32,56,0.12) }
            .service-card .ic{ font-size:2.15em; margin-bottom:0.6em }
            .service-card h3{ margin:0 0 0.5em;color:var(--manacus-primary) }
            .service-card p{ margin:0;color:#4b5568 }
            /* Espacio para foto y enlace dentro de cada service-card */
            .service-card .service-media{ height:120px; border-radius:8px; overflow:hidden; background:#f1f5f9; display:flex; align-items:center; justify-content:center; margin-bottom:10px; border:1px dashed rgba(15,53,95,0.04); }
            .service-card .service-media img{ width:100%; height:100%; object-fit:cover; display:block }
            .service-card .service-link{ margin-top:12px }
            .service-card .service-link a{ display:inline-block; padding:8px 12px; border-radius:8px; background:var(--manacus-primary); color:#fff; text-decoration:none; font-weight:700 }
            .service-card .service-link a:hover{ background:#113156 }
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
                        <img src="src/MANACUS_BN_SIN_FONDO.png" alt="Logo Fundación Manacus" style="background:rgba(32,46,80,0.06);">
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
    <div class="page-frame">
    <h2>Escuchar para convivir: reconstruyendo la historia de Nápoles a través del sonido de los animales</h2>
    <p class="lead">
        La vereda Nápoles está habitada por familias beneficiarias de programas de redistribución de tierras por parte del gobierno colombiano en una zona históricamente afectada por la violencia. Estos predios se ubican en la frontera de un gran parque de diversiones y cerca de lagos actualmente habitados por hipopótamos.
        En este lugar, algunas familias han desarrollado proyectos para el cuidado y la restauración del bosque, con el objetivo de proteger el hábitat de aves, monos, ardillas y otros animales que comparten el espacio con ellos.
        De febrero a junio de 2025, un grupo interdisciplinario de biólogos, antropólogos e ingenieros nos unimos a estas familias para ayudarlas a escuchar a los animales con los que conviven. Instalamos grabadoras de monitoreo acústico en dos iniciativas de conservación locales.</p>
        <h2>¿Cómo lo hicimos?</h2>
            <ul>
                      <li>Instalamos <a href="https://manacus.github.io/Manacus/tecnologia/Grillos/" target="_blank" rel="noopener">sensores acústicos Grill@s </a> en el cultivo agroforestal de cacao de Chocolate Napol’s y en el bosque del santuario Vibsionary Rescuing the planet ubicados en Napoles. </li>
                      <li>Durante el proceso, todos aprendimos a usar estos dispositivos, y ese aprendizaje contribuyó al ajuste de las grabadoras. </li>
                      <li>Además, en cada lugar buscamos la mejor forma de ubicar los equipos para protegerlos de la lluvia y la humedad. </li>
                      <li>Esta tecnología está diseñada para obtener información acústica de manera contínua, lo que nos permitió conocer cómo suenan estos lugares  incluso cuando no hay personas cerca.</li>
                      <li>De esta forma tenemos una información precisa sobre algunos animales que habitan este territorio. </li>
                      <li>Con este ejercicio obtuvimos grabaciones que pudieron ser analizadas para encontrar las especies que habitan en cada sitio.</li> 
                      </ul>
    <div class="seccion-destacada" style="background:#f8fafd;border-radius:12px;padding:1.2em 1em;margin-bottom:0.5em;box-shadow:0 1px 10px rgba(32,46,80,0.06);max-width:1000px;margin-left:auto;margin-right:auto;">
    <div style="width:100%;display:flex;justify-content:center;align-items:center;margin-top:0.5em;margin-bottom:0.5em;">
    <img src="src/Collage.png" alt="Logo Fundación Manacus" style="max-width:660px;width:100%;height:auto;display:block;background:#f8fafd">
    </div> 
    <section class="hero-audio">
        <div class="hero-card card">
            <h3 style="text-align: center; padding-top:12px;">Escucha aquí el paisaje sonoro de la región</h3>
            <p>Accede a un viaje sonoro construido a partir de los sonidos obtenidos en este ejercicio. Quisimos resaltar las especies que pueden ser escuchadas a medida que avanza el día. Este pequeño viaje empieza en el amanecer, un periodo de gran actividad sonora. A medida que avanza el día, algunos de nuestros músicos emplumados le ceden el turno a los demás, finalizando con esas especies de tonos graves que surgen al anochecer. En todos estos instantes, el entorno revela su identidad a través del eco de la fauna silvestre. Te invitamos a sintonizarte con este paisaje sonoro, recordando nuestra conexión intrínseca con la naturaleza y fomentando la escucha consciente del mundo vivo que nos rodea.</p>
            <audio controls style="display: block; margin: 6px auto;">
                <source src="src/Puerto triunfo.mp3" type="audio/mp3">
                Tu navegador no soporta el elemento de audio.
            </audio>
        </div>
    </section>
        <h2>Biodiversidad en las iniciativas locales</h2>
     <section class="services-section">
      <div class="service-grid">
        <div class="service-card">
          <div class="ic">🐝</div>
          <h3><a href="src/Ficha especies seleccionadas (Vibsionary).pdf" target="_blank" rel="noopener"> Diversidad en el Santuario "Vibsionary Rescuing the Planet" </a></h3>
          <p>Santuario de abejas creado y custodiado por una familia en un bosque que colinda con el parque de atracciones. Entra <a href="https://www.youtube.com/watch?v=px2sKoVeN0I" target="_blank" rel="noopener">aqui </a>para conocer más sobre esta iniciativa local</p>
          <p><a href="https://ebird.org/checklist/S277053898" target="_blank" rel="noopener">Listado completo de aves.</a></p>
          </div>
        <div class="service-card">
          <div class="ic">🍫</div>
          <h3><a href="src/Ficha especies seleccionadas (Chocolate Napols).pdf" target="_blank" rel="noopener"> Compañeros en Chocolate Napol's </a> </h3>
          <p>Es un cultivo agroforestal de cacao, donde la familia ha desarrollado estrategias sostenibles de producción. Entra <a href="https://www.facebook.com/chocolatesnapoles" target="_blank" rel="noopener">aqui</a> para conocer más sobre esta iniciativa local.</p>
          <p><a href="https://ebird.org/checklist/S277056154" target="_blank" rel="noopener">Listado completo de aves.</a></p>
        </div>
      </div>
    </section>
    <h3>A continuación puedes escuchar los sonidos de algunas aves registradas por medio del Monitoreo acústico pasivo en 2025.</h3>
    <div class="container">
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
    </div>
    <footer style="width:100%;background:#f8fafd;color:#19306c;text-align:center;padding:1.2em 0;font-size:1.08em;margin-top:2em;box-shadow:0 -1px 8px #19306c22;">
    <h3>Creditos:</h3>
        <ul>Colaboración desarrollada en el marco de la investigacion doctoral en Antropologia “Presencias inusuales en el Magdalena Medio”</ul>
        <ul>Alejandra Osejo Varona (Rice University) </ul>
        <ul>Apoyada por el Center for Latin American and Latinx Studies (CELAS) de Rice University</ul>
        <ul>Chocolate Napol’s: Diego Marín, Marcela Bernal, Daniel Marín</ul>
        <ul>Equipo Vibsionary Rescuing the planet</ul>
    <h3>Agradecimientos:</h3>
        <ul>Daniel David-Gutierrez</ul>
        contacto@manacus.co | Cali, Valle del Cauca, Colombia | NIT: 9 0 1 9 5 6 7 5 3 | © 2025 Manacus
    </footer>
</body>
</html>
