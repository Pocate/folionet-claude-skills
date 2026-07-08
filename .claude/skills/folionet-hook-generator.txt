---
name: folionet-hook-generator
description: >
  Genera 6 variaciones de hook (dos líneas) para un tema, adaptadas a los 7 ángulos de contenido de Folionet y filtradas por compliance. Usar cuando se pida "hooks para este tema", "openers para el post", "ideas de gancho", o cuando se pegue un tema y se pida cómo abrirlo. Salida rápida, sin preámbulo.
---

# Folionet Hook Generator
**Basado en:** hook-generator (Charlie Hills), adaptado a `folionet-voice` y `folionet-content-system`.

## CRÍTICO: Auto-inicio
Al activarse, ir directo al Paso 1. No resumir ni explicar la metodología antes de generar.

## Paso 1 — Obtener el tema
Si el usuario ya pegó un tema, úsalo. Si no, pregunta:
> ¿Sobre qué tema necesitas hooks?

## Paso 2 — Escribir 6 variaciones

Formato de cada hook:
- **Línea 1 (Apertura):** máximo 40 caracteres. Sin preguntas. Afirmación específica o inesperada.
- **Línea 2 (Contraste):** máximo 40 caracteres. Reencuadra o contradice la línea 1.

Los 6 ángulos — **estos reemplazan los del skill original**, que no pasan compliance (ver reglas abajo):

1. **Dato con fuente** — un número real, citable, sin implicar rendimiento futuro. Ej: "50 países ya tienen acceso." / "Cero en EE.UU. saben esto."
2. **Reencuadre de mito** — declara la creencia común, luego la desmiente. Formato "No es X. Es Y." (patrón ya validado en folionet-voice).
3. **Historia CEO** — experiencia personal/profesional, sin prometer resultados replicables para el lector.
4. **Autoridad regulatoria** — referencia a FINRA/SEC/respaldo legal como señal de confianza, nunca como garantía de resultado.
5. **Brecha de conocimiento** — "lo que nadie te explicó" — educativo, nunca marco de "lo que perdiste por no invertir".
6. **Costo del status quo** — el costo de no actuar (inflación, capital ocioso), siempre framed como riesgo real, nunca como pérdida garantizada si no actúan ahora (eso es urgencia manipuladora, prohibido en folionet-voice).

## Paso 3 — Formato de salida

```
HOOKS para [tema]

1. [Dato con fuente]
[Línea 1]
[Línea 2]

2. [Reencuadre de mito]
[Línea 1]
[Línea 2]

3. [Historia CEO]
[Línea 1]
[Línea 2]

4. [Autoridad regulatoria]
[Línea 1]
[Línea 2]

5. [Brecha de conocimiento]
[Línea 1]
[Línea 2]

6. [Costo del status quo]
[Línea 1]
[Línea 2]
```

## Paso 4 — Siguiente paso
Preguntar:
> ¿Quieres que convierta alguno de estos en un post completo? Dime el número y lo mando al prompt de folionet-content-system.

## REGLAS DE COMPLIANCE (no negociables — filtran cada hook antes de mostrarlo)

- ❌ Nunca un hook con cifra de rendimiento o retorno específico ("gana X%", "duplica tu dinero").
- ❌ Nunca framing de urgencia manipuladora ("si no inviertes ahora, pierdes para siempre").
- ❌ Nunca "confesión de pérdida personal" como ángulo (el skill original lo incluye — eliminado aquí porque puede leerse como advertencia de riesgo real de inversión, no como storytelling).
- ❌ Nunca predicción de mercado presentada como certeza ("el mercado va a subir/caer").
- ✅ Todo dato numérico debe ser verificable y, si se usa en el post final, necesita fuente citada (ver regla de folionet-voice sobre claims factuales).
- ✅ Palabras prohibidas de folionet-voice aplican también aquí: nada de "fácil", "rápido", "millonario", "gratis" (salvo que sea literal), "revolucionario", "empoderar".

## Reglas de formato
- Máximo 40 caracteres por línea — contarlos.
- Sin preguntas en la línea de apertura.
- Sin emojis.
- Preferir dígitos sobre números escritos (3, no "tres").
- Español, tono sofisticado y directo — nunca casual/meme.

---
*Adaptado del skill open-source hook-generator (charlie947/social-media-skills) — julio 2026.*
