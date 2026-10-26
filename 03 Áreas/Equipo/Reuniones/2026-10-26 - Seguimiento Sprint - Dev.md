---
tipo: reunión
fecha: 2026-10-26
hora: 09:15–10:45
sprint: Desarrollo 2026/17
sprint_dia: 7 de 14 (día hábil 5 de 10)
sprint_fin: 2026-11-02
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — 26/10, mitad del 2026/17 y semana del lanzamiento de Educación

> ⚠️ **Nota reconstruida a posteriori (~11:00) desde el tablero de Jira.** La reunión fue de 09:15 a 10:45 (Sala TIC + Meet),
> **no está en el calendario de Pilar** (en la sala figura *rechazada*) y **no hay notas de Gemini ni transcripción**. Lo que
> sigue es lo que dice Jira, no lo que se habló: si se decidió algo, va en *Acciones*.
> **No hay notas de los Seguimientos del 05, 19/10 ni de octubre en general** (el 12 fue festivo): la comparación es con el
> [[2026-09-28 - Seguimiento Sprint - Dev|28/09]], hace cuatro semanas.

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/17** (id 3108, tablero 3) |
| Fechas | **mar 20/10 → lun 02/11** |
| Hoy | lunes 26 · día **7 de 14** naturales · día hábil **5 de 10** |
| Días hábiles que quedan | **6** contando hoy (26, 27, 28, 29, 30 y 2/11) — **5 si el lunes 2/11 es festivo** |
| Tareas del equipo en el sprint | **94** (incluidas 6 genéricas de imputación y 7 `rq-rec` sin dueño): **20 cerradas, 74 abiertas** |

🟡 **Semana de ejecución, no de cierre**, pero con dos relojes externos:
- 🚀 **Miércoles 28: Educación abre a alumnos.** Quedan **P0 sin empezar** (ver Riesgos)
- 🚨 **Incidente de seguridad en Sede / Tramita** desde el sábado → [[26-10-2026]]. Toca a **Jesús** (experto en Sede) y
  se trata mañana en Responsables

❓ **¿Es festivo el lunes 2/11?** El 1/11 cae en domingo y [[Festivos y no lectivos 26-27]] no dice nada. Si lo es, **el cierre
real es el viernes 30** y el Seguimiento del 2/11 no se celebra.

## 👥 Reparto por persona

### Alex — 4 abiertas · 8 cerradas · *otra vez la quincena más limpia*
- ✅ Cerró **`TM-105`** *(campus de Madrid en Talleres, Muy Urgente)*, **`TM-106`** (hallazgos de seguridad r1 de Talleres),
  `GES-273`, `GES-274`, `GES-278`, `GES-279` (v1.9.1 de prácticas), `GES-280` (soporte a Enfermería en PRADO) y `ED-2068`.
- En curso **`TM-108`** (hallazgos r2, vence vie 30) y en TESTING **`TM-107`** *(migrar Talleres a un repo sin secretos en el
  historial — **venció el 22/10**)*.
- 🔴 Por hacer **`GES-229`** *(RF-35, bloqueo nominativo por DNI del Máster Bilingüe, **P0**)* — y Educación sale el miércoles.
  También `RDC-105` (`RQ-REC-14`).

### Juanma — 8 abiertas · 2 cerradas
- ✅ Cerró **`GES-252`** *(supervisar el impacto de las pantallas en la arquitectura, Muy Urgente)* y **`GES-251`** *(supervisar
  el algoritmo con Paco)*.
- 🔴 Por hacer **`GES-233`** *(RF-39, desdoblar plazas, **P0**)* y **`GES-239`** *(RF-45, correo de asignación al alumno, P1 —
  movida el 23)*. **Las dos son de Educación.**
- 🧊 Igual que hace un mes: `WD-384`, `FAC-32` y la deuda de Canvas Data (`CAN-337`, `CAN-340` **vencidas desde nov-2025**,
  `CAN-348`, `CAN-349`).

