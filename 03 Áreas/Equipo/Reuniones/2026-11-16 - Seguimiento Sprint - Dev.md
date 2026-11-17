---
tipo: reunión
fecha: 2026-11-16
hora: 09:15–10:45
sprint: Desarrollo 2026/18
sprint_dia: 14 de 14 (día hábil 10 de 10)
sprint_fin: 2026-11-16
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — 16/11, cierre del 2026/18

> ⚠️ **Nota preparada desde Jira a media mañana**, con la reunión ya en marcha. En el calendario se llama **"Revisión de Sprint"**
> (09:15–10:45, Meet + Sala de trabajo TIC; la convocas tú). No hay notas de Gemini ni transcripción: lo que sigue es lo que dice Jira,
> no lo que se habló. Si se decidió algo, va en *Acciones*.
> Comparación con la [[2026-11-02 - Seguimiento Sprint - Dev|nota del 02/11]] (el lunes 09/11 no hubo nota).
> **Cabina sin refrescar**: sigue siendo la del **30/10**. No he pasado `/cabina` hoy para no retrasar la nota; abajo uso la del 30/10
> corregida con lo que dice Jira.

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/18** (id 3109, tablero 3) |
| Fechas | **mar 03/11 → lun 16/11** (cierra hoy a las 18:00) |
| Hoy | día **14 de 14** naturales · día hábil **10 de 10**: **último día** |
| Festivos | ninguno en el sprint *(ver [[Festivos y no lectivos 26-27]])* |
| Tareas en el sprint | **138**: **54 cerradas, 84 abiertas** (incluye 6 genéricas de noviembre, 7 `RDCO` sin dueño, `GES-254` y las 5 epics de Educación) |
| Sprint siguiente | ⚠️ **No hay sprint futuro creado** → `/inicio-sprint` mañana, antes de Responsables (10:00) |

🏁 **Semana de cierre y arranque.** Lo que esté abierto a las 18:00 pasa al `2026/19`, y hoy es el momento de **decidir qué no pasa**.
Las genéricas de noviembre (`ED-2090`…`ED-2095`) valen también para el `2026/19`: el mes no cambia hasta el 01/12.

✅ **La limpieza del 02/11 se hizo:** ya no están en el sprint `MIG-45`/`MIG-46`, `EVT-14`…`18`, `ED-2014`…`2016`, la deuda de Canvas Data
(`CAN-337`…`349`), `WD-384`, `FAC-32` ni `IN-505`. El tablero mide mejor que hace dos semanas.

## 👥 Reparto por persona

### Alejandro — 2 abiertas · 23 cerradas
- ✅ La quincena más productiva del equipo, y **toda registrada en Jira**: desconexiones de Laurea (`CAN-374`, Muy Urgente), réplica de
  Laurea (`ED-2106`, `CAN-377`, `IN-573`), VPN (`CAN-373`), configuración de Cientia con iMarina (`ED-2112`), auditoría de seguridad y
  parcheo de Apache (`ED-2121`, `ED-2120`), revisión de Bitbucket (`ED-2124`), informes de seguridad (`ED-2088`, `ED-2114`) y la
  reactivación de altas en IDM (`EVT-24`).
- Abiertas: `IN-572` *Contextualización de Laurea* (en curso) y `EVT-25` *Carga de datos Pro → Pre* (vence el 18).
- 💡 **Es quien tiene capacidad** para el `2026/19`.

### Pablo — 13 abiertas · 2 cerradas
- ✅ `RDC-103` y `RDC-104` (`RQ-REC-06` y `-07`, Urgentes), los que salían quietos el 26/10.
- 🔴 **`GD-765` *"La app no sincroniza desde el 28 de octubre"*** (Urgente) **sigue en *Por hacer***: es **la segunda nota seguida** y
  ya son **19 días** de Gestión Docente sin sincronizar en producción.
- 🔴 **`ED-2100`, `ED-2101`, `ED-2102`** (*ficheros de datos*: oferta académica, demanda, profesorado), Urgentes, **vencidas el 10/11**,
  sin empezar. El de programación (`ED-2103`) lo cerró Paco el 09/11.
