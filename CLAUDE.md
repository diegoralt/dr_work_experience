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

## 🚫 REGLAS CRÍTICAS - Separación de Workspace

**NUNCA crear estos archivos en dr_work_experience:**
- ❌ `projects/*/prompts/` (código IA)
- ❌ `projects/*/docs/` (especificaciones técnicas del proyecto)
- ❌ `projects/*/tests/` (test cases)
- ❌ `projects/*/workflows/` (configuración n8n/técnica)

**SOLO permitido en dr_work_experience:**
- ✅ `generated/caso-1-status.md` (tracking de progreso)
- ✅ `generated/proyecto-ia-index.md` (índice de referencias)
- ✅ `generated/plan-*.md` (planes de ejecución)
- ✅ `source/` (CVs, perfil profesional)
- ✅ `.claude/` (memoria, settings)

**Por qué:**
- dr_work_experience = Master workspace para tu perfil profesional + tracking
- /projects-ai/ = Repos independientes con .git separado (publicable a GitHub)
- Evita duplicación, conflictos de merge, confusión de repositorios

**Protección automática:**
- Pre-commit hook en `.git/hooks/pre-commit` rechaza commits de código de proyecto
- .gitignore ignora archivos de proyecto por defecto

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

## Estructura de Archivos de Seguimiento de Postulaciones

Cada postulación activa tiene su archivo en `generated/[empresa]-[rol]-application.md`.
La plantilla estándar está en `generated/application-tracking-template.md`.

### Secciones Obligatorias (en este orden)
1. **Frontmatter YAML** — type, company, position, status, dates, tags
2. **Position Overview** — empresa, rol, tipo, URL de vacante, resumen del rol
3. **Application Status** — tabla de etapas con estado y fecha
4. **Datos Exactos del Formulario** — solo si hay formulario online; incluye siempre:
   - Education (datos fijos: FES Aragón UNAM, 2011-2015)
   - Work Experience summaries (en inglés, optimizados por rol)
   - Volunteer Experience (Casa Hogar San Martín de Porres y Juan XXIII, 14-11-2025)
   - Professional Associations (SCRUMstudy 27-12-2017, GDG Cloud México 08-11-2024, Lab10 08-05-2025)
   - Qualifications/Licenses (seleccionar relevantes de la lista maestra en skills.md)
5. **Mapeo Perfil vs Requisitos** — tabla de alineados y gaps con evidencia
6. **Competitive Advantages** — 3-5 ventajas con evidencia concreta
7. **STAR Stories Preparadas** — mínimo 3 historias completas (Situación/Tarea/Acción/Resultado)
8. **Preguntas Esperadas & Respuestas** — mínimo 4 preguntas con respuesta lista
9. **Preguntas a Hacer en la Entrevista** — mínimo 3 preguntas para el entrevistador
10. **Alignment Assessment** — fit level (1-5) + tabla de cobertura de requisitos
11. **Expected Timeline** — milestones con fechas target
12. **Contact Information** — datos fijos de Diego
13. **Notes** — observaciones específicas de esta aplicación

### Datos Fijos Reutilizables
- **Email:** diego.reyes.tcp@gmail.com
- **Phone:** +52 5551279802
- **Location:** Atenco, México
- **Education:** Computer Engineering, FES Aragón UNAM, 08/2011 - 05/2015
- **Voluntariado:** Casa Hogar San Martín de Porres y Juan XXIII, 14-11-2025
- **Certificado Scrum:** SCRUMstudy, 27-12-2017
- **GDG Cloud México:** desde 08-11-2024
- **Lab10 Community:** desde 08-05-2025

### Naming Convention
`generated/[empresa-kebab-case]-[rol-kebab-case]-application.md`
Ejemplo: `stori-tech-manager-application.md`, `clara-mobile-product-lead-application.md`

## Guías Importantes para Claude

- Lee este CLAUDE.md primero para entender la estructura
- Los archivos en source/ son la fuente única de verdad
- Siempre referencia archivos fuente al generar contenido
- Los archivos generados incluyen timestamp y referencias
- Usa Git con mensajes de commit claros
- Haz preguntas clarificadoras antes de generar
- Para nuevas postulaciones: usar `generated/application-tracking-template.md` como base
