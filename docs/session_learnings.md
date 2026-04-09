---
name: Session Learnings - Professional Profile & Lab10 Application
description: Documento de aprendizaje y referencia de sesión completa
type: referencia
last_updated: 2026-04-09
status: Completado
---

# Session Learnings - Professional Profile & Lab10 Application

## 📌 Resumen Ejecutivo

Sesión enfocada en:
1. Estructura de proyecto optimizada para Claude
2. Validación de tech stack mediante cuestionario
3. Documentación honesta de 3 proyectos reales
4. Generación de entregables para Lab10

**Resultado:** 2 documentos copiables listos para enviar + estructura privada de tracking de postulaciones.

---

## 🏗️ Estructura del Proyecto

### Arquitectura Implementada

```
dr_work_experience/
├── CLAUDE.md                          # Instrucciones persistentes
├── README.md                          # Guía general
├── .gitignore                         # (excluye .recruitment/)
│
├── source/                            # Source of Truth
│   ├── profile/
│   │   ├── personal.md               # Datos básicos
│   │   ├── links.md                  # LinkedIn, GitHub, proyectos
│   │   ├── skills.md                 # Hard + soft skills
│   │   └── experience.md             # Historial laboral
│   └── cvs/
│       ├── cv_latest.md              # CV principal
│       ├── cv_for_engineer_lead.md   # Variante liderazgo
│       ├── cv_for_android.md         # Variante mobile
│       └── cv_for_ia.md              # Variante IA
│
├── generated/                         # Contenido generado
│   ├── interview-responses.md        # (futuro)
│   ├── role-summaries.md             # (futuro)
│   └── qa-bank.md                    # (futuro)
│
├── .recruitment/                      # 🔒 PRIVADA (no en Git)
│   ├── applications.md               # Log maestro
│   └── active/
│       └── lab10_ai_product_engineer/
│           ├── requirements.md
│           ├── deliverables.md
│           ├── status.md
│           ├── notes.md
│           ├── deliverable_demos_final.txt
│           └── deliverable_intention_final.txt
│
├── .claude/
│   └── memory/
│       └── MEMORY.md
│
└── docs/
    ├── workflow.md
    ├── github_readme_wip.md
    └── session_learnings.md
```

**Principios aplicados:**
- ✅ Single source of truth (source/)
- ✅ Separación clear (source/ vs generated/)
- ✅ Privacidad (recruitment/ en .gitignore)
- ✅ Documentación para Claude (CLAUDE.md)

---

## 🔍 Tech Stack Validado

### Metodología: Cuestionario Robusto (15 preguntas)

**Formato:** Opción múltiple + respuestas verificadas contra proyectos reales

**Resultado final:** 13/15 correctas (87% general)

### Stack Confirmado (16 tecnologías)

| Categoría | Tecnologías | Nivel | ¿README? |
|-----------|-------------|-------|---------|
| **Lenguajes** | Kotlin, Java, SQL | 8/10 | ✅ |
| **Backend** | Spring Boot, REST APIs, Microservicios | 8/10 | ✅ |
| **Cloud & DevOps** | AWS, Kubernetes, Docker, Jenkins, Git | 8/10 | ✅ |
| **AI & LLMs** | Claude API, OpenAI API, Prompt Engineering | 8/10 | ✅ |
| **Mobile** | Android, Jetpack, MVVM, Clean Architecture | 8/10 | ✅ |

**Criterio:** Solo incluir techs donde tengo 7+/10 de confianza + experiencia real en producción.

---

## 📊 Tres Proyectos Documentados

### 1. Artify — App Android

**Estado:** Completado (Febrero 2026, 1 semana)  
**Repo:** https://github.com/diegoralt/Artify

**Aprendizajes clave:**
- ✅ Usar IA desde el kickoff, no a mitad
- ✅ Claude Code acelera arquitectura + scaffolding
- ✅ Clean Architecture + MVVM escalable

**Decisiones técnicas destacadas:**
- StateFlow<UiState> (lifecycle-aware)
- Hilt para inyección de dependencias
- GitHub Actions para CI/CD

---

