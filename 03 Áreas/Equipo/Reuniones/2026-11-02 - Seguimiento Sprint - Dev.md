---
tipo: reunión
fecha: 2026-11-02
hora: 09:15–10:45
sprint: Desarrollo 2026/17
sprint_dia: 14 de 14 (día hábil 10 de 10)
sprint_fin: 2026-11-02
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — 02/11, cierre del 2026/17 (Educación ya ha salido)

> ⚠️ **Nota reconstruida a posteriori (~11:30) desde el tablero de Jira.** La reunión fue de 09:15 a 10:45 (Sala TIC + Meet) y
> **coincidió con *Aplicativo docente* (09:00–10:00)**, al que fuiste. No está en tu calendario, no hay notas de Gemini ni
> transcripción: lo que sigue es lo que dice Jira, no lo que se habló. Si se decidió algo, va en *Acciones*.
> Comparación con la [[2026-10-26 - Seguimiento Sprint - Dev|nota del 26/10]].
> **Cabina sin refrescar hoy**: es del vie 30 a las 14:49 (un día hábil). La uso tal cual; pasa `/cabina` si quieres el corte de hoy.

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/17** (id 3108, tablero 3) |
| Fechas | **mar 20/10 → lun 02/11** (cierra hoy a las 18:06) |
| Hoy | día **14 de 14** naturales · día hábil **10 de 10** — **último día** |
| Festivos | ninguno: el 2/11 es laborable *(confirmado el 29/10 en [[Festivos y no lectivos 26-27]])* |
| Tareas en el sprint | **151**: **70 cerradas, 81 abiertas** (incluye 6 genéricas de octubre, 7 `RDCO` sin dueño y las 5 epics de Educación) |
| Sprint siguiente | ⚠️ **No hay ningún sprint futuro con tareas** en el tablero → `/inicio-sprint` mañana |

🏁 **Semana de cierre y arranque.** Lo que esté abierto a las 18:06 pasa al siguiente: este es el momento de **decidir qué no
pasa** (ver la propuesta de limpieza).

🚀 **Educación salió y salió bien**: apertura el 28/10, asignación el 30/10 con **690 alumnos con plaza, 73 % en 1ª opción y
ninguno sin plaza** entre los que eligieron. Esther publica hoy. Eso **libera a Juanma y a Alex** justo cuando
[[Reconocimientos]] se ha puesto en rojo.

## 👥 Reparto por persona

### Pablo — 8 abiertas · 29 cerradas · *la quincena más productiva del equipo*
- ✅ Cerró **todo el paso a `security-commons` en Gestión Docente** (`GD-738`…`GD-747`, fases 1 a 7), el pipeline de
  `jav-misplanillas` (`GD-755`), los pre-volcados de planes (`GD-700`, `GD-701`), el sustituto en horas de docencia (`GD-711`),
  el correo diario a coordinadores (`GD-597`) y el **módulo de Bajas y Sustituciones** (`GD-596`, la "paraguas" que salía quieta).
- 🔴 🆕 **`GD-765` — *"La app no sincroniza desde el 28 de octubre"*** (Urgente, **por hacer**, entró el sáb 31). Es una
  incidencia de producción y nadie la ha cogido. **Coincide con el despliegue de `security-commons` del 29/10.**
- En curso: **`RDC-103` y `RDC-104`** (`RQ-REC-06` y `-07`, Urgentes — **ya se mueven**: el 26/10 llevaban 10 días quietas),
  `GD-748` (reconocimientos previos al plugin de seguridad), `GD-749` (mejoras de solicitud), `GD-762`, `GD-763`.

### Alejandro — 9 abiertas · 10 cerradas · *por fin su trabajo está en el tablero*
- ✅ Esta mañana ha creado y cerrado su trabajo real: parches de seguridad y compilado (`ED-2082`), errores de Cientia
  (`ED-2083`, `ED-2086`), RIUCAM (`ED-2087`), soporte al despliegue de Mis Planillas (`ED-2081`), eventos de la segregación de
  facultades (`EVT-22`) y revisión de seguridad (`EVT-21`). Y cierra dos de las viejas: **`ED-2030`** (doble factor) y **`ED-2039`**
  (iMarina).
- 🆕 `ED-2088` *Informes Seguridad* (vence el dom 8).
- 🧊 Siguen las de agosto: `EVT-14`…`EVT-18` y `ED-2014`/`2015`/`2016` — **quinta nota seguida**. Ahora que lo real está en Jira,
  **esto ya solo es limpieza**: backlog o redatar.

