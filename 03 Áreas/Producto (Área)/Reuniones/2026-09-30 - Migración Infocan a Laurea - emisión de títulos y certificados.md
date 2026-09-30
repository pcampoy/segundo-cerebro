---
tipo: reunión
fecha: 2026-09-30
hora: 11:50–12:15
convoca: Sección de Títulos
proyecto:
asistentes: [Pilar, "Sección de Títulos (2 personas)"]
estado: acta
transcripcion: "_secretos/Transcripciones/2026-09-30 - Migracion Infocan a Laurea - emision de titulos y certificados.md"
confluence:
jira:
tags: [reunión, títulos, infocan, laurea, migración, certificados, dirección]
---
# 2026-09-30 - Migración Infocan → Laurea: emisión de títulos y certificados

> **Estado:** `transcrita` → **`acta`** → `requisitos` → `publicado` → `planificado`
> La transcripción cruda vive en `_secretos/` y **no sube a GitHub**.

> ⚠️ **Hablantes anonimizados** por Zoom. Aquí se habla por roles — *Títulos* y *TIC* — y **no se
> atribuye ninguna frase a nadie**. El reconocimiento de voz es malo: *Infocan*, *Laurea* y
> *Alfresco* aparecen deformados de diez maneras distintas en el original.

## 🎯 Objetivo

Decidir **cómo accede la Sección de Títulos a los datos de Infocan** para poder emitir certificados,
títulos y duplicados de alumnos antiguos, ahora que Infocan está en retirada y **los datos migrados
a Laurea no son fiables**.

---

# 🔴 Lo que hay que llevar a Dirección

Cinco conclusiones. Las tres primeras son el problema; las dos últimas, la decisión que se pide.

### 1. No son "algunos errores de migración": la proporción está invertida

Textual de Títulos:

> *"No todos los títulos están migrados, y los que están migrados, a lo mejor **uno entre un millón
> sale bien**. Si dijéramos «uno sale mal», vale, **pero es que es a la inversa**."*

Y el mecanismo está identificado, no es un misterio. En la migración **se usaron fechas estándar de
fin de curso** —del tipo 31/06 o 01/01— en lugar de la **fecha de acta de la última asignatura
aprobada**, que es la que usa Infocan y la que tiene valor académico:

> *"Se cogieron esas fechas estándares. No se vio porque tampoco había información, no se conocía
> que había que poner la fecha de acta."*

Resultado típico, con un caso real de la semana pasada: **fecha fin de febrero de 2017 en Laurea,
cuando la última asignatura aprobada es de diciembre**. Y las **convocatorias tampoco coinciden**.

### 2. No es un problema estético: es exposición legal

Los títulos **están regulados por ley y se comunican al Ministerio de Educación y Ciencia**. Un
certificado no puede decir una fecha fin distinta de la que el Ministerio ya tiene registrada.

> *"En título no hay margen de error, porque está todo regulado por ley."*
> *"Si el alumno ha terminado en junio, no se puede sacar un certificado con que termina en
> septiembre."*

**Por eso la Sección de Títulos emite desde Infocan y no desde Laurea.** No es preferencia: es que
emitir desde Laurea sería emitir un documento oficial con datos incorrectos.

### 3. Es coste diario, con dinero del alumno de por medio

- **Los duplicados se piden a diario**, no son un caso raro.
- Le cuestan al alumno **más de 300 €** *(150 € de tasas del BOE más las de expedición)*.
- El plazo comprometido es de **3 a 5 días hábiles**.
- Y hay un agujero que impide resolverlos bien: **en Laurea no consta si el alumno retiró el
  título**. Están *"todos abiertos o cerrados en disposición, pero no como retirado"*.

Eso importa porque **decide qué se le emite**: los alumnos de Primaria, por ley, **solo pueden tener
un título**. Si lo retiró, procede un duplicado; si no, una modificación interna del código ya
registrado. Sin ese dato, la discusión con el alumno es palabra contra palabra:

> *"Y los alumnos te exigen: ¿dónde está? Como que él retiró, porque yo no lo he retirado. Y tú me
> estás diciendo que sí, y yo te digo que no."*

### 4. Infocan no se puede apagar todavía — y la solución propuesta no lo resuelve del todo

La propuesta que se trajo a la reunión *(de Miguel Ángel, trabajada con Desarrollo)* es **exportar
el expediente completo de Infocan a PDF o JSON, guardarlo en Alfresco y buscarlo por DNI**.