- 🆕 Entran incidencias de Gestión Docente: `GD-767` (plan 178 de Arquitectura), `GD-768` (contrato activo en toda la app), `GD-769`
  (error de profesor en el prevolcado) y `GD-770` (*"la aplicación se queda cargando"*, desde RRHH-Informática).
- 🧊 En curso desde el 29/10 sin cambio de estado: `GD-87`, `GD-748`, `GD-749`, `GD-762`, `GD-763`.

### Jesús — 9 abiertas · 10 cerradas
- ✅ 🟢 **Mis Planillas y Mis Notas están en producción** (`IN-565`, `IN-567`, 13/11), con el módulo de planillas de corrección de
  exámenes (`IN-563`) y sus pruebas (`IN-566`). Es la app de [[Lectura y corrección de planillas]], que en la cabina sigue en rojo.
- ✅ Seguridad: secretos fuera de git y análisis en el CI (`IN-571`), arreglo de vulnerabilidades (`IN-570`). Sede: trámites (`ET-560`),
  alta de usuarios de títulos propios (`ET-561`), revisión de entorno (`ET-562`).
- 🟢 **El Gestor Documental se mueve**: `GESTDOC-13` (estudio inicial), `GESTDOC-15` (BD), `GESTDOC-16` (mantenimiento de trámites) y
  `ED-2116` (actualizar `jav-alfresco`), todo en curso → [[Alfresco - nuevo repositorio]].
- 🧊 `ED-2048` (servicios de Alfresco, en curso desde el 28/09) · `MIG-50` (en TESTING desde el 23/09) · `GESTDOC-11` y `ET-491` en
  *Por hacer* desde febrero y junio · `IN-494`.

### Paco — 16 abiertas · 8 cerradas
- ✅ `WD-426` y `WD-427` (Widgets: error 500 y CI/CD con Argo), `GES-281` (volcado a Laurea de la oferta de Educación), `ED-2103`
  (fichero de programación), arreglos de seguridad en `jav-personas` y `jav-misalumnos` (`ED-2105`, `ED-2072`), y `ED-2115`.
- 🟠 **Mi Docencia** (`AS-582`…`AS-590`): **7 en TESTING** y 2 en curso. Cuatro llevan en TESTING desde el **19/10** (`AS-582`…`585`).
  Se movieron el 13/11, así que ya no están quietas, pero hay que **sacarlas de TESTING**: alguien tiene que probarlas.
- 🔴 🆕 **`AS-595` *Error 503 al pasar lista en PROD*** (por las tablas de auditoría) y `AS-594` *Subida a PROD de Mi Calendario y Mis
  Asignaturas*, las dos para el **vie 20**.
- En curso: `WD-428` (Widgets a Spring Boot 4.1.2), `GES-289` (sincronizar asignaciones de gestorpracticas, **vencida el 11/11**).
  En TESTING: `GES-290`, `ED-2110` (la skill de limpiar secretos del historial).
- ❓ **`GES-255` (algoritmo de asignación) sigue en *Por hacer*** desde el 16/09: **tercera nota**, y la asignación de Educación se
  ejecutó el 30/10.

### Juanma — 13 abiertas · 0 cerradas
- ⚠️ **Ninguna tarea cerrada ni movida de estado en el sprint.** De sus 13 abiertas, 12 están en *Por hacer* y `GES-239` está en TESTING
  desde el 26/10. O ha trabajado en algo que no está en Jira, o algo le ha bloqueado: **hay que preguntarlo**.
- 🆕 Hoy le entran **seis tareas nuevas**: tres de refuerzo de seguridad (limpiar el historial y las credenciales en Learning Agreement y
  asignación-sede: `ED-2127`, `ED-2128`, `ED-2129`), el rediseño de Learning Agreement (`LA-57`), la asignación de tutor académico
  (`GES-291`) y la pérdida de facturas por SOAP (`FAC-41`).
- Siguen las del 02/11: `GES-286`, `GES-287`, `GES-288`, `TOOL-42`, `CAN-371`.
- ❓ **`GES-233`** (RF-39, P0) en *Por hacer* desde el 10/09: **tercera nota**.