### 2. Landing Page Despacho Jurídico

**Estado:** MVP v0.5 (Feb-Apr 2026)  
**Demo:** https://id-preview--057976af-cbdc-4865-b30f-2751d92c3122.lovable.app/

**Aprendizajes clave:**
- ✅ Diseñar flujo de datos ANTES de UI
- ✅ Arquitectura modular de prompts evita regresiones
- ✅ Lovable es válido para prototipado rápido (~2 semanas)

**Decisiones técnicas destacadas:**
- Prompts modulares en bloques (no monolíticos)
- 15 tokens de color para consistencia
- Template HTML desacoplado para n8n

---

### 3. Pipeline Agéntico TikTok

**Estado:** En desarrollo activo (Marzo 2026, Semana 3)  
**Portfolio:** https://www.tiktok.com/@almamexicana.ia

**Aprendizajes clave:**
- ✅ Implementar métricas ANTES de iterar
- ✅ Arquitectura modular permite trazabilidad exacta
- ✅ Separación semántica en prompts resuelve problemas específicos

**Decisiones técnicas destacadas:**
- Freepik → Kling → CapCut (stack coherente)
- Prompts modulares por herramienta
- ByteDance → ventaja algorítmica

---

## 📋 Entregables Lab10

### Validación contra requisitos

✅ **Campo 1:** Tu perfil de GitHub  
→ https://github.com/diegoralt

✅ **Campo 2:** Link a demos  
→ `deliverable_demos_final.txt` (copiable)

✅ **Campo 3:** Intención + Aporte  
→ `deliverable_intention_final.txt` (copiable)

### Estructura de respuestas

**Demos + Contexto:**
- 3 proyectos × 4 puntos (problema, construcción, decisiones, mejora)
- Conciso, directo, sin formalidad excesiva
- Links verificados y activos

**Intención + Aporte:**
- Coherencia con misión oficial Lab10 ("comunidad impulsando comunidad")
- Rol híbrido IC + mentoría
- Tono sincero y humano

---

## 🎓 Lecciones Aprendidas

### Sobre Estructura de Proyecto

1. **CLAUDE.md es crítico**
   - Claude lee automáticamente al inicio
   - Debe ser conciso (máx 200 líneas)
   - Define convenciones + directorio structure

