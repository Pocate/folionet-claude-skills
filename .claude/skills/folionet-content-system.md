# folionet-content-system
**Version:** v0 — Complete content production system. LinkedIn + Email + WhatsApp.
**Purpose:** Take a topic → output a complete, ready-to-publish piece with post text, CTA, link, hashtags, and format — nothing to fill in.

---
# folionet-content-system
**Version:** v0 — Complete content production system. LinkedIn + Email + WhatsApp.
**Purpose:** Take a topic → output a complete, ready-to-publish piece with post text, CTA, link, hashtags, and format — nothing to fill in.

---

## DIFERENCIACIÓN COMPETITIVA — TENER SIEMPRE PRESENTE

Investigación de competencia (Julio 2026) confirmó: el único competidor directo real es **Quiena Inversiones** (mismo modelo RIA, pero frío/automatizado). El resto (Hapi, Ualá, Trii) son brokers autogestionados — audiencia distinta, no compiten por el mismo servicio.

**El ángulo diferenciador central que todo contenido debe reforzar cuando sea relevante:**
> "Asesor humano y regulado — no un algoritmo frío (como Quiena) ni trading gamificado (como Hapi/Trii)."

**Reglas prácticas derivadas de esto:**
[... esto es lo que falta ...]

---
## CTA LIBRARY
*Use these exact CTAs. Never invent new ones. Pick based on funnel stage.*

### CTAs de captura por comentario (DM lead capture)
*Usar cuando el objetivo es generar un DM calificado a partir de un post educativo.*
- "Comenta '[PALABRA CLAVE]' y te envío la guía completa por privado."
- "Escribe '[PALABRA CLAVE]' en los comentarios — te la mando por mensaje."
- "¿Quieres la guía completa? Comenta '[PALABRA CLAVE]' y te la envío."

*Regla: [PALABRA CLAVE] debe coincidir exactamente con el tema del post (ej. 'ETF' solo en posts de ETF, 'IPO' solo en posts de IPO). Nunca reciclar la palabra clave de un tema distinto — es el error que encontramos en el batch de Mayo/Junio 2026, donde un CTA de "ETF" quedó pegado a un post sobre IPOs.*

### CTAs de conversión directa (bottom funnel)
- "¿Tienes capital que no está trabajando como debería? Conversemos. [LINK: discovery call]"
- "¿Quieres saber si una Cuenta Asesorada es para ti? Una llamada de 20 minutos lo responde. [LINK: discovery call]"
- "Abre tu cuenta en menos de 10 minutos. [LINK: app / sign up]"
- "Agenda una llamada sin costo con nuestro equipo. [LINK: discovery call]"

### CTAs de consideración (mid funnel)
- "¿Tienes preguntas? Las respondo en los comentarios."
- "¿En qué etapa estás tú? Cuéntame en los comentarios."
- "Guarda este post — es la pregunta que más me hacen."
- "¿Conoces a alguien en esta situación? Compártelo."

### CTAs de awareness (top funnel)
- "¿Qué tema de inversión quieres que cubra la próxima semana?"
- "¿Esto es algo que nadie te había explicado antes? Comenta."
- "Sígueme para más contenido sobre inversiones para latinoamericanos."

### CTA para email
- "Si tienes capital que no está trabajando como debería, [agenda una llamada aquí → LINK]."
- "¿Quieres saber si una Cuenta Asesorada tiene sentido para tu situación? [Hablemos → LINK]."
- "Da el primer paso. [Abre tu cuenta hoy → LINK]."

---

## LINK LIBRARY
*Actualizar con los links reales de Folionet antes de publicar.*

| Destino | Link placeholder | Cuándo usar |
|---------|-----------------|-------------|
| Discovery call | [LINK-DISCOVERY] | Bottom funnel — CA específico |
| Abrir cuenta | [LINK-SIGNUP] | Bottom funnel — self-directed |
| Página Cuenta Asesorada | [LINK-CA] | Mid funnel — educación CA |
| App download | [LINK-APP] | Bottom funnel — mobile |
| Newsletter signup | [LINK-NEWSLETTER] | Top funnel — captura email |
| Folionet.com | [LINK-WEB] | General referencia |

---

## THE FULL CONTENT PRODUCTION PROMPT

Copia y pega esto en Claude cuando necesites crear contenido:

