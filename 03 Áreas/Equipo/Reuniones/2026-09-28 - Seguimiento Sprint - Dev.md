---
tipo: reunión
fecha: 2026-09-28
hora: 09:15–10:45
sprint: Desarrollo 2026/15
sprint_dia: 13 de 16 (día hábil 9 de 12)
sprint_fin: 2026-10-01
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — 28/09, semana de cierre del 2026/15

> ⚠️ **Nota reconstruida a posteriori, a las 16:30, desde el tablero de Jira.** La reunión fue a
> las 09:15 (Meet + Sala de trabajo TIC) y **no hay notas de Gemini ni transcripción**. Lo que aquí
> sale es **lo que dice Jira**, no lo que se habló: si en la reunión se decidió algo, añádelo en
> *Acciones*. Tampoco hay acta del Seguimiento del **21/09**, así que la comparación es con el
> arranque del [[2026-09-16 - Seguimiento Sprint - Dev|16/09]].

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/15** (id 2941, tablero 3) |
| Fechas | **16/09 → jueves 01/10** |
| Hoy | lunes 28 · día **13 de 16** naturales · día hábil **9 de 12** |
| Días hábiles que quedan | **3** — martes 29, miércoles 30 y **jueves 1**, el cierre |
| Tareas del equipo en el sprint | **~103** (sin contar las 6 genéricas de imputación): **47 cerradas, 66 abiertas** de los seis devs + 8 de Pilar |

🔴 **Es semana de cierre.** Sin festivos dentro del sprint, pero el cierre cae el **jueves 1**, el
mismo día de la **consultoría de SIGMA (12:30–14:00)**: el cierre, **por la mañana del jueves** o
el viernes 2 después de la clase (10:30).

⚠️ **Y el lunes 5/10 hay corte de luz en Jerónimos de 8 a 14 h** → el primer Seguimiento del
sprint `2026/16` (09:15, en la sala) **no se puede hacer allí**: pasarlo a online o moverlo
→ [[Festivos y no lectivos 26-27]]

## 👥 Reparto por persona

### Alex — 3 abiertas · 8 cerradas · *la quincena más limpia del equipo*
- ✅ Cerró **`GES-246`** (el repaso visual que bloqueaba el resto), **`GES-247`**, **`GES-231`**, **`GES-262`**,
  y las dos de appcron que el 16 estaban vencidas (**`ED-2027`**, **`ED-2034`** Kubernetes/ArgoCD), más `ED-2045` y `ED-2049`.
- En curso **`GES-263`** (suplantación de alumnos por estudio activo, para probar). Por hacer
  **`GES-226`** (*RF-32, bloquear plaza sin certificado de delitos sexuales* — **la P0 que el 16 estaba sin
  dueño**, ya tiene) y `GES-237` (banco histórico de centros privados, P2).
- 💡 **Tiene hueco** para absorber algo del próximo sprint.

### Juanma — 12 abiertas · 12 cerradas
- ✅ **Cerró `CAN-350`** *(Muy Urgente, vencida desde el 20 de marzo)* y la selección de sede examinadora
  (`CAN-369`, `CAN-370`), además de `GES-232`, `GES-234` (periodos de Educación), `GES-253`, `GES-264` y
  varias de RPA/Facturas.
- En curso **`GES-252`** *(Muy Urgente — supervisar el impacto de las pantallas en la arquitectura)* y
  **`GES-233`** (*RF-39, desdoblar plazas*, P0) movida hoy.
- 🟡 **Quietas 11–12 días:** `GES-251` *(supervisar el algoritmo con Paco)*, `ED-2035`/`ED-2036` (Alsa),
  `WD-384`, `FAC-32`, `FAC-38`, y la deuda de Canvas Data (`CAN-337`, `CAN-340` — **vencidas desde nov-2025** —,
  `CAN-348`, `CAN-349`).