2. **Separación source/ vs generated/**
   - Evita redundancia
   - Single source of truth funciona
   - Versionable en Git

3. **Privacidad con .gitignore**
   - Tracking de postulaciones es sensible
   - .recruitment/ nunca debe publicarse
   - Permite trabajo local sin riesgo

### Sobre Context Engineering

1. **Metadata en YAML**
   - Frontmatter en archivos facilita búsqueda
   - Type, last_updated, tags son útiles

2. **Documentación estructurada**
   - Claude procesa mejor formato claro
   - Listas, tablas, secciones explícitas

3. **Honestidad > Perfección**
   - Documentar estado real (MVP v0.5, Semana 3)
   - Admitir qué harías diferente
   - Genera confianza

### Sobre Validación de Skills

1. **Cuestionario multivariable**
   - Años × Producción × Confianza × Proyecto Actual
   - Identifica skills reales vs teóricos
   - 87% de precisión en validación

2. **Solo incluir skills con 7+/10**
   - Evita inflación de CV
   - Entrevistas más honestas
   - Mejor match con reclutadores

3. **Proyectos como evidencia**
   - GitHub repos
   - Demos funcionales
   - Documentación técnica

### Sobre Entregables para Postulaciones

1. **Estructura importa**
   - Lab10 espera: problema → construcción → decisiones → mejora
   - Responder exactamente eso
   - No agregar "ruido"

2. **Tono es crítico**
   - Evitar formalidad excesiva
   - Lenguaje conversacional
   - Detalles específicos (no genéricos)

3. **Sinceridad genera impacto**
   - "Pasé horas en email" > "Optimicé flujo"
   - "Iteré a ciegas" > "Mejoré iteración"
   - "Hubiera ganado días" > "Aceleré desarrollo"

---

## 🔄 Workflow Validado

### Fase 1: Setup (✅ Completado)
- Estructura optimizada para Claude
- Datos de perfil cargados
- CVs por rol creados

### Fase 2: Validación (✅ Completado)
- Cuestionario tech stack (15 preguntas)
- Documentación honesta de 3 proyectos
- Coherencia verificada

### Fase 3: Postulaciones (✅ En curso)
- Lab10: Entregables completados
- Estructura de tracking implementada
- Template para futuras postulaciones

### Fase 4: Futuro
- Generar STAR responses (interview-responses.md)
- Role summaries (role-summaries.md)
- QA bank (qa-bank.md)

---

## 📝 Mejores Prácticas Implementadas

### Para Claude

✅ CLAUDE.md actualizado y conciso  
✅ Metadata en YAML frontmatter  
✅ Convenciones claras  
✅ Documentación estructurada  

### Para Git

✅ .gitignore configurado correctamente  
✅ Commits descriptivos  
✅ Estructura versionable  
✅ Privacidad respetada  

### Para Postulaciones

✅ Entregables honestos y específicos  
✅ Links verificados y activos  
✅ Tono conversacional (no generado por IA)  
✅ Estructura esperada respetada  

---

## 🚀 Próximos Pasos

### Inmediatos (Antes de 10 abril @ 2:00 PM UTC-5)
- [ ] Verificar 3 links de Lab10 (funcionan)
- [ ] Copiar `deliverable_demos_final.txt` al campo 2
- [ ] Copiar `deliverable_intention_final.txt` al campo 3
- [ ] Enviar aplicación

### Corto plazo (Semana siguiente)
- [ ] Retomar Pipeline TikTok (Video 4)
- [ ] Monitorear feedback de Lab10
- [ ] Prepararse para Paso 3 (Feedback)

### Mediano plazo
- [ ] Generar interview-responses.md (STAR format)
- [ ] Role summaries por posición
- [ ] QA bank personalizado

### Largo plazo
- [ ] Mantener .recruitment/ actualizado
- [ ] Agregar nuevas postulaciones usando template
- [ ] Iterar perfil según feedback recibido

---

## 🎯 Conclusiones Clave

1. **Estructura optimizada para Claude funciona**
   - Menos fricción
   - Mejor contexto
   - Iteración más rápida

2. **Validación de skills es importante**
   - Evita CV inflado
   - Mejora confianza en entrevistas
   - Identifica gaps reales

3. **Honestidad en documentación genera impacto**
   - "Qué harías diferente" es más poderoso que "qué hiciste"
   - Detalles específicos > generalizaciones
   - Tono humano > formalidad

4. **Tracking de postulaciones es valuable**
   - Estructura privada sin riesgo
   - Template reutilizable
   - Facilita múltiples procesos simultáneamente

5. **Proyectos reales son mejor marketing que CV**
   - Links a demos > descripción de skills
   - GitHub repos > claims técnicos
   - Documentación técnica > buzzwords

---

## 📚 Archivos Generados

| Archivo | Ubicación | Propósito |
|---------|-----------|----------|
| `CLAUDE.md` | Root | Instrucciones persistentes |
| `deliverable_demos_final.txt` | .recruitment/active/lab10 | Copiable Campo 2 |
| `deliverable_intention_final.txt` | .recruitment/active/lab10 | Copiable Campo 3 |
| `status.md` | .recruitment/active/lab10 | Tracking estado |
| `application_template.md` | .recruitment/templates | Para futuras postulaciones |
| `session_learnings.md` | docs/ | Este archivo |

---

## 🔗 Referencias

- [Best Practices for Claude Code](https://code.claude.com/docs/en/best-practices)
- [CLAUDE.md Guide - HumanLayer](https://www.humanlayer.dev/blog/writing-a-good-claude-md)
- [GitHub Profile README Best Practices](https://dev.to/github/10-standout-github-profile-readmes-h2o)
- [Lab10 - Comunidad de AI Builders](https://lab10.ai/)

---

**Documento completado:** 9 de abril, 2026  
**Próxima revisión:** Después de feedback Lab10  
**Versión:** 1.0
