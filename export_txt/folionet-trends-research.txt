# folionet-trends-research
**Version:** v0 — Weekly market trends research system for Folionet content.
**Purpose:** Find what LATAM investors are talking about right now → convert trends into LinkedIn content angles.
**Cadence:** Run every Monday morning. Takes 30-45 min. Feeds the week's content.

---

## THE SYSTEM IN ONE LINE
Monitor 5 sources → extract 3 trends → convert each trend into a content angle → pick 1 for the week's posts.

---

## STEP 1 — THE 5 SOURCES TO CHECK EVERY MONDAY

### Source 1 — Bloomberg Línea (10 min)
What to look for: Top 3 financial news stories in Spanish this week.
Focus: anything about LATAM economies, US market performance, dollar/currency news, investing behavior.
URL: bloomberglinea.com

### Source 2 — LinkedIn Search (10 min)
Search these terms, filter by "Top" posts from the last 7 days:
- "inversiones latinoamérica"
- "bolsa de valores"
- "dólar ahorro"
- "mercado americano"

What to look for: what's getting the most engagement, what questions people are asking in comments.

### Source 3 — Google Trends en español (5 min)
Check trending searches in: Venezuela, Colombia, Argentina, México, España
Terms to track weekly:
- "invertir en bolsa"
- "cuenta de inversión"
- "dólar inversión"
- "cómo proteger mis ahorros"

### Source 4 — Reddit & Foros LATAM (5 min)
Communities to check:
- r/finanzaspersonales
- r/argentina (flair: economía)
- r/vzla (flair: economía)
- r/Colombia (finanzas)

What to look for: questions people are asking about investing, fears, misconceptions.

### Source 5 — Competidor Hapi.trade (5 min)
Check their LinkedIn + Instagram.
What are they posting this week?
What's getting engagement?
Is there an angle they're NOT covering that Folionet could own?

---

## STEP 2 — THE WEEKLY RESEARCH PROMPT

Run this in Claude every Monday after checking the 5 sources:

```
Soy el equipo de contenido de Folionet — plataforma de inversión 
regulada por FINRA/SEC para inversores latinoamericanos. Foco 
actual: LinkedIn del CEO + email newsletter semanal.

Aquí están las noticias/tendencias que encontré esta semana:

[PEGAR: top 3 noticias de Bloomberg Línea]
[PEGAR: posts de LinkedIn con más engagement esta semana]
[PEGAR: términos trending en Google esta semana]
[PEGAR: preguntas frecuentes en foros LATAM esta semana]
[PEGAR: qué está posteando Hapi.trade]

Con base en esto:

1. Dame los 3 temas más relevantes para el ICP de Folionet 
   esta semana (profesional LATAM 35-54, capital $20K-$500K, 
   quiere invertir en EE.UU. sin convertirse en trader)

2. Para cada tema, dame:
   — Un hook de apertura para LinkedIn (máximo 2 líneas)
   — El ángulo: ¿es mito? ¿dato? ¿educación? ¿historia CEO?
   — Si hay urgencia real esta semana (evento de mercado, 
     noticia relevante) o es contenido evergreen

3. Recomienda cuál de los 3 usar esta semana y por qué.

Compliance: sin promesas de rendimiento, sin testimoniales.
Voz: Morgan Housel — sofisticado, datos, sin hype.
```

---

## STEP 3 — CONVERT TREND TO CONTENT ANGLE

Once you pick the weekly trend, run this:

```
Referencia /folionet-voice y /folionet-icp.

El tema de esta semana es: [TEMA/TENDENCIA]

Conviértelo en:

1. Un post de LinkedIn para el CEO (150-300 palabras)
   — Hook que conecte con el evento/tendencia actual
   — Idea central relevante para el ICP
   — CTA apropiado para la etapa del funnel

2. Un email para la lista de 63K suscriptores
   — Asunto (máximo 6 palabras)
   — Preview (no repite el asunto)
   — Cuerpo: 3 párrafos cortos
   — CTA: discovery call o link a recurso

Compliance: sin promesas de rendimiento.
Formato LinkedIn: líneas cortas, max 3 hashtags.
```

---

## TREND TRACKING LOG
*Actualizar cada semana. Máximo 8 semanas de historia.*

| Semana | Trend principal | Ángulo usado | Engagement |
|--------|----------------|--------------|------------|
| Jun 24 | — | — | — |
| — | — | — | — |

---

## SEÑALES DE ALTA OPORTUNIDAD
*Cuando ocurre uno de estos eventos, publicar dentro de 24-48 horas:*

- Fed anuncia cambio en tasas de interés → ángulo: qué significa para el inversor LATAM
- Devaluación o crisis cambiaria en Venezuela/Argentina/Colombia → ángulo: protección en dólares
- S&P 500 baja más del 5% → ángulo: el mito del "momento correcto"
- S&P 500 cierra año positivo → ángulo: dato histórico de rendimiento
- Competidor (Hapi) lanza campaña nueva → ángulo: la diferencia entre un broker y un asesor

---

## UPDATE LOG
- v0 — June 24 2026 — research system built. No tracking data yet.
- v1 — [update after 4 weeks of data to refine which sources produce better angles]
