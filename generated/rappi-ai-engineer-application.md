---
type: generado
last_updated: 2026-04-27
tags: [rappi, vacante, ai-engineer, preparación, aplicación]
---

# Análisis & Preparación: AI Engineer Mid-level @ Rappi

## Contexto de la Vacante
- **Posición**: AI Engineer Mid-level (conflicto: título dice "Senior AI Engineer I" pero descripción es Mid-level 2-4 años)
- **Foco**: Mixto LLMs/GenAI, MLOps, ML aplicado a producto
- **Stack Técnico**: Python, Cloud, LangChain/PyTorch
- **Responsabilidades**: RAG, Agentes, Fine-tuning, Despliegue en prod, Colaboración con Producto

---

## 🎯 Mapeo: Tu Perfil vs Requisitos

### ✅ ALINEADO - Experiencia de Producción

| Requisito | Tu Experiencia | Nivel | Evidencia |
|-----------|---|---|---|
| **Construir soluciones RAG** | Asistente Legal | 7/10 | MVP en producción: búsqueda docs jurídicos + OpenAI |
| **Agentes Autónomos** | TikTok Pipeline | 7/10 | Claude in Chrome, Freepik, Kling AI (pipeline agéntico) |
| **Integrar LLMs a APIs** | Proyecto Legal + Producción | 8/10 | OpenAI API + function calling, n8n orquestación |
| **Despliegue en Producción** | 3 proyectos activos | 8/10 | MVP Legal (cliente onboarding), TikTok (activo) |
| **Colaboración Cross-team** | Engineer Lead 4 años | 9/10 | Coordinaba 12 personas, múltiples equipos en Rappi |
| **Arquitectura de Sistemas** | Microservicios en Rappi | 8/10 | Spring Boot, APIs, documentación técnica |
| **Cloud & DevOps** | AWS + K8s en Rappi | 7/10 | ECS, S3, Kubernetes, Jenkins (años en Rappi) |

### ⚠️ PARCIAL - Necesita Amplificación

| Requisito | Tu Experiencia | Gap | Plan |
|-----------|---|---|---|
| **Python** | No en CV (pero...) | ❌ Gap crítico | Explicar: n8n tiene Python/JavaScript, APIs REST, scripts |
| **LangChain específicamente** | No mencionado | ⚠️ | Mencionar que has usado frameworks similares (n8n, Lovable) |
| **PyTorch** | No mencionado | ⚠️ | Reconocer: foco en aplicación vs entrenamiento |
| **MLOps específico** | DevOps (Jenkins, K8s) | ⚠️ | Conectar: CD/CD de modelos = versioning + deployment |
| **Fine-tuning** | No documentado | ❌ | Reconocer gap + mostrar interés en aprender |

### ❓ ACLARAR - Posible pero Implícito

| Requisito | Evidencia Implícita | Cómo Conectar |
|-----------|---|---|
| **ML aplicado a Producto** | Agentes que resuelven problemas de negocio | "Automatización de atención → ROI directo para cliente" |
| **RAG** | Búsqueda docs + generación en proyecto legal | "Indexación + retrieval de documentos jurídicos + contexto en prompts" |

---

## 🔴 GAPS CRÍTICOS A ABORDAR

### 1️⃣ Python
**El problema**: No está en CV. Rappi lo requiere explícitamente.

**Tu realidad**:
- n8n permite Python (Code Node)
- OpenAI/Claude APIs (usa JavaScript/TypeScript típicamente)
- Lovable → puede generar Python backend
- DevOps en Rappi (Jenkins, scripts)

**Estrategia de respuesta**:
- En entrevista: "Aunque mi CV enfatiza Kotlin/Java, he usado Python en n8n workflows y OpenAI scripts. Mi fortaleza es arquitectura y design patterns que transfiero entre lenguajes."
- **ACCIÓN RECOMENDADA**: Crear un pequeño proyecto en Python antes de entrevista (FastAPI + Claude API, por ejemplo)

### 2️⃣ Fine-tuning
**El problema**: No hay experiencia documentada.

**Tu realidad**:
- Prompt engineering 8/10 (es el precursor)
- OpenAI API con function calling (avanzado)
- No necesitas entrenamiento de modelos, necesitas optimizar prompts

**Estrategia de respuesta**:
- "Mi enfoque ha sido prompt engineering y retrieval optimization (RAG) más que fine-tuning de modelos. Dependiendo del caso de uso (low-latency vs alta precisión), fine-tuning sería la siguiente iteración."
- Mostrar que entiendes cuándo fine-tuning es necesario vs. RAG/prompt engineering

### 3️⃣ MLOps (no DevOps)
**El problema**: MLOps incluye versionamiento de modelos, feature stores, monitoring de drift.

