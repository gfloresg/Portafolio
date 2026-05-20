# Portafolio

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gabriel Flores Guzmán — CV</title>

<style>
  *{
    margin:0;
    padding:0;
    box-sizing:border-box;
  }

  :root{
    --bg:#0b1220;
    --card:#111b2e;
    --card2:#16233b;
    --accent:#2dd4a0;
    --text:#e6edf7;
    --muted:#9aa8bd;
    --border:rgba(255,255,255,0.08);
  }

  body{
    background:linear-gradient(180deg,#08101c 0%, #0f172a 100%);
    color:var(--text);
    font-family:Inter,Segoe UI,sans-serif;
    padding:40px 20px;
    line-height:1.6;
  }

  .container{
    max-width:1100px;
    margin:auto;
  }

  .card{
    background:rgba(17,27,46,0.95);
    border:1px solid var(--border);
    border-radius:22px;
    overflow:hidden;
    backdrop-filter:blur(10px);
    box-shadow:0 20px 60px rgba(0,0,0,.45);
  }

  .header{
    padding:50px;
    border-bottom:1px solid var(--border);
    display:flex;
    justify-content:space-between;
    gap:40px;
    flex-wrap:wrap;
  }

  .tag{
    color:var(--accent);
    text-transform:uppercase;
    letter-spacing:.18em;
    font-size:.75rem;
    margin-bottom:14px;
    font-weight:600;
  }

  .name{
    font-size:3rem;
    line-height:1;
    font-weight:800;
    margin-bottom:14px;
  }

  .name span{
    color:var(--accent);
  }

  .title{
    color:var(--muted);
    max-width:650px;
    font-size:1rem;
  }

  .contact{
    display:flex;
    flex-direction:column;
    gap:10px;
    min-width:250px;
  }

  .contact a{
    color:var(--muted);
    text-decoration:none;
    transition:.2s;
  }

  .contact a:hover{
    color:var(--accent);
  }

  .main{
    display:grid;
    grid-template-columns:2fr 1fr;
  }

  .left{
    padding:45px;
    border-right:1px solid var(--border);
  }

  .right{
    padding:45px 35px;
    background:rgba(255,255,255,0.02);
  }

  .section{
    margin-bottom:42px;
  }

  .section-title{
    display:flex;
    align-items:center;
    gap:12px;
    margin-bottom:20px;
    color:var(--accent);
    text-transform:uppercase;
    letter-spacing:.14em;
    font-size:.8rem;
    font-weight:700;
  }

  .section-title::after{
    content:"";
    flex:1;
    height:1px;
    background:var(--border);
  }

  .about{
    color:#c7d2e2;
    font-size:.98rem;
  }

  .item{
    background:rgba(255,255,255,0.03);
    border:1px solid var(--border);
    border-left:3px solid var(--accent);
    border-radius:14px;
    padding:20px;
    margin-bottom:14px;
  }

  .item-title{
    font-weight:700;
    margin-bottom:4px;
  }

  .item-sub{
    color:var(--muted);
    font-size:.95rem;
    margin-bottom:8px;
  }

  .item-text{
    color:#c8d2e1;
    font-size:.93rem;
  }

  .skill-group{
    margin-bottom:28px;
  }

  .skill-group h4{
    margin-bottom:12px;
    color:var(--muted);
    font-size:.82rem;
    letter-spacing:.08em;
    text-transform:uppercase;
  }

  .skills{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
  }

  .skill{
    padding:7px 12px;
    border-radius:999px;
    border:1px solid rgba(45,212,160,0.25);
    background:rgba(45,212,160,0.08);
    color:var(--accent);
    font-size:.82rem;
  }

  .lang{
    display:flex;
    justify-content:space-between;
    margin-bottom:10px;
    color:#dce6f4;
  }

  .lang span:last-child{
    color:var(--muted);
  }

  .footer{
    padding:20px 40px;
    border-top:1px solid var(--border);
    display:flex;
    justify-content:space-between;
    color:rgba(255,255,255,.35);
    font-size:.75rem;
    flex-wrap:wrap;
    gap:10px;
  }

  @media(max-width:900px){

    .main{
      grid-template-columns:1fr;
    }

    .left{
      border-right:none;
      border-bottom:1px solid var(--border);
    }

    .header{
      padding:35px;
    }

    .left,
    .right{
      padding:35px;
    }

    .name{
      font-size:2.4rem;
    }
  }

  @media(max-width:600px){

    body{
      padding:15px;
    }

    .header,
    .left,
    .right{
      padding:24px;
    }

    .name{
      font-size:2rem;
    }

    .title{
      font-size:.92rem;
    }
  }
</style>
</head>

<body>

<div class="container">

  <div class="card">

    <!-- HEADER -->
    <div class="header">

      <div>
        <div class="tag">Currículum Vitae</div>

        <div class="name">
          Gabriel Benjamin<br>
          Ignacio <span>Flores</span> Guzmán
        </div>

        <div class="title">
          Estudiante de Ingeniería de Ejecución en Informática orientado al desarrollo Full Stack, bases de datos y soluciones web modernas.
        </div>
      </div>

      <div class="contact">
        <a href="mailto:gabofloresg06@gmail.com">
          ✉ gabofloresg06@gmail.com
        </a>

        <div>📍 Chillán, Chile</div>

        <div>📞 +56 9 6637 2650</div>

        <a href="https://github.com/gfloresg" target="_blank">
          💻 github.com/gfloresg
        </a>

        <a href="https://linkedin.com/in/gabriel-benjamin-ignacio-flores-guzman" target="_blank">
          🔗 LinkedIn
        </a>
      </div>

    </div>

    <!-- BODY -->
    <div class="main">

      <!-- LEFT -->
      <div class="left">

        <!-- SOBRE MI -->
        <div class="section">

          <div class="section-title">
            Sobre mí
          </div>

          <p class="about">
            Estudiante de último año de Ingeniería de Ejecución en Informática con experiencia en desarrollo web, análisis de datos y proyectos académicos orientados a soluciones reales. He trabajado en aplicaciones Full Stack, bases de datos y metodologías ágiles, desarrollando habilidades técnicas y colaborativas para enfrentar entornos profesionales modernos.
          </p>

        </div>

        <!-- EDUCACION -->
        <div class="section">

          <div class="section-title">
            Educación
          </div>

          <div class="item">
            <div class="item-title">
              Ingeniería de Ejecución en Informática
            </div>

            <div class="item-sub">
              Universidad Católica de la Santísima Concepción · Chillán, Chile
            </div>

            <div class="item-text">
              2023 — Actualidad · Egreso estimado 2025
            </div>
          </div>

        </div>

        <!-- PROYECTOS -->
        <div class="section">

          <div class="section-title">
            Proyectos
          </div>

          <div class="item">
            <div class="item-title">
              Sitios web y e-commerce
            </div>

            <div class="item-sub">
              Proyectos universitarios y personales
            </div>

            <div class="item-text">
              Desarrollo de páginas web para tiendas y sistemas publicitarios utilizando HTML, CSS, JavaScript, bases de datos y lógica backend.
            </div>
          </div>

          <div class="item">
            <div class="item-title">
              Análisis de datos empresariales
            </div>

            <div class="item-sub">
              Trasmerino · Trabajo voluntario
            </div>

            <div class="item-text">
              Levantamiento de requerimientos, análisis de datos y apoyo tecnológico orientado a la mejora de procesos empresariales.
            </div>
          </div>

        </div>

        <!-- EXPERIENCIA -->
        <div class="section">

          <div class="section-title">
            Experiencia
          </div>

          <div class="item">
            <div class="item-title">
              Práctica Profesional — Desarrollo Web
            </div>

            <div class="item-sub">
              Colegio Bernardo O'Higgins · Chillán
            </div>

            <div class="item-text">
              Diseño e implementación de base de datos para sitio institucional.
            </div>
          </div>

          <div class="item">
            <div class="item-title">
              Práctica Profesional — Infraestructura y Sistemas
            </div>

            <div class="item-sub">
              Colegio Santa María · Chillán
            </div>

            <div class="item-text">
              Inventariado de equipos, clonación de computadores y mapeo de infraestructura de red.
            </div>
          </div>

          <div class="item">
            <div class="item-title">
              Proyectos Semestrales
            </div>

            <div class="item-sub">
              Universidad Católica de la Santísima Concepción
            </div>

            <div class="item-text">
              Desarrollo de soluciones funcionales utilizando Scrum, Kanban, bases de datos, interfaces gráficas y análisis de datos.
            </div>
          </div>

        </div>

      </div>

      <!-- RIGHT -->
      <div class="right">

        <!-- TECNOLOGIAS -->
        <div class="section">

          <div class="section-title">
            Tecnologías
          </div>

          <div class="skill-group">
            <h4>Lenguajes</h4>

            <div class="skills">
              <div class="skill">Java</div>
              <div class="skill">C#</div>
              <div class="skill">Python</div>
              <div class="skill">JavaScript</div>
              <div class="skill">PHP</div>
            </div>
          </div>

          <div class="skill-group">
            <h4>Desarrollo Web</h4>

            <div class="skills">
              <div class="skill">HTML</div>
              <div class="skill">CSS</div>
              <div class="skill">Bootstrap</div>
              <div class="skill">Node.js</div>
              <div class="skill">Django</div>
            </div>
          </div>

          <div class="skill-group">
            <h4>Bases de Datos</h4>

            <div class="skills">
              <div class="skill">SQL Server</div>
              <div class="skill">MySQL</div>
              <div class="skill">PostgreSQL</div>
              <div class="skill">MongoDB</div>
            </div>
          </div>

          <div class="skill-group">
            <h4>Herramientas</h4>

            <div class="skills">
              <div class="skill">Git</div>
              <div class="skill">GitHub</div>
              <div class="skill">VS Code</div>
              <div class="skill">Visual Studio</div>
              <div class="skill">Power BI</div>
              <div class="skill">Tableau</div>
              <div class="skill">REST APIs</div>
            </div>
          </div>

        </div>

        <!-- IDIOMAS -->
        <div class="section">

          <div class="section-title">
            Idiomas
          </div>

          <div class="lang">
            <span>Español</span>
            <span>Nativo</span>
          </div>

          <div class="lang">
            <span>Inglés</span>
            <span>Básico — Intermedio</span>
          </div>

        </div>

        <!-- HABILIDADES -->
        <div class="section">

          <div class="section-title">
            Capacidades
          </div>

          <div class="skills">
            <div class="skill">Frontend</div>
            <div class="skill">Backend</div>
            <div class="skill">Bases de datos</div>
            <div class="skill">Chatbots</div>
            <div class="skill">Análisis de datos</div>
            <div class="skill">Trabajo en equipo</div>
            <div class="skill">Aprendizaje rápido</div>
            <div class="skill">Interfaces gráficas</div>
          </div>

        </div>

      </div>

    </div>

    <!-- FOOTER -->
    <div class="footer">
      <div>
        GABRIEL FLORES GUZMÁN · 2026
      </div>

      <div>
        CHILLÁN · CHILE
      </div>
    </div>

  </div>

</div>

</body>
</html>