### Paco — 14 abiertas · 1 cerrada
- 🆕 **`ED-2069`** *(imagen base `ucam/microservice` fijada a la versión de Java, **Muy Urgente**, vence vie 30)* — es la
  respuesta a la pregunta de Adrián sobre el CVE de Java. Movida hoy.
- 🔴 **`AS-592`** *(volcado de asistencia, **Muy Urgente**)* en curso y **vencida el 23/10**.
- **Mi Docencia (`AS-582`…`AS-590`)**: 9 abiertas, 2 en TESTING, 2 en curso, 5 por hacer. Solo `AS-581` cerrada.
- ❓ **`GES-255` (algoritmo de asignación) sigue en *Por hacer*** aunque Juanma cerró su supervisión (`GES-251`) el 22/10.
  ¿Está hecho y sin cerrar, o no está? **Con Educación el miércoles, hay que saberlo hoy.**
- 🧊 `IN-505` *(vencida desde mayo)* — quinta semana · `ED-2067` (PoC de Qwen) en TESTING.
- Fuera del sprint: `GES-236` *(RF-42, P1, límite de 5 registros en asignaciones manuales)*.

### Alejandro — 10 abiertas · 0 cerradas
- 🔴 **Todo quieto**, lo mismo que el 28/09: `EVT-14`…`EVT-18` *(vencidas el 1 de agosto)*, `ED-2014`/`2015`/`2016`
  *(vencidas 1–4 de agosto)*, `ED-2030` *(doble factor, en curso, venció el 12/09)* y `ED-2039` (IMarina).
- 💡 Como hace un mes: **su trabajo real no está en el tablero** (Alma, Cientia, iMarina, Java, revisión de código…). Ni lo
  que hace aparece, ni lo que aparece se hace.

### Jesús — 10 abiertas · 6 cerradas
- ✅ **Cerró el certificado B2 de Primaria entero** (`ET-550`…`ET-554`, del 1 al 5) y `ET-558`.
- En curso **`ET-559` *Errores en Sede*** — 🚨 *con el incidente del fin de semana, esta tarea va a crecer*, **`IN-563`/`IN-564`**
  (módulo de planillas de corrección de exámenes, ya en PRE), `MIG-50` y `ED-2048` (servicios de Alfresco).
- 🔴 **`MIG-45` y `MIG-46` siguen sin tocar** — **quinta nota seguida** desde el 16/09. Y `IN-494`, `GESTDOC-11`, `ET-491`.

### Pablo — 8 abiertas · 1 cerrada
- ✅ `RDC-102` (vídeo de los reconocimientos previos).
- En curso: `GD-711` (sustituto en Gestión horas docencia), `GD-700`/`GD-701` (incidencias de pre-volcado de planes),
  `GD-597` (correo diario a coordinadores).
- 🟠 **`RDC-103` y `RDC-104`** *(`RQ-REC-06` y `-07`, **Urgentes**)* sin tocar en **10 días**, desde que se crearon.
- 🧊 `GD-87`, `GD-596` — las "paraguas" de Gestión Docente.

### Pilar — 6 abiertas · 2 cerradas
- ✅ `GES-235` (RF-41) y `ED-2066` (repositorios en Confluence).
- Abiertas: las 4 epics de Educación (`GES-222`…`GES-225`) y `GES-250` — **cerrarlas tras el lanzamiento del miércoles** —
  y `DT-310` (cierre de Infucam).

### Sin asignar
- 🔴 **`RDCO-182`…`RDCO-188`** — las 7 `rq-rec` de Reconocimientos (**4 Urgentes**), **10 días sin dueño**.
- ⚠️ **`GES-254`** *(descarga del mapa docente de Prado)* — **EN CURSO sin dueño**, ya **cuarta nota seguida**.
- Las genéricas de octubre (`ED-2054`…`ED-2059`), que vencen el **sáb 31** → la tanda de noviembre la crea `/inicio-sprint`.

## 🧊 Quieto desde hace días

