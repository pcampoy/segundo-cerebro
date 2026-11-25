---
tipo: seguimiento
sprint: Desarrollo 2026/19
tags: [sprint, equipo, vigía]
---
# Vigía — Desarrollo 2026/19

Bitácora del agente [[vigia-sprint]]: lo que ha visto en cada pasada y de qué hilos ha tirado.
Sprint `2026/19` (id 3143): **mar 17/11 → lun 30/11**, sin festivos. Nota de referencia: [[2026-11-16 - Seguimiento Sprint - Dev]].
Anterior: [[Vigía - Desarrollo 2026-18]].

## 2026-11-20 · 12:10 — viernes, día hábil 4 de 10

**Situación:** 96 tareas en el sprint (6 son genéricas). **34 cerradas de 90, un 38 %**, con 6 días hábiles por delante. El ritmo es bueno,
pero lo cerrado es casi todo trabajo que ha entrado esta semana (Gestión Docente, Mi Docencia, seguridad).

**🔴 Actúa ya**
- **`RDCO-182`…`188` (Reconocimientos, 4 Urgentes): siguen sin dueño, 35 días, cuarta nota.** La acción del lunes ("asignarlas en
  `/inicio-sprint`") **no se hizo**, y este era *el sprint de Reconocimientos*. En el correo no hay nada sobre ellas (solo la
  configuración de la app de Recos para los planes nuevos, 16/11): nadie las pide ni las persigue. Si no tienen dueño el lunes 23, el
  sprint cierra el 30 sin tocarlas y el rojo del proyecto pasa a diciembre.
  → Palanca: **Revisión de Sprint del lun 23 a las 09:15**. Juanma tiene **una sola tarea** en el sprint (`GES-233`), así que hay hueco.

**🟠 Vigila**
- **Juanma: una sola tarea en el sprint** (`GES-233`, quieta desde el 10/09). O no tiene trabajo asignado o vuelve a trabajar sin
  registrarlo (el 16/11 cerró 12 tareas de golpe).
- **Alex: 18 días sin un cambio de estado** (antes eran 14, así que ha empeorado). `TM-107` lleva en TESTING desde el 23/10 (cuarta nota) y `LA-56`, `RDCO-189` y
  `GES-285` están vencidas. No consta por qué; la pista sigue siendo el soporte a prácticas de Educación, que no está en Jira.
- **Acciones del lunes sin hacer:** `GES-229` y `GES-233` siguen abiertas, las epics de Educación (`GES-222`…`225` y `GES-250`) también,
  y `GES-254` sigue en curso sin dueño (séptima nota). `GES-255` sí está cerrada (18/11).
- **Trabajo registrado de golpe:** Pablo cerró **18 tareas el jueves 19** (entre ellas `GD-765` y los ficheros `ED-2100`…`2102`) sin
  movimientos previos. Es buena noticia, pero hasta ese día el tablero no lo reflejaba.

**⚪ Ruido**
- ✅ `GD-765` (Gestión Docente sin sincronizar) **cerrada el 19/11**. ✅ `AS-595` (503 al pasar lista) cerrada.
- `AS-594` (subida a PROD de Mi Calendario y Mis Asignaturas) vence hoy y está en curso, pero `AS-596` (*mejoras tras la subida a PROD*)
  está cerrada desde el 18: lo más probable es que la subida esté hecha y solo falte cerrar la tarea.
- Alejandro tiene `IN-572` y `EVT-25` vencidas (17 y 18/11) y en curso, más 6 nuevas por hacer. Hueco libre ya no le queda mucho.
- Jesús: `MIG-50` y `ED-2048` siguen en TESTING desde septiembre; los `GESTDOC` avanzan. Cerró 4 hoy.
- Tuyas: `ED-2099` vencida desde el 11/11; `ED-2109` en TESTING.
- Alcance que crece: han entrado unas 30 tareas desde el 17/11, pero la mayoría ya está cerrada. No preocupa.
- Agenda hasta el cierre: sin festivos ni ausencias del equipo en tu calendario. Revisión de Sprint lun 23 y lun 30, Responsables mar 24.

