# folionet-grader
**Versión:** v0 — inspirado en el patrón "post-grader" de sistemas de marketing con IA, adaptado a Folionet. Califica calidad (voz, hook, formato) — **nunca** reemplaza el chequeo de compliance, que sigue siendo 100% humano.

## Qué hace
Se ejecuta DESPUÉS de generar un borrador (`folionet-content-system`) y ANTES de mandarlo a aprobación humana. Pule lo que se puede pulir con IA — hook, tono, formato — para que el humano que aprueba no pierda tiempo en correcciones de estilo y se enfoque solo en lo que realmente le corresponde: compliance y criterio de negocio.

**Regla que nunca cambia:** este skill califica calidad, no compliance. El chequeo de FINRA/SEC (`folionet-content-system` → Compliance Checklist) es un gate separado, obligatorio, y siempre humano — pasar por `folionet-grader` con nota alta NO significa que el contenido está listo para publicar. Todavía falta el gate de compliance.

---

## CÓMO CALIFICA (escala 1-10, igual que el patrón de referencia)

### Criterios de evaluación

| Criterio | Peso | Qué evalúa |
|---|---|---|
| **Hook** | 30% | ¿Las primeras 1-2 líneas paran el scroll / abren el email? ¿O es genérico? |
| **Voz** | 25% | ¿Suena a `folionet-voice`? ¿Sofisticado sin ser técnico, directo sin ser agresivo? |
| **Alineación al pilar/ICP** | 20% | ¿Le habla claramente a uno de los 3 perfiles? ¿Está en el pilar correcto? |
| **Formato** | 15% | ¿Respeta las reglas del canal — longitud, hashtags, estructura de párrafos? |
| **CTA** | 10% | ¿El CTA corresponde a la etapa de funnel correcta (awareness/consideración/conversión)? |

**Nota:** ningún criterio de compliance está en esta tabla a propósito — eso vive en un gate aparte, nunca se mezcla con la nota de calidad.

---

## FORMATO DE SALIDA

```
NOTA: X.X/10

Hook: [comentario corto]
Voz: [comentario corto]
Alineación: [comentario corto]
Formato: [comentario corto]
CTA: [comentario corto]

TOP 3 AJUSTES (si la nota es menor a 8):
1. [ajuste concreto]
2. [ajuste concreto]
3. [ajuste concreto]

⚠️ RECORDATORIO: Esta nota es de calidad, no de compliance.
Este contenido TODAVÍA necesita pasar el chequeo de compliance
de folionet-content-system y la aprobación humana antes de publicarse.
```

---

## CÓMO USARLO — EL PROMPT

```
Referencia /folionet-grader.

Califica este borrador:
[PEGAR CONTENIDO]

Canal: [LinkedIn / Email / WhatsApp]
Pilar: [Categoría / Mitos / Data Breakdown / Autoridad del Fundador]
```

Si la nota es menor a 8, aplicar los 3 ajustes y volver a calificar antes de mandar a compliance — así como en el ejemplo de referencia (6.3 → ajustes → nota final más alta).

---

## DÓNDE VIVE EN EL LOOP COMPLETO

Se inserta entre el Paso 4 y el Paso 5 de cada workflow de canal (`folionet-workflow-linkedin`, `folionet-workflow-newsletter`, `folionet-workflow-whatsapp`):

```
... → 4. GENERAR → 4.5 CALIFICAR (folionet-grader) → 5. COMPLIANCE (humano) → 6. PUBLICAR → ...
```

No reemplaza ningún paso existente — se agrega como un filtro de calidad antes del gate humano, para que ese gate sea más rápido y se enfoque en lo que de verdad importa: compliance y criterio de negocio, no gramática o un hook débil.

## POR QUÉ NO CALIFICA COMPLIANCE (decisión de diseño, no limitación técnica)
Aunque técnicamente se podría pedirle a un modelo que revise reglas de FINRA/SEC, mezclar eso con una "nota de calidad" numérica crea el riesgo de que una nota alta se lea como "aprobado para publicar." Mantener los dos gates completamente separados evita esa confusión — la calidad se mide con una nota, el compliance se aprueba o no se aprueba, sin escala de grises.

## UPDATE LOG
- v0 — Julio 2026 — primer skill de calificación de calidad, compliance permanece separado y humano.
