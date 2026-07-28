---
name: folionet-channel-strategy
description: >
  Decisiones de canal para Folionet: qué operar bien (LinkedIn + Email), qué automatizar (Instagram + WhatsApp Mes 2+), qué pausar (X, Facebook, YouTube). Carga cuando se pregunte sobre prioridades de canal, WhatsApp, Instagram, o cuándo/cómo expandir a nuevos canales. Incluye tabla semanal de operación para un equipo de una persona.
---

# Folionet — Channel Strategy
**Versión:** v1 — Junio 2026. Actualizar cuando Metricool tenga 4+ semanas de datos reales.
**Constraint:** Un miembro de equipo interno (diseñador gráfico). Toda recomendación de canal debe ser ejecutable por una persona con soporte de IA.

---

## DECISIÓN DE CANALES

### ✅ OPERAR BIEN — Atención completa, contenido original

**LinkedIn (perfil personal del CEO)**
- ICP: Directors, VPs, Founders, emprendedores profesionales 35-54
- Contenido: 2x/semana (martes + jueves). Posts educativos, data breakdowns, perspectiva del CEO, definición de categoría CA.
- Operación: CEO aprueba. IA (Claude + `folionet-content-system`) genera borradores. Un paso de revisión. Publicar.
- Output esperado: 10-15 nuevos seguidores calificados/semana → suscriptores newsletter → discovery calls.

**Email (Mailchimp — lista existente de 63K)**
- Por qué: 63,000 contactos propios es el activo más valioso de Folionet. Sin algoritmo. Sin riesgo de plataforma.
- Contenido: 1x/semana (miércoles). Newsletter educativo. Un tema, un CTA, un link. Máximo 300 palabras.
- Operación: IA genera desde research semanal. Diseñador formatea. Una aprobación. Enviar.
- Output esperado: 2-3% click rate semanal → tráfico consistente a discovery call.

---

### ⚙️ AUTOMATIZAR — Template y repurpose, mínimo esfuerzo nuevo

**Instagram**
- Uso: refuerzo de identidad visual, no educación.
- Contenido: Repurpose de posts LinkedIn como carruseles (1x/semana) + data visuals (1x/semana). Diseñador ejecuta.
- Lo que NO hacer: no intentar drive discovery calls desde Instagram. Drive suscripciones al newsletter.

**WhatsApp — Añadir en Mes 2 (con infraestructura correcta)**
- Casos de uso válidos: (1) follow-up post-discovery call con one-pager CA, (2) alertas de mercado para clientes existentes, (3) reactivación de leads tibios que dieron opt-in.
- Lo que NO es: prospecting, outreach frío, broadcasts a listas no calificadas.
- Requisitos antes de activar: WhatsApp Business API (Twilio o similar), templates pre-aprobados por CCO, mecanismo de opt-in (Typeform qualifier), archivado de comunicaciones (FINRA).
- Timeline: proponer templates al CCO en Semana 3. Activar en Mes 2.

---

### ⏸️ PAUSAR — No está mal, simplemente no es ahora

| Canal | Razón de pausa | Cuándo revisitar |
|-------|---------------|-----------------|
| X (Twitter) | Alcance orgánico financiero en español casi nulo sin pago | Crisis de mercado real — responder puntualmente |
| Facebook | ICP lo usa personalmente, no para investigación financiera | Si existe presupuesto para paid ads (Mes 3+) |
| YouTube | Requiere producción (script, grabación, edición) que el equipo no tiene | Mes 3-4 cuando el podcast esté activo y se pueda repurpose |

---

## RESUMEN EJECUTIVO DE CANALES

| Canal | Decisión | Frecuencia | Tipo de contenido | Quién |
|-------|----------|------------|-------------------|-------|
| LinkedIn (CEO) | ✅ Operar | 2x/semana | Posts originales | CEO + IA |
| Email | ✅ Operar | 1x/semana | Newsletter | IA + diseñador |
| Instagram | ⚙️ Automatizar | 2x/semana | Carruseles repurposed | Diseñador |
| WhatsApp | ⚙️ Añadir (Mes 2) | Por evento | Mensajes templados | CEO |
| YouTube | ⏸️ Pausar | — | — | Mes 3-4 |
| X (Twitter) | ⏸️ Pausar | — | — | Solo crisis |
| Facebook | ⏸️ Pausar | — | — | Solo paid |

---

## LO QUE EL EQUIPO HACE CADA SEMANA (~2h activas)

| Día | Tarea | Tiempo | Herramienta |
|-----|-------|--------|-------------|
| Lunes | Research de tendencias (5 fuentes) | 45 min | Claude + `folionet-trends-research` |
| Martes | Aprobar + publicar post LinkedIn | 15 min | LinkedIn / Metricool |
| Miércoles | Aprobar + enviar email | 15 min | Mailchimp |
| Jueves | Aprobar + publicar post LinkedIn | 15 min | LinkedIn / Metricool |
| Viernes | Diseñador publica carrusel Instagram | 30 min | Canva + Instagram |

**Total: ~2 horas/semana de tiempo activo del equipo.** El resto lo genera la IA y lo ejecuta el diseñador.

---

## LINKS A ACTUALIZAR (placeholders)
- Discovery call: `[LINK-DISCOVERY]`
- Newsletter signup: `[LINK-NEWSLETTER]`
- Cuenta Asesorada página: `[LINK-CA]`
- App download: `[LINK-APP]`

*Actualizar en `folionet-content-system` cuando el equipo confirme los links reales.*