### Alex — 6 abiertas · 0 cerradas
- ⚠️ **Nada se ha movido en dos semanas**: las seis tienen el último cambio el **02/11** o antes. ¿Ha estado fuera?
- En curso: `RDCO-189` (seguridad r2 de Reconocimientos) y `GES-285` (Excel de asignaciones), **las dos vencidas el 06/11**.
- En TESTING: `RDC-105` (`RQ-REC-14`), `LA-56` (seguridad r2 de Learning Agreement, vencida el 30/10) y **`TM-107`** (secretos en el
  historial de Talleres, **vencida el 22/10 y en TESTING desde el 23/10**: **tercera nota**).
- ❓ `GES-229` (RF-35, P0) en *Por hacer* desde el 10/09: **tercera nota**.

### Pilar — 11 abiertas · 11 cerradas
- ✅ Las reuniones del sprint, imputadas y cerradas (Sigma, Gestor Documental, Aplicativo docente, Biblioteca, Pau, Nivaldo, repositorio
  de código DTIC).
- Abiertas: `ED-2109` Bitbucket (**vence hoy**), `ED-2117` (migración de las apps de Kubernetes al servicio de seguridad nuevo, para
  comentarla hoy), `ED-2099` (vencida 11/11), `CAN-372` (vencida 06/11), `RDC-107` (en curso, vencida 06/11) y `ED-2118` (nueva).
- 🧊 **Las epics de Educación (`GES-222`…`225`, `GES-250`) siguen abiertas**: segunda nota. El lanzamiento fue el 28/10.

### Sin asignar
- 🔴 **`RDCO-182`…`RDCO-188`**: las 7 `rq-rec` de Reconocimientos (**4 Urgentes**), **31 días sin dueño**, **tercera nota**. Siguen
  siendo **la causa del rojo** de [[Reconocimientos]].
- ⚠️ **`GES-254`** (descarga del mapa docente de Prado): **en curso sin dueño desde el 22/09, sexta nota**.
- Genéricas de noviembre (`ED-2090`…`ED-2095`): sin dueño, como siempre; valen hasta el 30/11.

## 🧊 Quieto desde hace días

> Medido con el **último cambio de estado** (`cambio_estado`), no con `updated`: el arrastre al sprint del 02/11 marcó muchas como
> tocadas.

| Días | Qué | De quién | Notas seguidas |
|---|---|---|---|
| **55** | `GES-254` *(en curso, sin dueño)* | — | **6ª** |
| **≥60** | `GES-229`, `GES-233`, `GES-255` (P0 de Educación) | Alex · Juanma · Paco | **3ª**: Educación salió hace tres semanas |
| **54** | `MIG-50` *(en TESTING)* | Jesús | 2ª |
| **49** | `ED-2048` (servicios de Alfresco) | Jesús | **3ª** |
| **≥150** | `GESTDOC-11`, `ET-491` | Jesús | **3ª** |
| **31** | `RDCO-182`…`188` *(sin dueño, 4 Urgentes)* | — | **3ª** |
| **24** | `TM-107` *(en TESTING, vencida el 22/10)* | Alex | **3ª**: secretos en el historial |
| **21** | `GES-239` *(en TESTING)* | Juanma | 2ª |
| **18** | `GD-87`, `GD-748`, `GD-749`, `GD-762`, `GD-763` | Pablo | 1ª |
| **16** | **`GD-765`** *(Urgente, por hacer: producción sin sincronizar)* | Pablo | **2ª** |
| **14** | Las seis de Alex (`RDCO-189`, `GES-285`, `RDC-105`, `LA-56`…) | Alex | 1ª |
| **11** | `ED-2100`, `ED-2101`, `ED-2102` *(Urgentes, vencidas el 10/11)* | Pablo | 1ª |
| **14** | Epics `GES-222`…`225`, `GES-250` | Pilar | 2ª |

**Atascos de varias semanas** (tres notas o más): `GES-254`, las P0 de Educación, los `RDCO`, `TM-107` y lo viejo de Jesús (`ED-2048`,
`GESTDOC-11`, `ET-491`). Ya no son despistes: **o tienen dueño y fecha en el `2026/19`, o salen al backlog**.

## 🚦 Proyectos en rojo y ámbar (cabina del 30/10, corregida con Jira)