> El "6 días" de Jira en casi todo es **el arrastre al sprint el 20/10**: llevan paradas desde mucho antes.

| Días | Qué | De quién | Notas seguidas |
|---|---|---|---|
| **≥40** | `EVT-14`…`EVT-18`, `ED-2014`/`2015`/`2016`, `ED-2030` | Alejandro | **4ª** — vencidas desde agosto |
| **≥40** | `MIG-45`, `MIG-46` | Jesús | **5ª** |
| **≥40** | `CAN-337`, `CAN-340`, `CAN-348`, `CAN-349` | Juanma | **4ª** — nov-2025 / mar-2026 |
| **≥40** | `IN-505` | Paco | **4ª** — vencida desde mayo |
| **≥30** | `GES-254` *(en curso, sin dueño)* | — | **4ª** |
| **10** | `RDCO-182`…`188` *(sin dueño)* · `RDC-103`, `RDC-104` | — · Pablo | 1ª — **4 + 2 Urgentes** |
| **6** | `GES-255` (algoritmo), `GES-229`, `GES-233` | Paco · Alex · Juanma | **ruta crítica de Educación (mié 28)** |

## ⚖️ Riesgos y equilibrado

- 🔴 **Educación sale el miércoles con tres P0 en *Por hacer*** (`GES-229`, `GES-233`) y el algoritmo (`GES-255`) sin cerrar. O
  están hechas y nadie ha movido Jira, o no llegan. **Es la pregunta de hoy.**
- 🔴 **El incidente de Sede cae sobre Jesús**, que ya lleva Sede, planillas, Alfresco y migraciones. Si mañana sale trabajo de
  Responsables, **algo suyo tiene que salir del sprint**: `MIG-45`/`MIG-46` llevan cinco notas quietas y son las candidatas.
- 🟠 **Paco** ha bajado de 30 a **14 abiertas** (bien), pero tiene **dos Muy Urgentes**, una ya vencida, y la cadena de Mi
  Docencia de 9 tareas. Con el criterio de siempre (*fuera de la ruta crítica, trocear*): `ED-2069` es plataforma y urgente —
  **¿debería llevarla Alejandro**, que es quien conoce las imágenes de Kubernetes?
- 🟠 **Reconocimientos sin dueño**: según el [[2026-10-08 - Mejoras de la app de Reconocimientos|acta del 08/10]], *el equipo
  está con Educación hasta el 28/10 y no hay hueco hasta mediados de noviembre*, y tú querías meter a **Alex**. Alex ha
  cerrado 8 esta quincena: **después del miércoles es el candidato natural** para las `RDCO`, con Juanma de mentor.
- 🟡 **Alejandro y el tablero no se parecen** (cuarta nota). Limpiar: redatar `EVT-*`/`ED-201x` o mandarlas al backlog, y que
  lo que hace de verdad (seguridad, Java, Alma) tenga issue.
- 🟡 **Nadie estima todavía**: sin puntos, el reparto sigue haciéndose por número de tareas.
- 🟡 **Seguridad de Talleres**: `TM-107` *(secretos en el historial del repo)* venció el 22/10 y sigue en TESTING. En la semana
  del incidente de Sede, **que no se quede ahí**.

### 💡 Propuesta de movimientos (para decidir tú; no se ha tocado Jira)

| Qué | De → a | Por qué |
|---|---|---|
| **`GES-229`, `GES-233`, `GES-255`** | — | **Confirmar estado hoy**; si no llegan al miércoles, decirlo a Educación antes, no después |
| **`RDCO-182`…`188`** | sin dueño → **Alex** (con Juanma) a partir del jueves | Tiene hueco y ritmo; el acta ya lo apuntaba |
| **`ED-2069`** (Java base) | Paco → **Alejandro** o con él | Plataforma y Muy Urgente; Alejandro conoce las imágenes |
| **`MIG-45`/`MIG-46`** | sprint → **backlog** | Cinco notas quietas; libera a Jesús para Sede |
| **`EVT-*`, `ED-2014`…`2016`, `CAN-*`, `IN-505`** | → **backlog o redatar** | Cuatro notas quietas; ensucian la medición |
| **`GES-254`** | sin dueño → **Juanma** o **Alex** | Cuarta nota en curso sin dueño |

