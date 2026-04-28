# Sistema de Perfil Profesional y Preparación para Entrevistas

## Propósito del Proyecto
Sistema IA que agrega tu experiencia técnica (CVs, LinkedIn, GitHub) y genera contenido personalizado para preparación de entrevistas de trabajo usando Claude API.

## Estructura del Proyecto

```
dr_work_experience/
├── source/                  # Fuente única de verdad (datos del perfil)
│   ├── profile/            # Información profesional core
│   │   ├── personal.md      # Datos básicos: nombre, ubicación, contacto
│   │   ├── links.md         # LinkedIn, GitHub, Portfolio
│   │   ├── skills.md        # Hard skills, soft skills, proficiencias
│   │   └── experience.md    # Historial completo y logros
│   └── cvs/                # Variaciones de CV por rol
│       ├── cv_latest.md     # CV actual/principal
│       └── cv_for_[role].md # Variantes específicas por rol
├── generated/              # Contenido generado para entrevistas y procesos de postulación
│   ├── interview-responses.md   # Respuestas STAR, historias clave
│   ├── role-summaries.md        # Perfiles adaptados por tipo de rol
│   ├── qa-bank.md               # Banco de preguntas y respuestas
│   └── [company]-application.md # Registros de procesos de postulación activos
├── .claude/
│   ├── memory/              # Memoria persistente entre sesiones
│   │   └── MEMORY.md        # Índice de memorias
│   └── agents/              # Definiciones de agentes especializados
└── docs/                    # Documentación del sistema
```

## Convenciones Clave

### Metadata en Archivos
Todos los archivos importantes incluyen frontmatter YAML:
```yaml
---
type: perfil | skill | experience | cv | generado
last_updated: YYYY-MM-DD
tags: [tag1, tag2]
---
```

### Contenido de Entrevista
- Las respuestas usan el framework **STAR**: Situación, Tarea, Acción, Resultado
- El contenido generado siempre referencia los archivos fuente
- Separación clara: source/ (datos raw) vs generated/ (contenido procesado)

## Flujo de Trabajo

1. **Setup de Perfil** (source/): CVs, LinkedIn, GitHub, inventario de skills
2. **Análisis**: Claude lee y estructura los datos del perfil
3. **Preguntas de Clarificación**: Claude hace preguntas dinámicas para llenar vacíos
4. **Generación**: Claude produce contenido de preparación para entrevistas
5. **Iteración**: El usuario refina el perfil, Claude regenera según sea necesario

## Comandos Recomendados

```bash
# Ver estado
git status
git log --oneline

# Guardar cambios
git add .
git commit -m "Actualizar: [descripción]"
```

## Guías Importantes para Claude

- Lee este CLAUDE.md primero para entender la estructura
- Los archivos en source/ son la fuente única de verdad
- Siempre referencia archivos fuente al generar contenido
- Los archivos generados incluyen timestamp y referencias
- Usa Git con mensajes de commit claros
- Haz preguntas clarificadoras antes de generar
