---
type: referencia
name: Guía de Flujo de Trabajo
description: Cómo usar el sistema paso a paso
---

# Flujo de Trabajo

## Fase 1: Setup Inicial (30-60 min)

1. **Completa tus datos en `source/profile/`:**
   - personal.md (datos básicos)
   - links.md (LinkedIn, GitHub)
   - skills.md (hard + soft skills)
   - experience.md (historial laboral)

2. **Carga tu CV:**
   - Copia tu CV actual a `source/cvs/cv_latest.md`

3. **Valida con Claude:**
   ```
   "Revisa mi perfil en source/ y dame feedback sobre qué información falta"
   ```

## Fase 2: Análisis & Complementación (30-45 min)

1. **Claude analiza tu perfil:**
   ```
   "Analiza mi perfil en source/ y hazme preguntas específicas para mejorar el contenido"
   ```

2. **Responde preguntas de Claude:**
   - Historias de logros importantes
   - Detalles sobre proyectos
   - Desafíos que resolviste
   - Impacto cuantificable

3. **Actualiza source/ con nueva información**

## Fase 3: Generación de Contenido (20-30 min)

1. **Solicita generación por tipo:**

   ```
   # Para respuestas STAR
   "Genera 10 respuestas STAR basadas en mi experiencia"
   
   # Para rol específico
   "Resume mi perfil para una posición de Senior Backend Engineer"
   
   # Para banco de preguntas
   "Genera preguntas frecuentes y respuestas basadas en mi experiencia"
   ```

2. **Claude genera contenido** en `generated/`

## Fase 4: Preparación para Entrevista (Variable)

1. **Antes de una entrevista:**
   ```
   "Genera preguntas posibles para una entrevista de [Tipo de Rol] y mis mejores respuestas"
   ```

2. **Practica con Claude:**
   ```
   "Hazme preguntas de entrevista de [Tipo] y dame feedback sobre mis respuestas"
   ```

## Fase 5: Actualización Continua

- Cuando cambies de rol o agregues nueva experiencia:
  - Actualiza `source/profile/experience.md`
  - Ejecuta generación nuevamente
  - Git commit de los cambios

---

## Comandos Git Recomendados

```bash
# Ver estado
git status
git log --oneline

# Después de cambios importantes
git add .
git commit -m "Actualizar: [descripción del cambio]"
```

## Tips para Mejores Resultados

1. **Sé específico**: En lugar de "trabajé en un proyecto", detalla: "Optimicé una API que servía 10k requests/min, reduciendo latencia 40%"
2. **Usa ejemplos reales**: Los ejemplos concretos generan mejor contenido
3. **Actualiza regularmente**: Mantén source/ actualizado para contenido fresco
4. **Itera**: No es perfecto a la primera - refina con Claude