### Paco — 30 abiertas · 11 cerradas · *la mitad del sprint abierto está a su nombre*
- ✅ Cerró **`GES-245`** (Fisioterapia, Muy Urgente) y **`GES-221`**, además de `GES-249`, `GES-256`–`GES-261`
  (preparación de Educación y bot de Automation) y `ED-2041` (login Microsoft de MFA).
- En curso: **`GES-230`** (17 especialidades, P0), **`ED-2047`** *(revertir el login de inf.ucam.edu/mfa —
  **vence mañana**)*, y **`GD-683`** *(análisis de Conferenciantes)*.
- 🆕 **Hoy le han entrado siete de Conferenciantes (`GD-683`…`GD-689`), todas con fecha 10/10.**
- 🔴 **Quietas:** las **13 de Investigadores** (`GD-572`…`GD-592`) — cuatro en TESTING y tres en curso,
  **sin tocar desde el 16** —, el **algoritmo de asignación** (`GES-255`, `GES-248`) **11 días**,
  `ED-2038`, **`AP-73`** *(Urgente, venció el 21/09)*, `IN-505` *(vencida desde mayo)* y `DT-306`
  *(LinkedIn de septiembre, vence el miércoles)*.

### Alejandro — 10 abiertas · 2 cerradas
- ✅ **Cerró hoy `ED-2032` y `ED-2033`** — las dos de iText (TFG-TFM y Recos) → [[Licencias iText]]
- 🔴 **Todo lo demás, quieto desde antes del 16:** `EVT-14`…`EVT-18` (RabbitMQ, endpoints, monitorización —
  **vencidas el 1 de agosto**), `ED-2014`/`ED-2015`/`ED-2016` (AppCron, códigos Cientia, titulaciones
  en IMarina — **vencidas 1–4 de agosto**), `ED-2030` *(doble factor, en curso, venció el 12/09)* y
  `ED-2039` (IMarina para Biblioteca).
- 💡 *Tiene sentido: esta quincena ha estado en iText, Cientia/Treelogic, iMarina, Alma y la
  recodificación de duplicados, **nada de lo cual está en el tablero como tarea suya**.* El tablero
  no refleja lo que hace.

### Jesús — 7 abiertas · 5 cerradas
- ✅ Cerró `MIG-44`, `MIG-48`, `MIG-49` (revisión de expedientes, alumnos en estado Abierto) y
  **`ED-2044` (instalación de Alfresco)**.
- En curso **`MIG-50`** (carga de alumnos en `SINC_EXPEDIENTES`) y **`ED-2048`** (servicios de Alfresco).
- 🔴 **`MIG-45` y `MIG-46` siguen sin tocar desde el 16/09** — tercera nota seguida. Y `IN-494`,
  `GESTDOC-11`, `ET-491`, quietas 12 días.

### Pablo — 4 abiertas · 6 cerradas
- ✅ Cerró **las seis de Bajas y Sustituciones** que tenía en TESTING/curso el 16 (`GD-658`, `GD-662`,
  `GD-664`, `GD-668`) más `GD-679` y `GD-680`, el 25/09.
- En curso **`GD-681`** (buscador de profesores para coordinadores), movida hoy.
- Quietas: `GD-87`, `GD-596`, `GD-597` — las tres "paraguas" de Gestión Docente, sin tocar desde el 16.
- 💡 **Es quien más hueco real tiene**, y Gestión Docente es su proyecto.

### Pilar — 8 abiertas · *todas quietas salvo una*
- `ED-2018` *(reorganización de septiembre — 28 días en curso)*, `GES-192` *(arquitectura de prácticas)*,
  `MIG-29` *(vencida desde el 19 de junio)*, las 4 epics de Educación (`GES-222`…`GES-225`), `GES-250` y
  `GES-235` *(RF-41, sello de convenio — movida el 25)*.

