---
tipo: revisión
fecha: 2026-09-08
proyecto: Gestión de la Docencia (GD)
fuentes: Confluence espacio GD (30 páginas) · Jira proyecto GD (16 epics)
tags: [producto, gestion-docencia, revision]
---
# Revisión del proyecto Gestión de la Docencia

> Hecha sobre las **30 páginas del espacio `GD` de Confluence** y los **16 epics del proyecto `GD`
> de Jira**, el 8 de septiembre de 2026.

## 🔴 El hallazgo principal

**El proyecto tiene más documentación que ejecución.** En marzo de 2026 se hicieron cinco
sesiones de requisitos con RRHH y Profesorado, se validaron prototipos y se escribieron PRDs
completos —con objetivos, métricas de éxito, historias de usuario y tabla de hitos—. De esos
módulos, **solo Investigadores llegó a Jira**. Los otros se quedaron en el documento.

| Módulo | Documentación en Confluence | Trabajo en Jira |
|---|---|---|
| Propuesta docente (MVP) | ✅ Requisitos MVP, secuencia de acciones, modelo BBDD | ✅ `GD-11` cerrada · en producción |
| **Investigadores** | ✅ PRD + prototipos (jun 2026) | ✅ 6 epics · 21 historias · **en desarrollo** |
| **Bajas y sustituciones** | ✅ PRD "Automatización de Bajas Temporales y permanentes + ARC" | 🔨 `GD-596` · revisión el jueves 10 |
| **Volcado a Laurea** | ✅ "VOLCADO DE DATOS - SERVICIO LAUREA" | 🔨 `GD-657` + `GD-656` + 15 tareas *(creadas el 7/09)* |
| **Reducciones horarias** | ✅ PRD (feb 2026) + validación de prototipos | ⚠️ `GD-539` abierta desde **mayo, sin movimiento** |
| **Ámbitos de conocimiento** | ✅ PRD completo con métricas e hitos | 🔴 **Sin epic. Sin historias.** Solo 3 issues cerradas de marzo: dos reuniones y una tarea |
| **Conferenciantes** | ✅ PRD "Centralización de la Gestión de Conferenciantes" | 🔴 **Cero issues** |
| Rediseño visual (UI/UX) | — | ⏳ `GD-619` sin planificar |
| Plantillas de planificación | — | ⚠️ `GD-25` sin tocar desde **julio de 2024** |

## 🕓 Ámbitos de conocimiento: el caso más claro