**No mirado:** la cabina (no se ha refrescado desde el 30/10) y las ausencias del equipo, que no salen en tu calendario.

## 2026-11-20 · 15:22 — viernes, segunda pasada

**Sin cambios de fondo desde las 12:10.** 98 tareas (6 genéricas): **36 cerradas de 92, un 39 %**. Ha entrado `IN-579` (Jesús, vence hoy).

- 🔴 `RDCO-182`…`188` **siguen igual**: sin dueño. Palanca, la misma: Revisión de Sprint del lun 23.
- 🟠 Alex, Juanma y las acciones del lunes, **igual que a las 12:10**. No han empeorado.
- ⚪ Fernando cerró esta mañana 5 tareas de seguridad (`ED-2139`…`2142`, `ED-2110`). `AS-594` sigue en curso y vence hoy.

## 2026-11-25 · 12:09 — miércoles, día hábil 7 de 10

**Situación:** 126 tareas (6 genéricas): **70 cerradas de 120, un 58 %**. Quedan hoy + 3 hábiles (26, 27 y 30). Ritmo bueno; lo que
falla no es el volumen sino las acciones del [[2026-11-23 - Seguimiento Sprint - Dev|lunes 23]].

**🔴 Actúa ya**
- **Spring Security 4.1.3: Mis Alumnos y Docentia siguen sin tarea.** La acción del lunes era tuya y "hoy o mañana"; en Jira no hay nada
  creado desde el 20/11 que las cubra, y en el correo no hay más hilo que el aviso de Alejandro (*Vulnerabilidad*) y el de INCIBE. Las demás
  apps de la lista ya están hechas (`IN-580`, `GES-294`); estas dos son las únicas expuestas.
  → Palanca: crearlas **hoy** (propuesta del lunes: Mis Alumnos → Paco, Docentia → Pablo, que tiene 4 abiertas).
- **`RDCO-182`…`188` sin dueño, quinta nota (40 días).** Ya no llegan al cierre del 30. Lo que queda por decidir es que **no pasen al
  `2026/20` otra vez sin dueño**. Juanma sigue con una sola tarea en el sprint (`GES-233`) y nada cerrado desde el lun 23.
  → Palanca: asignarlas esta semana para que arranquen el `2026/20` con dueño; las 4 Urgentes primero.

**🟠 Vigila**
- **`AS-594` (subida a PROD de Mi Calendario y Mis Asignaturas)**: en curso desde el 16/11, vencida el 20, y era la acción "ya" de Paco. Desde
  el lunes ha cerrado 7 tareas, pero esta no. Además le vencen hoy `AS-598` y `AS-599`.

**⚪ Ruido**
- ✅ Alex sacó de TESTING `RDCO-189` y `LA-56` (acción del lunes a medias: `RDC-105` sigue ahí desde el 02/11). Cerró `ED-2143`.
- ✅ Jesús cerró `IN-579`, `IN-580` (Spring Boot 4.1.3 en Mis Notas, Mis Planillas, `jav-documentos`, `jav-alfresco`) e `IN-581`. Lo viejo
  (`MIG-50`, `ED-2048`, `GESTDOC-11`, `ET-491`) y los `GESTDOC-13`…`16`, igual.
- Alejandro: `IN-572` (vencida 17/11) y `EVT-26` (vencida 24/11) en curso; cerró 12 el lunes 23 (bastantes eran clase, examen y evento).
- Igual que el lunes: `GES-229`, `GES-233`, epics `GES-222`…`225`/`GES-250`, `GES-254` sin dueño. Tuyas vencidas: `ED-2099`, `ED-2109`.
- Entra `GD-779` (Pablo, hoy). Sin tarea en Jira todavía: stock de Odontología y BONO CAMPUS (no buscado a fondo).

**No mirado:** agenda (la del lunes ya cubría hasta el 30) y cabina (sigue la del 30/10).