### Sin asignar
- ⚠️ **`GES-254`** *(descarga del mapa docente de Prado)* — **EN CURSO sin dueño** desde el 24.
- Las seis genéricas de imputación de **septiembre** (`ED-2019`…`ED-2024`), que vencen el **30/09**.

## 🧊 Quieto desde hace días

> Todas las fechas de "12 días" son **el toque de Jira al arrastrar el sprint el 16/09**: en
> realidad llevan paradas **desde antes**.

| Días | Qué | De quién | Notas seguidas |
|---|---|---|---|
| **16** | 6 de Investigadores (`GD-573`, `GD-576`…`GD-579`, `GD-581`) | Paco | 2ª |
| **≥12** | `EVT-14`…`EVT-18`, `ED-2014`/`2015`/`2016`, `ED-2030` | Alejandro | **3ª** — vencidas desde agosto |
| **≥12** | `CAN-337`, `CAN-340`, `CAN-348`, `CAN-349` | Juanma | **3ª** — nov-2025 / mar-2026 |
| **≥12** | 7 de Investigadores en TESTING/curso (`GD-572`, `574`, `575`, `580`, `586`, `587`, `588`) | Paco | 2ª |
| **≥12** | `IN-505` | Paco | **3ª** — vencida desde mayo |
| **≥12** | `ED-2018`, `GES-192`, `MIG-29` | Pilar | **3ª** |
| **11** | `MIG-45`, `MIG-46` | Jesús | **3ª** |
| **11** | `GES-255`, `GES-248` (algoritmo) + `GES-251` (supervisión) | Paco + Juanma | 2ª — **ruta crítica de Educación** |
| **7** | `AP-73` *(Urgente, vencida el 21/09)* | Paco | — |
| **4** | `GES-254` *(sin dueño)* | — | 2ª |

## ⚖️ Riesgos y equilibrado

- 🔴 **Paco lleva 30 de las 66 abiertas del equipo (45 %)** y **75 de los ~95 puntos estimados** del
  sprint. Es el reparto más desigual del trimestre, y encima **le entran siete tareas nuevas hoy**
  con fecha 10/10. Con el criterio de siempre —*no ponerlo en la ruta crítica y trocear*—, esto no
  cuadra.
- 🔴 **El algoritmo de asignación de Educación está en la ruta crítica** (10/10 parte básica, 25/10
  pruebas, 28/10 apertura a alumnos) **y lleva 11 días quieto**. Depende de Paco con Juanma
  supervisando: **es la dependencia A-espera-a-B de esta semana**.
- 🟡 **Casi nada está estimado fuera de Investigadores:** Alex, Juanma, Jesús y Pablo tienen sus
  tareas abiertas **sin story points**. La velocidad del sprint no se puede medir.
- 🟡 **El tablero de Alejandro no refleja su trabajo real** (iText, Cientia, Alma, iMarina,
  recodificación): 10 abiertas quietas y una quincena llena.
- 🟡 **Capacidad de esta semana:** Pilar pierde el **miércoles entero** (Qualtrics) y el **jueves de 12:30
  a 14:00** (SIGMA). Jesús tiene una **ausencia pendiente de validar** hoy.

### 💡 Propuesta de movimientos (para decidir tú, no se ha tocado Jira)

| Qué | De → a | Por qué |
|---|---|---|
| **Conferenciantes `GD-684`…`GD-689`** (las de desarrollo) | Paco → **Pablo** | Gestión Docente es su proyecto, tiene 4 abiertas y cierra rápido. Paco se queda con `GD-683` (análisis) y `GD-689` (verificación) |
| **Las 13 de Investigadores** | sprint → **backlog / 2026/16 troceado** | María dijo el 10/09 que *"bastaría con que esté listo para finales de año"*: no es de este sprint ni del siguiente entero |
| **Algoritmo (`GES-255`)** | Paco solo → **Juanma lidera, Paco ejecuta** | Es ruta crítica con fecha externa; `GES-251` ya dice "junto con Paco" |
| **`GES-254`** (mapa docente de Prado) | sin dueño → **Alex** o **Juanma** | Se trabajó en la reunión del 24; Alex tiene hueco |
| **`EVT-*`, `ED-2014`…`2016`** | Alejandro → **redatar o backlog** | Vencidas desde agosto y tres notas quietas: o tienen fecha nueva o no son de este sprint |
| **`CAN-337`/`340`/`348`/`349`** | Juanma → **backlog** | Diez meses. O se cierran o salen |

