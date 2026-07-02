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
- [x] Reescribir historia STAR #1: RappiCard Chile migration
- [x] Reescribir historia STAR #2: Design System (+20% velocity)
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

### Historia #1: RappiCard Chile Migration (PRACTICADA ✅)

**Versión actual (débil):**
> "Con la guía de mi líder y el apoyo de compañeros expertos, pude definir la correcta solución..."

**Versión final (con ownership, practicada 30-06-2026):**
> "Estuve a cargo del proyecto de migración de RappiCard de la app de Rappi a la plataforma de Itau. Tuve que coordinar diferentes equipos — interno, Itau y proveedores externos — para actualizar el flujo de reemplazo de tarjeta, ya que era un flujo crítico.
>
> Definí utilizar un endpoint ya conocido por el equipo de Itau para evitar retrasos en su desarrollo. Determiné que el nuevo flujo pudiera integrarse sin afectar el canal de reemplazo ya existente, dando un periodo donde los usuarios podían ejecutar el reemplazo desde los 2 canales en paralelo. Planifiqué una liberación en fases que nos permitió detectar errores antes del despliegue total.
>
> Resultado: migramos las 54 mil tarjetas activas en Chile con solo 5 incidencias reportadas — menos del 0.01% — y 200 reemplazos de tarjeta procesados exitosamente durante la operación dual."

**Calificación:** 9/10 (ownership 9, razonamiento técnico 8, estructura STAR 9, métrica de resultado 9)

**Estado:** ✅ Lista para entrevista real

---

### Historia #2: Design System +20% Velocity (PRACTICADA ✅)

**Versión débil conocida:** "Lideré el desarrollo de un Design System"

**Versión final (con ownership, practicada 01-07-2026):**
> "El equipo de producto detectó diferencias en la experiencia de usuario que brindaban los flujos en el app dependiendo si el usuario tenía Android o iOS, lo que provocaba confusión entre los usuarios — esto dio auge a una iniciativa llamada Design System. La meta fue generar vistas nuevas o existentes rápido y con consistencia entre ambas plataformas.
>
> Mi rol para este proyecto fue definir el plan de desarrollo, contemplando fecha de liberación de primera versión, plan de implementación de componentes, revisión con equipo de UX para revisión y validación de componentes, y sobre todo empujar con los equipos de desarrollo de producto la importancia de su adopción para priorizar la integración a los flujos.
>
> El proyecto inició su desarrollo con un equipo pequeño. Cuando detectaba una entrega de componentes críticos, gestionaba capacidad adicional de otros equipos, lo que me permitió cumplir las fechas de entrega comprometidas.
>
> Al final, el Design System es utilizado por más de 7 equipos de desarrollo mobile, con un aumento del 20% en la velocidad de desarrollo y una experiencia de usuario más homogénea sin importar el SO que tiene el usuario final en su dispositivo."

**Calificación:** 8.5/10 (ownership 8.5, razonamiento técnico 7.5, estructura STAR 8, métrica de resultado 9)

**Estado:** ✅ Lista para entrevista real

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
