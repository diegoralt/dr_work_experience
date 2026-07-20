---
type: generado
last_updated: 2026-04-26
status: superseded
tags: [plan-ejecutable, 4-semanas, linkedin, desarrollo, balanceado]
---

> **⚠️ Superado (2026-07-20):** ejecución detenida tras el miércoles 29-abril (día 2 de 20) — el resto del plan (mayo completo) nunca se marcó como ejecutado. Mismo motivo que `linkedin-plan-1month.md`: se priorizaron aplicaciones directas sobre content marketing. Se conserva como referencia histórica, no como plan activo.

# Plan Semanal Balanceado: 4 Semanas (Mayo 2026)

**Disponibilidad**: 4 horas diarias (lunes-viernes, 10am-1pm bloqueado)
**Objetivo**: 2 case studies producción + 12 posts LinkedIn + Networking directo + Portfolio visible
**Timing LinkedIn**: Martes-Jueves 9am CDMX
**Networking**: Semana 4 Jueves, 3 horas dedicadas

---

## 📅 SEMANA 1 (Abril 28 - Mayo 2): Caso 1 - Agente de Soporte

### **MARTES (Abril 28) ✅ COMPLETADO**

#### 🔨 DESARROLLO (2.5 horas) ✅
- [x] Setup Supabase: Proyecto creado + 4 tablas + 20 FAQs
- [x] .env.example: Credential management configurado
- [x] setup-secrets.sh: Script interactivo para secretos
- [x] TECHNICAL-SPECIFICATION.md: Documento completo en español
- [x] GitHub: Código pusheado (4 commits)

**Entregable**: Setup completo + documentación + GitHub sincronizado

#### 📱 LINKEDIN (30 min) ✅
**Post 1 - Problem Discovery + Building in Public** ✅ PUBLICADO
Tema: Reforzar IA + Proyectos compartibles + Building in Public
Estado: ✅ Publicado (29 abril, 9am CDMX)
Objetivo: Posicionar como AI engineer construyendo en público
Link: Ver en linkedin.com/in/diego-reyes-altamirano/

**Acción Completada**: Post publicado + engagement iniciado

---

### **MIÉRCOLES (Abril 29) ⏳ HOY - EN PROGRESO****

#### 🔨 DESARROLLO (3 horas)
- [ ] Prompt engineering: Diseñar prompt para clasificación de tickets
- [ ] Definir categorías: Billing, Technical, Feature Request, Bug, Other
- [ ] Definir prioridades: Critical, High, Medium, Low
- [ ] Claude API calls: test con 10 tickets de ejemplo
- [ ] Validar: ¿clasifica correctamente? (meta: 90%+)

**Entregable**: Prompt validado, 10/10 tickets clasificados correctamente

#### 📱 LINKEDIN (30 min)
**Repost/Engagement Day**: 
- [ ] Responder comentarios del post anterior
- [ ] Buscar 3 posts de #AIEngineering, dejar comentarios valuosos
- [ ] Objetivo: iniciar conversación, generar engagement

---

### **JUEVES (Abril 30)**

#### 🔨 DESARROLLO (3 horas)
- [ ] n8n workflow setup: 
  - Trigger: Webhook que recibe tickets
  - Paso 1: Claude API (clasificación)
  - Paso 2: Guardar en Supabase
  - Paso 3: Decisión de respuesta automática
- [ ] Probar workflow end-to-end con 5 tickets
- [ ] Documentar flow (diagrama simple)

**Entregable**: n8n workflow funcionando, diagrama documentado

#### 📱 LINKEDIN (45 min)
**Post 3 - Solution Architecture**
```
Así es como estoy resolviendo el problema:

🏗️ ARQUITECTURA: Agente Inteligente de Soporte

┌─ INGRESO ─────────────────────┐
│  Webhook: Nuevo ticket        │
└──────────────┬────────────────┘
               ↓
┌─ ANÁLISIS ────────────────────┐
│  Claude API:                  │
│  - Categoriza                 │
│  - Asigna prioridad           │
│  - Detecta si es FAQ          │
└──────────────┬────────────────┘
               ↓
┌─ DECISIÓN ────────────────────┐
│  Si FAQ → Respuesta auto      │
│  Si técnico → Asigna dev      │
│  Si crítico → Escala leader   │
└──────────────┬────────────────┘
               ↓
┌─ PERSISTENCIA ────────────────┐
│  Supabase: Registro + notif   │
└───────────────────────────────┘

🔧 Stack:
- Claude API (análisis)
- n8n (orquestación)
- Supabase PostgreSQL (BD)
- Webhooks (integración)

Mañana: implementación completa.

#Architecture #AI #APIDesign
```

**Acción**: Publish + incluir diagrama simple

---

### **VIERNES (Mayo 1)**

