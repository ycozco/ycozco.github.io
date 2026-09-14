---
layout: home
---

<section class="portfolio-hero">
  <div class="hero-kicker">Software Engineering · Architecture · AI · DevOps</div>
  <h1>Construyo sistemas<br><span class="hero-gradient">que funcionan.</span></h1>
  <p>Diseño y desarrollo productos de software con foco en arquitectura, datos, automatización e infraestructura. Esta selección resume proyectos donde el valor está tanto en la experiencia de uso como en las decisiones técnicas que permiten operar y escalar.</p>
  <div class="hero-actions">
    <a class="btn-portfolio btn-primary" href="{{ '/projects/' | relative_url }}">Explorar proyectos</a>
    <a class="btn-portfolio btn-secondary" target="_blank" rel="noopener" href="https://github.com/ycozco">GitHub ↗</a>
  </div>
  <div class="hero-proof">
    <div class="proof-item"><strong>Arquitectura</strong><span>SaaS, modularidad, multi-tenancy y sistemas distribuidos.</span></div>
    <div class="proof-item"><strong>Producto</strong><span>Web, desktop, PWA, APIs y experiencias orientadas a usuarios reales.</span></div>
    <div class="proof-item"><strong>Operación</strong><span>Docker, CI/CD, despliegue, observabilidad y documentación técnica.</span></div>
  </div>
</section>

<div class="section-header">
  <h2>Proyectos destacados.</h2>
  <p>Cinco trabajos seleccionados para mostrar distintas capacidades: producto SaaS, arquitectura, liderazgo técnico, IA aplicada y entrega web empresarial.</p>
</div>

<div class="project-grid">
  <article class="project-card project-card--wide project-crm">
    <span class="project-number">01</span>
    <div class="project-meta">SaaS · Arquitectura · Realtime</div>
    <h3>QP Secure CRM</h3>
    <p>CRM multitenant diseñado para centralizar conversaciones y contactos sin mezclar información entre organizaciones. PostgreSQL RLS protege el aislamiento de datos, mientras Redis, BullMQ y Socket.IO desacoplan integraciones y mantienen el frontend sincronizado en tiempo real.</p>
    <div class="tech-list"><span>NestJS</span><span>PostgreSQL RLS</span><span>Redis</span><span>BullMQ</span><span>Socket.IO</span><span>React</span><span>Docker</span></div>
    <a class="project-link" href="{{ '/projects/qp-secure-crm/' | relative_url }}">Explorar case study →</a>
  </article>

  <article class="project-card project-gym">
    <span class="project-number">02</span>
    <div class="project-meta">SaaS · Full Stack · PWA</div>
    <h3>SAS Gym</h3>
    <p>Plataforma de gestión para gimnasios con API NestJS, cliente Flutter Web/PWA, administración React y servicios PostgreSQL/Redis preparados para ejecución en Docker.</p>
    <div class="tech-list"><span>NestJS</span><span>Flutter</span><span>React</span><span>Prisma</span><span>PostgreSQL</span></div>
    <a class="project-link" href="{{ '/projects/sas-gym/' | relative_url }}">Ver proyecto →</a>
  </article>

  <article class="project-card project-infounsa">
    <span class="project-number">03</span>
    <div class="project-meta">Arquitectura · Equipo · CI/CD</div>
    <h3>INFOUNSA</h3>
    <p>Case study de una plataforma universitaria modular con asistencia, inventario, aplicaciones Electron, APIs y despliegue coordinado entre distintos subproyectos.</p>
    <div class="tech-list"><span>Electron</span><span>NestJS</span><span>PostgreSQL</span><span>Docker</span><span>CI/CD</span></div>
    <a class="project-link" href="{{ '/projects/infounsa/' | relative_url }}">Ver case study →</a>
  </article>

  <article class="project-card project-card--wide project-agro">
    <span class="project-number">04</span>
    <div class="project-meta">IA aplicada · XAI · Data</div>
    <h3>Agro-Intelligence Oversight</h3>
    <p>Software de supervisión para analizar valores FOB en exportaciones agroalimentarias. Integra predicción con XGBoost, detección de anomalías con PyOD, explicaciones TreeSHAP y recuperación de contexto normativo mediante RAG + pgvector.</p>
    <div class="tech-list"><span>Python</span><span>Flask</span><span>XGBoost</span><span>PyOD</span><span>SHAP</span><span>pgvector</span><span>React</span></div>
    <a class="project-link" href="{{ '/projects/agro-intelligence/' | relative_url }}">Explorar sistema →</a>
  </article>

  <article class="project-card project-card--wide project-decolumax">
    <span class="project-number">05</span>
    <div class="project-meta">Web empresarial · SEO · Deployment</div>
    <h3>Decolumax Jardinería</h3>
    <p>Entrega web empresarial enfocada en velocidad, presentación de marca y descubrimiento orgánico. Astro genera una experiencia estática ligera; Docker, Nginx, SSL y SEO técnico completan el flujo de publicación.</p>
    <div class="tech-list"><span>Astro</span><span>Tailwind CSS</span><span>SEO</span><span>Docker</span><span>Nginx</span></div>
    <a class="project-link" href="{{ '/projects/decolumax/' | relative_url }}">Ver proyecto →</a>
  </article>
</div>

<div class="section-header">
  <h2>De código a operación.</h2>
  <p>El objetivo no es solo construir interfaces: es entender cómo se integran frontend, backend, datos, infraestructura y operación dentro de una solución mantenible.</p>
</div>

<div class="project-facts">
  <div class="fact"><strong>Backend & sistemas</strong>NestJS, Node.js, Flask, APIs, workers, WebSockets, integración y diseño modular.</div>
  <div class="fact"><strong>Datos & inteligencia</strong>PostgreSQL, Redis, Prisma, pgvector, XGBoost, PyOD, SHAP y pipelines de análisis.</div>
  <div class="fact"><strong>Infraestructura</strong>Docker, Nginx, VPS, CI/CD, automatización, despliegue y documentación operativa.</div>
</div>