### Alex — 6 abiertas · 13 cerradas
- ✅ Cerró **`TM-108`** (hallazgos r2 de Talleres), `RDC-106` (soporte al portal de reconocimientos previos) y todo el
  acompañamiento de Educación: videotutorial (`GES-282`), apertura de la elección (`GES-283`) y Enfermería (`GES-284`).
- En curso: **`RDCO-189`** (seguridad r2 de Reconocimientos, vence vie 6) y `GES-285` (Excel de asignaciones definitivo).
  En TESTING: **`RDC-105`** (`RQ-REC-14`, movida hoy), `LA-56` (seguridad r2 de Learning Agreement, venció el 30/10) y
  **`TM-107`** *(secretos en el historial del repo de Talleres — **venció el 22/10 y lleva 10 días en TESTING**)*.
- ❓ **`GES-229`** (RF-35, bloqueo por DNI del Máster Bilingüe, **P0**) sigue en *Por hacer* desde el 20/10 — y Educación ya ha
  asignado. ¿Se resolvió de otra forma o se cayó?

### Paco — 14 abiertas · 7 cerradas
- ✅ Cerró los dos **Muy Urgentes**: **`ED-2069`** (imagen base de Java — la respuesta al CVE de Adrián) y **`AS-592`** (volcado de
  asistencia), más `ED-2070` (seguridad en procesos-asistencia), `AS-593`, `ED-2067` (PoC de Qwen) y `ED-2071` (automatización de
  Tempo).
- En TESTING: **`GES-281`** (volcado a Laurea de la oferta pública de Educación, vence mar 3), `AS-582`, `AS-583`.
- 🧊 **Mi Docencia** (`AS-584`…`AS-590`): 7 abiertas, **5 sin tocar desde el 20/10**.
- ❓ **`GES-255` (algoritmo de asignación) sigue en *Por hacer*** — y la asignación **ya se ejecutó el 30/10 sin errores**. Está
  hecho: hay que cerrarlo (o explicar qué falta).
- 🧊 `IN-505` (vencida desde mayo) — **quinta nota seguida**.

### Jesús — 11 abiertas · 7 cerradas
- ✅ Cerró **`ET-559` *Errores en Sede*** (30/10), además del B2 de Primaria entero (`ET-550`…`ET-554`) y `ET-558`.
- 🟢 **Mis Planillas va a producción**: `IN-565` (subida a producción, en curso), `IN-566` (pruebas de subida), `IN-563`/`IN-564`
  en TESTING. Es la app de [[Lectura y corrección de planillas]], **que está en rojo y venció el sábado**: el avance es real,
  falta que la ficha lo refleje y que la fecha se mueva.
- En TESTING `MIG-50` (carga en `SINC_EXPEDIENTES`). En curso `IN-494` y `ED-2048` (servicios de Alfresco, quieto desde el 20/10).
- 🔴 **`MIG-45` y `MIG-46` sin tocar — sexta nota seguida** (desde el 16/09). Y `GESTDOC-11`, `ET-491`.

### Juanma — 13 abiertas · 2 cerradas
- ✅ `GES-251` y `GES-252` (supervisión del algoritmo y de las pantallas de Educación).
- 🆕 Hoy entran **cinco tareas nuevas** a su nombre: `GES-286` (puesta en marcha del proceso de selección), `GES-287`
  (reconciliación de plazas Erasmus), `GES-288` (motor reutilizable de videotutoriales), `TOOL-42` (segregación de facultades en la
  personalización) y `CAN-371` (remediación de la auditoría de seguridad de Canvas).
- En TESTING `GES-239` (RF-45, correo de asignación).
- ❓ **`GES-233`** (RF-39, desdoblar plazas, **P0**) en *Por hacer* desde el 20/10 — misma pregunta que `GES-229`.
- 🧊 `WD-384`, `FAC-32` y la deuda de Canvas Data (`CAN-337`, `CAN-340` **vencidas desde nov-2025**, `CAN-348`, `CAN-349`) —
  **quinta nota seguida**.

### Pilar — 6 abiertas · 2 cerradas
- Las 4 epics de Educación (`GES-222`…`GES-225`) y `GES-250`: **Educación ya ha salido → cerrarlas**. Y `DT-310` (Infucam).

### Sin asignar
- 🔴 **`RDCO-182`…`RDCO-188`** — las 7 `rq-rec` de Reconocimientos (**4 Urgentes**), **17 días sin dueño** (desde el 16/10).
  Son **la causa del rojo** de [[Reconocimientos]].
