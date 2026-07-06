# Folionet — Mapa de Integración (Soporte, Producto, Marketing)
**Preparado por:** creator:you
**Fecha:** Julio 2026
**Basado en:** Parte 03 del plan de 30 días (Infraestructura de Datos)
**Estado:** Borrador — mapea dónde vive la información hoy y da 3 opciones. Producto decide cuál implementar.

---

## DÓNDE VIVE LA INFORMACIÓN HOY

| Fuente | Vive en | Estado |
|---|---|---|
| Registro de usuarios (país, fuente) | Plataforma/base de datos del producto | Existe, no exportado regularmente |
| Primera operación completada | Plataforma/base de datos del producto | Existe, no cruzado con registro |
| Tickets de soporte | Herramienta de soporte (CRM/helpdesk) | Existe, sin analizar ni taggear |
| HowDidYouFindUs | Campo del producto | Existe pero no se está capturando activamente |
| Suscriptores de newsletter | Mailchimp | Existe, exportable como CSV |
| Métricas de LinkedIn/Instagram | Metricool (parcial) | Configurado, sin reportes automáticos aún |
| Referidos | No existe campo dedicado | Falta instrumentar |

**El problema no es falta de datos — es que viven en 5+ lugares distintos y nadie los cruza.**

---

## LAS 3 OPCIONES

### Opción 1 — Ligera (sincronización manual semanal)
**Cómo funciona:** Cada lunes, alguien de producto exporta un CSV de la plataforma; marketing exporta Metricool y Mailchimp; todo se pega manualmente en el Google Sheet de KPIs (`folionet-data`).
**Costo:** $0 en herramientas.
**Esfuerzo:** ~20-30 min/semana de una persona.
**Riesgo:** Depende de que alguien lo haga cada semana sin falta — se rompe con vacaciones o carga de trabajo.
**Recomendado si:** El equipo es muy pequeño (como ahora) y no hay urgencia de datos en tiempo real.

### Opción 2 — Media (Zapier)
**Cómo funciona:** Zaps automáticos que mueven datos entre plataforma → Google Sheet, Mailchimp → Google Sheet, Metricool → Google Sheet, sin intervención manual.
**Costo:** ~$20-50/mes dependiendo del volumen de zaps.
**Esfuerzo:** Configuración inicial de 1 persona técnica, ~1 semana. Después, mantenimiento mínimo.
**Riesgo:** Zapier se puede romper si una plataforma cambia su API — necesita revisión ocasional.
**Recomendado si:** El equipo quiere automatizar sin construir infraestructura propia, y tiene alguien que pueda configurar Zapier una vez.

### Opción 3 — Completa (integración API directa)
**Cómo funciona:** Conexiones API directas entre la plataforma, el CRM de soporte, y el dashboard de marketing — datos en tiempo real, sin exports manuales ni Zapier.
**Costo:** Desarrollo interno (tiempo de un desarrollador) + posible costo de infraestructura.
**Esfuerzo:** Semanas de trabajo de producto/tech, no algo que se resuelve en Semana 4.
**Riesgo:** Requiere mantenimiento continuo de código propio.
**Recomendado si:** Folionet ya tiene o va a tener un equipo técnico dedicado, y el volumen de datos/decisiones justifica la inversión.

---

## LA DECISIÓN — QUÉ PUEDEN REALMENTE MANTENER

La pregunta correcta no es "¿cuál es la mejor opción?" — las tres funcionan. Es: **¿cuál puede mantenerse funcionando sin depender de una sola persona que se puede ir o enfermar?**

Con el equipo actual (1 persona en marketing, sin equipo técnico dedicado mencionado), la recomendación es:
- **Empezar con Opción 1** (ya está funcionando vía `folionet-data`)
- **Evaluar Opción 2** una vez que Metricool y el CSV de plataforma sean rutina — es el salto natural cuando la sincronización manual empiece a sentirse pesada
- **Opción 3 solo si** Folionet contrata un desarrollador dedicado a esto específicamente

---

## HANDOFF A PRODUCTO
Este documento se entrega, no se implementa por marketing (fuera de nuestro carril, según el plan). Producto decide cuál opción implementar y cuándo.

## UPDATE LOG
- v0 — Julio 2026 — mapa inicial basado en el plan de 30 días. Actualizar con costos reales una vez producto evalúe herramientas específicas.