#### 🔨 DESARROLLO (3 horas)
- [ ] FAQ base: Crear 15 FAQs reales de soporte SaaS
- [ ] Integrar búsqueda de FAQs en Claude prompt
- [ ] Generar respuestas automáticas para 20 tickets de ejemplo
- [ ] Validar: ¿Respuestas son sensatas? (manual review)
- [ ] Crear dataset de 50 tickets para testing final

**Entregable**: FAQ base + 50 tickets de prueba + respuestas generadas

#### 📱 LINKEDIN (45 min)
**Post 4 - Live Development**
```
Building in public 🔴 LIVE:

Acabo de integrar el FAQ base del agente. Así funcionan las respuestas automáticas:

📝 ENTRADA:
Usuario: "¿Cómo cambio mi plan?"

🤖 AGENTE:
1. Clasifica: Feature Request
2. Busca FAQ
3. Encuentra: "Change Plan - Guide"
4. Genera respuesta contextualizada

📤 SALIDA:
"Tu plan actual es X. Para cambiar a Y:
1. Ve a Configuración
2. Click en 'Plan'
3. Selecciona nuevo plan..."

✅ 18/20 respuestas son sensatas (90% accuracy)

Repo actualizando en tiempo real:
github.com/diegoralt/support-agent-ai

#BuildingInPublic #AIEngineering
```

**Acción**: Publish + incluir ejemplo de salida

---

### **SÁBADO (Mayo 2) - Si aplica para horas extra**

#### 🔨 DESARROLLO (Opcional - 2.5 horas)
- [ ] Testing final: Pasar 50 tickets reales por el sistema
- [ ] Métricas:
  - [ ] Accuracy de clasificación: ¿90%+?
  - [ ] Tiempo promedio: ¿2 min?
  - [ ] Respuestas automáticas: ¿X% de tickets?
- [ ] Documentar resultados en README.md
- [ ] Crear video demo (3-5 min): ticket → respuesta automática
- [ ] Git push: código + resultados

**Entregable**: Sistema funcionando validado, video demo, repo público

#### 📱 LINKEDIN (1.5 horas, incluye video)
**SÁBADO 9am**: Post 5 - Resultados Finales
**SÁBADO 11:30am**: Upload video demo (comentario del post)

```
✅ RESULTADO FINAL: Agente de Soporte AI

Después de 1 semana de desarrollo, aquí están los números:

📊 MÉTRICAS:

Before (Manual):
- 200 tickets/día
- 2.5 minutos/ticket
- 400-500 minutos = 8.3 horas/día

After (IA):
- 180 tickets automáticos (90%)
- 2 minutos/ticket solo complejos (10%)
- ~40 minutos/día
- 🎯 6 HORAS AHORRADAS

📈 ACCURACY: 90% en clasificación, 95% en FAQs

🔧 Stack usado:
- Claude API
- n8n
- Supabase PostgreSQL
- Python + Webhooks

📁 Código abierto: github.com/diegoralt/support-agent-ai

Video demo en comentarios 👇

¿Cuántas horas podría ahorrar tu equipo con IA?

#AIEngineering #Automation #LLMs #ProductBuilding
```

**Acciones**:
- [ ] Publish post principal
- [ ] Comentario: Link a video demo en YouTube
- [ ] Comentario: Link a GitHub repo
- [ ] Responder todas las preguntas en comentarios

#### 📊 SEMANA 1 - Resumen Esperado
- **Posts LinkedIn**: 5 posts (9am CDMX: 28 abril, 29 abril, 30 abril, 1 mayo, 2 mayo)
- **Videos**: 1 video demo (Sábado)
- **Engagement esperado**: 500-700 impresiones/post, 15+ comentarios totales
- **Código**: Repo público con workflow completo
- **Validación**: 50 tickets procesados con 90%+ accuracy

#### ✅ SEMANA 1 - Progreso Real
- **Día 1 (28 abril)**: Setup + Documentación + Post 1 ✅ COMPLETADO
- **Día 2 (29 abril)**: Prompt validation + Post 2 ⏳ HOY
- **Días 3-6**: En progreso

---

## 📅 SEMANA 2 (Mayo 5-9): Caso 2 - RAG - Parte 1 (Setup)

### **LUNES (Mayo 5)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Crear repo: `document-rag-system`
- [ ] Setup Supabase:
  - [ ] Crear tabla `documents` (id, name, content, created_at)
  - [ ] Crear tabla `embeddings` (id, doc_id, text_chunk, vector, metadata)
  - [ ] Habilitar pgvector extension
- [ ] Test conexión a Supabase desde Python
- [ ] Instalar dependencias: langchain, openai, supabase

**Entregable**: Supabase setup completo, conexión confirmada

#### 📱 LINKEDIN (30 min)
**Post 5 - New Case Study Teaser**
```
Próximo reto: RAG (Retrieval-Augmented Generation)

Acabo de terminar un agente de soporte (results abajo 👇).

Ahora es momento de algo más ambicioso:

🎯 El problema: 
Empresas reciben 100s de documentos mensuales (contratos, reportes, PDFs)
Buscar información = 30-40 minutos por documento
Lento, manual, error-prone.

💡 La solución: 
Agente RAG que:
- Entiende contenido de documentos
- Búsqueda instantánea por pregunta
- Respuestas exactas en segundos

Arquitectura viene mañana.

#RAG #VectorSearch #AIArchitecture
```