- ⚠️ **`GES-254`** (descarga del mapa docente de Prado) — **EN CURSO sin dueño, quinta nota seguida**.
- Las genéricas de octubre (`ED-2054`…`ED-2059`), **vencidas el sáb 31** → cerrarlas tras imputar; la tanda de noviembre la crea
  `/inicio-sprint`.

## 🧊 Quieto desde hace días

> Hoy es 02/11: todo lo que tiene `updated` del 20/10 lleva **13 días** — y en la mayoría es solo el arrastre al sprint.

| Días | Qué | De quién | Notas seguidas |
|---|---|---|---|
| **≥45** | `MIG-45`, `MIG-46` | Jesús | **6ª** |
| **≥45** | `EVT-14`…`EVT-18`, `ED-2014`/`2015`/`2016` | Alejandro | **5ª** — vencidas desde agosto |
| **≥45** | `CAN-337`, `CAN-340`, `CAN-348`, `CAN-349`, `WD-384`, `FAC-32` | Juanma | **5ª** |
| **≥45** | `IN-505` | Paco | **5ª** — vencida desde mayo |
| **≥30** | `GES-254` *(en curso, sin dueño)* | — | **5ª** |
| **17** | `RDCO-182`…`188` *(sin dueño)* | — | **2ª** — 4 Urgentes |
| **13** | `GES-229`, `GES-233`, `GES-255` | Alex · Juanma · Paco | **2ª** — Educación ya salió: ¿hechas o descartadas? |
| **13** | `AS-584`…`AS-590` (Mi Docencia) | Paco | 1ª |
| **13** | `ED-2048` (Alfresco), `GESTDOC-11`, `ET-491` | Jesús | 2ª |
| **10** | `TM-107` *(en TESTING, vencida el 22/10)* | Alex | **2ª** — secretos en el historial |

## 🚦 Proyectos en rojo y ámbar (cabina del 30/10)

- 🔴 [[Reconocimientos]] *(desde el 30/10)* — 7 tareas quietas 7+ días hábiles: son los `RDCO` sin dueño. Se arregla asignándolos
- 🔴 [[Lectura y corrección de planillas]] *(desde el 26/10)* — **venció el 31/10**. Mis Planillas está subiendo a producción
  (`IN-565`): **mover la fecha** y revisar si el rojo sigue teniendo sentido
- 🔴 [[Alfresco - nuevo repositorio]] *(desde el 26/10)* — `ED-2048` quieto desde el 20/10; bloquea Infucam y planillas
- 🔴 [[Cierre de Infucam]] *(desde el 26/10)* — depende del Alfresco
- 🔴 [[Remediación Protocolo]] *(desde el 26/10)*

## ⚖️ Riesgos y equilibrado

- 🔴 **`GD-765` — Gestión Docente sin sincronizar desde el 28/10**, Urgente y sin empezar. Es producción, y cae después del
  despliegue de `security-commons`. **Lo primero del sprint nuevo**, a Pablo (es su código).
- 🔴 **Reconocimientos lleva 17 días sin dueño** y ahora hay capacidad: Educación ha salido. El acta del 08/10 apuntaba a **Alex**,
  que ya está en Reconocimientos (`RDC-105`, `RDCO-189`) y cierra a buen ritmo.
- 🟠 **Juanma acumula**: 13 abiertas, 2 cerradas, cinco nuevas hoy y la deuda de Canvas. Además es quien mentoriza a Alex. Si Alex
  coge los `RDCO`, **algo de Juanma tiene que salir** (la deuda `CAN-337`…`349`, al backlog).
- 🟠 **Jesús** tiene Planillas en producción, Alfresco y la Sede. `MIG-45`/`MIG-46` llevan seis notas sin tocarse: **al backlog**.
- 🟡 **Las P0 de Educación (`GES-229`, `GES-233`, `GES-255`)** siguen abiertas con el proceso terminado. O están hechas y nadie
  ha movido Jira, o se descartaron: **cerrarlas o pasarlas a deuda con nombre**, no arrastrarlas al sprint nuevo.
- 🟡 **Seguridad**: `TM-107` (secretos en el historial) y `LA-56` siguen en TESTING y vencidas. Con la [[Seguridad (Proyecto)|semana
  de Tramita]] reciente, que no se queden ahí.
- 🟡 **Nadie estima**: sin puntos, el reparto se sigue midiendo por número de tareas.

### 💡 Propuesta de movimientos (para decidir tú; no se ha tocado Jira)

