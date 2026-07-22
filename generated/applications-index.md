---
type: index
last_updated: 2026-07-20
tags: [index, aplicaciones, tracking, cvs]
---

# Índice de Aplicaciones

Tabla maestra de todas las aplicaciones activas y pausadas: empresa, rol, estado, y dónde vive cada archivo relacionado (CV fuente, PDF, tracking). Actualizar esta tabla cada vez que se crea o modifica una aplicación o CV.

| Empresa | Rol | Estado | CV Fuente (Markdown) | PDF | Tracking | Última actualización |
|---|---|---|---|---|---|---|
| Aplazo | Technical Lead Manager | ⏸️ Pausada (bloqueo por rechazo previo <3 meses) | [cv_for_aplazo-technical-lead-manager.md](../source/cvs/cv_for_aplazo-technical-lead-manager.md) | [PDF](cvs-pdf/diego-reyes-altamirano-aplazo-technical-lead-manager.pdf) | *(sin tracking — no se pudo enviar)* | 2026-07-01 |
| Multiplica Talent | Android Developer (Semi Senior/Senior) | ✅ Submitted (sin respuesta 10 días — ver 2ª aplicación abajo) | [cv_for_multiplica-talent-android-developer.md](../source/cvs/cv_for_multiplica-talent-android-developer.md) | [PDF](cvs-pdf/diego-reyes-altamirano-multiplica-talent-android-developer.pdf) | [multiplica-talent-android-developer-application.md](multiplica-talent-android-developer-application.md) | 2026-07-11 |
| Stori | Tech Manager | ⚫ Cerrada por inactividad (76 días sin feedback) | *(CV hecho fuera de este proyecto, previo al flujo actual — no aplica identificar)* | — | [stori-tech-manager-application.md](stori-tech-manager-application.md) | 2026-07-20 |
| Clara | Mobile Product Lead | Rejected (16-06-2026) | *(CV eliminado 2026-07-01 — contenía datos no verificados: Statsig/Amplitude sin respaldo, "Bilingüe/Fluent" contradice B1 confirmado, fecha de GDG inconsistente con CLAUDE.md)* | — | [clara-mobile-product-lead-application.md](clara-mobile-product-lead-application.md) | 2026-06-16 |
| ALTEN México | Android Developer | ⚫ Cerrada por inactividad (77 días sin feedback) | [cv_for_android.md](../source/cvs/cv_for_android.md) *(confirmado por nombre de archivo: "CV Android.pdf")* | — | [alten-mexico-android-developer-application.md](alten-mexico-android-developer-application.md) | 2026-07-20 |
| Rappi | AI Engineer Mid-level | Rejected (29-04-2026) | *(no identificado — cerrado sin resolver por decisión del usuario, no se investigará más)* | — | [rappi-ai-engineer-application.md](rappi-ai-engineer-application.md) | 2026-05-05 |
| Rappi | AI Engineer (reaplicación) | Rejected (21-07-2026) — "avanzaron con otro candidato" | *(no identificado — cerrado sin resolver)* | — | [rappi-ai-engineer-application-new.md](rappi-ai-engineer-application-new.md) | 2026-07-21 |
| GBM | Engineering Manager | ⚫ Cerrada por inactividad (90 días sin feedback tras Entrevista 2) | *(tracking en `.recruitment/`, sistema previo al índice actual)* | — | `.recruitment/active/gbm_engineering_manager/status.md` | 2026-07-20 |
| Lab10 | AI Product Engineer | ⚫ Cerrada por inactividad (101 días sin feedback tras entregables) | *(tracking en `.recruitment/`, sistema previo al índice actual)* | — | `.recruitment/active/lab10_ai_product_engineer/status.md` | 2026-07-20 |
| ACL | Desarrollador Mobile Android | ✅ Submitted | [cv_for_acl-android-developer.md](../source/cvs/cv_for_acl-android-developer.md) | [PDF](cvs-pdf/diego-reyes-altamirano-acl-android-developer.pdf) | [acl-android-developer-application.md](acl-android-developer-application.md) | 2026-07-10 |
| Monato | Senior Software Engineer | ✅ Submitted | [cv_for_monato-senior-software-engineer.md](../source/cvs/cv_for_monato-senior-software-engineer.md) | [PDF](cvs-pdf/diego-reyes-altamirano-monato-senior-software-engineer.pdf) | [monato-senior-software-engineer-application.md](monato-senior-software-engineer-application.md) | 2026-07-11 |
| Confidencial (Positivo S+) | Líder Técnico Mobile | 📨 Enviado como referencia, en espera de más información | [cv_for_positivosmais-lider-tecnico-mobile.md](../source/cvs/cv_for_positivosmais-lider-tecnico-mobile.md) | [PDF](cvs-pdf/diego-reyes-altamirano-positivosmais-lider-tecnico-mobile.pdf) | [positivosmais-lider-tecnico-mobile-application.md](positivosmais-lider-tecnico-mobile-application.md) | 2026-07-11 |
| Ready. | Desarrollador Senior Android / Lead Android | ✅ Submitted | [cv_for_ready-senior-android-lead-android.md](../source/cvs/cv_for_ready-senior-android-lead-android.md) | [PDF](cvs-pdf/diego-reyes-altamirano-ready-senior-android-lead-android.pdf) | [ready-senior-android-lead-android-application.md](ready-senior-android-lead-android-application.md) | 2026-07-11 |
| Multiplica | Android Developer (Semi Senior/Senior) — 2ª aplicación | ✅ Submitted | [cv_for_multiplica-android-developer.md](../source/cvs/cv_for_multiplica-android-developer.md) | [PDF](cvs-pdf/diego-reyes-altamirano-multiplica-android-developer.pdf) | [multiplica-android-developer-application.md](multiplica-android-developer-application.md) | 2026-07-11 |