**Acción**: Publish + Momentum building

---

### **MARTES (Mayo 6)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Prompt engineering para document analysis
- [ ] Crear función: leer PDF → extraer contenido
- [ ] Crear función: texto → embeddings (Claude API)
- [ ] Test: 3 PDFs de ejemplo → embeddings generados
- [ ] Validar: ¿embeddings se guardan en Supabase?

**Entregable**: Pipeline de embedding funcionando

#### 📱 LINKEDIN (45 min)
**Post 6 - RAG Architecture Deep Dive**
```
🏗️ ARQUITECTURA RAG EXPLICADA:

¿Qué es RAG? Retrieval-Augmented Generation

= AI que busca información ANTES de responder

Flujo:

1️⃣ INDEXACIÓN (Se hace una sola vez por documento)
   Documento PDF
   ↓
   Claude extrae contenido
   ↓
   Divide en chunks (fragmentos)
   ↓
   Convierte a vectors (embeddings)
   ↓
   Almacena en DB vectorial (Supabase pgvector)

2️⃣ BÚSQUEDA (Usuario pregunta)
   Usuario: "¿Cuál es el monto del contrato?"
   ↓
   Pregunta → embedding
   ↓
   Busca vectores similares en DB
   ↓
   Retorna chunks relevantes
   ↓
   Claude responde basado en chunks

🔧 Ventajas:
✅ Búsqueda semántica (entiende significado)
✅ Respuestas precisas (basadas en documento)
✅ Información actualizada (sin reentrenamiento)

Stack:
- Claude API (embeddings + análisis)
- Supabase pgvector (vector DB)
- Python (orchestración)

Mañana: primer documento indexado.

#RAG #VectorDatabase #SemanticSearch
```

**Acción**: Publish + Educacional content

---

### **MIÉRCOLES (Mayo 7)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Crear 10 documentos de prueba (PDFs):
  - 3 Contratos
  - 3 Reportes financieros
  - 2 Estados de cuenta
  - 2 Términos y condiciones
- [ ] Indexar los 10 documentos
- [ ] Verificar en Supabase: ¿10 documentos con embeddings?
- [ ] Documentar: # chunks creados, # embeddings, tamaño total

**Entregable**: 10 documentos indexados, métricas de indexación

#### 📱 LINKEDIN (45 min)
**Post 7 - Building Live: Document Indexing**
```
🔴 LIVE BUILDING: Indexando documentos con RAG

Acabo de indexar 10 documentos reales en mi sistema RAG:

📊 ESTADÍSTICAS:
- 10 documentos
- ~50 chunks por documento (promedio)
- 500 embeddings totales
- Tiempo indexación: ~2 minutos
- BD: Supabase pgvector

📝 DOCUMENTOS INDEXADOS:
✅ 3 Contratos (800 págs total)
✅ 3 Reportes financieros
✅ 2 Estados de cuenta
✅ 2 Terms & Conditions

⚡ PRÓXIMO PASO:
Buscar información en estos docs con preguntas naturales.

Ejemplo:
"¿Cuál es la cláusula de terminación?"
"¿Cuándo vence?"
"¿Cuál es el monto?"

Las respuestas vendrán del contenido real de los docs.

#RAG #VectorSearch #DocumentProcessing
```

**Acción**: Publish + Share progress metrics

---

### **JUEVES (Mayo 8)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Crear función de búsqueda:
  - [ ] User query → embedding
  - [ ] Vector similarity search en pgvector
  - [ ] Retornar top 3 chunks relevantes
- [ ] Crear función de respuesta:
  - [ ] Claude: "Responde basado en estos chunks"
- [ ] Test: Hacer 20 preguntas de ejemplo a los documentos
- [ ] Validar resultados: ¿Respuestas correctas? (80%+)

**Entregable**: Búsqueda y respuesta funcionando, 20 queries testeadas

#### 📱 LINKEDIN (45 min)
**Post 8 - Search Results Live**
```
🎯 BÚSQUEDA RAG EN ACCIÓN:

Acabo de hacer 20 preguntas a mi base de documentos.

Aquí están algunos ejemplos:

PREGUNTA 1:
"¿Cuál es la cláusula de terminación del contrato?"
RESPUESTA (en 2 segundos):
"La cláusula de terminación indica que cualquiera de las partes puede 
rescindir este acuerdo con 30 días de notificación escrita..."

PREGUNTA 2:
"¿Cuál es el monto del pago?"
RESPUESTA (en 2 segundos):
"El monto del contrato es USD $50,000 pagadero en cuotas mensuales 
de USD $4,166.67..."

PREGUNTA 3:
"¿Cuándo vence este reporte?"
RESPUESTA (en 2 segundos):
"El reporte es válido hasta el 31 de Diciembre de 2025..."

✅ ACCURACY: 18/20 respuestas correctas (90%)

Esto toma 30-40 minutos de lectura manual.
Con RAG: 2 segundos.

15x más rápido. Cero errores.

#RAG #VectorSearch #ProductDevelopment
```

