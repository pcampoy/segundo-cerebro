---
tipo: reunión
fecha: 2026-09-08
hora: —
sprint: Desarrollo 2026/14
sprint_dia: 9 de 16 (día hábil 7 de 10)
sprint_fin: 2026-09-15
ultimo_dia_habil: 2026-09-11
estado: acta
tags: [reunión, sprint, equipo, dev]
---
# Seguimiento Sprint - Dev — revisión de mitad de sprint

> ⚠️ **Fuera de ciclo.** El *Seguimiento Sprint - Dev* del **lunes 14 no se celebra**: ese día es
> no lectivo con actividad suspendida (peregrinación institucional) y el **martes 15 es festivo en
> Murcia**. Ver [[Festivos y no lectivos 26-27]].
>
> ✅ **Decidido el 08/09: el cierre del sprint se hace el miércoles 16.** Ya dentro del sprint
> siguiente, así que es **cierre + planificación en la misma sesión** (ver abajo).

## 📊 Dónde estamos en el sprint

| | |
|---|---|
| Sprint | **Desarrollo 2026/14** (id 2842, tablero 3) |
| Fechas | 31/08 → **15/09** |
| Hoy | martes 8 · día **9 de 16** naturales · día hábil **7 de 10** |
| **Días hábiles que quedan** | **3** — miércoles 9, jueves 10 y **viernes 11** |
| **Último día hábil real** | **viernes 11 de septiembre** |
| Tareas en el sprint | **111** · 83 abiertas · 28 finalizadas |

**El sprint no termina el 15: termina el 11.** Todo lo comprometido "para el 15" tiene en realidad
tres días.

## 🔴 El dato que manda

De las ~75 tareas de trabajo real abiertas, **unas 55 no se han actualizado desde el 31 de
agosto** — el día que arrancó el sprint. No es que vayan lentas: es que **entraron al sprint y no
se han vuelto a tocar**. Lo único con movimiento es lo de ayer y hoy.

Con tres días hábiles por delante, **este sprint no se cierra**. La conversación no es "cómo
acabamos" sino **qué se salva y qué se replanifica**.

## 👥 Reparto por persona

### Paco — 25 abiertas
- **21 son las historias de Investigadores** (`GD-572`…`GD-592`), las que salieron de la captura de
  requisitos. Entraron el 31/08 y **solo 3 se han movido** (`GD-572`, `GD-586`, `GD-580` en curso).
  Las 18 restantes siguen en *Tareas por hacer* con 7–8 días parados.
- **Urgentes de Asistencia/Datio, y con fecha encima:**
  - `AS-549` — *Error en el proceso de Asistencia Leer Datio* · **Urgente** · TESTING · **vence hoy**
  - `AS-546` — *Cambio AsistenciaDatio* · **Urgente** · en curso · **vencida el 4/09**
- `IN-505` — *Acceder según rol y ámbito a my.ucam.edu* · **vencida desde el 4 de mayo**
- `DT-306` — publicación mensual de LinkedIn de septiembre · vence 30/09

### Pablo — 19 abiertas
- **15 entraron ayer**: toda la ráfaga `GD-642`…`GD-655` sobre el volcado a PDS, borrados masivos
  de asignaturas y asignaciones, timeouts de `jav-estudio` y la cascada JPA. **Es el incendio de
  las horas de docencia desaparecidas**, ya desglosado en tareas.
- Las 4 anteriores llevan 8 días: `GD-596` (Bajas y Sustituciones), `GD-565`, `GD-87`, y
  `GD-610` en **TESTING** (pantalla de sustituto y detalle).
- Ojo: 15 tareas nuevas a tres días del cierre **no caben**. Esto es alcance del sprint siguiente.

### Jesús — 9 abiertas
- **4 en TESTING paradas 8 días**: `MIG-38`, `MIG-42`, `MIG-43` (migración: volcado de expedientes
  y revisión de datos) e `IN-541` (vista de introducción de notas). **Es lo más barato de cerrar
  esta semana** — están a un empujón de FINALIZADA.
- `MIG-44` sí se movió ayer (revisión de datos tras vacaciones).
- Paradas: `IN-562`, `IN-494` (reunión de seguimiento con cliente), `GESTDOC-11`, `ET-491`.

### Alejandro — 11 abiertas
- **8 paradas 8 días y TODAS vencidas**: `EVT-14`…`EVT-18` (RabbitMQ, endpoints y monitorización
  de eventos) vencían el **1 de agosto**; `ED-2014`, `ED-2015`, `ED-2016` (AppCron Microsoft,
  códigos Cientia, nuevas titulaciones) vencían el **1–4 de agosto**.
- **3 nuevas de ayer con fecha crítica:** `ED-2030` (doble factor), `ED-2032` (iText TFG-TFM),
  `ED-2033` (iText Recos) — **vencen el 12/09**, un día después del último día hábil.