El PRD es bueno: espacio de problemas, objetivos, cinco requisitos con prioridad, diseño de
pantallas, política de notificaciones y **métricas de éxito** ("95% de los profesores con su
ámbito registrado en los primeros 6 meses"). Lo firmó Pilar y se modificó por última vez el
**13/03/2026**.

Su tabla de hitos, tal cual está hoy en Confluence:

| Hito | Fecha objetivo | Estado en la página |
|---|---|---|
| Definición de requisitos y wireframes | 15/03/2026 | **No iniciado** |
| Desarrollo del módulo | 15/04/2026 | **No iniciado** |
| Integración con BBDD de RRHH | 30/04/2026 | **No iniciado** |
| Pruebas y ajustes | 15/05/2026 | **No iniciado** |
| **Lanzamiento y formación** | **31/05/2026** | **No iniciado** |

Es decir: **el lanzamiento estaba previsto para el 31 de mayo y hace tres meses que pasó**, con
todos los hitos sin arrancar. Y parte de eso no es cierto —la definición de requisitos **sí** se
hizo, y los prototipos se validaron en marzo (`GD-510`, `GD-516`, cerradas)—, así que el problema
es doble: **el módulo está parado y además el estado documentado no refleja la realidad.**

**Ojo con quién es el cliente de este módulo:** el PRD dice que sirve a **RRHH, coordinadores y
dirección académica**. RRHH es el área que supervisa **María Mendoza**. No es un módulo cualquiera
para ella.

## 🗂️ Estado del espacio de Confluence

- **El Home es la plantilla por defecto de Confluence**, sin editar desde abril de 2024
  ("¡Te damos la bienvenida a tu nuevo espacio!"). El espacio **no tiene índice ni descripción del
  proyecto**: para saber qué hay, toca abrir las 30 páginas.
- **El Cronograma está congelado en febrero de 2026** y solo contiene las cinco reuniones de
  requisitos de marzo. **No hay ninguna planificación hacia delante.**
- **El "Informe seguimiento de implantación propuesta docente"** es únicamente un enlace a una
  hoja de Google, de septiembre de 2025, y **su autor ya no está en la organización**.
- **Hay dos páginas de reuniones duplicadas**: "Reuniones de seguimiento" y "Reuniones de
  seguimiento Gestión Docente".
- Actas de 2024 mezcladas al mismo nivel que documentación viva de 2026.

## ✅ Lo que sí está bien

- **La documentación de requisitos es de calidad.** Los PRDs tienen estructura, prioridades
  MoSCoW, métricas y consideraciones técnicas. El de Investigadores llegó hasta 21 historias en
  Jira con criterios de aceptación.
- **La trazabilidad requisito → Jira funciona cuando se completa el circuito** (Investigadores lo
  demuestra).
- **El incidente del volcado está bien tratado**: diagnosticado y desglosado en 15 tareas,
  agrupadas en dos epics nuevas con nombres que dicen lo que hacen (integridad de asignaciones,
  volcado a PDS).

## 📋 Decisiones que hay que tomar

1. **Ámbitos de conocimiento: ¿se retoma o se aparca formalmente?** Si se retoma, necesita epic,
   historias, sprint y fechas nuevas. Si se aparca, hay que decirlo — y decírselo a RRHH, que lo
   validó en marzo y lleva desde entonces esperando.
2. **Conferenciantes: igual.** PRD escrito y nada más.
3. **Reducciones horarias:** `GD-539` lleva abierta desde mayo. ¿Vive o se cierra?
4. **`GD-25` (plantillas de planificación)** no se toca desde julio de 2024. Candidata a cerrarse.
5. **Rehacer el Cronograma** con el plan real de aquí a diciembre, y **poner un índice en el
   Home**. Sin eso, cualquiera que entre al espacio —incluida gerencia— se lleva la impresión
   equivocada del proyecto.

## 📅 Cronograma propuesto (borrador para revisar)

Basado en lo que hay vivo y en el cierre de sprint del **miércoles 16**:

| Cuándo | Qué |
|---|---|
| **Sept (resto)** | Cerrar el incidente del volcado a Laurea: recuperar asignaciones perdidas y trazabilidad de borrados. Es la prioridad y bloquea confianza en el sistema |
| **Sept — jueves 10** | Revisión de Bajas y Sustituciones con Profesorado |
| **Oct** | Investigadores: cerrar las historias P0 (alta, ficha, control de horas, autorizaciones) |
| **Oct** | Decidir Ámbitos y Conferenciantes. Si entran, epic y fechas |
| **Nov** | Investigadores P1 · Bajas y Sustituciones en producción |
| **Dic** | Integración de solicitudes docentes con el sistema de tickets *(ya comprometido "hasta diciembre")* |
| **Sin fecha** | Rediseño visual · Reducciones horarias · Ámbitos y Conferenciantes si no se deciden en octubre |

⚠️ **Esto es un borrador mío a partir de los datos.** Las fechas de octubre y noviembre no salen
de ninguna parte: hay que ponerlas con el equipo, y contando con que el sprint que viene ya está
comprometido con el volcado.

## 🔗 Enlaces

- Espacio **Gestión Docente** en Confluence · proyecto `GD` en Jira
- [[2026-09-08 - Summary Gestión de la Docencia (María Mendoza)]]
- [[Proyectos y claves Jira]] · [[Producto (Área)]]