```
Referencia /folionet-voice, /folionet-icp, y /folionet-content-calendar.

Crea contenido completo para Folionet sobre el siguiente tema:

TEMA: [descripción del tema o tendencia]
ÁNGULO: [mito / dato / educación / historia CEO / categoría / 
         costo del status quo / comparación]
SEMANA: [número de semana o fecha]
FUNNEL STAGE: [awareness / consideración / conversión]
CANAL PRINCIPAL: [LinkedIn CEO / Email / WhatsApp]

Output requerido:

── LINKEDIN CEO ──
Post completo (150-300 palabras)
CTA: [del CTA library según funnel stage]
Link: [del link library]
Hashtags: máximo 3
Día recomendado: martes o jueves
Nota de compliance: ¿hay algo que revisar?

── EMAIL ──
Asunto: (máximo 6 palabras)
Preview text: (máximo 10 palabras, no repite el asunto)
Cuerpo: 3 párrafos cortos
CTA final con link
Nota de compliance: ¿hay algo que revisar?

── WHATSAPP ──
Mensaje corto (máximo 150 palabras)
Tono: más personal, más directo que LinkedIn
Sin hashtags
CTA con link

Compliance universal: sin promesas de rendimiento,
sin testimoniales sin aprobación, escenarios hipotéticos
claramente framed como hipotéticos.
```

---

## LINKEDIN — FORMATO COMPLETO

### Template base
```
[HOOK — 1-2 líneas que paran el scroll]

[Línea en blanco]

[DESARROLLO — 3-5 párrafos cortos o bullets]
[Una idea por párrafo]
[Línea en blanco entre cada uno]

[CIERRE — 1-2 líneas que reencuadran el tema]

[Línea en blanco]

[CTA — del CTA library]

[Línea en blanco]

#Hashtag1 #Hashtag2 #Hashtag3
```

### Reglas de formato LinkedIn
- Primera línea: sola, sin contexto previo. Para el scroll.
- Cero emojis o máximo 1 — nunca decorativo
- Línea en blanco entre cada idea — se lee mejor en mobile
- 150-300 palabras — nunca más
- Hashtags al final, nunca en medio del texto
- Nunca terminar con "¡Sígueme para más!" — suena a spam

---

## EMAIL — FORMATO COMPLETO

### Template base
```
Asunto: [curiosidad o dato — 6 palabras]
Preview: [amplía el asunto, no lo repite — 10 palabras]

──────────────────────────────

Hola [nombre],

[Párrafo 1 — gancho: situación que el ICP reconoce (2-3 líneas)]

[Párrafo 2 — contexto: por qué importa (3-4 líneas)]

[Párrafo 3 — idea accionable: lo que cambia si actúan (2-3 líneas)]

[CTA — una acción, directa, sin presión]
[LINK]

──────────────────────────────
Folionet Financial LLC — Miembro FINRA/SIPC
Folionet Advisers LLC — Asesor de Inversiones Registrado
Florida, Estados Unidos

[Unsubscribe] · [Ver en el navegador]
```

### Reglas de formato email
- Asunto sin signos de exclamación — restan credibilidad
- Preview no empieza con "En este email..." ni "Hoy hablamos de..."
- Un solo CTA por email — nunca dos
- Footer regulatorio siempre incluido
- Longitud ideal: 200-300 palabras en el cuerpo

---

## WHATSAPP — FORMATO COMPLETO

### Cuándo usar WhatsApp
- Broadcast a lista de prospectos que dieron opt-in
- Seguimiento post-discovery call
- Alertas de mercado urgentes (Fed, devaluaciones)
- Reactivación de leads fríos

### Template base
```
Hola [nombre] 👋

[1-2 líneas: por qué te escribo ahora / contexto relevante]

[2-3 líneas: el valor — qué está pasando en el mercado 
o qué oportunidad existe para ellos específicamente]

[CTA directo — una acción]
[LINK]

Cualquier duda me escribes aquí mismo.
— [Nombre del CEO / asesor]
```

### Reglas de formato WhatsApp
- Tono más personal que LinkedIn — como un mensaje de un conocido
- Máximo 150 palabras — se lee en 20 segundos
- 1-2 emojis máximo — solo si el tono lo pide
- Nunca sonar como spam masivo — siempre personalizado en la apertura
- Siempre con opt-out implícito: "Si prefieres no recibir más mensajes, avísame"
- No enviar más de 1x/semana al mismo contacto

### Templates de WhatsApp por situación

**Post-discovery call:**
```
Hola [nombre], fue un gusto hablar hoy.

Como quedamos, te comparto el link para 
abrir tu Cuenta Asesorada cuando estés listo:
[LINK-CA]

Si tienes alguna pregunta antes de decidir,
escríbeme aquí mismo. Sin presión.

— [Nombre]
```

**Alerta de mercado:**
```
Hola [nombre],

Esta semana la Fed anunció [X].
Para un inversor latinoamericano esto significa [Y].

Si tienes capital sin estrategia ahora mismo,
es buen momento para conversar.
[LINK-DISCOVERY]

— [Nombre], Folionet
```

**Reactivación lead frío:**
```
Hola [nombre], hace un tiempo hablamos 
sobre invertir en el mercado americano.

El contexto cambió bastante desde entonces.

¿Sigues evaluando opciones?
Te cuento las novedades en 10 minutos.
[LINK-DISCOVERY]

— [Nombre], Folionet
```