### Juanma — 8 abiertas
- **Todas paradas 8 días, y 5 vencidas hace mucho:**
  - `CAN-350` — *Bloquear acceso a usuarios que no han seleccionado sede* · **Muy Urgente** ·
    TESTING · **vencida el 20 de marzo**
  - `CAN-337` y `CAN-340` — datos y tablas de Canvas Data 2 · **vencidas el 21 de noviembre de 2025**
  - `CAN-348`, `CAN-349` — carga y sincronización de logs · vencidas en marzo
- Y `WD-384`, `FAC-32`, `FAC-38` (unificación de seguridad y login corporativo de Facturas).

### Alex — 1 abierta
- `ED-2027` — *Migrar el inicio de sesión de appcron a Microsoft* · en curso · **vencida el 4/09**.
- **Una sola tarea.** Ver el apartado de equilibrado.

### Pilar (no es del reparto del equipo)
- `ED-2018` — *Reorganización Planificación Septiembre* · en curso **desde el 31/08**. Es
  literalmente la reasignación del sprint, y lleva 8 días sin moverse.
- `GES-192` — reunión de arquitectura de prácticas · 8 días.
- `MIG-29` — reunión del equipo de migraciones Sigma · **vencida desde el 19 de junio**.

## ⚖️ Riesgos y equilibrado

**1. El reparto está roto: 25 tareas contra 1.** Paco lleva 25 abiertas y Alex 1. Y las 21
historias del módulo de Investigadores están todas en la misma persona: es un módulo entero
—roles, reglas de horas, autorizaciones— sobre un solo par de manos. Hay margen evidente para
mover parte a Alex, con acompañamiento, y para que Alejandro absorba las de más complejidad.

**2. Nadie ha tocado nada en 8 días.** El patrón es demasiado uniforme para ser casualidad: 55
tareas con la misma fecha de actualización sugiere que se metieron en bloque al abrir el sprint y
que **el tablero no se está usando como herramienta de trabajo diario**. Merece una pregunta
directa en la reunión, sin reproche: si el estado real no está en Jira, el semanal no sirve de
nada.

**3. Deuda vencida acumulada.** 20 tareas del sprint están vencidas, algunas desde 2025. `CAN-350`
es **Muy Urgente** y lleva vencida desde marzo. O se replanifican con fecha nueva o se sacan del
sprint: arrastrarlas oculta lo que sí es de esta quincena.

**4. Lo que sí tiene fecha esta semana:**
- `AS-549` vence **hoy** · `AS-546` ya vencida — las dos Urgentes, las dos de Datio
- `ED-2030`, `ED-2032`, `ED-2033` (iText) vencen el **12/09**, con el sprint cerrado el 11

**5. Basura en el tablero que falsea las cuentas:**
- `ED-631` — *Cambiar el mensaje de mantenimiento* · **vencía el 13/09/2024**. Dos años en el sprint.
- Las tareas de imputación de **JULIO** (`ED-1987`…`ED-1990`) siguen en el sprint activo, ya
  finalizadas. Deberían haber salido al cerrar julio.

## 📅 Hitos y agenda

- **Miércoles 9** · Tangram, seguimiento semanal (11:00) · Comunidad IA (13:00)
- **Jueves 10** · Educación Prácticas 26-27 (9:30) · Revisión sustituciones (11:30) · Tangram 26/27 (13:30)
- **Viernes 11** · Clase 8:30–10:30 · Reunión equipo TIC cambios del modelo 9:30–10:30 **(solapan)**
  · **último día hábil del sprint**
- **Lunes 14** · no lectivo, actividad suspendida · **Martes 15** · festivo · el sprint muere aquí
- **Miércoles 16** · primer día hábil del sprint siguiente · empiezan las clases de 1º
- **Miércoles 23** · arranca la docencia online (" 3º IR", 16:00–17:00)
- **Miércoles 30** · formación IZO, día completo · **martes 22** · reunión Apryse/iText (12:00)

## ✅ El cierre: miércoles 16

Decisión de Pilar: el cierre se hace el **miércoles 16**, primer día hábil tras el puente.

**Lo que eso implica:**

- **El viernes 11 sigue siendo la fecha real de trabajo.** El 16 es la ceremonia, no una prórroga:
  entre el 11 y el 16 no hay ningún día hábil. Lo que no esté el viernes, no está.
- **Es cierre y planificación a la vez.** El sprint siguiente ya habrá arrancado, así que en la
  misma sesión hay que revisar lo que no llegó, replanificarlo y repartir el nuevo. Con 83 tareas
  abiertas y un rebalanceo pendiente, **90 minutos no bastan**: o se reserva más tiempo o se
  parte en dos (cierre por la mañana, reparto por la tarde).
- ⚠️ **Cuidado con la hora:** el miércoles 16 hay *UCAM, seguimiento semanal* con Tangram de
  **11:00 a 12:00**. El hueco de la mañana es **antes de las 11:00** — el horario habitual de
  09:45–11:15 se solaparía.
- **No hace falta `/inicio-sprint`:** las tareas de imputación van por mes natural y la tanda de
  **septiembre ya existe** (`ED-2019`…`ED-2024`). Dos sprints consecutivos comparten tanda. Solo
  habrá que crear la de octubre cuando toque.
