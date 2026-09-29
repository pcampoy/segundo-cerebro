---
tipo: reunión
fecha: 2026-09-29
hora: 09:18–10:00
convoca: Sección de Títulos
proyecto:
asistentes: [Pilar, "Sección de Títulos", "Desarrollo"]
estado: planificado
transcripcion: "_secretos/Transcripciones/2026-09-29 - Nuevo proceso en sede - certificado B2 de Primaria.md"
confluence: "ESE/1239678978"
jira: "ET-549"
tags: [reunión, sede-electrónica, títulos, certificados, laurea]
---
# 2026-09-29 - Nuevo proceso en sede: certificado B2 de Primaria

> **Estado:** `transcrita` → **`acta`** → `requisitos` → `publicado` → `planificado`
> La transcripción cruda vive en `_secretos/` y **no sube a GitHub**.
>
> 📘 **Publicado en Confluence** — espacio *Sede Electrónica* (ESE), bajo
> *Certificados*: [Certificado de nivel B2 — Grado en Educación Primaria](https://ucam.atlassian.net/wiki/spaces/ESE/pages/1239678978/Certificado+de+nivel+B2+Grado+en+Educaci+n+Primaria)

> ⚠️ **Hablantes anonimizados** por Zoom (`Speaker 1..5`). Aquí **no se atribuye ninguna frase a
> nadie**: se habla por roles — *Títulos* y *Desarrollo/TIC*.
>
> ⚠️ **El acta recoge solo la parte de trabajo.** El tramo final de la reunión derivó a otros
> asuntos que no son de este procedimiento y se ha dejado fuera.

## 🎯 Objetivo

Montar en la **sede electrónica** un procedimiento automático para que los alumnos del **Grado en
Educación Primaria** obtengan su **certificado de nivel B2**, que **desde 2019 se emite a mano**.

**Por qué ahora:** el párrafo del B2 salía solo en los certificados de Infocan y **en Laurea ya no
sale**. Desde entonces, por cada solicitud hay que salir del módulo de títulos, entrar en el
expediente, comprobar qué asignaturas ha cursado y superado, y pegar a mano el párrafo del idioma
que corresponda. Con **unos 4.000 trámites anuales**, pico en junio, y **un equipo de tres personas**,
se describió como insostenible: *"ya no damos abasto"*.

## ✅ Decisiones

- **El alumno lo pide él mismo en sede**, igual que el certificado de no sanción: inicia el
  procedimiento y el sistema resuelve solo, sin que Títulos toque nada
- **El certificado se emite solo si se cumplen las tres condiciones a la vez:**
  1. Tener **superado el bloque de asignaturas** del idioma — inglés, francés o alemán. *Títulos
     pasa los bloques; no están en base de datos y hay que definirlos*
  2. **Fecha fin a partir del 1 de septiembre de 2015** *(antes de esa fecha no corresponde)*
  3. Estado de la solicitud en uno de estos cuatro: **confirmado por el MEC, enviado a imprenta,
     pendiente de entrega o retirado**
- **Si no cumple**, sale un mensaje en pantalla remitiéndole a la **Sección de Títulos**. No se
  emite nada
- **Alcance: el estudio completo, no plan a plan.** Entran **todos los planes** del Grado en
  Educación Primaria, y se define por estudio a propósito — *"por si luego se inventan un plan
  nuevo"*
- **El documento lleva CSV, escudo y firma del Secretario General**
- **No pasa por el gestor documental**: se queda en sede. Se descartó guardarlo también allí
- 📌 **Unificar la nomenclatura de la universidad como «Universidad Católica San Antonio»**, que es
  como está registrada en el Ministerio *(código 060)*. Se señaló que **el certificado de beca dice
  «Universidad Católica de Murcia»**, que no es el nombre registrado. En los títulos oficiales y en
  el certificado de fin de estudios sí aparece bien

## 📌 Acciones (quién / cuándo)

**Sección de Títulos** — *se comprometieron a mandarlo hoy mismo: "te lo mando todo ahora"*

- [ ] Los **bloques de asignaturas por idioma** (inglés, francés, alemán)
- [ ] Los **cuatro estados de solicitud** que hay que comprobar
- [ ] La **descripción del proceso** para la página de inicio en sede y **cómo se va a llamar**
- [ ] El **texto del mensaje** que ve el alumno que no cumple los requisitos
- [ ] El **correo de envío** del certificado

**Desarrollo**

- [ ] La **consulta automática al expediente** con las tres condiciones
- [ ] La **plantilla del certificado**, con escudo y firma del Secretario General
- [ ] El **alta del procedimiento en sede**

**Pilar**

- [ ] **Dar una fecha.** No se comprometió ninguna en la reunión: *"pues hablo con Jesús y te lo
      digo"*. Se dijo que no parece complicado y que es cuestión de encajarlo en un hueco

## 🖥️ Lo que nos toca a nosotros

- El desarrollo es de **Jesús March**, y en la reunión se calificó de sencillo. **Lo que falta es el
  hueco**, no el análisis
- ⚠️ **El sprint `2026/15` cierra el jueves 1**, así que esto entra en el siguiente. Conviene decir
  la fecha antes de que Títulos la pida otra vez: llevan **desde 2019** haciéndolo a mano y lo que
  pidieron fue *"cuanto antes"*, sin presionar con una fecha concreta
- Bloqueante menor: **los bloques de asignaturas no existen como dato**. Hay que definirlos en
  alguna estructura y decidir qué pasa **cuando cambien los planes**

## 🕓 Para tener en cuenta más adelante

- 🔴 **La migración de Infocan a Laurea no está bien, y Títulos no puede emitir con datos irreales.**
  En Laurea **no salen bien las convocatorias ni la fecha fin**. Son certificados que el alumno
  **paga** y que tienen un plazo de **3 a 5 días hábiles**; esta misma semana había certificados
  pendientes que hubo que sacar de Infocan. Dicho tal cual: *"yo al alumno que te paga 40 € no le
  voy a sacar un certificado inventado"*
- 📌 **Petición concreta y pequeña:** un **volcado de expedientes con asignaturas, convocatorias y
  fecha fin**, aunque sea *"en un folio en blanco"* y sin validez, para que Títulos **corrija Laurea
  a mano**. No piden una integración, piden el dato. En la reunión se situó el desarrollo formal
  **en 2027**, pero se admitió que el volcado simple podría mirarse antes
- ⚠️ **Mientras tanto, Infocan no se puede apagar.** Títulos depende de él para dar datos reales.
  Si se retira sin resolver esto, se quedan sin salida
- 🔴 **El gestor documental hay que renovarlo.** Falla justo cuando se necesita: en la **retirada de
  títulos** hay alumnos que dicen no haber retirado el título, se tira del gestor y **el documento
  no aparece**. Y otros departamentos están pidiendo usarlo
- 🔴 **La modalidad sale mal en el SET, y por el RD 2025 la modalidad va en el título.** Es decir,
  la universidad puede estar emitiendo **dos documentos con información contraria** —virtual en uno,
  presencial en el otro— sobre el mismo alumno. Ya hay referencia abierta a Sigma y se describió
  como que lleva **un mes** sin respuesta. **Esto es más grave que el B2 y no es de Títulos:
  necesita que alguien de Ordenación Académica lo coja**
- ⚠️ **Tiempos de respuesta de la consultora**: se planteó abrir el asunto formalmente en la próxima
  reunión con ellos, **dejando por escrito los incumplimientos de plazo**

## ❓ Puntos abiertos

- **Sin fecha de entrega.** Es lo único que Títulos se llevó sin cerrar
- **Cómo se definen los bloques de asignaturas** y qué pasa cuando cambie un plan
- **Quién unifica la nomenclatura** en el certificado de beca, que lo emite otra persona
- **Si el volcado de Infocan se puede adelantar** a 2026 o se queda en 2027
- **No consta el nombre de los asistentes**: Zoom no los dio. En el calendario la reunión estaba
  convocada por Títulos con Pilar y Jesús March

## ✉️ Borrador de correo a los asistentes

> **Borrador**: no se envía hasta que le des a enviar.
> **Convocó Títulos, no tú**, así que esto son *tus notas*, no el acta oficial.

**Asunto:** Mis notas del B2 en sede — y las dos cosas que os llevo aparte

```
Hola:

Os paso lo que apunté esta mañana, para que quede por escrito lo que tenéis
que mandarnos y lo que hacemos nosotros. Corregidme si me he dejado algo.

El procedimiento, tal y como quedó:
- El alumno lo pide en sede, como el certificado de no sanción, y el sistema
  resuelve solo.
- Se emite si se cumplen las tres cosas: bloque de asignaturas del idioma
  superado, fecha fin a partir del 1 de septiembre de 2015, y estado de la
  solicitud en confirmado por el MEC, enviado a imprenta, pendiente de entrega
  o retirado.
- Si no cumple, le sale un mensaje remitiéndole a la Sección de Títulos.
- Entra el Grado en Educación Primaria completo, todos los planes.
- Lleva CSV, escudo y firma del Secretario General, y no pasa por el gestor
  documental.

Lo que necesitamos de vosotras para empezar:
- Los bloques de asignaturas por idioma.
- Los cuatro estados de solicitud.
- El nombre y la descripción del procedimiento para la sede.
- El texto del mensaje para quien no cumple.
- El correo con el que se le manda el certificado.

Lo hablo con Jesús y os digo fecha esta semana.

Y me llevo aparte dos cosas que salieron y que no son de este procedimiento:
el listado de expedientes de Infocan con convocatorias y fecha fin para que
podáis corregir Laurea a mano, y lo de la modalidad en el SET, que con el real
decreto de 2025 ya afecta al título. Esa segunda la muevo yo.

Un saludo,
Pilar
```

## ✉️ Borrador interno — para mover lo de la modalidad

> El que de verdad mueve tu trabajo. Decide tú a quién va: Ordenación Académica y/o Dirección TIC.

```
Hola:

Sale de una reunión con Títulos de esta mañana y creo que hay que cogerlo antes
de que nos lo encuentren de fuera.

La modalidad que sale en el SET no coincide con la que va en el título. Con el
Real Decreto de 2025 la modalidad aparece en el título, así que estamos en
condiciones de emitir a un mismo alumno dos documentos oficiales que se
contradicen: uno dice virtual y el otro presencial.

Hay una referencia abierta con la consultora que lleva semanas sin respuesta.
Os pido dos cosas: que alguien de Ordenación Académica se haga cargo del
criterio, y que decidamos si esto sube de prioridad en el seguimiento con
Sigma.

Un saludo,
Pilar
```

## 🏃 Desglose en Jira — proyecto Tramita (`ET`)

Creado el 29/09. **Todo asignado a Jesús March**, componente *REGPNP*, equipo *Desarrollo*.

| Clave | Qué | Prioridad | Depende de |
|---|---|---|---|
| **`ET-549`** | 🧩 **Epic** · Certificado de nivel B2 en sede — Grado en Educación Primaria | Media | — |
| `ET-550` | 1 · Modelado y carga de los bloques de asignaturas por idioma | **Urgente** | — *(espera dato de Títulos)* |
| `ET-551` | 2 · Consulta de verificación de requisitos contra el expediente | Media | bloqueada por `ET-550` |
| `ET-552` | 3 · Plantilla del certificado (escudo, CSV, firma) | Media | — *(en paralelo)* |
| `ET-553` | 4 · Alta del procedimiento en sede y flujo del alumno | Media | bloqueada por `ET-551` y `ET-552` |
| `ET-554` | 5 · Validación con muestra real antes de producción | Media | bloqueada por `ET-553` |

**El camino crítico es 1 → 2 → 4 → 5.** La 3 va en paralelo. La 1 está en Urgente porque
**bloquea todo y depende de que Títulos mande los bloques de asignaturas**.

## 🔗 Enlaces

- Transcripción cruda: `_secretos/Transcripciones/2026-09-29 - Nuevo proceso en sede - certificado B2 de Primaria.md` *(no sube a GitHub)*
- Nota en Zoom My Notes: https://us01docs.zoom.us/doc/glQ3SWuoRpaipDHKmboXtw
- **Jira:** https://ucam.atlassian.net/browse/ET-549
- **Confluence (ESE):** https://ucam.atlassian.net/wiki/spaces/ESE/pages/1239678978/Certificado+de+nivel+B2+Grado+en+Educaci+n+Primaria
- [[29-09-2026]] · [[Producto (Área)]] · [[Cronograma de proyectos (hasta dic 2026)]]
- [[2026-09-04 - Criterios de implantación de modificaciones de planes]] — *el mismo asunto de la modalidad y el RD*