---

## CALENDARIO DE DISTRIBUCIÓN SEMANAL

| Día | Canal | Contenido |
|-----|-------|-----------|
| Lunes | — | Research de tendencias (folionet-trends-research) |
| Martes | LinkedIn CEO | Post principal de la semana |
| Miércoles | Email | Newsletter semanal |
| Jueves | LinkedIn CEO | Post secundario / complementario |
| Viernes | LinkedIn Company | Repurpose visual del post del martes |
| Sábado | WhatsApp | Solo si hay evento de mercado urgente |

---

## COMPLIANCE CHECKLIST
*Antes de publicar cualquier pieza, verificar:*

- [ ] Sin promesas de rendimiento específico ("ganarás X%")
- [ ] Sin referencias a rendimientos pasados como garantía de futuros
- [ ] Sin testimonios de clientes sin aprobación del CCO
- [ ] Escenarios hipotéticos claramente framed ("si hubieras invertido...")
- [ ] Footer regulatorio en todos los emails
- [ ] Afirmaciones comparativas con sustentación factual
- [ ] Contenido de Folionet Advisers LLC revisado por CCO antes de publicar

---

## PROMPT DE AUDITORÍA
*Antes de publicar cualquier pieza:*

```
Revisa este contenido para Folionet antes de publicarlo.

[PEGAR CONTENIDO]

Canal: [LinkedIn / Email / WhatsApp]

Evalúa:
1. ¿Pasa el compliance check de FINRA/SEC? 
   ¿Hay algo que necesite revisión del CCO?
2. ¿El hook para el scroll / abre el email en las primeras 2 líneas?
3. ¿Habla específicamente al ICP de Folionet 
   (profesional LATAM 35-54, capital medio-alto)?
4. ¿El CTA es apropiado para la etapa del funnel?
5. ¿El tono es sofisticado sin ser técnico?

Calificación 1-10 y máximo 3 cambios concretos si los necesita.
```

---

## PRE-PUBLISH AUDIT
*Run this before anything goes live — LinkedIn, email, WhatsApp, or landing pages. This is the final gate after the compliance note in the content prompt above.*

Copia y pega esto en Claude antes de publicar:

\`\`\`
Audita este contenido antes de publicar.

Revisa:
- Voz de marca: ¿suena a Folionet según /folionet-voice, o genérico?
- Riesgo de compliance: promesas de retorno específicas, performance 
  pasado presentado como garantía, testimonios sin aprobación de CCO, 
  falta el footer regulatorio
- Links rotos o faltantes: ¿el CTA tiene link? ¿es el correcto? 
  ¿quedó algún placeholder tipo [LINK-DISCOVERY] sin reemplazar?
- UTM tracking: ¿todos los links trackeables están tageados?
- Claims factuales: números, comparaciones o estadísticas que 
  necesitan fuente o aprobación de CCO
- Typos / formato: hashtags dentro del límite, día y canal 
  correctos, formato correcto en mobile

Para cada problema: nombra el post/archivo, el riesgo, y el fix.

Luego califica: LISTO / NECESITA AJUSTES / NO LISTO
\`\`\`

**Cuándo correrlo:** siempre, después de generar contenido con el prompt de arriba y antes de que un humano lo apruebe para publicar. Es el checklist de 30 segundos, no una cadena de aprobación corporativa.

---

---

## UPDATE LOG
- v0 — June 24 2026 — sistema completo LinkedIn + Email + WhatsApp. Links placeholder — actualizar con URLs reales de Folionet antes de activar.
- ## DIFERENCIACIÓN COMPETITIVA — TENER SIEMPRE PRESENTE

Investigación de competencia (Julio 2026) confirmó: el único competidor directo real es **Quiena Inversiones** (mismo modelo RIA, pero frío/automatizado). El resto (Hapi, Ualá, Trii) son brokers autogestionados — audiencia distinta, no compiten por el mismo servicio.

**El ángulo diferenciador central que todo contenido debe reforzar cuando sea relevante:**
> "Asesor humano y regulado — no un algoritmo frío (como Quiena) ni trading gamificado (como Hapi/Trii)."

**Reglas prácticas derivadas de esto:**
- Cuando el contenido hable de gestión de portafolio, mencionar o implicar que hay una persona real detrás — no un robo-advisor.
- Cuando sea relevante, nombrar el dolor específico del país (CCL en Argentina, impuestos por invertir afuera en Colombia, riesgo cambiario en Venezuela) en vez de generalizar a "LATAM."
- Nunca comparar a Folionet contra un competidor por nombre en contenido público — la diferenciación se comunica por posicionamiento propio, no atacando a otros.