- **El seguimiento del lunes 21** vuelve al ciclo normal, y ya será de ejecución del sprint nuevo.

## 📌 Acciones (quién / cuándo)

- [x] **Pilar — 08/09:** decidido, el cierre se hace el **miércoles 16**
- [ ] **Pilar — hoy:** **avisar al equipo** de dos cosas: que el trabajo acaba el **viernes 11**
      (no el 15) y que el cierre se hace el **miércoles 16**
- [ ] **Pilar — hoy:** crear el evento del cierre del miércoles 16, **antes de las 11:00** para no
      pisar el seguimiento con Tangram. Y reservar más tiempo del habitual: es cierre + reparto
- [ ] **Paco — hoy:** `AS-549` vence hoy y `AS-546` está vencida. Son las dos Urgentes
- [ ] **Jesús — esta semana:** cerrar las 4 de TESTING (`MIG-38`, `MIG-42`, `MIG-43`, `IN-541`)
- [ ] **Alejandro — antes del 11:** las tres de iText, que vencen el 12
- [ ] **Pilar + Juanma:** replanificar o sacar las 5 tareas de Canvas vencidas desde 2025
- [ ] **Pilar:** rebalancear Investigadores — mover parte de `GD-573`…`GD-592` de Paco a Alex y Alejandro
- [ ] **Pilar:** limpiar el tablero — `ED-631` y la tanda de imputación de julio fuera del sprint

## 🕓 Para tener en cuenta más adelante

- **Las 15 tareas nuevas de Pablo sobre el volcado a PDS** son el alcance del sprint siguiente, no
  de este. Conviene agruparlas para no repartirlas a ciegas: varias apuntan al mismo problema
  (borrados masivos y cascada JPA).
- **`ED-2018` es la reasignación del sprint** y lleva 8 días en curso. Mientras no se cierre, el
  reparto desigual sigue.
- El **1 de julio** como fecha de no retorno para modificaciones de planes ya es un hito del
  calendario del equipo → [[2026-09-04 - Criterios de implantación de modificaciones de planes]].
- **Ediciones de plan en Laurea**, objetivo curso 27-28: hay que empezar a moverlo a mediados de
  2027 como muy tarde.

## ✉️ Borrador de correo al equipo

> **Borrador**: no se envía sin que Pilar le dé a enviar.
> Redactado en tono neutro a propósito en el punto del tablero — endurécelo si quieres.

**Para:** Alejandro, Pablo, Juanma, Alex, Jesús, Paco
**Asunto:** Sprint 2026/14 — el trabajo acaba el viernes 11 y cerramos el miércoles 16

```
Hola a todos,

Aviso de fechas, porque la semana que viene tiene un puente por medio y
cambia el calendario del sprint.

El lunes 14 es no lectivo y se suspende la actividad por la peregrinación
institucional, y el martes 15 es festivo en Murcia. El sprint 2026/14
termina oficialmente el 15, pero como esos dos días no se trabaja, la
fecha real es el viernes 11. Lo que no esté el viernes, no entra.

Por eso: el seguimiento del lunes 14 no se celebra, y el cierre del
sprint lo hacemos el miércoles 16 por la mañana. Os paso convocatoria.
Será cierre y reparto del siguiente en la misma sesión, así que llevará
algo más de tiempo del habitual.

Lo que os pido para el viernes, por orden de urgencia:

- Paco: AS-549 y AS-546, las dos de AsistenciaDatio. Son las dos
  Urgentes y una vence hoy. De Investigadores, cierra lo que tengas en
  curso y no abras más frentes.
- Alejandro: las tres de iText y doble factor (ED-2030, ED-2032,
  ED-2033). Vencen el 12, así que en la práctica es el viernes.
- Jesús: las cuatro que tienes en TESTING (MIG-38, MIG-42, MIG-43 e
  IN-541). Están a un empujón y son las que mejor cierran la quincena.
- Juanma: CAN-350, que está en TESTING y es Muy Urgente. Y dime qué
  hacemos con las de Canvas que llevan vencidas desde el año pasado:
  las replanificamos con fecha nueva o las sacamos del sprint, pero
  arrastrándolas no nos sirven.
- Alex: ED-2027, la migración del login de appcron.
- Pablo: no metas más de la tanda nueva del volcado a PDS. Dime cuáles
  son imprescindibles esta semana y el resto lo repartimos el 16.

Y una cosa que os pido a todos: antes de irnos el viernes, dejad el
tablero al día. Ahora mismo hay bastantes tareas que no se han movido
desde que abrimos el sprint, y necesito que el estado de Jira sea el
real para que el cierre del miércoles sirva de algo y para repartir con
criterio. Si algo está bloqueado o esperando a otro, ponedlo también:
eso es justo lo que quiero ver.

Cualquier duda, me decís.

Un saludo,
Pilar
```

## 🔗 Enlaces

- 📌 [Tablero del sprint](https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3)
- Lunes anterior: [[2026-09-01 - Seguimiento Sprint - Dev]]
- [[Equipo (Área)]] · [[Festivos y no lectivos 26-27]] · [[Pendientes - Septiembre 2026]]
