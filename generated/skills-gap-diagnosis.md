---
type: diagnóstico
date: 2026-06-30
session: Skills Gap Diagnostic Session
status: active
last_updated: 2026-06-30
tags: [diagnóstico, gaps, soft-skills, hard-skills, storytelling, android, entrevistas]
---

# Diagnóstico de Gaps - Sesión 30-06-2026

## Contexto de la Sesión

**Formato:** Role-play y simulacros con hiring manager técnico
**Duración:** 90 minutos
**Objetivo:** Identificar qué gaps están bloqueando la búsqueda laboral

### Ejercicios Realizados

1. **Pitch de 2 minutos** (espontáneo, sin preparación)
2. **Pregunta técnica de experiencia:** Decisión técnica más difícil
3. **Pregunta situacional:** Arquitectura legacy que nadie quiere tocar
4. **Pregunta de presión:** Defender decisión que stakeholders no querían
5. **Diagnóstico Lyft:** Reconstrucción del ejercicio técnico fallido

---

## Diagnóstico: Los 3 Gaps Principales

---

### GAP #1 — PRIMARIO 🔴
**Ownership y Storytelling de Experiencia Pasada**

**Descripción:**
Cuando habla del futuro (hipotético) → líder claro, decisiones propias → 8/10
Cuando habla del pasado (experiencia real) → se minimiza, atribuye a otros → 4/10

**Evidencia de la sesión:**
- *"Con la guía de mi líder pude definir la correcta solución..."* (RappiCard migration)
- *"El equipo de negocio cerró la conversación..."* (Datadog vs SignalFX)
- Pitch inicial: 4 roles mencionados, sin foco claro
- Nunca se posiciona como el protagonista que decide

**Impacto en búsqueda:**
El hiring manager termina el screening sin convicción de que puede liderar sin supervisión constante. La experiencia existe pero no convence porque se cuenta desde un rol pasivo.

**Causa probable:**
Transición de IC a líder en Rappi bajo managers con poco tiempo (VPs/CTOs con mucha gente a cargo). Aprendió a moverse con autonomía pero verbalizando siempre las decisiones como "equipo" o "con guía de líder".

**Estado:** ⏳ En trabajo
**Tiempo estimado para corregir:** 2-3 semanas de práctica estructurada

---

### GAP #2 — SECUNDARIO 🟡
**Velocidad de Código Bajo Presión**

**Descripción:**
El conocimiento técnico Android existe. La ejecución rápida en entrevista técnica timed no.

**Evidencia de la sesión:**
- Ejercicio Lyft: completó 2/5 pruebas en 45 minutos
- Prueba 1 (memorama básico): fricción al definir el modelo de datos de cartas
- Problema específico: no resolvió inmediatamente el uso de `imageId` como identificador de pares

**Causa:**
4 años como Engineering Lead con ~15% de tiempo en código directo. El conocimiento está presente pero la velocidad de ejecución bajo presión disminuye sin práctica diaria.

**Impacto en búsqueda:**
Fallas en coding interviews para roles de Android Senior o Android Tech Lead con prueba técnica.

**Estado:** ⏳ Pendiente iniciar
**Tiempo estimado para corregir:** 4-6 semanas (30 min diarios)

---

### GAP #3 — POSICIONAMIENTO 🟡
**Targeting Difuso — Demasiados Roles Simultáneos**

**Descripción:**
En el pitch mencionó 4 roles distintos: AI Engineer + Engineering Lead + Tech Lead + Android Developer. Cada aplicación va a un rol diferente sin narrativa coherente.

**Impacto en búsqueda:**
- Un hiring manager no sabe para qué rol específico lo buscan
- Señal de dispersión = falta de convicción = sin urgencia de contratarlo
- Probablemente explica la alta tasa de silencio en aplicaciones

**Rol más sólido identificado:** Android Tech Lead
**Estado:** ⏳ Pendiente aplicar foco
**Tiempo estimado para corregir:** Esta semana

---

## Plan de Acción

### SEMANA 1 (Hoy - 06-07-2026)
- [ ] Definir UN rol principal: **Android Tech Lead**
- [ ] Reescribir pitch de 60 segundos específico para ese rol
- [ ] Practicar pitch 10 veces en voz alta con cronómetro
- [ ] Identificar las 4 historias STAR principales a reescribir

### SEMANAS 2-3 (07-07 al 20-07-2026)
- [ ] Reescribir historia STAR #1: RappiCard Chile migration
- [ ] Reescribir historia STAR #2: Design System (+20% velocity)
- [ ] Reescribir historia STAR #3: Optimización infraestructura (-20% costos)
- [ ] Reescribir historia STAR #4: Datadog/SignalFX → solución creativa
- [ ] Practicar cada historia con cronómetro (máx 2 min, sin notas)
- [ ] Sesión de simulacro con Claude (verificar mejora)

### SEMANAS 4-8 (21-07 al 24-08-2026)
- [ ] 30 min de código Android diario:
  - Semana 4-5: RecyclerView + state management
  - Semana 6-7: Coroutines + Flow
  - Semana 8: Ejercicio timed completo (1 hora, 5 pruebas)
- [ ] Una sesión de simulacro técnico mensual

---

## Historial de Sesiones de Práctica

| Fecha | Tipo | Resultado | Notas |
|-------|------|-----------|-------|
| 2026-06-30 | Diagnóstico inicial | Gap #1, #2, #3 identificados | Primera sesión de role-play |

---

## Las 4 Historias STAR a Trabajar

### Historia #1: RappiCard Chile Migration (EN PROGRESO)

**Versión actual (débil):**
> "Con la guía de mi líder y el apoyo de compañeros expertos, pude definir la correcta solución..."

**Versión objetivo (con ownership):**
> "Identifiqué que el flujo de reemplazo de tarjeta era el más crítico — si fallaba, el usuario quedaba sin acceso a fondos. Diseñé un token temporal que permitía a Itau iniciar el reemplazo sin exponer datos PCI. Coordiné los equipos internos de Rappi, el equipo de Itau y proveedores externos. Resultado: migración completada en el timeline acordado, cero incidentes de reemplazo durante el mes de operación dual."

**Estado:** ⏳ Pendiente practicar

---

### Historia #2: Design System +20% Velocity (PENDIENTE)

**Versión débil conocida:** "Lideré el desarrollo de un Design System"
**Versión objetivo:** TBD en sesión de trabajo

**Estado:** ⏳ Pendiente reescribir

---

### Historia #3: Optimización Infraestructura -20% Costos (PENDIENTE)

**Estado:** ⏳ Pendiente reescribir

---

### Historia #4: Datadog → SignalFX Solución Creativa (PENDIENTE)

**Versión débil conocida:** "El negocio cerró la conversación... tuve que acotar la solución"
**Versión objetivo:** Enfocar en la solución creativa con Jenkins CI

**Estado:** ⏳ Pendiente reescribir

---

## Notas de la Sesión

**Hallazgo clave:**
El gap no es de conocimiento técnico — es de cómo se presenta ese conocimiento. Cuando habla de escenarios hipotéticos futuros, muestra criterio de líder claro (8/10). Cuando habla de experiencias pasadas reales, se minimiza (4/10).

**Causa probable del patrón:**
Cultura de Rappi con managers senior muy ocupados. Aprendió autonomía real pero verbalizando siempre las decisiones como colectivas o validadas por el líder, no como propias.

**Mejor rol objetivo actual:** Android Tech Lead
- Mayor profundidad técnica
- Menor gap vs. otros roles
- Más credibilidad en entrevista técnica (con práctica de código)