**Acción**: Publish + ejemplos reales

---

### **VIERNES (Mayo 9)**

#### 🔨 DESARROLLO (2.5 horas)
- [ ] Crear interfaz simple (n8n o Lovable):
  - [ ] Upload documento
  - [ ] Ask question
  - [ ] Get answer
- [ ] Video demo: Upload → Question → Answer
- [ ] Documentar en README.md
- [ ] Git push: código funcional

**Entregable**: Sistema completo, interfaz, video demo, repo

#### 📱 LINKEDIN (1 hora)
**Post 9 - Semana 2 Recap**
```
✅ HITO 2: Sistema RAG Funcionando

Una semana después, mi sistema RAG está listo:

📊 LO QUE CONSTRUIMOS:

1. Vector Database (Supabase pgvector)
   - 10 documentos indexados
   - 500 embeddings
   - Búsqueda en milisegundos

2. Document Processing Pipeline
   - Extrae contenido de PDFs
   - Divide en chunks inteligentes
   - Genera embeddings semánticos

3. Search + Response Engine
   - Búsqueda vectorial (entiende significado)
   - Generación de respuestas con Claude
   - 90% accuracy en 2 segundos

🎬 COMPARACIÓN:

ANTES (Manual):
- 10 documentos = 4-5 horas de lectura
- Búsqueda: 30-40 minutos por documento
- Errores frecuentes

DESPUÉS (RAG):
- 10 documentos = 2 minutos de indexación
- Búsqueda: 2 segundos
- 90% accuracy

⏱️ AHORRO: 95% del tiempo

🔗 Repo: github.com/diegoralt/document-rag-system

Semana 3: Optimización y refinamiento.

#RAG #VectorDatabase #AIProduct
```

**Acciones**: Publish + Engagement

#### 📊 SEMANA 2 - Resumen
- **Posts LinkedIn**: 5 (teaser, architecture, live building, results, recap)
- **Código**: RAG system funcional con interfaz
- **Validación**: 20 queries con 90% accuracy
- **Engagement**: Building in public, momentum building

---

## 📅 SEMANA 3 (Mayo 12-16): Caso 2 - Refinamiento + Optimización

### **LUNES (Mayo 12)**

#### 🔨 DESARROLLO (2.5 horas)
- [ ] Performance optimization:
  - [ ] Medir tiempo de búsqueda actual
  - [ ] Analizar queries lentos
  - [ ] Optimizar índices en pgvector
- [ ] Metadata enrichment:
  - [ ] Agregar tipo de documento
  - [ ] Agregar fecha
  - [ ] Agregar autor
- [ ] Test: ¿búsqueda mejorada?

**Entregable**: Sistema más rápido, metadata enriquecida

#### 📱 LINKEDIN (30 min)
**Engagement focus**: 
- [ ] Buscar 5 posts sobre #RAG o #VectorDatabase
- [ ] Dejar comentarios thoughtful
- [ ] Objetivo: Network building

---

### **MARTES (Mayo 13)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Advanced prompting:
  - [ ] Few-shot examples para mejor respuesta
  - [ ] Instrucciones más específicas a Claude
  - [ ] Handl de edge cases
- [ ] Test con casos complejos:
  - [ ] Preguntas ambiguas
  - [ ] Preguntas que requieren múltiples documentos
  - [ ] Preguntas fuera del scope
- [ ] Iteración: mejorar prompts

**Entregable**: Prompts optimizados, 100% de casos cubiertos

#### 📱 LINKEDIN (45 min)
**Post 10 - Advanced RAG Techniques**
```
🚀 TÉCNICAS AVANZADAS EN RAG:

Después de optimizar mi sistema, aquí aprendí:

1️⃣ FEW-SHOT PROMPTING
Darle ejemplos a Claude de preguntas → respuestas 
ANTES de hacer su pregunta real.

Resultado: 15% mejor accuracy

2️⃣ HYBRID SEARCH
No solo búsqueda vectorial (semántica)
También búsqueda por palabras clave (exactitud)

Resultado: 20% mejor para preguntas específicas

3️⃣ CONTEXTUALIZACIÓN
No solo enviar chunks relevantes
Enviar el "contexto" alrededor del chunk

Resultado: Respuestas 30% más precisas

4️⃣ FALLBACK HANDLING
Si no encuentra respuesta:
- Decir "No encontré respuesta exacta"
- Sugerir documentos relevantes
- Preguntar al usuario por clarificación

Resultado: 0 alucinaciones de IA

💡 LECCIÓN:
RAG no es solo "busca + responde"
Es: "busca bien + responde inteligentemente + maneja errores"

#RAG #PromptEngineering #LLMs
```

