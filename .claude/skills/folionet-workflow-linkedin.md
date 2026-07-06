# folionet-workflow-linkedin
**Versión:** v0 — loop independiente para LinkedIn. Antes vivía dentro de `folionet-workflow` (deprecado), ahora es su propio sistema.

## Qué hace
El ciclo completo de contenido de LinkedIn: idea → filtro → pilar → generación → compliance → publicar → feedback. Cadencia: martes y jueves (post CEO), viernes (repurpose en página de empresa).

---

## EL LOOP

### 1 — IDEA
Fuente: `folionet-trends-research` (research de tendencias, lunes), calendario de contenido, o algo puntual del mercado.

### 2 — FILTRO DE VOZ + ICP
Carga: `folionet-icp` + `folionet-voice`
¿A cuál perfil le habla? ¿Es coherente con el tono de Folionet?

### 3 — UBICAR EN PILAR
Carga: `07-linkedin-pillars-audit.md` (4 pilares) + `16-competencia-latam-final.md` (diferenciador vs. Quiena/Hapi/Trii)
¿Categoría, Mitos, Data Breakdown, o Autoridad del Fundador?

### 4 — GENERAR
Carga: `folionet-content-system` (sección LinkedIn específicamente — template, CTA library, reglas de formato)
Salida: post completo 150-300 palabras, CTA de la etapa de funnel correcta, máximo 3 hashtags.

### 4.5 — CALIFICAR
Carga: `folionet-grader`
Califica hook, voz, alineación al pilar/ICP, y formato (1-10). Si la nota es menor a 8, aplicar los ajustes sugeridos antes de continuar. Esto NO califica compliance — ese sigue siendo el siguiente paso, siempre humano.

### 5 — COMPLIANCE (obligatorio)
Checklist estándar de `folionet-content-system`. Aprobación humana siempre.

### 6 — PUBLICAR
Martes/jueves vía Metricool (o manual si Metricool no está listo). Viernes: repurpose visual en página de empresa.

### 7 — FEEDBACK
Carga: `folionet-data`
Cada lunes: ¿qué pilar/formato tuvo mejor engagement? Esa respuesta alimenta la próxima idea (vuelve al Paso 1).

---

## PROMPT MAESTRO
```
Referencia /folionet-workflow-linkedin.

Idea: [tu idea en una frase]

Llévame paso a paso hasta el post de LinkedIn listo para publicar,
incluyendo a qué pilar pertenece y el chequeo de compliance.
```

## MÉTRICA DE ÉXITO DE ESTE LOOP
Engagement rate (3-5% benchmark) + follower growth (+50-100/semana) — ver `folionet-data` para benchmarks completos.

## LO QUE SIGUE MANUAL
Publicar y pegar el feedback semanal — igual que todos los loops de canal, hasta que exista integración API.