Es razonable y Títulos la acepta. Pero **resuelve la consulta, no el dato**:

> *"Esto está muy bien, pero yo necesito completar el expediente sí o sí, para seguir el envío que
> tiene que hacerse sí o sí por Laurea."*

Es decir: **el expediente de Laurea hay que seguir corrigiéndolo uno a uno**, porque el envío al
Ministerio va por ahí. La exportación evita depender de que Infocan siga vivo, pero **no corrige
Laurea**.

### 5. La decisión que se pide a Dirección

Dos cosas, y ninguna es técnica:

- **¿Se corrige Laurea de forma masiva o se asume la consulta dual para siempre?** La fecha fin es
  recalculable a partir de la fecha de acta de la última asignatura aprobada. Nadie ha decidido si
  eso se hace.
- **¿Se le da a Títulos permiso para mecanizar directamente lo que encuentre?** Hoy dependen de que
  otra persona les corrija cada expediente en Laurea, uno a uno:

  > *"O me dais permiso para poder mecanizar lo que yo encuentre en el motor de búsqueda y paso la
  > información directamente a Laurea. […] Si no podemos hacer nada, pues tenemos que estar dando
  > el tostón."*

---

## ✅ Decisiones de la reunión

- **Exportar el expediente completo de Infocan** a **PDF o JSON** — formato por concretar.
- **Almacenarlo en Alfresco**, preferiblemente **una carpeta por alumno** que vaya acumulando el
  expediente y las solicitudes posteriores.
- **Generar los documentos con plantilla**, procesando el PDF, para títulos y duplicados.
- **Buscador simple por DNI.** Es requisito explícito de Títulos, no un adorno:
  > *"No me vale que me digas «sí, lo vas a tener» y luego vamos buscando y no tenemos."*
- **Criterio de fecha, cerrado en la reunión:** para los certificados se usa la **fecha de acta de
  la última asignatura aprobada**, que es la que aplica Infocan. **No** las fechas estándar de
  Laurea.

## 📋 Qué tiene que contener la exportación

Lista cerrada por Títulos en la reunión:

| Bloque | Detalle |
|---|---|
| **Expediente académico completo** | Asignaturas, **convocatorias**, créditos de **libre configuración**, **socioculturales** y **nota media** |
| **Fechas** | **Fecha de acta** de cada asignatura y **fecha de resguardo del título** *(= fecha de expedición)* |
| **Estado del título** | **Si el alumno lo ha retirado o no** — hoy es el dato que falta |
| **Reconocimientos** | Los reconocimientos **y su origen**. Salen en el certificado de Infocan |
| **Horas** | Hoy se ponen a mano en Laurea consultando Infocan |
| **Certificado bilingüe** | Español/inglés, para **diplomaturas y licenciaturas**: el Suplemento Europeo al Título **no se emite de oficio** en esos casos, se paga a solicitud del alumno. Sale de Infocan |

## 📌 Acciones (quién / cuándo)

**TIC / Desarrollo**

- [ ] 🔍 **Buscar la fecha de retirada del título en la base de datos.** La pista que dio Títulos:
      estaría **en la misma tabla y la misma fila donde aparecen las claves alfanuméricas**, y si el
      campo está en blanco es que no se ha retirado. *"Buscaremos nosotros, no os preocupéis de eso."*
- [ ] Definir el **formato de exportación** (PDF, JSON o ambos) y el **modelo de carpetas** en Alfresco.
- [ ] Montar el **buscador por DNI**.
- [ ] Diseñar las **plantillas** de los documentos a partir de los ejemplos que mande Títulos.

**Sección de Títulos**

- [ ] Mandar **ejemplos de certificado bilingüe** y del resto de documentos específicos, para que se
      puedan diseñar las plantillas. Se ofrecieron a rescatarlos de la sede electrónica de Infocan.

**Pendiente de decisión**

- [ ] ⚖️ **Dirección**: corrección masiva de Laurea, sí o no.
- [ ] ⚖️ **Dirección**: permiso a Títulos para mecanizar directamente en Laurea.

## 🕓 Para tener en cuenta más adelante

- ⚠️ **Alfresco.** Títulos avisó de entrada: *"cuidado con el Alfresco, que no funciona"*. Se aclaró
  que el que se usaría es **el nuevo**. Si se va a apoyar ahí el acceso a los expedientes históricos,
  **su fiabilidad deja de ser un asunto menor**: pasa a ser la única puerta a datos que hoy están en
  Infocan.