**Acción**: Publish + Technical depth

---

### **MIÉRCOLES (Mayo 14)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Create comprehensive test suite:
  - [ ] 50 preguntas variadas (fáciles, medianas, difíciles)
  - [ ] Documentar respuestas correctas esperadas
  - [ ] Pasar todas por el sistema
  - [ ] Medir accuracy final
- [ ] Casos de prueba:
  - [ ] Búsquedas simples (números, fechas)
  - [ ] Búsquedas complejas (interpretación)
  - [ ] Preguntas fuera de scope
  - [ ] Preguntas en idiomas alternos

**Entregable**: Test suite con 50 casos, metrics finales

#### 📱 LINKEDIN (45 min)
**Post 11 - Comprehensive Testing**
```
📊 TESTING FINAL: 50 QUERIES CONTRA EL SISTEMA

Acabo de pasar 50 preguntas variadas por mi RAG system:

📈 RESULTADOS:

Preguntas Fáciles (búsqueda directa):
- "¿Cuál es el monto?" → 100% (10/10)
- "¿Cuándo vence?" → 100% (10/10)

Preguntas Medianas (requieren interpretación):
- "¿Cuáles son los términos?" → 90% (9/10)
- "¿Quién puede rescindir?" → 85% (8.5/10)

Preguntas Difíciles (conexión de múltiples fragmentos):
- "¿Qué pasa si ambas partes quieren cancelar?" → 75% (7.5/10)
- "¿Cuál es el escenario más probable?" → 70% (7/10)

Out of Scope:
- "¿Cuál es tu opinión?" → Correctamente rechazada ✅

ACCURACY GENERAL: 88% 

No es 100%, pero para un RAG sin fine-tuning, es SÓLIDO.

Y estos errores son:
- Respuestas parciales (no completamente erróneas)
- Casos edge (poco frecuentes)
- Preguntas ambiguas

PRODUCCIÓN-READY ✅

#Testing #ProductQuality #RAG
```

**Acción**: Publish + Show rigor

---

### **JUEVES (Mayo 15)**

#### 🔨 DESARROLLO (3 horas)
- [ ] Create demo presentation:
  - [ ] Grabar video 5-7 minutos
  - [ ] Mostrar upload de documento
  - [ ] Hacer 5 preguntas de ejemplo
  - [ ] Mostrar métricas finales
- [ ] Create comprehensive README:
  - [ ] Architecture diagram
  - [ ] Setup instructions
  - [ ] Usage examples
  - [ ] Performance metrics
  - [ ] Lessons learned
- [ ] Polish repo: Clean code, comments

**Entregable**: Professional README, video demo, polished code

#### 📱 LINKEDIN (1 hora)
**Post 12 - Case Study Completo**
```
✅ CASO 2 COMPLETADO: Sistema RAG de Análisis de Documentos

Aquí está el resultado final después de 2 semanas:

📊 EL PROYECTO:
Problema: Empresas tardan 30-40 minutos por documento
Solución: RAG system que busca respuestas en 2 segundos

🏗️ ARQUITECTURA:
- Claude API (análisis + embeddings)
- Supabase pgvector (vector database)
- Python + n8n (orquestación)
- 10 documentos reales (500+ págs)

📈 RESULTADOS:
✅ 88% accuracy en 50 queries
✅ 15x más rápido (40 min → 2 seg)
✅ Zero alucinaciones con fallback handling
✅ Producción-ready

💾 STACK:
```
User Query
   ↓
Embedding (Claude)
   ↓
Vector Search (pgvector)
   ↓
Context Assembly
   ↓
LLM Response (Claude)
   ↓
Answer
```

📁 CÓDIGO ABIERTO:
github.com/diegoralt/document-rag-system

🎬 DEMO VIDEO:
[Link en comentario abajo]

🎓 LECCIONES APRENDIDAS:
1. RAG es 80% búsqueda, 20% generación
2. Metadata es crítica para relevancia
3. Few-shot prompting > zero-shot
4. Error handling es key para producción

Próximo: Consolidación y career insights.

#RAG #ProductBuilding #AIEngineering
```

**Acciones**: Publish + Video comment + Engagement

---

### **VIERNES (Mayo 16)**

#### 🔨 DESARROLLO (2 horas)
- [ ] Final polish:
  - [ ] Code review (Claude Code)
  - [ ] Fix any bugs
  - [ ] Add error handling
  - [ ] Final git push
- [ ] Create summary document:
  - [ ] Learnings técnicos
  - [ ] Learnings de producto
  - [ ] Qué haría diferente
  - [ ] Siguientes pasos posibles

**Entregable**: Production-ready code, comprehensive learnings doc

#### 📱 LINKEDIN (30 min)
**Engagement + Momentum**:
- [ ] Respond to all comments on week's posts
- [ ] Share learnings in comments
- [ ] Mention people en tech (non-spammy)

