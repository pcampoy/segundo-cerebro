---
tipo: reunión
fecha: 2026-11-23
hora: 09:15–10:45
sprint: Desarrollo 2026/19
sprint_dia: 7 de 14 (día hábil 5 de 10)
sprint_fin: 2026-11-30
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — 23/11, mitad del 2026/19

> ⚠️ **Nota hecha a posteriori, a las 14:00**, con la *Revisión de Sprint* (09:15–10:45, Meet + Sala de trabajo TIC) ya celebrada. Sin notas
> de Gemini ni transcripción: **esto es lo que dice Jira, no lo que se habló**. Si se decidió algo, apúntalo en *Acciones*.
> Comparación con la [[2026-11-16 - Seguimiento Sprint - Dev|nota del 16/11]]. **Cabina sin refrescar** (sigue la del 30/10): no he pasado
> `/cabina` para no alargar esto; abajo uso la del 30/10 corregida con Jira.

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/19** (id 3143, tablero 3) |
| Fechas | **mar 17/11 → lun 30/11** (cierra a las 18:00) |
| Hoy | día **7 de 14** naturales · día hábil **5 de 10** → quedan **5 hábiles** (24, 25, 26, 27 y 30) |
| Festivos | ninguno en el sprint *(ver [[Festivos y no lectivos 26-27]])*. ⚠️ El **puente del 7–8/12** no está en la nota y caería en el `2026/20` |
| Tareas en el sprint | **121**: **56 cerradas, 65 abiertas** (incluye 6 genéricas de noviembre, 7 `RDCO` sin dueño, `GES-254` y las 5 epics de Educación) |

🏃 **Semana de ejecución.** El **lunes 30 es el cierre** (y el seguimiento de ese día será el de cierre) → `/inicio-sprint` el 30 o el 1/12.
Las genéricas de noviembre (`ED-2090`…`2095`) acaban con el mes: **el `2026/20` necesita las de diciembre**.

## 👥 Reparto por persona

### Alejandro — 8 abiertas · 12 cerradas
- ✅ Imágenes Docker Java 21 y 25 por el CVE (`ED-2138`) — **cierra el punto del JDK 21** del panel · mitigación del `CVE-2026-59273` (`ED-2158`) ·
  informes de seguridad de `jav-alfresco`, `jav-misplanillas` y `jav-misnotas` (`ED-2148`) · servidor de Infucam actualizado (`ED-2147`) ·
  carga Pro → Pre (`EVT-25`) · reunión con iMarina (`ED-2135`).
- 🆕 Abre línea de **IDM / LDAP / eventos**: carga de datos de IDM (`ED-2146`, en curso), atributos (`EVT-26`, `ED-2136`), cruce de personas
  Elasticsearch–LDAP (`ED-2150`), integración de `replicalaurea` con Alexia (`ED-2137`), y **eventos a Spring Boot 4.1.3** (`ED-2155`, `ED-2156`).
- 🧊 `IN-572` *Contextualización de Laurea*, en curso desde el 16/11 y **vencida el 17/11**.
- 🆕 Fuera de Jira todavía: **el stock del Preclínico Odontológico** (Miguel Ángel, hoy) — *"5 minutos para ver los detalles"*.

### Pablo — 3 abiertas · 17 cerradas
- ✅ 🟢 **`GD-765` resuelta** (19/11): Gestión Docente vuelve a sincronizar tras **22 días**. Y con ella una tanda de incidencias de GD
  (`GD-762`…`776`), las mejoras de Reconocimientos previos (`GD-748`, `GD-749`) y **los tres ficheros de datos Urgentes** (`ED-2100`…`2102`).
  La quincena de Pablo, de un tirón.
- Abiertas: `GD-777` (grupos en el Doctorado de Ciencias…), `GD-774` (planes de la Escuela de Doctorado) y `GD-87` (paraguas, en curso desde el 29/10).
- ❓ **Docentia** es suya y está en la lista de Spring Security de Alejandro: **no hay tarea**.

### Jesús — 12 abiertas · 5 cerradas
- ✅ Mis Notas y Mis Planillas: correcciones, rendimiento, impresión y estadísticas (`IN-575`…`577`) · `jav-alfresco` con los documentos de
  trámites de la sede (`IN-574`) · reunión con el SOIL (`GES-292`).
- 🟢 **Spring Boot 4.1.3** en Mis Planillas, Mis Notas, `jav-documentos` y `jav-alfresco` (`IN-580`, en curso desde hoy).
- En curso: importar notas desde Canvas (`IN-578`), hojas de solución en exámenes escaneados (`IN-579`, **vencida el 20/11**), y el Gestor
  Documental (`GESTDOC-13`, `-15`, `-16`, quietos desde el 3–4/11).
