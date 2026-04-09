# Sistema de Perfil Profesional y Preparación para Entrevistas

Sistema IA que agrega tu experiencia técnica y genera contenido personalizado para preparación de entrevistas de trabajo.

## Objetivo

Crear un banco estructurado de tu perfil profesional que permita generar:
- ✅ Respuestas STAR para preguntas de entrevista
- ✅ Resúmenes de competencias por tipo de rol
- ✅ Banco de preguntas y respuestas frecuentes
- ✅ Perfiles adaptados para diferentes posiciones

## Estructura

Proyecto organizado para que Claude trabaje de forma óptima:

- **source/** - Tus datos (CVs, perfil, skills) - Fuente única de verdad
- **generated/** - Contenido generado para entrevistas
- **.claude/** - Memoria y configuración del sistema
- **docs/** - Documentación del proyecto

## Cómo Usar

1. **Setup inicial**: Carga tus CVs y datos de perfil en `source/`
2. **Interactúa con Claude Code**: Claude lee automáticamente `CLAUDE.md`
3. **Pide contenido**: "Genera respuestas STAR" o "Resume mis skills para una entrevista de Backend"
4. **Refina**: Actualiza `source/`, Claude regenera contenido

## Flujo de Trabajo Recomendado

```
1. Cargar CVs           → source/cvs/
2. Completar perfil     → source/profile/
3. Consultar Claude     → "Analiza mi perfil"
4. Responder preguntas  → Claude hace preguntas dinámicas
5. Generar contenido    → Claude produce interview prep
6. Usar contenido       → Prepararse para entrevistas
```

## Próximos Pasos

- [ ] Cargar CV en `source/cvs/cv_latest.md`
- [ ] Completar perfil básico en `source/profile/`
- [ ] Agregar links de LinkedIn y GitHub
- [ ] Listar skills principales
- [ ] Ejecutar análisis con Claude: "Analiza mi perfil y haz preguntas para complementar"

## Documentación

Ver `docs/workflow.md` para guía detallada de uso.
