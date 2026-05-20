# Portafolio

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CV — Gabriel Flores Guzmán</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --navy: #0f1b2d;
    --navy-mid: #1a2d47;
    --accent: #2dd4a0;
    --accent-dim: #1a7f61;
    --text: #e8edf3;
    --muted: #8a9bb0;
    --border: rgba(255,255,255,0.07);
    --card: rgba(255,255,255,0.04);
    --font: 'DM Sans', sans-serif;
    --mono: 'DM Mono', monospace;
  }

  @media print {
    body { background: var(--navy) !important; padding: 0 !important; }
    .page { box-shadow: none !important; width: 100% !important; }
    .download-btn { display: none !important; }
    @page { size: A4; margin: 0; }
  }

  body {
    font-family: var(--font);
    background: #080f1a;
    color: var(--text);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 40px 20px;
  }

  .page {
    width: 794px;
    background: var(--navy);
    box-shadow: 0 40px 100px rgba(0,0,0,0.6);
    overflow: hidden;
  }

  /* HEADER */
  .header {
    padding: 52px 52px 44px;
    border-bottom: 1px solid var(--border);
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 32px;
    align-items: end;
  }

  .header-left {}

  .tag {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--accent);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 12px;
  }

  .name {
    font-size: 40px;
    font-weight: 600;
    line-height: 1.05;
    letter-spacing: -0.02em;
    color: var(--text);
  }

  .name span {
    color: var(--accent);
  }

  .title {
    margin-top: 10px;
    font-size: 15px;
    font-weight: 300;
    color: var(--muted);
    letter-spacing: 0.01em;
  }

  .contact-grid {
    display: flex;
    flex-direction: column;
    gap: 8px;
    align-items: flex-end;
  }

  .contact-item {
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .contact-item a {
    color: var(--muted);
    text-decoration: none;
    transition: color 0.2s;
  }

  .contact-item a:hover { color: var(--accent); }

  .contact-dot {
    width: 4px;
    height: 4px;
    border-radius: 50%;
    background: var(--accent);
    flex-shrink: 0;
  }

  /* BODY */
  .body {
    display: grid;
    grid-template-columns: 1fr 260px;
    align-items: stretch;
  }

  .main {
    padding: 44px 52px;
    border-right: 1px solid var(--border);
  }

  .sidebar {
    padding: 44px 36px;
    background: var(--navy);
  }

  /* SECTIONS */
  .section {
    margin-bottom: 40px;
  }

  .section:last-child { margin-bottom: 0; }

  .section-label {
    font-family: var(--mono);
    font-size: 10px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .section-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: var(--border);
  }

  /* SOBRE MI */
  .about-text {
    font-size: 14px;
    line-height: 1.75;
    color: #c2cedb;
    font-weight: 300;
  }

  /* EDUCACION */
  .edu-item {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 20px 22px;
    position: relative;
    overflow: hidden;
  }

  .edu-item::before {
    content: '';
    position: absolute;
    left: 0; top: 0; bottom: 0;
    width: 3px;
    background: var(--accent);
    border-radius: 0 2px 2px 0;
  }

  .edu-degree {
    font-size: 14px;
    font-weight: 500;
    color: var(--text);
    margin-bottom: 4px;
  }

  .edu-institution {
    font-size: 13px;
    color: var(--muted);
    margin-bottom: 6px;
  }

  .edu-period {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--accent-dim);
  }

  /* PROYECTOS - placeholder -->  */
  .project-placeholder {
    border: 1px dashed rgba(45, 212, 160, 0.2);
    border-radius: 8px;
    padding: 20px 22px;
    text-align: center;
  }

  .project-placeholder p {
    font-size: 13px;
    color: var(--muted);
    font-style: italic;
  }

  /* SIDEBAR SKILLS */
  .skill-group {
    margin-bottom: 28px;
  }

  .skill-group-title {
    font-size: 12px;
    font-weight: 500;
    color: var(--muted);
    margin-bottom: 10px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    font-size: 11px;
  }

  .skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .skill-tag {
    font-family: var(--mono);
    font-size: 11px;
    background: rgba(45, 212, 160, 0.08);
    border: 1px solid rgba(45, 212, 160, 0.2);
    color: var(--accent);
    padding: 4px 10px;
    border-radius: 4px;
  }

  /* IDIOMAS */
  .lang-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
  }

  .lang-name {
    font-size: 13px;
    color: var(--text);
  }

  .lang-level {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--muted);
  }

  /* FOOTER */
  .footer {
    border-top: 1px solid var(--border);
    padding: 18px 52px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .footer-note {
    font-family: var(--mono);
    font-size: 10px;
    color: rgba(138, 155, 176, 0.4);
    letter-spacing: 0.08em;
  }

  .skill-list {
    display: flex;
    flex-direction: column;
    gap: 5px;
  }

  .skill-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .skill-name {
    font-size: 12px;
    color: var(--text);
  }

  .skill-level {
    font-family: var(--mono);
    font-size: 10px;
    color: var(--accent-dim);
  }

  .accent-bar {
    width: 32px;
    height: 2px;
    background: var(--accent);
    opacity: 0.4;
    border-radius: 1px;
  }
</style>
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
</head>
<body>
<div style="width:794px;margin:0 0 8px;display:flex;justify-content:flex-end;">
  <button class="download-btn" onclick="descargarPDF()" title="Descargar PDF" style="width:28px;height:28px;padding:0;background:transparent;border:1px solid rgba(255,255,255,0.12);border-radius:6px;cursor:pointer;color:var(--muted);font-size:13px;display:flex;align-items:center;justify-content:center;opacity:0.5;transition:opacity 0.2s;" onmouseover="this.style.opacity=1" onmouseout="this.style.opacity=0.5">⬇</button>
</div><div class="page">

  <!-- HEADER -->
  <div class="header">
    <div class="header-left">
      <div class="tag">Currículum Vitae</div>
      <div class="name">Gabriel Benjamin<br>Ignacio <span>Flores</span> Guzmán</div>
      <div class="title">Estudiante de Ingeniería de Ejecución en Informática</div>
    </div>
    <div class="contact-grid">
      <div class="contact-item">
        <div class="contact-dot"></div>
        <a href="mailto:gabofloresg06@gmail.com">gabofloresg06@gmail.com</a>
      </div>
      <div class="contact-item">
        <div class="contact-dot"></div>
        +56 9 6637 2650
      </div>
      <div class="contact-item">
        <div class="contact-dot"></div>
        Chillán, Chile
      </div>
      <div class="contact-item">
        <div class="contact-dot"></div>
        <a href="https://github.com/gfloresg" target="_blank">github.com/gfloresg</a>
      </div>
      <div class="contact-item">
        <div class="contact-dot"></div>
        <a href="https://linkedin.com/in/gabriel-benjamin-ignacio-flores-guzman" target="_blank">LinkedIn</a>
      </div>
    </div>
  </div>

  <!-- BODY -->
  <div class="body">

    <!-- MAIN -->
    <div class="main">

      <!-- SOBRE MÍ -->
      <div class="section">
        <div class="section-label">Sobre mí</div>
        <p class="about-text">
          Estudiante de último año de Ingeniería de Ejecución en Informática, con orientación al desarrollo web Full Stack. Durante mi formación he trabajado en proyectos prácticos que me han dado una visión completa del ciclo de desarrollo de software, desde el diseño hasta la implementación. Soy una persona colaborativa, comprometida y con disposición para seguir aprendiendo en un entorno profesional real. Busco mi primera oportunidad laboral en el área del desarrollo web para aportar mis conocimientos y crecer como desarrollador.
        </p>
      </div>

      <!-- EDUCACIÓN -->
      <div class="section">
        <div class="section-label">Educación</div>
        <div class="edu-item">
          <div class="edu-degree">Ingeniería de Ejecución en Informática</div>
          <div class="edu-institution">Universidad Católica de la Santísima Concepción · Chillán, Chile</div>
          <div class="edu-period">2023 — En curso · Egreso estimado 2025</div>
        </div>
      </div>

      <!-- PROYECTOS -->
      <div class="section">
        <div class="section-label">Proyectos</div>

        <div class="edu-item" style="margin-bottom:12px;">
          <div class="edu-degree">Sitios web — Tiendas y comercio electrónico</div>
          <div class="edu-institution">Proyectos universitarios y personales</div>
          <div class="edu-period">Desarrollo de páginas web para tiendas, e-commerce y sitios publicitarios, aplicando diseño, lógica de negocio e integración con bases de datos.</div>
        </div>

        <div class="edu-item">
          <div class="edu-degree">Análisis de datos para empresas</div>
          <div class="edu-institution">Trasmerino · Trabajo voluntario</div>
          <div class="edu-period">Levantamiento de requerimientos, análisis de datos y entrega de soluciones tecnológicas trabajando directamente con el cliente.</div>
        </div>
      </div>

      <!-- EXPERIENCIA -->
      <div class="section">
        <div class="section-label">Experiencia</div>

        <div class="edu-item" style="margin-bottom:12px;">
          <div class="edu-degree">Práctica profesional — Desarrollo web</div>
          <div class="edu-institution">Colegio Bernardo O'Higgins · Chillán</div>
          <div class="edu-period">Diseño e implementación de base de datos para sitio web institucional.</div>
        </div>

        <div class="edu-item" style="margin-bottom:12px;">
          <div class="edu-degree">Práctica profesional — Infraestructura y sistemas</div>
          <div class="edu-institution">Colegio Santa María · Chillán</div>
          <div class="edu-period">Inventariado de equipos, clonación de equipos y mapeo de la infraestructura de red del colegio (racks, switches y puntos de red).</div>
        </div>

        <div class="edu-item">
          <div class="edu-degree">Proyectos Semestrales</div>
          <div class="edu-institution">Universidad Católica de la Santísima Concepción</div>
          <div class="edu-period">Durante la carrera desarrollé proyectos semestrales basados en casos reales, simulando entornos de trabajo profesional. Cada proyecto incluyó levantamiento de requerimientos, trabajo en equipo, uso de metodologías ágiles (Scrum y Kanban) y entrega de soluciones funcionales como sitios web, bases de datos, interfaces gráficas y análisis de datos.</div>
        </div>
      </div>

    </div>

    <!-- SIDEBAR -->
    <div class="sidebar">

      <!-- HABILIDADES TÉCNICAS -->
      <div class="section">
        <div class="section-label">Tecnologías</div>

        <div class="skill-group">
          <div class="skill-group-title">Lenguajes de programación</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">Java</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">C#</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">Python</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">JavaScript</span><span class="skill-level">Intermedio alto</span></div>
            <div class="skill-row"><span class="skill-name">PHP</span><span class="skill-level">Básico</span></div>
          </div>
        </div>

        <div class="skill-group">
          <div class="skill-group-title">Desarrollo web</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">HTML</span><span class="skill-level">Intermedio alto</span></div>
            <div class="skill-row"><span class="skill-name">CSS</span><span class="skill-level">Intermedio alto</span></div>
            <div class="skill-row"><span class="skill-name">Bootstrap</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">Node.js</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">Django</span><span class="skill-level">Básico</span></div>
          </div>
        </div>

        <div class="skill-group">
          <div class="skill-group-title">Bases de datos</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">SQL Server</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">MySQL</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">PostgreSQL</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">MongoDB</span><span class="skill-level">Básico</span></div>
          </div>
        </div>

        <div class="skill-group">
          <div class="skill-group-title">Sistemas operativos</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">Windows</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">VirtualBox</span><span class="skill-level">Intermedio</span></div>
          </div>
        </div>

        <div class="skill-group">
          <div class="skill-group-title">Herramientas</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">Git</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">GitHub</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">Postman</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">VS Code</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">Visual Studio</span><span class="skill-level">Intermedio</span></div>
            <div class="skill-row"><span class="skill-name">Power BI</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">Tableau</span><span class="skill-level">Básico</span></div>
            <div class="skill-row"><span class="skill-name">APIs REST</span><span class="skill-level">Básico</span></div>
          </div>
        </div>

        <div class="skill-group">
          <div class="skill-group-title">Metodologías</div>
          <div class="skill-list">
            <div class="skill-row"><span class="skill-name">Scrum</span><span class="skill-level">Ágil</span></div>
            <div class="skill-row"><span class="skill-name">Kanban</span><span class="skill-level">Ágil</span></div>
          </div>
        </div>
      </div>

      <!-- IDIOMAS -->
      <div class="section">
        <div class="section-label">Idiomas</div>
        <div class="lang-item">
          <span class="lang-name">Español</span>
          <span class="lang-level">Nativo</span>
        </div>
        <div class="lang-item">
          <span class="lang-name">Inglés</span>
          <span class="lang-level">Básico-Intermedio</span>
        </div>
      </div>

      <!-- HABILIDADES BLANDAS -->
      <div class="section">
        <div class="section-label">Capacidades</div>
        <div class="skill-tags">
          <span class="skill-tag">Desarrollo web: Sitios/Paginas web</span>
          <span class="skill-tag">Interfaces gráficas</span>
          <span class="skill-tag">Bases de datos</span>
          <span class="skill-tag">Chatbots</span>
          <span class="skill-tag">Análisis de datos</span>
          <span class="skill-tag">Trabajo en equipo</span>
          <span class="skill-tag">Aprendizaje rápido</span>
          <span class="skill-tag">Frontend</span>
          <span class="skill-tag">Backend</span>
        </div>
      </div>

    </div>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <span class="footer-note">GABRIEL FLORES GUZMÁN · 2025</span>
    <div class="accent-bar"></div>
    <span class="footer-note">CHILLÁN, CHILE</span>
  </div>

</div>
<script>
function descargarPDF() {
  const elemento = document.querySelector('.page');
  const opciones = {
    margin: 0,
    filename: 'CV_Gabriel_Flores.pdf',
    image: { type: 'jpeg', quality: 1 },
    html2canvas: { scale: 2, useCORS: true },
    jsPDF: { unit: 'px', format: [794, 1123], orientation: 'portrait' }
  };
  html2pdf().set(opciones).from(elemento).save();
}
</script>
</body>
</html>