**Tu realidad**:
- DevOps: CI/CD, Kubernetes, monitoring (Jenkins)
- Falta: Model registry (MLflow), feature stores, data pipelines

**Estrategia de respuesta**:
- Conectar DevOps existente: "CI/CD de modelos es similar a microservicios: versioning, testing, deployments automatizados."
- Reconocer gap: "He trabajado DevOps clásico. MLOps es especialización que puedo aprender rápido (concepto = similar, herramientas = nuevas)."

---

## 📋 RESPUESTAS STAR PREPARADAS

### STAR #1: RAG en Producción
**Situación**: Necesitabas automatizar atención de clientes para despacho jurídico
**Tarea**: Diseñar solución que recupere documentos relevantes y genere respuestas coherentes
**Acción**:
- Indexé documentos jurídicos en n8n
- Construí prompt que contextualiza búsqueda de docs + OpenAI API
- Iteré en prompts hasta validar calidad de respuestas legales
- Desplegué con feedback loop para refinamiento
**Resultado**: MVP en producción en tiempo récord, cliente en onboarding, automatiza >80% de consultas iniciales

### STAR #2: Agentes Autónomos en Escala
**Situación**: Necesitabas pipeline recurrente de generación de contenido para TikTok (@almamexicana.ia)
**Tarea**: Automatizar: concepto → imagen → video → edición → publicación
**Acción**:
- Diseñé arquitectura de agentes encadenados (Claude → Freepik → Kling → CapCut)
- Implementé validación de outputs entre etapas
- Construí orquestación en Claude in Chrome (agente que controla navegador)
- Configuré loop de feedback para quality control
**Resultado**: Pipeline semi-automatizado, producción activa, consistencia visual garantizada

### STAR #3: Despliegue en Producción (Old Stack pero Aplicable)
**Situación**: Necesitabas desplegar cambios de forma confiable en Rappi (millones de usuarios)
**Tarea**: Implementar CI/CD automatizado con análisis estático
**Acción**:
- Implementé Jenkins pipeline: build → análisis estático → tests → deployment
- Configuré Kubernetes para orquestación y rollback automático
- Documenté rutas de despliegue y monitoreo
**Resultado**: Reducción de errores en producción, confianza en deployments automatizados

### STAR #4: Colaboración Producto + IA
**Situación**: Como Engineer Lead en Rappi, necesitabas traducir problemas de negocio a soluciones técnicas
**Tarea**: Trabajar con PMs para definir features que balanceen impacto + viabilidad técnica
**Acción**:
- Establecí sesiones de design thinking con Product
- Documenté trade-offs técnicos en lenguaje de negocio
- Priorizé features basadas en ROI vs esfuerzo técnico
**Resultado**: Definición clara de features, mejor estimación, faster time-to-market

---

## 🎤 PREGUNTAS ESPERADAS & RESPUESTAS PREFORMULADAS

### P1: "¿Tienes experiencia con LangChain o frameworks similares?"
**Respuesta**:
"He trabajado principalmente con APIs nativas (OpenAI, Claude) y n8n para orquestación. LangChain es una abstracción sobre LLMs que simplifica chain composition. Viendo documentación, es similar a lo que ya hago manualmente con prompts encadenados y function calling. Estoy completamente listo para aprender la sintaxis específica de LangChain; lo importante es que entiendo los conceptos detrás (memory management, agent loops, tool use)."

### P2: "¿Por qué no tienes experiencia explícita en fine-tuning?"
**Respuesta**:
"Mi estrategia ha sido maximalizar valor con prompt engineering y RAG antes de invertir en fine-tuning (que es costoso y lento). Para los proyectos que he trabajado, RAG + prompt engineering ha sido suficiente. Entiendo cuándo fine-tuning es necesario: cuando tienes datos específicos que no caben en contexto, o necesitas latencia ultrabajos. Tengo interés en aprender, y OpenAI/Anthropic tienen APIs para esto que puedo explorar rápido."

### P3: "¿Cómo explicarías MLOps si vienes de DevOps clásico?"
**Respuesta**:
"DevOps es about application deployments: versioning, testing, monitoring. MLOps es similar pero para modelos: versionamiento de modelos, data validation, monitoring de model drift. Las herramientas son diferentes (MLflow vs Jenkins), pero los principios son iguales. Tengo experiencia en los principios; las herramientas específicas las aprendo rápido."

### P4: "¿Por qué haces transición de liderazgo técnico a IC (Individual Contributor) en IA?"
**Respuesta**:
"Mi rol como Engineer Lead fue muy rewarding, pero reconocí que mi pasión está en resolver problemas técnicos complejos, no en gestión. IA es donde veo oportunidad de aplicar arquitectura + sistemas thinking en problemas nuevos. Además, Rappi ya conoce mi trabajo y cultura; puedo aportar valor inmediatamente sin curva de aprendizaje en procesos."