- 🧊 Lo viejo, **cuarta nota**: `ED-2048` (en TESTING desde el 28/09), `MIG-50` (TESTING desde el 23/09), `GESTDOC-11` (feb.) y `ET-491` (jun.).

### Paco — 11 abiertas · 12 cerradas
- ✅ 🟢 **`AS-595` (503 al pasar lista en PRO) resuelta** el 20/11. Mi Docencia: mejoras tras la subida (`AS-596`, `AS-597`), planificación y
  suplantación (`AS-587`), comprobación de alumno-profesor (`AS-591`). Seguridad en `jav-estudio`, `jav-asistencia` y `jav-cursos-academicos`
  (`ED-2139`…`2141`), JDK de Oracle → Corretto (`ED-2142`), Widgets a Spring Boot 4.1.2 (`WD-428`) y la skill de secretos (`ED-2110`).
- ✅ **`GES-255` (algoritmo de asignación) cerrada** el 18/11, a la tercera nota.
- ⚠️ **`AS-594` *Subida a PROD de Mi Calendario y Mis Asignaturas*** sigue en curso desde el 16/11 y **venció el 20/11**.
- En curso, 7 a la vez: Widgets (`WD-429`, `-430`, `-431`) y Mi Docencia (`AS-589`, `-598`, `-601`, `-602`). Nuevas: `AS-599`, `AS-600` y
  seguridad en `jav-widgets` (`ED-2145`, vence el 27).
- ❓ Widgets quedó en **Spring Boot 4.1.2**: ¿le afecta el aviso de Spring Security? No está en la lista de Alejandro; preguntarlo.

### Juanma — 1 abierta en el sprint · 5 cerradas esta semana (13 en 7 días)
- ✅ **El "cero cerrado" del 16/11 era un desfase de registro**: ese mismo día por la tarde cerró `GES-286`…`288`, `CAN-371`, `GES-291`,
  `ED-2127` y `TOOL-42`. Esta semana: carga asistida de oferta privada de Educación (`GES-295`), sedes examinadoras (`CAN-379`), app de acceso
  a Spring Boot 4.2 y Java 21 (`CAN-380`) y **análisis del alta de estudios previos en Reconocimientos** (`RDCO-190`, `RDC-108`).
- ❓ En el sprint solo le queda **`GES-233`** (RF-39, P0), en *Por hacer* desde el 10/09: **cuarta nota**.
- 💡 **Tiene hueco en el sprint.** Fuera del sprint arrastra **5 JSM en curso** (`TICAM-14135` Urgente, `TICAM-15607` Muy Urgente, `TICAM-13852`,
  `TICAM-14296`, `TICAM-6180`) y deuda vieja de Canvas Data.

### Alex — 6 abiertas · 4 cerradas
- ✅ **Se ha movido**: `TM-107` (secretos de Talleres, a la cuarta nota), `GES-285` (Excel de asignaciones), credenciales de prácticas a un
  Secret de Kubernetes (`GES-293`) y **prácticas a Spring Boot 4.1.3** (`GES-294`).
- En TESTING desde el 02/11 (**21 días**): `RDCO-189`, `LA-56` (seguridad r2) y `RDC-105`. Tocadas hoy, pero siguen sin salir.
- 🆕 `ED-2143` (`appcron`: parches y Spring Boot 4) y `ED-2144` (`personasucam`: hallazgo app002), las dos para el **vie 27**.
- ❓ `GES-229` (RF-35, P0) en *Por hacer* desde el 10/09: **cuarta nota**.

### Pilar — 9 abiertas · 1 cerrada
- ✅ `RDC-107` (estrategia de la base 44 de previos).
- Abiertas: `ED-2109` Bitbucket (TESTING, vencida el 16) · `ED-2117` Kubernetes al servicio de seguridad nuevo · `ED-2099` (vencida el 11) ·
  `ALFR-1` · y las **epics de Educación** `GES-222`…`225` y `GES-250`, **tercera nota**.

### Sin asignar
- 🔴 **`RDCO-182`…`RDCO-188`**: 7 `rq-rec` de Reconocimientos (**4 Urgentes**), **38 días sin dueño, cuarta nota**. Siguen siendo la causa del
  rojo de [[Reconocimientos]]. Juanma ya ha hecho el análisis del flujo (`RDCO-190`): **es el momento de repartirlas**.
- ⚠️ **`GES-254`** (mapa docente de Prado): **en curso sin dueño desde el 22/09, séptima nota**.

## 🧊 Quieto desde hace días

> Medido con `cambio_estado` (último cambio de categoría): el arrastre al `2026/19` del 18/11 marcó todo como tocado.