- 🔴 [[Reconocimientos]] *(desde el 30/10)*: los `RDCO` siguen sin dueño. En el acta del 08/10 quedó que **hasta mediados de noviembre
  no había hueco**, y ya estamos ahí → [[2026-10-08 - Mejoras de la app de Reconocimientos]]
- 🔴➡️🟢? [[Lectura y corrección de planillas]] *(desde el 26/10)*: **Mis Planillas está en producción desde el 13/11** (`IN-565`). El rojo
  ya no se sostiene: **mueve la fecha o ciérralo** al pasar `/cabina`. Queda abierto el modelo de roles (responsable vs. docente)
- 🔴 [[Alfresco - nuevo repositorio]] *(desde el 26/10)*: **se ha movido**, Jesús tiene en curso el estudio, la BD y el mantenimiento de
  trámites (`GESTDOC-13`, `-15`, `-16`). `ED-2048` sigue quieto
- 🔴 [[Cierre de Infucam]] *(desde el 26/10)*: depende del Alfresco
- 🔴 [[Remediación Protocolo]] *(desde el 26/10)*: sin tareas en este sprint

## ⚖️ Riesgos y equilibrado

| Persona | Abiertas | Cerradas en el sprint |
|---|---|---|
| Paco | 16 | 8 |
| Pablo | 13 | 2 |
| Juanma | 13 | 0 |
| Jesús | 9 | 10 |
| Alex | 6 | 0 |
| Alejandro | 2 | 23 |

- 🔴 **Dos incidencias de producción**: `GD-765` (Gestión Docente sin sincronizar desde el 28/10, **19 días**) y `AS-595` (error 503 al
  pasar lista). Las dos van primero en el `2026/19`.
- 🔴 **Pablo no da abasto**: 13 abiertas con `GD-765` y tres ficheros de datos Urgentes vencidos. Los ficheros son trabajo de datos y BD:
  encajan con **Alejandro**, que tiene capacidad. Así Pablo queda libre para `GD-765` y las incidencias nuevas de Gestión Docente.
- 🟠 **Juanma y Alex, cero cerrado** en el sprint, y son los dos que tienen que coger Reconocimientos. Antes de repartir, **saber por
  qué**: ausencia, trabajo fuera de Jira o bloqueo.
- 🟠 **Paco acumula TESTING**: 9 tareas a la espera de prueba. Cerrar Mi Docencia (`AS-582`…`590`) y subirla a PRO (`AS-594`) libera
  más que darle nada nuevo.
- 🟡 **Seguridad repetitiva a Juanma**: las tres de limpieza de secretos (`ED-2127`…`2129`) son el mismo trabajo tres veces, y Paco ya
  escribió la skill para hacerlo (`ED-2110`). Se pueden pasar a quien use la skill en cuanto salga de TESTING.
- 🟡 **Nadie estima**: sin puntos, el reparto se sigue midiendo por número de tareas.

### 💡 Propuesta de movimientos para el `2026/19` (para decidir tú; no se ha tocado Jira)

| Qué | De → a | Por qué |
|---|---|---|
| **`GD-765`** (no sincroniza) | Pablo, **primera del sprint** | Producción caída desde el 28/10; segunda nota sin empezar |
| **`ED-2100`, `ED-2101`, `ED-2102`** (ficheros de datos) | Pablo → **Alejandro** | Datos y BD; Alejandro tiene capacidad y Pablo tiene producción |
| **`AS-595`** (503 al pasar lista) | Paco, con apoyo de Alejandro si hace falta | Producción; vence el vie 20 |
| **`RDCO-182`…`188`** | sin dueño → **Alex**, con Juanma de mentor | Causa del rojo de Reconocimientos; Alex ya está en la app (`RDC-105`, `RDCO-189`). **Solo si se aclara por qué no se ha movido nada** |
| **`ED-2127`…`2129`** (limpieza de secretos) | Juanma → quien aplique la skill de `ED-2110` | Trabajo repetido; ya hay herramienta |
| **`GES-229`, `GES-233`, `GES-255`** | → **cerrar** o deuda con nombre | Tercera nota; Educación asignó el 30/10 |
| **Epics `GES-222`…`225`, `GES-250`** | → **cerrar** (tú) | Lanzamiento hecho |
| **`GES-254`** | sin dueño → **Juanma** o **cerrar** | Sexta nota en curso sin dueño |
| **`GESTDOC-11`, `ET-491`, `MIG-50`** | → backlog o cerrar | Quietas desde hace meses; el Gestor Documental ya avanza por `GESTDOC-13`…`16` |
| **`TM-107`, `LA-56`** | Alex → sacarlas de TESTING esta semana | Seguridad, vencidas |

