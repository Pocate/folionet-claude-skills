# Folionet — Alerta de Dashboard + Calendario de Reels
**Preparado por:** creator:you
**Fecha:** Julio 2026
**Basado en:** folionet-data, folionet-content-calendar
**Estado:** Marco de alerta listo (activar en cuanto exista el Google Sheet en vivo). Calendario de Reels listo para producción del equipo de diseño.

---

## PARTE 1 — ALERTA DE DASHBOARD

### Qué dispara la alerta
Registros mensuales caen por debajo del umbral esperado (a definir una vez exista el baseline real del CSV de plataforma — mientras tanto, usar el mes anterior como referencia).

### Umbral sugerido (ajustar con datos reales)
- **Amarillo:** Registros del mes 15% por debajo del mes anterior
- **Rojo:** Registros del mes 30%+ por debajo del mes anterior, o 2 meses consecutivos en amarillo

### Quién la recibe
El CEO y quien maneje marketing (tú) — no necesita ir a todo el equipo.

### Protocolo de respuesta
1. **Amarillo:** Revisar qué canal cayó específicamente (LinkedIn, newsletter, referidos) en la próxima sesión semanal de `folionet-data`. No es necesariamente una crisis — puede ser estacionalidad.
2. **Rojo:** Reunión ad-hoc de 15 min con el CEO — decisión rápida: ¿ajustar contenido, acelerar algo ya planeado (webinar, evento), o es un problema de producto/activación y no de marketing?

### Cómo implementarlo (técnicamente)
Una vez el Google Sheet de KPIs esté en vivo, esto se puede hacer con una fórmula simple + Google Apps Script que mande un email automático cuando el número cruce el umbral. No requiere herramienta nueva — corre sobre lo que ya se está construyendo.

---

## PARTE 2 — CALENDARIO DE REELS (4 semanas)

Usa los mismos 4 pilares ya definidos en `07-linkedin-pillars-audit.md`, adaptados a formato vertical corto (15-30 seg). El equipo de diseño ejecuta sin necesitar que el CEO inicie cada uno.

| Semana | Pilar | Idea de Reel | Formato |
|---|---|---|---|
| 1 | Categoría (CA) | "3 cosas que no sabías que existían: Cuentas Asesoradas en EE.UU." | Texto en pantalla + voz en off o CEO hablando a cámara |
| 1 | Data Breakdown | Un dato de mercado + reacción rápida a cámara | CEO a cámara, 15-20 seg |
| 2 | Mitos | "Mito: necesitas ser ciudadano americano" — formato mito/realidad | Texto grande, transición rápida |
| 2 | Autoridad del Fundador | Behind-the-scenes: "un día en Folionet" o clip de una conversación real (anonimizada) | Estilo casual, no producido |
| 3 | Categoría (CA) | Repurpose del carrusel de la Semana 1 de la serie CA en versión Reel | Slides animadas del carrusel existente |
| 3 | Data Breakdown | Comparación visual rápida (inflación LATAM vs. mercado americano) | Gráfico simple animado |
| 4 | Mitos | "Mito: las inversiones son solo para ricos" | Mismo formato mito/realidad |
| 4 | Autoridad del Fundador | Clip corto de una respuesta a una pregunta frecuente | CEO a cámara respondiendo directo |

### Reglas de producción (para que el equipo no necesite preguntar)
- Máximo 30 segundos por Reel
- Subtítulos siempre (la mayoría ve sin sonido)
- Sin música con copyright — usar librería de audio de la plataforma
- Mismo chequeo de compliance que cualquier otro contenido: sin promesas de rendimiento, footer regulatorio en la descripción

---

## SIGUIENTE PASO
El calendario de Reels puede pasar a producción de inmediato — no depende de ningún dato pendiente. La alerta de dashboard queda lista para activarse en cuanto el Google Sheet en vivo (`folionet-data`) tenga al menos 2-3 meses de datos reales para calcular el umbral con precisión.

## UPDATE LOG
- v0 — Julio 2026 — calendario listo para producción. Umbral de alerta es una estimación inicial, ajustar con datos reales del CSV de plataforma.