## Convención de Naming (a partir de 2026-07-01)

Todo archivo relacionado a una misma aplicación comparte el mismo slug base `[empresa-kebab-case]-[rol-kebab-case]`:

- **CV fuente:** `source/cvs/cv_for_[slug].md`
- **PDF:** `generated/cvs-pdf/diego-reyes-altamirano-[slug].pdf`
- **Tracking:** `generated/[slug]-application.md`

Esto permite encontrar todo lo relacionado a una aplicación con un solo patrón de búsqueda, sin necesidad de abrir cada archivo.

**Nota:** los CVs genéricos por tipo de rol (`cv_for_android.md`, `cv_for_engineer_lead.md`, `cv_for_ia.md`, `cv_latest.md`) son variantes reutilizables, no atadas a una aplicación específica — no siguen esta convención de slug porque no representan un proceso de aplicación puntual.

## Auditoría de CVs genéricos (completada 2026-07-01)

`cv_latest.md`, `cv_for_android.md`, `cv_for_engineer_lead.md` y `cv_for_ia.md` fueron revisados línea por línea contra `source/profile/experience.md` y `skills.md` — sin datos inflados ni inconsistencias. `cv_for_mobile_product_lead.md` sí tenía problemas (ver fila de Clara arriba) y fue eliminado.

## Caso Monato — reconstrucción por datos inventados (2026-07-11)

Un borrador previo de `cv_for_monato-senior-software-engineer.md` y su tracking (creados en otra sesión el mismo día) contenían STAR stories y respuestas de entrevista con métricas y herramientas inventadas (99.9% uptime, 40% reducción de latencia, SonarQube, Datadog, HikariCP, cobertura "30%→72%", entre otras — ninguna verificable en `source/profile/`). Se detectó vía `/review-application` y se reconstruyeron ambos archivos desde cero, verificados línea por línea. Ver notas completas en [monato-senior-software-engineer-application.md](monato-senior-software-engineer-application.md).

## Auditoría de proyecto (2026-07-20)

- **`.recruitment/` reconciliado**: era un sistema de tracking huérfano (abril 2026, anterior a este índice). GBM Engineering Manager y Lab10 AI Product Engineer se cerraron por inactividad y quedan referenciados arriba para no perder el historial — detalle completo en `.recruitment/applications.md`.
- **Rappi aclarado**: no son "2 versiones duplicadas" — son un rechazo histórico (abril) y una reaplicación activa (29-junio, contacto Mike) sin respuesta hace 21 días. Ambos quedan como filas separadas arriba.
- **Stori y ALTEN cerrados** por inactividad (76 y 77 días sin feedback respectivamente).
- **Worktree huérfano eliminado**: `.claude/worktrees/strange-brown/` — confirmado 100% fusionado en `main`, sin pérdida. De paso se encontró y corrigió un link roto en `source/profile/personal.md` que apuntaba a un archivo eliminado a propósito en abril.
- **Planes de LinkedIn marcados como superados**: `linkedin-plan-1month.md` y `plan-semanal-4semanas.md` (content marketing, abandonados a los 2 días de arrancar) — se decidió mantener LinkedIn enfocado 100% en búsqueda de empleo, sin fusionar con `dr_kings_ia` (consultoría de IA independiente que el usuario opera en paralelo, público distinto). Detalle en memoria `project_linkedin_status`.

## Pendientes de esta reorganización

- ~~Identificar qué CV se usó realmente para Stori, ALTEN y Rappi~~ — resuelto 2026-07-20: ALTEN confirmado (`cv_for_android.md`), Stori fue externo al proyecto (no aplica), Rappi original queda cerrado sin identificar por decisión del usuario (aplicación rechazada, no se reabre el tema).
- ~~Seguimiento con Mike (Rappi reaplicación)~~ — resuelto 2026-07-21: respondió en 9 horas, avanzaron con otro candidato. Proceso cerrado.
- Seguimiento para ACL, Monato, Ready y Multiplica (2ª aplicación) programado para ~2026-07-25 (14 días desde el envío) si no hay respuesta antes.
