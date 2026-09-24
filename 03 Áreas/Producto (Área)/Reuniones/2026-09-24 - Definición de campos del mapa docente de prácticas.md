---
tipo: reunión
fecha: 2026-09-24
hora: 12:57–13:13
convoca:
proyecto:
asistentes: [Pilar, "+4 sin identificar"]
estado: acta
transcripcion: "_secretos/Transcripciones/2026-09-24 - Definicion de campos del mapa docente de practicas.md"
confluence:
jira:
tags: [reunión, prácticas, mapa-docente, educación]
---
# 2026-09-24 - Definición de campos del mapa docente de prácticas

> **Estado:** `transcrita` → **`acta`** → `requisitos` → `publicado` → `planificado`
> La transcripción cruda vive en `_secretos/Transcripciones/` y **no sube a GitHub**.

> ⚠️ **Los hablantes vienen anonimizados** (`Speaker 2/3/4/5`, sin nombres). **Aquí no se atribuye
> ninguna frase a nadie**: se habla por roles —*funcional* y *técnico*—. En la conversación se
> nombra de pasada a Juanma, Paco, Álex, Isaac y Elena, pero **no consta quién dijo qué**.
>
> ⚠️ **No fue una reunión de Zoom**: es una captura de **My Notes** de una reunión presencial o de
> Meet, con transcripción del lado asistente y **reconocimiento de voz malo**. Varios tramos están
> marcados como dudosos.

## 🎯 Objetivo

Cruzar campo a campo el **mapa docente de enfermería**, que ya existe, con el **mapa docente de
prácticas** que hay que montar para **Educación**, y dejar definida la estructura antes de pedirle
nada a Prado ni a la Consejería.

## ✅ Decisiones

- **`localidad` = `área`.** En Educación **no hay áreas**, así que la localidad (Abarán, Águilas…)
  hace ese papel y se corresponde "más o menos" con las áreas de enfermería. Es la decisión que
  sostiene todo lo demás
- **Los centros se mantienen como campo**, cambiando los de enfermería por los de Educación
  (se citó como ejemplo un *Centro Infantil y Primaria*, "Santo Tomás")
- **El código de prácticas lo genera el equipo**, como ya se hacía
- **Al mapa de Prado se le añade el campo de correspondencia área ↔ localidad**
- **Tutores: dos versiones de visualización** — una **corta** y una **ampliada** al pinchar en el
  tutor, con nombre, apellidos y las asignaturas que imparte
- **Se conservan** `fecha inicio`, `fecha fin` y **`plazas disponibles`** *(estas se van a
  actualizar)*
- **Las menciones no entran en la asignación.** Son de grado, no de máster; se podrán guardar
  **a modo informativo**. Las **especialidades** sí cuentan, para el máster
- **`destinatario` sale.** Se identificó como el ID del centro y quedó como **candidato a
  eliminar** del mapa
- **No hacen falta más ficheros**: bastan los que ya hay — mapa docente, carga, centros privados
  y alumnos

## 📌 Acciones (quién / cuándo)

> No se puso fecha a ninguna. Sin nombres en la transcripción, van por rol.

**Técnico / base de datos**

- [ ] Revisar en la BD **qué relación hay entre centro, servicio y unidad** — en la reunión nadie
      lo recordaba, y de ahí depende dónde cuelga la especialidad
- [ ] Averiguar **a qué apunta el `alias`**: ¿a la unidad o al servicio? Es la pieza que decide
      dónde se guarda la especialidad
- [ ] Comprobar si **el área vive dentro de la tabla de servicio** — se apuntó que **no existe
      tabla de áreas** como tal
- [ ] Traer la **información del tutor desde el mapa de Prado** e insertarla en la tabla de
      tutores, **añadiendo las columnas que hagan falta** *(se comentó que no es problema: esa
      tabla no se relaciona con otras)*

**Funcional / con Educación**

- [ ] **Confirmar con ellos** qué información del tutor necesitan de verdad
- [ ] **Confirmar** si las menciones se quedan solo como informativas
- [ ] **Preguntar** si quieren ver las asignaturas del tutor en pantalla o les basta con que
      salgan en la descarga ampliada

## 🖥️ Lo que nos toca a nosotros

- Las cuatro de **Técnico / base de datos** son del equipo. La de la relación
  **centro–servicio–unidad** es la que **bloquea** a las demás: hasta que no se sepa, no se puede
  decidir dónde se guarda la especialidad
- Esto conecta con **`GES-254` Descarga del mapa docente de Prado**, dentro de la automatización de
  prácticas `GES-192` → [[2026-09-16 - Seguimiento Sprint - Dev]]

## 🕓 Para tener en cuenta más adelante

