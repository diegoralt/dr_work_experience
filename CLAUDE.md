# Sistema de Perfil Profesional y Preparación para Entrevistas
## + Workspace Master para 2 Proyectos AI (Mayo 2026)

## Propósito del Proyecto (Dual)

**MASTER WORKSPACE** (este directorio):
- Sistema IA que agrega tu experiencia técnica (CVs, LinkedIn, GitHub)
- Genera contenido personalizado para preparación de entrevistas de trabajo
- **Punto de entrada centralizado** para 2 proyectos independientes
- Memory compartido + Settings unificados
- Registro de procesos de postulación

**EXTERNAL PROJECTS** (en `/projects-ai/`):
- `support-agent-ai`: Sistema de automatización de tickets (Semana 1)
- `document-rag-system`: Sistema RAG de búsqueda de documentos (Semanas 2-3)
- Cada uno: su propio `.git` independiente (publicable a GitHub)

## Arquitectura: Workspace References

Lee `workspace.json` para la configuración completa.

```
dr_work_experience/ (MASTER WORKSPACE - Single Source of Truth)
├── workspace.json           ← Define estructura + referencias
├── CLAUDE.md (this file)   ← Master config
├── .claude/
│   ├── settings.json       ← Settings base
│   └── memory/             ← Memory centralizado (compartido)
├── source/                 ← Data única verdad (perfil)
│   └── profile/, cvs/      ← Experience, skills, links
└── generated/              ← PLANES + Procesos de postulación
    ├── linkedin-plan-1month.md          ← Plan ejecutivo (4 semanas)
    ├── plan-semanal-4semanas.md         ← Timeline detallado (ejecución)
    └── rappi-ai-engineer-application.md ← Proceso activo

/projects-ai/ (EXTERNAL - git independiente)
├── INDEX.md                ← Referencia a planes en dr_work_experience
├── support-agent-ai/       ← Proyecto 1 (.git propio)
│   └── README.md
└── document-rag-system/    ← Proyecto 2 (.git propio)
    └── README.md
```

**Estructura Definitiva:**
- **Master Workspace**: dr_work_experience (planes + memory + perfil)
- **Projects**: /projects-ai/ (desarrollo + git independiente)
- **Single Source of Truth**: Plans en dr_work_experience/generated/

## Cómo Funciona

1. **Abres dr_work_experience en Claude Code**
2. **Claude Code lee workspace.json** → detecta /projects-ai/
3. **Memory centralizado** accesible desde cualquier proyecto
4. **Context switching** optimizado entre proyectos
5. **Settings base** + overrides por proyecto cuando necesario

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