#### 📊 SEMANA 3 - Resumen
- **Posts LinkedIn**: 4 (optimization, advanced techniques, testing, case study)
- **Código**: Production-ready RAG system
- **Validación**: 50 queries, 88% accuracy
- **Documentation**: Professional README + learnings

---

## 📅 SEMANA 4 (Mayo 19-23): Consolidación + Portfolio

### **LUNES (Mayo 19)**

#### 🔨 DESARROLLO (2 horas)
- [ ] Create comparison document:
  - [ ] Caso 1 vs Caso 2
  - [ ] Métricas comparativas
  - [ ] Tech stack differences
  - [ ] Use cases for each
- [ ] Portfolio cleanup:
  - [ ] Update GitHub profile
  - [ ] Add both projects to pinned repos
  - [ ] Create GitHub org or collection

**Entregable**: Portfolio visibly improved

#### 📱 LINKEDIN (45 min)
**Post 13 - Career Reflection**
```
🤔 REFLEXIÓN: De Android Engineer a AI Engineer

Hace 9 años empecé como Android Developer.
Hace 6 meses decidí transición a AI.
Hace 4 semanas construí 2 sistemas AI en producción.

Lo que aprendí sobre esta transición:

✅ LA BUENA NOTICIA:
Mi base técnica (architecture, systems, backend) transferida perfectamente
No necesité reaprender foundations
Solo necesité nuevas herramientas (Claude, vectorial DBs, prompting)

⚠️ LO DESAFIANTE:
- AI requiere "pensar diferente" (probabilidad, no determinismo)
- Prompt engineering es half art, half science
- Debugging es más complejo (no hay stack traces)
- Testing requiere otro mindset

💡 LOS SKILLS QUE IMPORTAN:
1. Problem decomposition (viene del backend)
2. System thinking (viene de microservicios)
3. Documentation (viene de liderazgo)
4. Curiosity (nueva)

🎯 OPORTUNIDAD REAL:
Engineers con base TÉCNICA que aprenden IA
> Generalists sin foundation

Porque no es "aprender IA"
Es "aplicar engineering a IA"

#CareerTransition #AIEngineering #LearningJourney
```

**Acción**: Publish + Vulnerable pero real

---

### **MARTES (Mayo 20)**

#### 🔨 DESARROLLO (2.5 horas)
- [ ] Create unified demo:
  - [ ] Single GitHub org con ambos proyectos
  - [ ] Shared documentation
  - [ ] Comparison guide
  - [ ] Deployment instructions
- [ ] Create showcase website (simple):
  - [ ] Lovable o HTML simple
  - [ ] 2 case studies featured
  - [ ] Links a repos + videos
  - [ ] Contact info

**Entregable**: Unified portfolio online

#### 📱 LINKEDIN (45 min)
**Post 14 - Lessons Learned (Technical)**
```
3 LECCIONES TÉCNICAS CONSTRUYENDO 2 SISTEMAS AI:

Caso 1: Agente de Soporte

Lección 1: Prompt Engineering is 80% of the work
→ Pasé 40% del tiempo tuneando prompts
→ Pequeños cambios = grandes impactos en accuracy
→ La mejor "arquitectura" es una prompt clara

Lección 2: n8n es subestimado
→ No escribí código para orquestación
→ Todo visual, fácil de debuggear
→ Perfect para MLOps sin DevOps

Lección 3: Error handling > Happy path
→ 20% del tiempo: qué cuando falla
→ Fallback, retry, escalation
→ Eso define si es producción-ready

---

Caso 2: RAG System

Lección 4: Metadata es crítica
→ El 50% del accuracy viene de metadata
→ No solo "busca", sino "busca bien"
→ chunking strategy > raw vector search

Lección 5: Hybrid search > pure vector search
→ Keyword search + semantic search
→ Algunos casos necesitan exactitud
→ Otros necesitan comprensión

Lección 6: RAG costo/beneficio es ALTO
→ Complejidad: media
→ ROI: muy alto
→ Aplica a 80% de empresas

---

Si construyes AI systems, estas 6 lecciones son oro puro.

#AIEngineering #LessonLearned #ProductDevelopment
```

**Acción**: Publish + Technical insights

---

### **MIÉRCOLES (Mayo 21)**

#### 🔨 DESARROLLO (2.5 horas)
- [ ] Create comprehensive blog post:
  - [ ] "Building 2 AI Products in 4 Weeks"
  - [ ] Problem → Solution → Metrics
  - [ ] Technical deep dives
  - [ ] Lessons learned
  - [ ] Next steps
- [ ] Format para LinkedIn native + Medium
- [ ] Add visuals/diagrams

**Entregable**: Comprehensive writeup