- 🔴 **El DNI del tutor es dato personal y NO quedó decidido.** El resumen automático de Zoom lo da
  por aprobado; **la transcripción dice otra cosa** — se pidió "toda la información del tutor,
  es decir, el DNI", y acto seguido alguien respondió **"no me han pedido el DNI"**. Antes de crear
  esa columna conviene dejar escrito **para qué se necesita**: es minimización de datos, y una
  columna de DNI que nadie ha pedido es exactamente lo que luego hay que justificar
- **`localidad = área` es una convención cómoda, no una equivalencia real.** Si Educación acaba
  teniendo áreas propias, o si la localidad no cubre algún centro, hay que deshacerla. Merece
  quedar escrito en el modelo, no solo en la cabeza de quien lo montó
- **Si la especialidad se queda "colgada"** por no haber servicio en Educación, el problema no se
  queda en el mapa: se arrastra al algoritmo de asignación de plazas
- Se mencionó que **faltaría el centro de salud** relacionado con centros — no se cerró si entra o
  no en este mapa

## ❓ Puntos abiertos

- **¿Dónde se guardan las menciones y las especialidades?** Se habló de que van "a nivel de
  unidad", pero **no se decidió la tabla**
- **¿A qué hace referencia el `alias`?** Sin eso no se puede colocar la especialidad
- **¿Hace falta guardar el DNI del tutor?** Ver el aviso de arriba
- **¿Entra el centro de salud** en este mapa?
- ⚠️ **Tramos que no se entienden** en la transcripción y que **no se han interpretado**:
  "¿cómo la relacionas con un centro para hacerle daño?", "esto es chaco to chaco",
  "Jaime Mata", "algún ejermán álex". Y **un fragmento entero que no es de la reunión**
  (*"camareros rubios de corta chaqueta azul…"*), que es ruido o basura del reconocedor
- **No consta quién convocó** ni la lista real de asistentes: Zoom no dio nombres

## ✉️ Borrador de correo a los asistentes

> **Borrador**: no se envía hasta que le des a enviar.
> Redactado como **tus notas**, no como acta oficial, porque **no consta quién convocó**. Si la
> convocaste tú, dímelo y lo reescribo repartiendo acciones con nombre y fecha.

**Asunto:** Mis notas de lo de hoy — campos del mapa docente de prácticas

```
Hola:

Os paso lo que apunté esta mañana de la revisión de campos del mapa docente de
prácticas, por si se nos escapa algo. Corregidme lo que haga falta.

Lo que dimos por cerrado:
- Localidad hace de área. En Educación no tenemos áreas, y la localidad se
  corresponde bastante bien con las áreas de enfermería.
- Los centros se quedan, cambiando los de enfermería por los nuestros.
- El código de prácticas lo seguimos generando nosotros.
- Al mapa de Prado le añadimos la correspondencia área-localidad.
- Tutores en dos versiones: una corta, y una ampliada al pinchar, con nombre,
  apellidos y las asignaturas que imparte.
- Se mantienen fecha de inicio, fecha de fin y plazas disponibles.
- Las menciones no entran en la asignación (son de grado); como mucho, las
  guardamos a modo informativo. Las especialidades sí, para el máster.
- El campo "destinatario" nos lo cargamos.
- No hacen falta ficheros nuevos: con el mapa, la carga, los centros privados y
  los alumnos vamos servidos.

Lo que quedó en el aire y necesito que alguien mire:
- La relación entre centro, servicio y unidad en la base de datos. Es lo que
  bloquea decidir dónde guardamos la especialidad.
- A qué apunta el alias, si a la unidad o al servicio.
- Si el área está dentro de la tabla de servicio (parece que tabla de áreas
  no hay).
- El DNI del tutor: no me quedó claro si lo necesitamos de verdad. Antes de
  crear la columna prefiero saber para qué, que es dato personal.
- Si entra o no el centro de salud.

Y tres cosas que hay que preguntar a Educación: qué información del tutor
necesitan realmente, si las menciones se quedan solo informativas, y si quieren
ver las asignaturas en pantalla o les vale con la descarga ampliada.

Un saludo,
Pilar
```

## 🔗 Enlaces

- Transcripción cruda: `_secretos/Transcripciones/2026-09-24 - Definicion de campos del mapa docente de practicas.md` *(no sube a GitHub)*
- Nota en Zoom My Notes: https://us01docs.zoom.us/doc/FOhP0uU-QeawghcPA3Oa4g
- [[2026-09-16 - Seguimiento Sprint - Dev]] — `GES-253` / `GES-254`, descarga del mapa docente de Prado
- [[2026-09-10 - Prácticas Educación 26-27]]
- [[2026-09-09 - Automatización prácticas - Fisioterapia y Podología]]
- [[Producto (Área)]]