| Qué | De → a | Por qué |
|---|---|---|
| **`GD-765`** (no sincroniza) | sin empezar → **Pablo**, primera del sprint | Producción caída desde el 28/10 |
| **`RDCO-182`…`188`** | sin dueño → **Alex** (con Juanma de mentor) | Causa del rojo de Reconocimientos; Alex ya está en la app |
| **`GES-229`, `GES-233`, `GES-255`** | → **cerrar** o deuda explícita | Educación ya asignó; no deben arrastrarse |
| **Epics `GES-222`…`225`, `GES-250`** | → **cerrar** (tú) | Lanzamiento hecho |
| **`MIG-45`/`MIG-46`** | sprint → **backlog** | Seis notas quietas |
| **`EVT-14`…`18`, `ED-2014`…`2016`, `CAN-337`…`349`, `IN-505`, `WD-384`, `FAC-32`** | → **backlog o redatar** | Cinco notas quietas; ensucian la medición del `2026/18` |
| **`GES-254`** | sin dueño → **Juanma** o **cerrar** | Quinta nota en curso sin dueño |
| **Genéricas de octubre** (`ED-2054`…`2059`) | → cerrar tras imputar | Vencidas el 31/10 |

## 📅 Hitos y agenda de la semana

| Día | Qué |
|---|---|
| **lun 2** | 🏁 **Cierre del `2026/17` a las 18:06** · Esther publica la asignación de Educación |
| **mar 3** | 🚀 **Arranque del sprint siguiente** → `/inicio-sprint` (genéricas de noviembre + Responsables) · **Responsables 10:00–11:30** · Repositorio de documentación DTIC 13:00 (Adrián) · vence `GES-281` |
| **mié 4** | Sigma 10:00 (seguimiento de referencias) · Tangram 11:00 |
| **jue 5** | Repaso de migraciones Biblioteca 09:30 (con Alejandro) |
| **vie 6** | 🎓 Examen IR 08:30 · Gestión de repositorio de código DTIC 12:00 (Adrián) · vencen `RDCO-189` y `GES-285` |

## 📌 Acciones (quién / cuándo)

- [ ] **Pilar** · hoy, antes de las 18:06 — decidir qué pasa al sprint nuevo y qué va al backlog (ver la tabla de propuesta)
- [ ] **Pilar** · mañana — `/inicio-sprint` (no hay sprint futuro creado) y asignar **`RDCO-182`…`188`**
- [ ] **Pablo** · ya — coger `GD-765` (Gestión Docente no sincroniza desde el 28/10)
- [ ] **Paco / Alex / Juanma** · hoy — cerrar o explicar `GES-255`, `GES-229` y `GES-233`
- [ ] **Pilar** · esta semana — cerrar las epics de Educación (`GES-222`…`225`, `GES-250`)
- [ ] **Pilar** · hoy — fecha nueva para [[Lectura y corrección de planillas]] (Mis Planillas sube a producción con `IN-565`)
- [ ] **Alex** · esta semana — sacar de TESTING `TM-107` y `LA-56`
- [ ] **Alguien** · ya — `GES-254` a su nombre o cerrarla *(quinta vez que se apunta)*
- [ ] *(Si en la reunión de hoy se decidió algo, apúntalo aquí)*

## 🕓 Para tener en cuenta más adelante

- **Cinco Seguimientos sin acta.** Sin Gemini ni Zoom, cada nota se reconstruye desde Jira. Hoy además **la reunión chocó con
  *Aplicativo docente*** y no te enteraste de lo que se dijo. Las dos salidas siguen siendo las mismas: **activar Gemini** en el
  Meet o **pasarlo a Zoom**.
- **La hora del Seguimiento**: la sala dice **09:15–10:45** y la tarea del daily de los lunes dice 09:45–11:15. Si la buena es
  09:15, el daily de los lunes debería correr a las **08:45**, y hoy ha llegado a las 10:50.
- **Alejandro ha empezado a registrar su trabajo real en Jira** (nueve issues creadas y cerradas hoy). Si se mantiene, las `EVT-*`
  y `ED-201x` de agosto ya no tienen sentido en el sprint.
- **Tras Educación viene Medicina** (acta de Reconocimientos). El `2026/18` tiene que elegir entre Reconocimientos y Medicina, y
  Reconocimientos está en rojo.

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Anterior: [[2026-10-26 - Seguimiento Sprint - Dev]] · [[2026-09-28 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[Reconocimientos]] · [[2026-10-08 - Mejoras de la app de Reconocimientos]] · [[Lectura y corrección de planillas]]
- [[Cabina - Cartera]] · [[Festivos y no lectivos 26-27]] · [[02-11-2026]]