## 📅 Hitos y agenda de la semana

| Día | Qué |
|---|---|
| **mar 29** | `ED-2047` vence (Paco) · 10:00 Reunión responsables (Pilar) |
| **mié 30** | Pilar en **Qualtrics 09:00–14:00** · Tangram 11:00 (delegar en Jesús) · vencen `DT-306` y las **genéricas de septiembre** |
| **jue 1/10** | 🔴 **Cierre del sprint `2026/15`** · 10:45 demo de la aplicación a Educación *(propuesta)* · 12:30 consultoría SIGMA |
| **vie 2/10** | Arranque del `2026/16` → **`/inicio-sprint`**: toca **tanda de octubre** de las genéricas (y cerrar las de septiembre) |
| **lun 5/10** | ⚠️ Corte de luz 8–14 h: el Seguimiento de las 09:15 no puede ser en la sala |

## 📌 Acciones (quién / cuándo)

- [ ] **Pilar** · antes del jueves — decidir los movimientos de la tabla de arriba (sobre todo Paco → Pablo y el algoritmo)
- [ ] **Pilar** · hoy/mañana — decir a **Jesús** en qué sprint caen `MIG-45`/`MIG-46`, y que lleve él Tangram el miércoles
- [ ] **Pilar** · jueves mañana — **cerrar el sprint** y llevar al `2026/16` solo lo que tenga dueño y fecha
- [ ] **Pilar** · jueves/viernes — encadenar [`/inicio-sprint`](../../../) para las genéricas de octubre
- [ ] **Alguien** · ya — ponerse `GES-254` a su nombre
- [ ] **Pilar** · esta semana — cerrar o mover `ED-2018`, `GES-192` y `MIG-29` *(tercera nota seguida)*
- [ ] **Pilar** · antes del 5/10 — pasar el Seguimiento de ese día a online
- [ ] *(Si en la reunión de hoy se decidió algo, apúntalo aquí)*

## 🕓 Para tener en cuenta más adelante

- **Tercera nota seguida con las mismas tareas quietas** (`EVT-*`, `CAN-*`, `MIG-45/46`, `IN-505` y las
  tres de Pilar). Ya no es un despiste: **son tareas que nadie va a hacer en este sprint** y ensucian
  la medición. Vale la pena una limpieza de backlog antes de arrancar el `2026/16`.
- **Sin actas de los Seguimientos del 21 y del 28** (Meet, sin Gemini). Si quieres medir el sprint
  de verdad, **el Seguimiento en Zoom** o activar las notas de Gemini en la invitación.
- **Casi nadie estima**: sin puntos no hay velocidad, y sin velocidad el reparto se hace por número
  de tareas, que es lo que ha llevado a Paco al 45 %.
- El algoritmo de Educación va a necesitar **la respuesta a "PR1+PR2, ¿una plaza o dos?"**, que
  sigue sin contestar → [[2026-09-10 - Prácticas Educación 26-27]]

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Anterior: [[2026-09-16 - Seguimiento Sprint - Dev]] · [[2026-09-08 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[2026-09-10 - Prácticas Educación 26-27]] · [[2026-09-24 - Definición de campos del mapa docente de prácticas]]
- [[Licencias iText]] · [[Festivos y no lectivos 26-27]] · [[Cronograma de proyectos (hasta dic 2026)]] · [[28-09-2026]]