| Días | Qué | De quién | Notas seguidas |
|---|---|---|---|
| **≥150** | `GESTDOC-11`, `ET-491` | Jesús | **4ª** |
| **74** | `GES-229`, `GES-233` *(P0 de Educación)* | Alex · Juanma | **4ª** |
| **74** | Epics `GES-222`…`225`, `GES-250` | Pilar | **3ª** |
| **62** | `GES-254` *(en curso, sin dueño)* | — | **7ª** |
| **61** | `MIG-50` *(TESTING)* | Jesús | **3ª** |
| **56** | `ED-2048` *(TESTING)* | Jesús | **4ª** |
| **38** | `RDCO-182`…`188` *(sin dueño, 4 Urgentes)* | — | **4ª** |
| **25** | `GD-87`, `IN-494` | Pablo · Jesús | 2ª |
| **21** | `RDCO-189`, `LA-56`, `RDC-105` *(TESTING)* | Alex | 2ª |
| **19–20** | `GESTDOC-13`, `-15`, `-16` *(en curso)* | Jesús | 1ª |
| **11** | `ED-2116` *(TESTING)* | Jesús | 1ª |
| **7** | `AS-594` *(subida a PROD, vencida el 20/11)* · `IN-572` *(vencida el 17/11)* | Paco · Alejandro | 1ª |

**Atascos de varias semanas**: los de siempre — `GES-254`, las P0 `GES-229`/`233`, los `RDCO`, lo viejo de Jesús y las epics. La propuesta del
16/11 (*"o tienen dueño y fecha en el `2026/19`, o salen al backlog"*) **no se ha aplicado**: siguen todos en el sprint.

## 🔐 Seguridad: Spring Security 4.1.3 (aviso de INCIBE, 20/11)

Alejandro listó las apps con `@PreAuthorize` que **tienen que** subir a la 4.1.3. Cómo está cada una:

| App | Tarea | Estado |
|---|---|---|
| Mis Notas · Mis Planillas | `IN-580` (Jesús) | 🟡 en curso |
| Prácticas | `GES-294` (Alex) | ✅ hecha |
| **Mis Alumnos** | — | 🔴 **sin tarea** |
| **Docentia** | — | 🔴 **sin tarea** |
| *(además)* eventos | `ED-2155` (Alejandro) | ⚪ por hacer |
| *(¿?)* Widgets | `WD-428` lo dejó en **4.1.2** | ❓ preguntar si le afecta |

## 🚦 Proyectos en rojo y ámbar (cabina del 30/10, corregida con Jira)

- 🔴 [[Reconocimientos]]: los `RDCO` siguen sin dueño, pero Juanma ya ha analizado el flujo y el alta de estudios previos (`RDCO-190`).
- 🔴➡️🟢? [[Lectura y corrección de planillas]]: en producción desde el 13/11 y con mejoras esta semana (`IN-575`…`577`). **El rojo no se sostiene**.
- 🔴 [[Alfresco - nuevo repositorio]]: `jav-alfresco` avanza (`IN-574`, `IN-580`), pero el Gestor Documental (`GESTDOC-13`…`16`) lleva 20 días quieto.
- 🔴 [[Cierre de Infucam]]: depende del Alfresco. Alejandro ha actualizado el servidor de Infucam (`ED-2147`).
- 🔴 [[Remediación Protocolo]]: sin tareas en este sprint.

## ⚖️ Riesgos y equilibrado

| Persona | Abiertas | Cerradas en el sprint |
|---|---|---|
| Jesús | 12 | 5 |
| Paco | 11 | 12 |
| Alejandro | 8 | 12 |
| Alex | 6 | 4 |
| Pablo | 3 | 17 |
| Juanma | 1 | 5 *(+8 el 16/11)* |

- 🟢 **Las dos incidencias de producción del 16/11 están resueltas** (`GD-765` y `AS-595`).
- 🔴 **Dos apps sin tarea de Spring Security** (Mis Alumnos y Docentia), con un aviso de INCIBE de por medio.
- 🟠 **Paco tiene 7 en curso a la vez** y la subida a PROD (`AS-594`) vencida. Mejor cerrar la subida antes de abrir más frentes.
- 🟠 **Jesús acumula 12**, con tres TESTING de hace meses que inflan la cuenta.
- 🟢 **Pablo y Juanma tienen hueco**: Pablo con 3 abiertas tras vaciar su cola; Juanma con 1 en el sprint.
- 🟡 **Trabajo que entra sin pasar por el sprint**: el stock de Odontología (Alejandro) y Academicship (Tomás, reunión hoy a las 16:00).
- 🟡 **Nadie estima**: el reparto se sigue midiendo por número de tareas.

### 💡 Propuesta de movimientos (para decidir tú; no se ha tocado Jira)