- ⚠️ **Las "pestañas" de Infocan.** Un mismo expediente puede tener **varias pestañas de título**
  porque las importaciones fallidas generaban una nueva cada vez. Solo una es la buena, y es la que
  se mecanizó a mano. **Al exportar hay que decidir qué pestaña se toma**, o se arrastra el problema.
- ⚠️ **Casuística que la solución no cubre todavía:** el alumno que **cambia de documento de
  identidad**. Ahí el título no se duplica, pero el certificado sí hay que reemitirlo con el DNI
  nuevo, y ese movimiento **se comunica al Ministerio**.
- 📌 **Títulos antiguos en el gestor documental anterior**: existe la vía de recuperar la
  *"cartulina"* de los títulos gestionados desde 2011-2012. Si no se recupera, la diligencia se
  puede emitir de forma genérica *(por extravío o deterioro)* — **no es incorrecto, pero se pierde
  información**.

## ❓ Puntos abiertos

- **Formato de la exportación**: PDF, JSON o los dos. Quedó sin cerrar.
- **Si existe realmente la fecha de retirada** en alguna tabla. Es una hipótesis de Títulos basada
  en cómo se construyó la pestaña en su día; **nadie lo ha verificado**.
- **Qué pestaña de Infocan se exporta** cuando hay varias.
- **Volumen**: no se cuantificó cuántos expedientes hay ni cuántos están mal migrados. **Para llevar
  esto a Dirección conviene tener el número**, aunque sea aproximado.
- **Ninguna fecha comprometida** para nada de lo anterior.

## ✉️ Borrador de correo — a Dirección

> **Borrador**: no se envía hasta que le des a enviar.
> Es el que de verdad mueve esto. Decide tú el destinatario: Dirección TIC, o Dirección TIC y
> Ordenación Académica juntas.

**Asunto:** Emisión de títulos y certificados de alumnos antiguos — dos decisiones que os pido

```
Hola:

Os escribo después de una reunión con la Sección de Títulos sobre la emisión de
certificados y duplicados de alumnos antiguos. Resumo y os pido dos decisiones.

La situación:

- La Sección de Títulos emite hoy desde Infocan, no desde Laurea, porque en
  Laurea las fechas de fin y las convocatorias no se corresponden con la
  realidad académica. En la migración se usaron fechas estándar de fin de curso
  en lugar de la fecha de acta de la última asignatura aprobada.
- No es marginal: según Títulos, la proporción está invertida y lo excepcional
  es el expediente que sale bien.
- No es estético: los títulos están regulados por ley y se comunican al
  Ministerio. Un certificado con una fecha distinta de la registrada no se puede
  emitir.
- Es coste diario. Los duplicados se piden a diario, al alumno le cuestan más de
  300 euros y el plazo es de 3 a 5 días hábiles. Además, en Laurea no consta si
  el alumno retiró el título, que es justo el dato que decide si procede un
  duplicado o una modificación interna.

Lo que ya estamos haciendo: exportar el expediente completo de Infocan a un
formato consultable, guardarlo en Alfresco con una carpeta por alumno y darle a
Títulos un buscador por DNI. Eso resuelve el acceso, y nos permite no depender de
que Infocan siga vivo.

Lo que NO resuelve, y por eso os escribo: el expediente de Laurea hay que seguir
corrigiéndolo uno a uno, porque el envío al Ministerio va por ahí.

Os pido dos decisiones:

1. Si corregimos Laurea de forma masiva. La fecha de fin es recalculable a partir
   de la fecha de acta de la última asignatura aprobada. La alternativa es asumir
   la consulta dual de forma indefinida.
2. Si damos a la Sección de Títulos permiso para mecanizar directamente en Laurea
   lo que localicen. Hoy dependen de que otra persona les corrija cada expediente,
   y eso es lo que alarga los plazos.

Quedo a vuestra disposición para verlo con más detalle.

Un saludo,
Pilar
```

## 🔗 Enlaces

- Transcripción cruda: `_secretos/Transcripciones/2026-09-30 - Migracion Infocan a Laurea - emision de titulos y certificados.md` *(no sube a GitHub)*
- Nota en Zoom My Notes: https://us01docs.zoom.us/doc/RJ0mmZ4ASwW4RqGVsTtQvg
- [[2026-09-29 - Nuevo proceso en sede - certificado B2 de Primaria]] — *la reunión de ayer, donde ya salió este mismo problema como dependencia*
- [[30-09-2026]] · [[Producto (Área)]] · [[Cronograma de proyectos (hasta dic 2026)]]
