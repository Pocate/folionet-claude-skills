---
name: folionet-cta
description: >
  Genera el CTA correcto para un post o email de Folionet según etapa del funnel (awareness / consideración / conversión) y canal (LinkedIn / Email / WhatsApp). El CTA cierra lo que el hook abrió. Usar cuando se pida "¿con qué CTA cierro esto?", "dame el cierre del post", o al final de cualquier pieza de contenido. Salida directa, sin preámbulo.
---

# Folionet — CTA Generator
**Regla central:** el CTA corresponde siempre a la etapa del funnel del post — no al canal. Un post de awareness en LinkedIn no puede cerrar con "agenda una llamada"; un email de conversión no puede cerrar con "¿qué opinas?".

---

## PASO 1 — DETERMINAR ETAPA DE FUNNEL

Si no se especifica, inferir del contenido:

| Señal en el contenido | Etapa |
|----------------------|-------|
| Educativo, dato, mito, concepto nuevo | Awareness |
| Comparación, caso hipotético, "cómo funciona" | Consideración |
| "¿Es para mí?", objeción, proceso de apertura | Conversión |

---

## PASO 2 — SELECCIONAR CTA

### Awareness (top funnel)
Objetivo: generar conversación, no acción transaccional.
```
— "¿Qué tema de inversión quieres que cubra la próxima semana?"
— "¿Esto es algo que nadie te había explicado antes? Comenta."
— "Sígueme para más contenido sobre inversiones para latinoamericanos."
— "¿Cuál de estos puntos te sorprendió más?"
```

### Consideración (mid funnel)
Objetivo: mover a un recurso o profundizar la relación.
```
— "¿Tienes preguntas? Las respondo en los comentarios."
— "¿En qué etapa estás tú? Cuéntame en los comentarios."
— "Guarda este post — es la pregunta que más me hacen."
— "¿Conoces a alguien en esta situación? Compártelo."
— "Suscríbete al newsletter — cada semana un tema así. [LINK-NEWSLETTER]"
```

### Conversión (bottom funnel)
Objetivo: discovery call o apertura de cuenta.
```
— "¿Tienes capital que no está trabajando como debería? Conversemos. [LINK-DISCOVERY]"
— "¿Quieres saber si una Cuenta Asesorada es para ti? Una llamada de 20 minutos lo responde. [LINK-DISCOVERY]"
— "Agenda una llamada sin costo con nuestro equipo. [LINK-DISCOVERY]"
— "Da el primer paso. [LINK-SIGNUP]"
```

### CTAs para Email (siempre más directos que LinkedIn)
```
— "Si tienes capital que no está trabajando como debería, agenda una llamada aquí → [LINK-DISCOVERY]"
— "¿Quieres saber si una Cuenta Asesorada tiene sentido para tu situación? Hablemos → [LINK-DISCOVERY]"
— "Da el primer paso → [LINK-SIGNUP]"
```

---

## REGLAS (no negociables)

- Nunca dos CTAs en el mismo post — uno solo, al final.
- Nunca el mismo CTA dos posts seguidos — rotar.
- LinkedIn: el CTA es una línea. Nunca un párrafo.
- Email: el CTA va después del último párrafo, con flecha → o en negrita.
- Compliance: ningún CTA puede implicar rendimiento ("invierte y gana"), urgencia artificial ("solo por esta semana"), o garantía de resultado.
- `[LINK-DISCOVERY]`, `[LINK-NEWSLETTER]`, `[LINK-SIGNUP]` son placeholders — reemplazar con los links reales de Folionet antes de publicar.

---

## FORMATO DE SALIDA

```
CTA recomendado ([etapa] · [canal]):
"[texto del CTA]"

Alternativa si se usó recientemente:
"[texto alternativo]"
```

---

## PROMPT DE USO

```
Referencia /folionet-cta.

Post/email: [pegar contenido]
Canal: [LinkedIn / Email / WhatsApp]
Etapa del funnel: [awareness / consideración / conversión — o inferir]

Dame el CTA correcto para cerrar esta pieza.
```