#### 📱 LINKEDIN (1 hora)
**Post 15 - Complete Case Study**
```
📝 CONSTRUCCIÓN DE 2 PRODUCTOS AI EN 4 SEMANAS: CASE STUDY COMPLETO

Resumen ejecutivo:
Problema: Identificar procesos que IA puede optimizar
Tiempo: 4 semanas (3-4h diarias)
Resultado: 2 sistemas en producción, documentados, replicables

---

PROYECTO 1: Agente Inteligente de Soporte

Problem: 200 tickets/día, 8.3 horas/día en triage manual

Solution Architecture:
- Webhook ingesta
- Claude API clasificación
- n8n orquestación
- Supabase persistencia
- Fallback escalation

Results:
- 90% automation
- 6 horas/día ahorradas
- 90% accuracy

Time: 4 días

Tech:
- Claude API
- n8n
- PostgreSQL

---

PROYECTO 2: RAG Document Analysis System

Problem: 30-40 min por documento, búsqueda manual

Solution Architecture:
- PDF ingestion
- Claude embeddings
- pgvector storage
- Semantic search
- Context-aware responses

Results:
- 95% time reduction (40 min → 2 sec)
- 88% accuracy
- 500+ documents indexed capacity

Time: 10 días

Tech:
- Claude API
- Supabase pgvector
- Python
- n8n

---

PORTFOLIO IMPACT:

Before:
- 3 proyectos IA demostrados
- Nivel: prototipo

After:
- 5 proyectos IA demostrados
- Nivel: producción
- Story: clara (Android → AI Engineer)
- Skills: evidentes (3-5 year level)

---

📚 FULL DOCUMENTATION:

Repo 1: github.com/diegoralt/support-agent-ai
Repo 2: github.com/diegoralt/document-rag-system
Blog: [medium article link]
Demos: [youtube playlist]

Si buscas inspiración para construir IA products,
Este case study está 100% open source.

#BuildingInPublic #AIProducts #OpenSource
```

**Acciones**: 
- Publish main post
- Share blog post link in comment
- Share repos in comment
- Answer all questions

---

### **JUEVES (Mayo 22)**

#### 🔨 DESARROLLO (1.5 horas)
- [ ] Final polishing:
  - [ ] Check all repos one last time
  - [ ] Verify all links work
  - [ ] Test videos play
  - [ ] Ensure READMEs are professional
- [ ] Create one-page summary:
  - [ ] 2 projects
  - [ ] Key metrics
  - [ ] Tech stack
  - [ ] Impact
  - [ ] Next steps

**Entregable**: Everything polished and ready

#### 🔴 NETWORKING DIRECTO (3 horas) - CRÍTICO
**Este es el bloque más importante para conseguir oportunidad**

- [ ] Identifica 10 reclutadores/hiring managers targets:
  - [ ] 3-4 de Rappi (busca "Rappi + Hiring Manager/Recruiter" en LinkedIn)
  - [ ] 2-3 de Sezzle, Yuno, Banregio, PMG
  - [ ] 2-3 de startups AI en México
  
- [ ] Para cada uno, personaliza mensaje:
  ```
  "He pasado las últimas 4 semanas construyendo sistemas IA en producción:
  1. Agente de clasificación de tickets (Claude API + n8n)
  2. Sistema RAG de análisis de documentos (pgvector + embeddings)
  
  Resultado: 2 repos públicos con validación técnica clara.
  
  Estoy explorando roles de AI Engineer donde pueda aplicar 
  esta base técnica + 9 años de experiencia en arquitectura.
  
  ¿Conversamos sobre oportunidades en [Company]?"
  ```

- [ ] Send 5-10 messages personalizados
- [ ] Identifica 2-3 roles específicos en LinkedIn/company sites
- [ ] Apply directamente con cover letter mencionando projects

**Entregable**: 5-10 mensajes enviados, 2-3 aplicaciones directas

#### 📱 LINKEDIN (30 min)
- [ ] Responde comentarios del post de Miércoles
- [ ] No publiques nuevo post (ahorra energy para viernes)

---

### **VIERNES (Mayo 23)**

#### 🔨 DESARROLLO (1 hora)
- [ ] Meta work:
  - [ ] Review all 12 posts
  - [ ] Analyze performance
  - [ ] Document learnings
  - [ ] Document outreach results (who answered, interest level)
  - [ ] Plan next month

**Entregable**: Complete portfolio + outreach performance analysis

#### 📱 LINKEDIN (1.5 hora)
**VIERNES 9am**: Post 12 - Month Recap + Career Transition

