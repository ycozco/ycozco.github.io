---
title: SAS Gym
layout: page
permalink: /projects/sas-gym/
---

<div class="project-page project-gym">
<div class="eyebrow">SaaS · Full Stack · PWA · Infraestructura</div>

# SAS Gym

<p class="lead">Todo el gimnasio dentro de una sola plataforma. SaaS compuesto por API backend, aplicación Flutter Web/PWA, panel administrativo y servicios de datos desplegados mediante Docker.</p>

<div class="project-facts">
  <div class="fact"><strong>Tipo</strong>Plataforma SaaS</div>
  <div class="fact"><strong>Arquitectura</strong>Backend + PWA + Admin + datos</div>
  <div class="fact"><strong>Estado</strong>Base funcional preparada para entorno local y productivo</div>
</div>

## Componentes principales

- API construida con NestJS y TypeScript.
- Acceso a datos mediante Prisma.
- PostgreSQL como base de datos principal.
- Redis para caché y pub/sub.
- Aplicación Flutter Web/PWA.
- Panel administrativo web en React.
- Docker Compose para desarrollo y producción.
- Documentación técnica, operativa y arquitectónica separada.

## Arquitectura

```text
Flutter Web / PWA ─┐
                   ├── NestJS API ── PostgreSQL
React Admin ───────┘       │
                           └── Redis
```

## Tecnologías

<div class="tech-list">
<span>NestJS</span><span>Node.js</span><span>TypeScript</span><span>Prisma</span><span>PostgreSQL</span><span>Redis</span><span>Flutter</span><span>React</span><span>Docker Compose</span>
</div>

## Aspectos técnicos destacables

- Separación clara entre backend, aplicación cliente, panel administrativo e infraestructura.
- Configuración independiente para desarrollo local y producción.
- Despliegue preparado para integrarse con un proxy reverso externo en VPS.
- Variables de entorno versionadas mediante plantillas y secretos excluidos del repositorio.
- Documentación de despliegue y operación para reducir dependencia del entorno del desarrollador.

<div class="callout"><strong>Repositorio:</strong> público. <a target="_blank" rel="noopener" href="https://github.com/ycozco/sas-gym-qp">Ver código y documentación en GitHub →</a></div>

</div>
