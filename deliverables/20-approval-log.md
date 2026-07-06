# Folionet — Log de Aprobaciones
**Propósito:** Registro trazable de qué contenido se aprobó, cuándo, por quién y por qué canal — para tener evidencia disponible si algún día se necesita (auditoría interna, revisión de FINRA/SEC, o simplemente para saber qué se dijo que sí y cuándo).
**Regla:** Cada pieza de contenido publicada debe tener una fila aquí ANTES de publicarse, no después.

---

## CÓMO SE LLENA

Una fila por pieza de contenido (o una fila por "lote semanal" si se aprobó todo junto por email). Nunca borrar filas — si algo se rechazó, se deja constancia también.

| Fecha | Pieza de contenido | Canal | Nota del grader | Aprobado por | Canal de aprobación | Resultado |
|---|---|---|---|---|---|---|
| *(ejemplo)* 2026-07-10 | Post LinkedIn — "Mito: necesitas ciudadanía americana" | LinkedIn | 8.5/10 | [Nombre presidente] | Email (lote semanal) | ✅ Aprobado |
| *(ejemplo)* 2026-07-10 | Newsletter — "Qué significa el anuncio de la Fed" | Email | 7/10 → 9/10 tras ajuste | [Nombre presidente] | Email (lote semanal) | ✅ Aprobado con ajuste de hook |
| *(ejemplo)* 2026-07-12 | CA Semana 5 — Objeciones | LinkedIn | 9/10 | [Nombre presidente] | Loom async | ✅ Aprobado |

*(Borrar las filas de ejemplo cuando empiece el uso real — se dejan aquí solo como referencia de formato.)*

---

## NIVELES DE APROBACIÓN — QUÉ CANAL USAR

| Tipo de contenido | Canal de aprobación | Frecuencia |
|---|---|---|
| Posts rutinarios de LinkedIn/newsletter | Email, lote semanal (viernes → aprobación antes del lunes) | Semanal |
| WhatsApp (post-llamada, alertas, reactivación) | Aprobación puntual del template general una sola vez — no cada mensaje individual, ya que son plantillas pre-aprobadas de `folionet-content-system` | Una vez por plantilla, no por envío |
| Serie CA Semanas 5-6, one-pager, email de migración, testimonios | Reunión corta o Loom async, respuesta explícita | Por pieza, alto riesgo |

---

## EL PROCESO SEMANAL (rutinario)

1. **Viernes:** se manda el correo de lote con todo el contenido de la semana siguiente — ya pasado por `folionet-grader` (nota incluida) y por el compliance checklist de `folionet-content-system`.
2. **Antes del lunes:** el presidente responde "Aprobado" o con ajustes puntuales por el mismo hilo de correo.
3. **Al aprobarse:** se agrega la fila correspondiente a este log — fecha, pieza, canal, nota del grader, quién aprobó, resultado.
4. **Si se rechaza o pide ajuste:** se registra igual, con la nota de qué cambió y se vuelve a mandar si aplica.

---

## PLANTILLA DEL CORREO DE LOTE SEMANAL

```
Asunto: Contenido para aprobar — semana del [fecha]

Hola [nombre],

Aquí está el contenido programado para la próxima semana, ya revisado:

1. [Canal] — [Título/tema] — Nota del grader: [X/10]
[contenido completo o link]

2. [Canal] — [Título/tema] — Nota del grader: [X/10]
[contenido completo o link]

¿Todo aprobado, o hay algo que ajustar antes del lunes?

Gracias,
[Tu nombre]
```

## UPDATE LOG
- v0 — Julio 2026 — plantilla inicial del log de aprobaciones + proceso de lote semanal por email.