## 📅 Hitos y agenda de la semana

| Día | Qué |
|---|---|
| **lun 26** | Seguimiento 09:15 · 🗂️ **UCAMSEGRE2 en Explotación** (Alicia) |
| **mar 27** | 🚨 **10:00 Responsables** — probablemente monográfica de la vulnerabilidad de Sede |
| **mié 28** | 🚀 **Educación abre a alumnos** · Tangram 11:00 *(choca con Instructure)* |
| **vie 30** | Vencen `ED-2069` y `TM-108` · Reunión de vulnerabilidades 09:00 *(si no se absorbe el martes)* |
| **sáb 31** | Vencen las genéricas de octubre |
| **lun 2/11** | 🏁 **Cierre del `2026/17`** *(o el vie 30 si el 2 es festivo)* → arranque del `2026/18` y **`/inicio-sprint`** con la tanda de **noviembre** |

## 📌 Acciones (quién / cuándo)

- [ ] **Pilar** · hoy — confirmar con Alex, Juanma y Paco si `GES-229`, `GES-233` y `GES-255` llegan al miércoles
- [ ] **Pilar** · antes del jueves — asignar `RDCO-182`…`188` *(propuesta: Alex con Juanma)*
- [ ] **Pilar** · tras Responsables (mar 27) — ver qué trabajo de Sede le cae a Jesús y sacar `MIG-45`/`MIG-46` del sprint
- [ ] **Pilar** · esta semana — decidir quién lleva `ED-2069` (Java base)
- [ ] **Alguien** · ya — ponerse `GES-254` a su nombre *(cuarta vez que se apunta)*
- [ ] **Alex** · esta semana — cerrar `TM-107` (secretos en el historial de Talleres)
- [ ] **Pilar** · antes del vie 30 — confirmar si el lunes 2/11 es festivo y, si lo es, añadirlo a [[Festivos y no lectivos 26-27]]
- [ ] **Pilar** · jue/vie — cerrar las epics de Educación (`GES-222`…`225`, `GES-250`) si el lanzamiento sale bien
- [ ] *(Si en la reunión de hoy se decidió algo, apúntalo aquí)*

## 🕓 Para tener en cuenta más adelante

- **Cuatro semanas sin nota de Seguimiento.** Sin acta ni Gemini, cada nota se reconstruye desde Jira y no recoge lo que se
  dice. Dos salidas: **activar las notas de Gemini** en la invitación de Meet o **pasar el Seguimiento a Zoom**, que es lo que el
  conector puede leer.
- **El Seguimiento no está en tu calendario** (en la Sala TIC figuras como *rechazada*) y la tarea programada del lunes cree que
  es de 09:45 a 11:15. Una de las dos cosas está mal: si la hora buena es 09:15, **el daily de los lunes debería correr a las
  08:45**.
- **Las mismas tareas quietas desde septiembre** (`EVT-*`, `CAN-*`, `MIG-45/46`, `IN-505`, `GES-254`). Una limpieza de backlog
  en el cierre del 2/11 dejaría el `2026/18` medible.
- **Tras Educación viene Medicina** (acta de Reconocimientos), y Reconocimientos espera desde el 16/10. El `2026/18` tiene que
  elegir.

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Anterior: [[2026-09-28 - Seguimiento Sprint - Dev]] · [[2026-09-16 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[2026-09-10 - Prácticas Educación 26-27]] · [[2026-10-08 - Mejoras de la app de Reconocimientos]]
- [[Seguridad (Proyecto)]] · [[Festivos y no lectivos 26-27]] · [[Cronograma de proyectos (hasta dic 2026)]] · [[26-10-2026]]
