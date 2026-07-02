---
type: index
last_updated: 2026-07-01
tags: [index, aplicaciones, tracking, cvs]
---

# Índice de Aplicaciones

Tabla maestra de todas las aplicaciones activas y pausadas: empresa, rol, estado, y dónde vive cada archivo relacionado (CV fuente, PDF, tracking). Actualizar esta tabla cada vez que se crea o modifica una aplicación o CV.

| Empresa | Rol | Estado | CV Fuente (Markdown) | PDF | Tracking | Última actualización |
|---|---|---|---|---|---|---|
| Aplazo | Technical Lead Manager | ⏸️ Pausada (bloqueo por rechazo previo <3 meses) | [cv_for_aplazo-technical-lead-manager.md](../source/cvs/cv_for_aplazo-technical-lead-manager.md) | [PDF](cvs-pdf/diego-reyes-altamirano-aplazo-technical-lead-manager.pdf) | *(sin tracking — no se pudo enviar)* | 2026-07-01 |
| Multiplica Talent | Android Developer (Semi Senior/Senior) | ✅ Submitted | [cv_for_multiplica-talent-android-developer.md](../source/cvs/cv_for_multiplica-talent-android-developer.md) | [PDF](cvs-pdf/diego-reyes-altamirano-multiplica-talent-android-developer.pdf) | [multiplica-talent-android-developer-application.md](multiplica-talent-android-developer-application.md) | 2026-07-01 |
| Stori | Tech Manager | Ver tracking | *(no generado en este flujo — CV usado no identificado, pendiente de auditar)* | — | [stori-tech-manager-application.md](stori-tech-manager-application.md) | — |
| Clara | Mobile Product Lead | Rejected (16-06-2026) | *(CV eliminado 2026-07-01 — contenía datos no verificados: Statsig/Amplitude sin respaldo, "Bilingüe/Fluent" contradice B1 confirmado, fecha de GDG inconsistente con CLAUDE.md)* | — | [clara-mobile-product-lead-application.md](clara-mobile-product-lead-application.md) | 2026-06-16 |
| ALTEN México | Android Developer | Sin respuesta (timeout 56 días) | *(no identificado — pendiente de auditar)* | — | [alten-mexico-android-developer-application.md](alten-mexico-android-developer-application.md) | 2026-06-29 |
| Rappi | AI Engineer | Ver tracking (2 versiones de tracking existen) | *(no identificado — pendiente de auditar)* | — | [rappi-ai-engineer-application.md](rappi-ai-engineer-application.md), [rappi-ai-engineer-application-new.md](rappi-ai-engineer-application-new.md) | 2026-06-29 |

## Convención de Naming (a partir de 2026-07-01)

Todo archivo relacionado a una misma aplicación comparte el mismo slug base `[empresa-kebab-case]-[rol-kebab-case]`:

- **CV fuente:** `source/cvs/cv_for_[slug].md`
- **PDF:** `generated/cvs-pdf/diego-reyes-altamirano-[slug].pdf`
- **Tracking:** `generated/[slug]-application.md`

Esto permite encontrar todo lo relacionado a una aplicación con un solo patrón de búsqueda, sin necesidad de abrir cada archivo.

**Nota:** los CVs genéricos por tipo de rol (`cv_for_android.md`, `cv_for_engineer_lead.md`, `cv_for_ia.md`, `cv_latest.md`) son variantes reutilizables, no atadas a una aplicación específica — no siguen esta convención de slug porque no representan un proceso de aplicación puntual.

## Auditoría de CVs genéricos (completada 2026-07-01)

`cv_latest.md`, `cv_for_android.md`, `cv_for_engineer_lead.md` y `cv_for_ia.md` fueron revisados línea por línea contra `source/profile/experience.md` y `skills.md` — sin datos inflados ni inconsistencias. `cv_for_mobile_product_lead.md` sí tenía problemas (ver fila de Clara arriba) y fue eliminado.

## Pendientes de esta reorganización

- Identificar qué CV se usó realmente para Stori, Clara (ya resuelto, CV eliminado), ALTEN y Rappi, y enlazarlo aquí.
- Considerar consolidar `rappi-ai-engineer-application.md` y `rappi-ai-engineer-application-new.md` si una reemplaza a la otra.
