---
title: INFOUNSA
layout: page
permalink: /projects/infounsa/
---

<div class="project-page project-infounsa">
<div class="eyebrow">Arquitectura · Equipo · Electron · CI/CD</div>

# INFOUNSA

<p class="lead">Una plataforma, múltiples sistemas. Case study de una solución universitaria modular orientada a asistencia, inventario y servicios institucionales, con aplicaciones de escritorio, APIs, bases de datos separadas y automatización de despliegue.</p>

<div class="project-facts">
  <div class="fact"><strong>Tipo</strong>Plataforma modular universitaria</div>
  <div class="fact"><strong>Rol</strong>Project Management, integración y CI/CD</div>
  <div class="fact"><strong>Contexto</strong>Proyecto colaborativo con múltiples módulos</div>
</div>

## Alcance del sistema

INFOUNSA fue planteado como una plataforma modular en la que distintos subsistemas pueden evolucionar de forma relativamente independiente, manteniendo integración común a nivel de despliegue, redes y operación.

### Módulo de asistencia

- API para registro y sincronización de asistencias.
- Aplicación Electron para kiosco de escritorio.
- Lectura de DNI y flujo de registro asistido.
- Persistencia local y sincronización con servidor.
- Manejo transaccional en operaciones de sincronización.
- Base de datos PostgreSQL.

### Módulo de inventario

- API independiente.
- Base de datos PostgreSQL separada.
- Aplicación de escritorio asociada al módulo.
- Servicios y despliegue aislados respecto al módulo de asistencia.

### Portal e infraestructura

- Portal general web.
- Servicios desacoplados por puertos y contenedores.
- Docker y proxy reverso para integración del entorno.
- CI/CD por subproyecto.
- Estructura monorepo modular.

## Arquitectura conceptual

```text
                    INFOUNSA
                       │
        ┌──────────────┼──────────────┐
        │              │              │
        ▼              ▼              ▼
   Asistencia      Inventario       Portal
        │              │              │
   API + Desktop   API + Desktop      Web
        │              │
 PostgreSQL      PostgreSQL
        │
 Electron / almacenamiento local
```

## Tecnologías

<div class="tech-list">
<span>Node.js</span><span>NestJS</span><span>React</span><span>Electron</span><span>PostgreSQL</span><span>SQLite</span><span>Docker</span><span>Nginx</span><span>CI/CD</span>
</div>

## Responsabilidades destacadas

- Coordinación técnica del proyecto y seguimiento de integración.
- Organización del trabajo por subproyectos y responsables.
- Definición y mantenimiento del flujo CI/CD.
- Integración entre aplicaciones de escritorio, APIs y bases de datos.
- Revisión de despliegue y documentación técnica.

<div class="callout"><strong>Nota:</strong> el código principal del proyecto no se publica desde este portafolio. La ficha funciona como case study de arquitectura, integración y trabajo colaborativo.</div>

</div>
