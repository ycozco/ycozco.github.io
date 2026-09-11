---
title: Agro-Intelligence Oversight
layout: page
permalink: /projects/agro-intelligence/
---

<div class="project-page">
<div class="eyebrow">IA aplicada · XAI · Datos · Full Stack</div>

# Agro-Intelligence Oversight

<p class="lead">Sistema de análisis de valor FOB declarado en exportaciones agroalimentarias. Combina predicción, detección de anomalías, explicabilidad y recuperación normativa dentro de una aplicación web de supervisión.</p>

<div class="project-facts">
  <div class="fact"><strong>Origen</strong>Software desarrollado como componente tecnológico de tesis</div>
  <div class="fact"><strong>Enfoque</strong>Análisis de valor FOB y alertas operativas</div>
  <div class="fact"><strong>Estado</strong>Pipeline IA y vistas principales implementadas</div>
</div>

## Qué hace el sistema

El flujo principal toma información de operaciones de exportación y evalúa posibles desviaciones en el valor FOB declarado. El objetivo es priorizar casos que requieren revisión, explicar por qué fueron considerados anómalos y asociar contexto normativo relevante.

## Pipeline implementado

1. **Predicción FOB esperado con XGBoost.**
2. **Detección de anomalías con ensemble PyOD** usando Isolation Forest, LOF y ECOD.
3. **Explicabilidad local con TreeSHAP** para identificar qué variables impulsan la desviación.
4. **RAG con PostgreSQL + pgvector** para recuperar normativa y producir contexto trazable.

## Arquitectura

```text
Datos de exportación
        │
        ▼
XGBoost → FOB esperado
        │
        ▼
PyOD Ensemble → score de anomalía
        │
        ▼
TreeSHAP → explicación por variables
        │
        ▼
RAG + pgvector → contexto normativo
        │
        ▼
Frontend de supervisión / decisión
```

## Componentes implementados

- Backend Flask con endpoints de autenticación, alertas, configuración, dashboard y telemetría.
- PostgreSQL con pgvector.
- Modelos de usuarios, alertas, decisiones, explicaciones SHAP, documentos normativos y logs de seguridad.
- Frontend con login, dashboard, alertas, historial, telemetría, integridad/fairness, explorador de datos, configuración y usuarios.
- Autoentrenamiento y serialización de modelos al iniciar el entorno.
- Docker Compose con frontend, backend y base de datos.

## Tecnologías

<div class="tech-list">
<span>Python</span><span>Flask</span><span>XGBoost</span><span>PyOD</span><span>SHAP</span><span>PostgreSQL</span><span>pgvector</span><span>React</span><span>Docker</span><span>Nginx</span>
</div>

## Qué se muestra aquí

Esta ficha se enfoca únicamente en el **software desarrollado** y su arquitectura técnica. La investigación académica sirve como contexto, pero no es el centro del portafolio.

<div class="callout"><strong>Repositorio:</strong> público. <a target="_blank" href="https://github.com/ycozco/tesis_v1_md">Ver código y documentación en GitHub →</a></div>

</div>