```
🎉 MES 1 COMPLETADO: De idea a 2 productos en producción + networking activo

Hace 30 días, decidí ser serio sobre transición a AI Engineer:
"Construir 2 sistemas en producción y comunicar el journey"

Hoy, es realidad.

---

📊 RESULTADOS:

Posts publicados: 12 (quality > quantity)
Total reach: 8,000+ impresiones
Engagement: 60+ comentarios, 150+ reacciones (estimate)
**Conversaciones iniciadas**: 5-10 mensajes de reclutadores + 2-3 aplicaciones directas enviadas

Proyectos completados: 2
- Agente de soporte: 90% automation, 6h/day saved, 90% accuracy
- RAG system: 95% faster, 88% accuracy, 500+ docs capacity

Código abierto: 2 repos, 300+ líneas production code, profesional

Validación: 70 test cases, 90%+ accuracy average

**Networking**: 5-10 mensajes personalizados, 2-3 aplicaciones directas

---

🎓 LO QUE APRENDÍ:

✅ Building in public genera credibilidad real (no clicks vacíos)
✅ La gente quiere ver el proceso, no solo los resultados
✅ Timing + persistence en networking > esperar contactos pasivos
✅ Tu base técnica (9 años) + IA reciente = perfil raro + valioso
✅ 4 semanas SÍ es suficiente para MVP→ Producción

⚠️ LO DESAFIANTE:
- Documentación toma 30% del tiempo (pero es crítica)
- Testing es tedioso pero define si es production-ready
- Prompt engineering es iterativo
- Outreach activo es incómodo pero necesario

---

🎯 PRÓXIMOS PASOS:

Mes 2: 
- Seguimiento a conversaciones iniciadas
- Profundizar en agents + workflows complejos
- Multi-modal systems (vision + audio)
- Open source contributions
- Convertir una conversación en oferta

---

🔑 INSIGHT FINAL:

No es "aprender IA"
Es "aplicar 9 años de engineering a IA"

Eso es raro.
Eso es valioso.
Eso es lo que diferencia.

Repos:
github.com/diegoralt/support-agent-ai
github.com/diegoralt/document-rag-system

#TransitionAIEngineer #BuildingInPublic #CareerGrowth
```

**Acciones**: 
- Publish recap
- Responde comentarios activamente
- Document outreach feedback

---

## 📊 PLAN SUMMARY - 4 SEMANAS (AJUSTADO)

### **Por Números**:
| Métrica | Total |
|---------|-------|
| **LinkedIn Posts** | 12 (quality > quantity) |
| **Videos demostrados** | 2 |
| **Desarrollo horas** | ~55-60h |
| **Proyectos completados** | 2 |
| **Código líneas** | ~400-500 |
| **Test cases** | 70+ |
| **Repos abiertos** | 2 |
| **Validación accuracy** | 90%+ promedio |
| **Networking directo** | 5-10 mensajes, 2-3 aplicaciones |

### **Por Semana**:
- **Semana 1**: Agente soporte (MVP → Validación → Publicación) + 1 video
- **Semana 2**: RAG setup (Indexación → Búsqueda)
- **Semana 3**: RAG refinamiento (Optimización → Testing → Producción) + 1 video
- **Semana 4**: Portfolio consolidación + **NETWORKING DIRECTO** (critical)

### **Impacto Esperado**:
- ✅ Portfolio de 2 proyectos en producción visible
- ✅ 12 posts de alto valor mostrando progreso real
- ✅ 8,000-11,000 impresiones (LinkedIn reach)
- ✅ **5-10 conversaciones iniciadas activamente** (no pasivo)
- ✅ **2-3 aplicaciones directas enviadas**
- ✅ Posicionamiento como "AI Engineer Mid (3-5 años)"
- ✅ Atracción real de reclutadores objetivo
- ✅ Probabilidad oportunidad: **85%** (con networking)

---

## ✅ PRÓXIMO PASO - CHECKLIST PRE-LAUNCH

**Antes de Lunes 28 de Abril**:
- [ ] Confirmar disponibilidad: ¿4h/día bloqueadas 10am-1pm sin interrupciones?
- [ ] Setup técnico: Supabase, n8n, Claude API keys listos
- [ ] GitHub: 2 repos creados y públicos
- [ ] Research: Identificar 10 reclutadores target (para Semana 4)
- [ ] Video: Verificar micrófono/cámara para demos

**Lunes 28 de Abril - START**:
- [ ] Crear repo `support-agent-ai`
- [ ] Setup inicial (Claude API, Supabase, n8n)
- [ ] Publicar Post 1 a las 9am CDMX
- [ ] Responder comentarios en 15min

---

**Plan creado**: 2026-04-26
**Última actualización**: 2026-04-29
**Inicio**: Martes 28 de Abril, 2026 (Zona CDMX)
**Duración**: 4 semanas (hasta Viernes 23 de Mayo)
**Status**: ✅ EN EJECUCIÓN - Day 1 Completado

**Avance Real**:
- Day 1 (28 abril): Setup + Documentación + Post 1 ✅ COMPLETADO
- Días 2-5: En progreso ⏳
- Documentación: caso-1-status.md + proyecto-ia-index.md creados

**Cambios clave aplicados**:
- Posts: 16 → 12 (quality focus)
- Timing: Martes/Jueves 9am CDMX agregado
- Networking: 3 horas directo Semana 4 (CRÍTICO)
- Videos: Asignadas explícitamente (Viernes)
- Reach esperado: 4,000 → 8,000-11,000 impresiones
- Oportunidad: 60% → 85% con networking directo
