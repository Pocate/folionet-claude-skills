# Folionet — Brief del Sistema: Estado Actual, Pendientes, y Arquitectura
**Preparado por:** creator:you
**Fecha:** Julio 2026
**Propósito:** Punto de referencia único — qué existe, qué falta, dónde vive todo, y qué decisiones quedan abiertas.

---

## 1. DÓNDE VIVE EL SISTEMA

**Decisión ya tomada:** GitHub (`folionet-claude-skills`) + Claude Code — no un sitio web, no una app nueva.

```
folionet-claude-skills/
├── .claude/skills/          ← lo que Claude carga automáticamente
│   ├── folionet-icp
│   ├── folionet-voice
│   ├── folionet-content-system
│   ├── folionet-content-calendar
│   ├── folionet-trends-research
│   ├── folionet-strategy-exercises
│   ├── folionet-linkedin-30posts
│   ├── folionet-data
│   ├── folionet-pitch
│   ├── folionet-webinar
│   ├── folionet-events
│   ├── folionet-grader
│   ├── folionet-workflow-linkedin
│   ├── folionet-workflow-newsletter
│   └── folionet-workflow-whatsapp
└── deliverables/             ← documentos de referencia, 01 a 20
```

**Estado real de esto:** construido y empaquetado en 8 zips a lo largo de esta conversación. **Pendiente: que tú (o quien tenga acceso) los suba realmente al repo.** Nada de esto vive en GitHub todavía — vive en tus descargas.

---

## 2. QUÉ ESTÁ 100% CONSTRUIDO

- Sistema de contenido completo para 3 canales (LinkedIn, Email, WhatsApp) con templates, CTAs, compliance checklist
- 15 skills de Claude, cada uno con su propósito específico
- Serie completa de Cuenta Asesorada — las 6 semanas, carruseles + guiones de video
- Loop de trabajo independiente por canal (idea → voz → generar → calificar → compliance → publicar → feedback)
- Sistema de calificación de calidad (`folionet-grader`) separado del gate de compliance (siempre humano)
- Log de aprobaciones con proceso semanal por email definido
- Mapa de competencia LATAM con datos reales (5 competidores, 3 gaps confirmados)
- Typeform qualifier, mapa de integración, guías de autoservicio, calendario de Reels + alerta de dashboard
- Roadmap de 60 días + estructura de presentación final
- Plan de cierre de 7 días (dado el acortamiento del engagement)

---

## 3. QUÉ FALTA CONSTRUIR (todavía no existe)

| Falta | Por qué no se ha hecho | Quién lo desbloquea |
|---|---|---|
| Consolidar los 8 zips en el repo real | Nadie lo ha subido todavía | Tú |
| `approval-log.md` con datos reales (no ejemplos) | Necesita que empiece a correr el proceso semanal | Tú, esta semana |
| Ajustar los 3 workflows de canal con el Paso 4.5 (grader) | Es solo pegar el texto, no está hecho | Tú, 10 minutos |
| Addendum de diferenciación en `folionet-content-system` | Dijiste que lo harías tú directamente | Confirmar que ya se hizo |
| Validación de ICP con datos reales de plataforma | Depende del CSV | Producto/tech lead |
| Auditoría real de tickets de soporte | Depende del export | Líder de soporte |
| Conexión de Metricool | Acceso lo tiene el diseñador, canales sin confirmar | Diseñador/social media manager |
| Conector tipo Blotato para automatizar publicación real | Búsqueda de conectores quedó pendiente de tu opt-in | Tú (confirmar el prompt de conectores) |

---

## 4. QUÉ FALTA DEFINIR (decisiones, no construcción)

| Decisión | Estado |
|---|---|
| Substack vs. Mailchimp | Mailchimp ya está en uso — pendiente confirmación formal del presidente |
| LinkedIn: perfil personal vs. página de empresa como principal | Pendiente — reunión del lunes |
| Quién puede publicar sin aprobación (diseño autónomo vs. sign-off siempre) | Pendiente — misma reunión |
| Incentivo del programa de referidos (Opción A/B/C) | Pendiente — recomendado empezar con Opción A (sin costo) |
| Quién opera Claude Code día a día | Pendiente — ¿tú, el diseñador, alguien más? |
| Automatización Fase 2: API directa confirmada, pero sin fecha ni responsable técnico asignado | Pendiente |

---

## 5. CAMBIOS PENDIENTES EN LOS SKILLS EXISTENTES

Esto es trabajo de edición, no de construcción desde cero — todos son ajustes cortos:

1. **`folionet-content-system`** → pegar el addendum de diferenciación competitiva (Quiena/Hapi/Trii) al final del archivo. *(Dijiste que lo harías tú — confirmar.)*
2. **`folionet-workflow-linkedin`**, **`folionet-workflow-newsletter`**, **`folionet-workflow-whatsapp`** → insertar el Paso 4.5 (`folionet-grader`) entre Generar y Compliance en cada uno. Texto exacto ya está en el README del paquete del grader.
3. **`folionet-pitch`** → actualizar cuando el presidente confirme si $5,000 sigue siendo el mínimo real (marcado como pendiente de verificar desde que se creó).
4. **`folionet-data`** → sigue "vacío" de datos reales — se activa solo cuando entre el primer CSV o export de Metricool.
5. **`10-competencia-latam-marco.md`** → ya reemplazado por `16-competencia-latam-final.md`, borrar el archivo viejo del repo cuando subas.
6. **`folionet-workflow`** (el combinado original) → eliminar del repo, reemplazado por los 3 independientes.

---

## 6. LO QUE NO CAMBIA — LA REGLA DE ORO

Sin importar cuánto se automatice después (API directa, conector tipo Blotato, lo que sea): el gate de compliance (`folionet-content-system` → Compliance Checklist) siempre lo aprueba un humano. Ningún cambio de infraestructura futuro debe tocar esa regla.

---

## 7. PRÓXIMO PASO INMEDIATO (hoy, no esta semana)

De todo lo de arriba, esto es lo único verdaderamente bloqueante para que el sistema exista de verdad y no solo en zips:

**Subir los 8 zips al repo de GitHub.** Todo lo demás — decisiones del presidente, datos de producto, conectores — puede esperar. Esto no.

## UPDATE LOG
- v1 — Julio 2026 — primer brief consolidado del sistema completo.
