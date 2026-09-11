---
title: QP Secure CRM
layout: page
permalink: /projects/qp-secure-crm/
---

<div class="project-page">
<div class="eyebrow">SaaS · Arquitectura · Backend · Realtime</div>

# QP Secure CRM

<p class="lead">Sistema SaaS CRM multitenant orientado a centralizar contactos y conversaciones, con aislamiento de datos por tenant, procesamiento asíncrono e interacción en tiempo real.</p>

<div class="project-facts">
  <div class="fact"><strong>Tipo</strong>SaaS CRM multitenant</div>
  <div class="fact"><strong>Rol técnico</strong>Arquitectura, backend, infraestructura e integración</div>
  <div class="fact"><strong>Estado</strong>MVP funcional con pruebas e integración continua</div>
</div>

## Qué problema aborda

La solución busca centralizar la operación comercial de distintas organizaciones sin mezclar sus datos. Cada tenant trabaja sobre la misma plataforma, pero sus registros permanecen aislados mediante políticas de seguridad a nivel de fila en PostgreSQL.

## Funcionalidades implementadas

- Gestión de tenants y resolución por subdominio.
- Autenticación con JWT y bcrypt.
- Roles `ADMIN` y `SELLER` con RBAC.
- Gestión de contactos y conversaciones.
- Inbox omnicanal en tiempo real.
- Procesamiento de webhooks de integraciones externas.
- Worker asíncrono para colas y tareas de integración.
- Redis Pub/Sub y Socket.IO para actualización en vivo.
- Rate limiting y logs estructurados.
- Swagger para documentación de API.
- Pruebas unitarias y E2E.
- Pipeline CI con GitHub Actions.

## Arquitectura

```text
Cliente web / React
        │
        ▼
NestJS API Gateway
        │
        ├── PostgreSQL + Row Level Security
        ├── Redis / BullMQ
        ├── Socket.IO
        └── Integration Worker
                  │
                  ▼
          Webhooks / Integraciones
```

## Tecnologías

<div class="tech-list">
<span>Node.js</span><span>TypeScript</span><span>NestJS</span><span>React</span><span>Vite</span><span>PostgreSQL</span><span>Prisma</span><span>Redis</span><span>BullMQ</span><span>Socket.IO</span><span>Docker</span><span>Jest</span>
</div>

## Decisiones técnicas destacadas

- **Multi-tenancy seguro:** uso de PostgreSQL RLS para que el aislamiento no dependa únicamente de filtros a nivel de aplicación.
- **Procesamiento desacoplado:** uso de worker y colas para sacar tareas de integración del ciclo de petición HTTP.
- **Tiempo real:** Redis Pub/Sub distribuye eventos hacia WebSockets para mantener sincronizada la interfaz.
- **Validación:** pruebas E2E cubren aislamiento entre tenants, permisos y flujo de mensajería.

<div class="callout"><strong>Repositorio:</strong> privado. Esta ficha documenta la arquitectura y funcionalidades sin exponer código ni credenciales del proyecto.</div>

</div>
