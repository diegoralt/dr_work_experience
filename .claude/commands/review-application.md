---
description: Corre el pipeline drafter-reviewer + ATS-check sobre una aplicación ya generada, antes de enviarla
argument-hint: [slug-empresa-rol]
---

Slug: $ARGUMENTS

1. Resuelve rutas por convención de slug:
   - CV: `source/cvs/cv_for_$ARGUMENTS.md`
   - Tracking: `generated/$ARGUMENTS-application.md`
   - PDF: `generated/cvs-pdf/diego-reyes-altamirano-$ARGUMENTS.pdf`
   Si alguno no existe, dilo y detente.

2. Lanza el subagente `cv-reviewer` con las tres rutas. Si ya leíste el CV en este paso, pásale el contenido inline en el prompt en vez de pedirle que lo vuelva a leer.

3. Con la respuesta del reviewer:
   - Aplica la Parte A (ediciones puntuales) directamente con Edit sobre `source/cvs/cv_for_$ARGUMENTS.md`, una por una.
   - Para la Parte B, decide junto con el usuario qué incorporar — no la apliques mecánicamente.
   - Nunca incorpores una sugerencia que invente datos no verificados en source/profile/.

4. El ATS-check aplica solo al CV (no hay cover letter en este flujo). Extrae las keywords requeridas/preferidas de la sección "Mapeo Perfil vs Requisitos" del tracking file y corre:
   `python3 .claude/scripts/ats_check.py "generated/cvs-pdf/diego-reyes-altamirano-$ARGUMENTS.pdf" "kw1,kw2,kw3,..."`
   Si el CV se editó en el paso 3, regenera el PDF antes de correr el check.

5. Presenta: reporte del reviewer (Parte A aplicada / Parte B pendiente de decisión) + resultado del ATS-check. No marques la aplicación como lista sin aprobación explícita del usuario.
