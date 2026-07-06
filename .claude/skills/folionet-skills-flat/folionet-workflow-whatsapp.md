# folionet-workflow-whatsapp
**Versión:** v0 — loop independiente para WhatsApp. A diferencia de LinkedIn/Newsletter, este NO corre en calendario fijo — se dispara por eventos específicos.

## Qué hace
El ciclo de WhatsApp para 3 situaciones puntuales: seguimiento post-discovery-call, alerta de mercado urgente, reactivación de lead frío. Cada una tiene su propio trigger, no una cadencia semanal.

---

## LOS 3 TRIGGERS (no hay Paso 1 "idea" genérico — cada trigger dispara su propio flujo)

### Trigger A — Post-discovery-call
**Cuándo:** inmediatamente después de que alguien tuvo su llamada con el CEO.
**Objetivo:** cerrar el loop con el link de apertura de cuenta, sin presión.

### Trigger B — Alerta de mercado
**Cuándo:** evento relevante (anuncio de la Fed, devaluación, noticia que afecta directamente al ICP).
**Objetivo:** posicionar a Folionet como quien explica lo que pasa, con un CTA suave a conversar.

### Trigger C — Reactivación de lead frío
**Cuándo:** alguien tuvo contacto (llamada o inscripción) hace tiempo y no avanzó.
**Objetivo:** reabrir la conversación sin sonar a spam — máximo 1x cada varias semanas por contacto.

---

## EL LOOP (aplica a los 3 triggers)

### 1 — DETECTAR EL TRIGGER
¿Cuál de los 3 aplica ahora?

### 2 — FILTRO DE VOZ
Carga: `folionet-voice`
WhatsApp es más personal y directo que LinkedIn — nunca copiar/pegar el tono de un post de LinkedIn aquí.

### 3 — GENERAR
Carga: `folionet-content-system` (sección WHATSAPP — ya tiene las 3 plantillas exactas por situación)
Salida: mensaje máx. 150 palabras, 1-2 emojis máximo, siempre personalizado con el nombre, opt-out implícito.

### 3.5 — CALIFICAR
Carga: `folionet-grader`
Califica voz y formato (1-10) — en WhatsApp el criterio de "hook" pesa menos, el de tono personal pesa más. Si la nota es menor a 8, ajustar antes de compliance.

### 4 — COMPLIANCE
Mismo checklist universal — sin promesas de rendimiento, sin presión. Aprobación humana.

### 5 — ENVIAR
Manual hoy — quien maneje la relación con el cliente (CEO o quien haga seguimiento) lo envía directamente.

### 6 — FEEDBACK
No hay "reporte semanal" aquí como LinkedIn/Email — el feedback es cualitativo: ¿respondió? ¿agendó/reactivó? Registrar esto informalmente (puede alimentar `folionet-data` como un número más: "reactivaciones de WhatsApp exitosas/mes").

---

## REGLA DE FRECUENCIA — LA MÁS IMPORTANTE DE ESTE LOOP
Máximo 1 mensaje de WhatsApp por semana al mismo contacto, sin excepción. Este canal se quema rápido si se abusa — a diferencia de LinkedIn/Email, aquí el costo de sentirse invasivo es alto.

---

## PROMPT MAESTRO
```
Referencia /folionet-workflow-whatsapp.

Trigger: [post-discovery-call / alerta de mercado / reactivación de lead frío]
Contexto: [nombre del contacto, qué pasó, qué quieres lograr]

Dame el mensaje listo para enviar.
```

## LO QUE SIGUE MANUAL
Todo — este es el loop más manual de los 3, por diseño. WhatsApp no se automatiza tan fácil (ni se debería) porque pierde el toque personal que lo hace funcionar.