| Qué | De → a | Por qué |
|---|---|---|
| **Spring Security 4.1.3 en Mis Alumnos** | nueva → **Paco** | Ya tocó `jav-misalumnos` (`AS-591`) y hizo las de `jav-estudio`/`asistencia` |
| **Spring Security 4.1.3 en Docentia** | nueva → **Pablo** | Es su proyecto y tiene hueco |
| **`RDCO-182`…`188`** | sin dueño → **Juanma + Alex** | Juanma acaba de analizar el flujo (`RDCO-190`) y tiene hueco; Alex ya está en la app. Las 4 Urgentes primero |
| **`AS-594`** (subida a PROD) | Paco, **primera** | Vencida; desbloquea Mi Docencia |
| **`GES-229`, `GES-233`** | → **cerrar** o deuda con nombre | Cuarta nota |
| **Epics `GES-222`…`225`, `GES-250`** | → **cerrar** (tú) | Tercera nota; Educación lanzada el 28/10 |
| **`GES-254`** | sin dueño → **cerrar** o Juanma | Séptima nota |
| **`GESTDOC-11`, `ET-491`, `MIG-50`, `ED-2048`** | → backlog o cerrar (Jesús) | Cuarta nota; el Gestor Documental avanza por otras tareas |
| **Stock de Odontología** | nueva → **Alejandro**, con proyecto y sprint | Ya se ha decidido fuera; que se vea en el tablero |

## 📅 Hitos y agenda de la semana

| Día | Qué |
|---|---|
| **lun 23** | ~~Revisión de Sprint~~ · ~~Clase 11:00~~ · Darwined 13:00 · 🛰️ **Academicship 16:00** (Tomás) |
| **mar 24** | **Responsables 10:00–11:30** (Zoom) · 🩺 Medicina *posible desde las 12:00* |
| **mié 25** | Tangram 11:00 · Claustro extraordinario GII 12:30 · 🎓 online 16:00 |
| **jue 26** | 🔐 caduca el `BITBUCKET_TOKEN` de `iswteam/jav-widgets` · vence `AS-600` |
| **vie 27** | 🎓 Clase 08:30 · vencen `ED-2143`, `ED-2144`, `ED-2145`, `AS-602`, `WD-431` |
| **lun 30** | 🏁 **Cierre del `2026/19`** · cierre de imputación de noviembre |
| **mar 1/12** | 🚋 **BONO CAMPUS** sin recarga · 🧩 **licencias Atlassian** sin modalidad mensual |

## 📌 Acciones (quién / cuándo)

- [ ] **Pilar** · hoy o mañana — crear las tareas de **Spring Security 4.1.3** de **Mis Alumnos** y **Docentia** (proyecto, persona y sprint)
- [ ] **Pilar** · esta semana — asignar **`RDCO-182`…`188`** *(cuarta nota)*
- [ ] **Pilar** · antes del 1/12 — tarea para quitar el **BONO CAMPUS** de las peticiones online *(en Jira no hay ninguna)*
- [ ] **Paco** · ya — cerrar `AS-594` (subida a PROD de Mi Calendario y Mis Asignaturas)
- [ ] **Alejandro** · esta semana — ¿le afecta a Widgets (4.1.2) el aviso? · pasar a Jira el **stock de Odontología**
- [ ] **Equipo** · esta semana — quién prueba la **SQL de Eloi** contra `SINC_EXPEDIENTES` *(arrastrado desde el 18/11)*
- [ ] **Alex** · esta semana — sacar de TESTING `RDCO-189`, `LA-56` y `RDC-105`
- [ ] **Jesús** · esta semana — decidir qué hacer con `ED-2048`, `MIG-50`, `GESTDOC-11` y `ET-491`
- [ ] **Pilar** · antes del 30 — `/inicio-sprint` y genéricas de **diciembre**
- [ ] *(Si en la reunión de hoy se decidió algo, apúntalo aquí)*

## 🕓 Para tener en cuenta más adelante

- **Siete Seguimientos sin acta.** Gemini en la invitación de la serie, o pasarla a Zoom.
- **La hora del daily de los lunes**: hoy corrió a las 13:44, después de la reunión. Para que llegue antes de las 09:15, `daily-pilar-lunes`
  debería ir a las **08:45**, y esta skill dice todavía 09:45–11:15.
- **El `2026/20` empieza con el puente del 7–8/12** (sin confirmar) y con **Medicina** como candidata: si se convoca esta semana, encaja.
- **Las apps que llegan de fuera** (Academicship, stock de Odontología): mientras no pasen por Responsables, entran al equipo sin sprint.

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Anterior: [[2026-11-16 - Seguimiento Sprint - Dev]] · [[2026-11-02 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[Reconocimientos]] · [[Lectura y corrección de planillas]] · [[Alfresco - nuevo repositorio]] · [[Cierre de Infucam]]
- [[Cabina - Cartera]] · [[Festivos y no lectivos 26-27]] · [[23-11-2026]]