### P5: "¿Qué te diferencia de otros candidatos?"
**Respuesta**:
"Tres cosas: (1) Experiencia real en producción con LLMs, no solo proyectos de sandbox. (2) Puedo ligar problemas de negocio a soluciones técnicas (pasé 4 años como Engineer Lead en Rappi entendiendo esto). (3) Stack completo: desde prompt engineering hasta deployment, no solo una pieza. No soy especialista en fine-tuning o training, pero eso no es típicamente el bottleneck en aplicaciones GenAI; es architecture, prompt design, y integration."

---

## 📝 ADAPTACIONES PARA CV & APLICACIÓN

### VERSIÓN NUEVA DEL CV: Enfatizar Python & MLOps

**OPCIÓN A - Agregar Python explícitamente:**
```markdown
### Technical Skills - Backend/MLOps
- **Python**: 6/10 (APIs, n8n workflows, scripting)
- **OpenAI API (GPT-4)**: 8/10 - Prompt engineering, function calling
- **Anthropic API (Claude)**: 8/10 - Agents, system design
- **LangChain**: Frameworks similares (n8n, custom chains)
- **n8n**: 7/10 - Automation, model orchestration
- **AWS**: 7/10 - ECS, S3, ML deployment patterns
```

**OPCIÓN B - Reescribir proyecto legal para enfatizar MLOps:**
```markdown
### Asistente Legal - RAG + Production Deployment
- **Arquitectura**: Retrieval-Augmented Generation (RAG)
- **Stack**: OpenAI API, n8n (Python Code Node), Lovable (Backend)
- **MLOps**: Model versioning (GPT-4), prompt versioning, A/B testing outputs
- **Monitoring**: Usage patterns, response quality, latency
- **Resultado**: Production desde día 1, cliente en onboarding
```

### COVER LETTER / MOTIVACIÓN

**Párrafo clave**:
```
"Tras 4 años en Rappi como Engineer Lead, desarrollé experiencia profunda 
en arquitectura de sistemas y colaboración cross-team. En 2024, reconocí 
que mi pasión está en resolver problemas complejos de ingeniería. La 
transición natural fue hacia IA: donde arquitectura de sistemas meets 
autonomous agents. Mis 3 proyectos en producción demuestran capacidad 
de llevar LLMs desde concepto a cliente. Vuelvo a Rappi no como 
manager, sino como especialista técnico con skin in the game."
```

---

## 📊 TIMELINE RECOMENDADO

### Antes de Entrevista (2-3 semanas si aplicas ahora)

**Semana 1**:
- ✅ Aprende fundamentos de LangChain (1-2 horas)
- ✅ Crea mini-proyecto: FastAPI + Claude API + LangChain simple
- ✅ Documenta: "Aprendiendo LangChain para [problema específico]"

**Semana 2**:
- ✅ Prepara demostraciones de proyectos (legal, TikTok)
- ✅ Practica respuestas STAR (mock interview)
- ✅ Estudia: "MLOps fundamentals" (Andrew Ng course snippet)

**Semana 3**:
- ✅ Refina CV con versión adaptada
- ✅ Revisa arquitectura de Rappi (si puedes)
- ✅ Prepara preguntas para entrevistador

---

## 🎯 POSICIÓN IDEAL PARA ENTREVISTA

> "Soy Software Engineer con 9 años de experiencia, especialista en arquitectura 
> de sistemas distribuidos. Mi transición actual es hacia AI Engineering, donde 
> combino systems thinking con LLMs y agentes autónomos. Tengo 3 proyectos en 
> producción usando RAG, function calling, y agentes. La brecha es que me falta 
> profundidad en Python (6/10 actualmente) y MLOps formal (tengo DevOps clásico). 
> Pero los conceptos fundamentales los tengo claros, y ambos son learnable en 
> 2-3 semanas. Vuelvo a Rappi porque entiendo la cultura y productos; puedo 
> aportar valor desde día 1."

---

## ❓ PREGUNTAS A HACER EN ENTREVISTA

1. "¿Cuál es el stack de LLMs que usan hoy en Rappi? ¿OpenAI, Claude, custom?"
2. "¿Cuál es el maior bottleneck actual: prompt engineering, data availability, o infrastructure?"
3. "¿Hay proyectos específicos de RAG o agentes donde necesitan hands-on?"
4. "¿Qué experiencia esperan realmente en fine-tuning? ¿O es nice-to-have?"
5. "¿Quién sería mi manager? ¿Equipo de IA centralizado o distribuido por productos?"

---

**Fecha de Aplicación**: [PENDIENTE]  
**Última Actualización**: 2026-04-27  
**Estado**: Listo para aplicar + entrevista