## 📅 Hitos y agenda de la semana

| Día | Qué |
|---|---|
| **lun 16** | 🏁 **Cierre del `2026/18` a las 18:00** · 🎓 Clase IR 11:00–12:30 (coincide con la Eucaristía del 30 aniversario) · vence `ED-2109` |
| **mar 17** | 🚀 **Arranque del `2026/19`** → `/inicio-sprint` · **Responsables 10:00–11:30** (Zoom) · 🔬 CV iMarina 12:00 (Luis, con Scimarina) · 🎓 entrega de prácticas / parcial |
| **mié 18** | Tangram 11:00 · 🎓 online 16:00 · vence `EVT-25` |
| **jue 19** | 🩺 Pilar fuera 12:00–14:00 |
| **vie 20** | 🎓 Clase 08:30 · 🔬 **iMarina: fin de la fase 3** · Sigma, seguimiento 12:00 (Teams; **pisa tu Hi-Tech**) · vencen **`AS-594` y `AS-595`** |

## 📌 Acciones (quién / cuándo)

- [ ] **Pilar** · hoy, antes de las 18:00 — decidir qué pasa al `2026/19` y qué va al backlog (tabla de propuesta)
- [ ] **Pilar** · mañana antes de las 10:00 — `/inicio-sprint` (no hay sprint futuro creado) y asignar **`RDCO-182`…`188`**
- [ ] **Pablo** · ya — `GD-765` (Gestión Docente no sincroniza desde el 28/10)
- [ ] **Paco** · antes del vie 20 — `AS-595` (503 en PRO) y `AS-594` (subida de Mi Calendario y Mis Asignaturas)
- [ ] **Juanma y Alex** · hoy — contar qué ha pasado con sus tareas este sprint
- [ ] **Paco / Alex / Juanma** · hoy — cerrar o explicar `GES-255`, `GES-229` y `GES-233` *(tercera vez que se apunta)*
- [ ] **Pilar** · esta semana — cerrar las epics de Educación y pasar `/cabina` (Planillas ya en producción)
- [ ] **Equipo** · hoy — `ED-2117`: inventario de apps de Kubernetes, orden y quién lleva cada una · `ED-2109`: quién cambia `known_hosts` y pipelines
- [ ] **Alguien** · ya — `GES-254` a su nombre o cerrarla *(sexta vez que se apunta)*
- [ ] *(Si en la reunión de hoy se decidió algo, apúntalo aquí)*

## 🕓 Para tener en cuenta más adelante

- **Seis Seguimientos sin acta.** La de hoy es en Meet: **activa Gemini** en la invitación de la serie, o pásala a **Zoom**, que es lo
  que el conector puede leer.
- **La hora del lunes, confirmada:** la reunión es **09:15–10:45** (ahora titulada *Revisión de Sprint*). El daily de los lunes corre a las
  09:00 y esta skill sigue diciendo 09:45–11:15. Si quieres leerlo antes de entrar, **el daily debería ir a las 08:45** y conviene corregir
  la hora en esta skill.
- **Alejandro registra ya todo en Jira** (23 cerradas). Es la primera quincena en que su carga se ve de verdad, y muestra **capacidad libre**.
- **Tras Reconocimientos viene Medicina** (acta del 08/10), con la reunión con la titulación aún sin convocar. El `2026/19` es el sprint de
  Reconocimientos; Medicina, como pronto, el `2026/20`.

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Anterior: [[2026-11-02 - Seguimiento Sprint - Dev]] · [[2026-10-26 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[Reconocimientos]] · [[2026-10-08 - Mejoras de la app de Reconocimientos]] · [[Lectura y corrección de planillas]]
- [[Alfresco - nuevo repositorio]] · [[Cabina - Cartera]] · [[Festivos y no lectivos 26-27]] · [[16-11-2026]]
