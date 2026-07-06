# folionet-workflow-newsletter
**Versión:** v0 — loop independiente para el newsletter/email. Cadencia semanal fija (miércoles), distinta a LinkedIn.

## Qué hace
El ciclo completo del newsletter semanal: idea → filtro → estructura → generación → compliance → enviar → feedback (open/click rate). Corre en Mailchimp hoy.

---

## EL LOOP

### 1 — IDEA
Fuente: tema de la semana del calendario de Substack/newsletter, ticket themes (una vez exista el audit), o el mismo tema del post de LinkedIn de esa semana, adaptado a formato largo.

### 2 — FILTRO DE VOZ + ICP
Carga: `folionet-icp` + `folionet-voice`
El email permite más profundidad que LinkedIn — usar eso, no comprimir el tema.

### 3 — ESTRUCTURA
Newsletter spine: gancho (situación que el ICP reconoce) → contexto (por qué importa) → idea accionable → un solo CTA.
Nunca dos CTAs en el mismo email.

### 4 — GENERAR
Carga: `folionet-content-system` (sección EMAIL — template de asunto, preview text, cuerpo, footer regulatorio)
Salida: asunto (máx. 6 palabras, sin signos de exclamación), preview (máx. 10 palabras), cuerpo 200-300 palabras, footer FINRA/SIPC obligatorio.

### 4.5 — CALIFICAR
Carga: `folionet-grader`
Califica hook, voz, alineación al pilar/ICP, y formato (1-10). Si la nota es menor a 8, aplicar los ajustes sugeridos antes de continuar. Esto NO califica compliance — ese sigue siendo el siguiente paso, siempre humano.

### 5 — COMPLIANCE (obligatorio, sin excepción para email)
El footer regulatorio (Folionet Financial LLC — Miembro FINRA/SIPC / Folionet Advisers LLC — RIA) es obligatorio en cada envío, no opcional. Verificar antes de cada envío.

### 6 — ENVIAR
Miércoles, vía Mailchimp. Confirmar segmentación de audiencia si aplica (nuevos suscriptores en welcome sequence se excluyen del envío regular esa semana).

### 7 — FEEDBACK
Carga: `folionet-data`
Métrica clave: open rate (benchmark 35-45%) y click rate del CTA (benchmark 5-8%). Qué asunto funcionó mejor alimenta la próxima idea.

---

## PROMPT MAESTRO
```
Referencia /folionet-workflow-newsletter.

Tema de esta semana: [tema]

Llévame paso a paso hasta el email completo listo para Mailchimp,
con asunto, preview, cuerpo, CTA y footer regulatorio.
```

## MÉTRICA DE ÉXITO DE ESTE LOOP
Open rate 35-45%, click rate del CTA 5-8%, nuevos suscriptores/semana 20-50 (ver `folionet-data`).

## NOTA — SUBSTACK
Si el equipo decide migrar de Mailchimp a Substack, este loop no cambia de estructura — solo cambia el Paso 6 (dónde se envía). El resto del proceso es idéntico.

## LO QUE SIGUE MANUAL
Enviar en Mailchimp y pegar el reporte de apertura/clics cada semana en `folionet-data`.
