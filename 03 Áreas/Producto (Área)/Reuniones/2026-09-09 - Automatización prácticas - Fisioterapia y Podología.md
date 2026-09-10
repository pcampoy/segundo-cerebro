---
tipo: reunión
fecha: 2026-09-09
hora: 10:07–11:37
proyecto: "[[Producto (Área)]]"
convoca: Pilar Campoy
asistentes: [Pilar Campoy, coordinación de Fisioterapia y Podología, equipo de Desarrollo]
estado: publicado
transcripcion: "_secretos/Transcripciones/2026-09-09 - Automatizacion practicas - Fisioterapia.md"
confluence: "https://ucam.atlassian.net/wiki/spaces/GDP/pages/1196392450"
jira: "sin desglosar todavía — objetivo curso 27-28, se planifica en diciembre de 2026"
tags: [reunión, requisitos, practicas, fisioterapia, podologia]
---
# Automatización de prácticas — Fisioterapia y Podología

> **La convocas tú.** Sala de trabajo TIC + Meet, y la grabaste en Zoom en paralelo.
>
> ⚠️ **Dos avisos sobre las fuentes:**
> 1. Zoom atribuyó las 339 intervenciones a Pilar (presencial, un solo micro), así que esto va por
>    **roles**, no por personas. **La lista exacta de asistentes no consta**: el evento del
>    calendario de esa hora llevaba a Educación, y el Zoom se tituló "Fisioterapia". Confirma los
>    nombres antes de enviar el correo.
> 2. Esta acta está montada sobre **tus notas de la reunión y el resumen de Zoom**, que son muy
>    detallados, **no sobre la transcripción literal** — a diferencia de las dos del 10/09. Si
>    quieres que la repase palabra por palabra, dímelo.

## 🎯 Objetivo

Enseñar a **Fisioterapia y Podología** la aplicación de gestión de prácticas que ya funciona en
Enfermería, y empezar a definir cómo se adapta a sus dos grados: automatizar inscripción,
asignación de plazas y certificados, **acabando con las permutas y con la gestión manual**.

## 📅 Calendario: esto va para el curso 27-28

| Cuándo | Qué |
|---|---|
| **Diciembre de 2026** | Reunión de seguimiento: revisar el diseño de procesos y el orden de asignación. **Pilar manda el correo de coordinación** |
| **Antes de fin de año** | Fisio y Podología definen el grafo de procesos, el orden de elección y los criterios de prioridad |
| **Enero de 2027** | Empiezan las pruebas con el feedback recibido y ajustes de configuración |
| **Mayo de 2027** | Contactar con los centros para recopilar oferta de plazas de todo el año |
| **Junio–julio de 2027** | Apertura de prematrículas y configuración de la oferta |
| **Principios de septiembre de 2027** | **Fecha objetivo del despliegue completo** |

Es un plazo cómodo comparado con Educación — pero el trabajo de definición empieza **ahora**, y la
parte que depende de ellos (criterios y orden) vence **en diciembre**.

## ✅ Decisiones

1. **Se adapta la aplicación de Enfermería** a Fisioterapia y Podología. No se hace nada nuevo.
2. **Modelo de asignación por prioridades y turnos**: el alumno ordena sus criterios (especialidad,
   cercanía al domicilio, nota) y el sistema asigna. Se manejaron **cinco categorías** ordenables y
   **tres turnos** de entrada por grupos y periodos.
   - **El objetivo del modelo es garantizar plazas en las especialidades menos populares**, como
     trauma, que si no nadie pide.
3. **No se puede repetir especialidad ya cursada.** Si un alumno hizo urgencias en el Práctico 1, no
   puede pedirla en el 3.
4. **Cada sede y turno es una línea de oferta independiente**, para que el recuento de plazas sea
   exacto.
5. **La asignación está atada a la matrícula formalizada.** Sin matrícula no hay plaza, y **después
   de julio no se pueden hacer más asignaciones**: la matrícula no se manipula fuera de plazo.
6. **Al enviar la selección, queda bloqueada.** Sin cambios posteriores, igual que en Enfermería.
7. **Certificados electrónicos automáticos** a partir de los datos de la aplicación —horas,
   especialidades y periodos completados—, firmados por la dirección del centro. Sustituyen a los
   informes que hoy se hacen a mano.
8. **Formularios estandarizados para tutores externos**, con evaluación y **firma electrónica** del
   proceso.
9. **Volcado a Auria** de la información final, para seguridad social y expedientes.
10. **Permisos jerárquicos** en la aplicación: por facultad, por estudio y por plan de estudios.
    *(Ejemplo que salió: Ana María es coordinadora de facultad y de Enfermería, pero no lleva las
    prácticas de máster — el permiso tiene que poder distinguirlo.)*
11. **Prueba piloto con un grupo reducido**, del orden de **50 alumnos**, antes del lanzamiento
    general.
12. **Contactar con los centros desde mayo**, no en verano. Los que no respondan a tiempo se quedan
    **en reserva** hasta la siguiente ampliación de matrícula.
13. Solo prácticas **curriculares**. Las extracurriculares se seguirán gestionando aparte.

## 📌 Acciones

### Fisioterapia y Podología — vence en diciembre

- [ ] **Definir el grafo de procesos**: cómo quieren que funcione de principio a fin
- [ ] **Definir el orden de elección de los alumnos** y los **criterios de prioridad**
- [ ] Decidir el orden en que los alumnos completan sus especialidades

### Pilar

- [ ] **Mandar el correo de coordinación en diciembre** para preparar la revisión del proceso
- [ ] **Consultar a Jesús** si se pueden **leer los metadatos de los certificados de delitos
      sexuales** para validarlos automáticamente. Hoy el alumno los sube por formulario y **el
      sistema no puede leerlos**, así que la comprobación es manual
- [ ] **Pasar la plantilla de la oferta del año pasado** para poder hacer pruebas
- [ ] **Coordinar con planificación académica** para adelantar los plazos de matrícula, y que los
      alumnos estén dados de alta antes del proceso de asignación
- [ ] Preparar **material de explicación para los alumnos** sobre el nuevo proceso
- [ ] **Campaña en enero** para los alumnos de segundo sobre el certificado de delitos sexuales

### TIC / equipo

- [ ] Completar **generación de certificados electrónicos** e **integración con Prado JS**
- [ ] Desarrollar el **formulario de tutores externos** con firma electrónica
- [ ] Implementar la **jerarquía de permisos** (facultad / estudio / plan)

## 🖥️ Lo que nos toca a nosotros

Nada urgente **esta semana**: la fecha objetivo es septiembre de 2027. Lo que sí es de ahora es
**la consulta a Jesús sobre los metadatos de los certificados**, porque es la misma pieza que salió
en la reunión de Educación del 10/09 — allí también se busca cómo minimizar esa comprobación
manual. **Es un requisito compartido por Educación, Enfermería y Fisioterapia**: merece resolverse
una vez.

## 🕓 Para tener en cuenta más adelante

- **La firma electrónica es el riesgo blando del proyecto:** puede que tutores externos no sepan o
  no quieran usarla, y eso retrasa la certificación. Hay que simplificarlo al máximo o tener un
  plan B.
- **El retraso en subir actas de notas bloquea la matriculación**, y sin matrícula no hay
  asignación. Es una dependencia externa que hay que vigilar.
- **Si faltan plazas en una especialidad**, habrá que asignar por criterios mínimos o de forma
  aleatoria. Conviene decidir la regla antes de que pase.
- **Zonas problemáticas identificadas**: Cataluña, Asturias, Navarra y Galicia. Con el proceso
  actual, conseguir plazas allí supone medio año de trabajo extra.
- **Alumnos Erasmus** que hacen exámenes en verano: los criterios de matrícula hay que ajustarlos
  para ellos.
- El **80 % de los centros** ya había respondido sobre plazas disponibles cuando se celebró la
  reunión.
- Referencia del calendario de Enfermería, por si sirve de patrón: las plazas se abren el **12 de
  julio**, los alumnos tienen **dos días** para elegir, y el proceso se cierra antes del **8 de
  septiembre**.

## ❓ Puntos abiertos

- **Quién estuvo exactamente en la reunión.** No consta la lista; hay que confirmarla antes de
  mandar el correo.
- **Si se pueden leer los metadatos de los certificados** de delitos sexuales — pendiente de Jesús.
- **Qué pasa cuando un alumno no obtiene ninguna de sus opciones.** Se habló de la probabilidad y
  de cómo tratar los casos restantes, pero no se cerró la regla.
- Cómo encaja la **verificación de seguridad social** en el flujo.

## ✉️ Borrador de correo a los asistentes

> **Convocaste tú**, así que es el acta. ⚠️ **Confirma antes la lista de destinatarios**, que en
> esta reunión no consta. **Borrador: no se envía hasta que le des a enviar.**

**Para:** *(por confirmar — coordinación de Fisioterapia y Podología)*
**Asunto:** Acta de la reunión de automatización de prácticas — Fisioterapia y Podología

```
Hola a todos,

Os paso el acta de la reunión del miércoles, en la que vimos cómo funciona
la aplicación de prácticas que ya usamos en Enfermería y empezamos a
definir cómo la adaptamos a Fisioterapia y Podología. Si algo no está como
lo entendisteis, decídmelo y lo corrijo.

La idea de fondo: adaptar lo que ya tenemos, no hacer nada nuevo, para
automatizar la inscripción, la asignación de plazas y los certificados, y
quitarnos de encima las permutas y la gestión manual.

Lo que decidimos:

- La asignación va por prioridades y turnos: el alumno ordena sus criterios
  (especialidad, cercanía, nota) y el sistema asigna. Así garantizamos que
  las especialidades menos demandadas, como trauma, no se queden vacías.
- Un alumno no puede repetir una especialidad que ya haya cursado en un
  periodo anterior.
- Cada sede y cada turno son una línea de oferta independiente, para que el
  recuento de plazas sea exacto.
- La asignación va atada a la matrícula formalizada, y después de julio no
  se pueden hacer más asignaciones.
- Cuando el alumno envía su selección, queda bloqueada.
- Los certificados pasan a ser electrónicos y automáticos, con los datos de
  la aplicación, firmados por la dirección del centro.
- Los tutores externos tendrán un formulario estandarizado con firma
  electrónica para la evaluación.
- Los permisos serán jerárquicos: por facultad, por estudio y por plan.
- Antes del lanzamiento haremos una prueba piloto con unos 50 alumnos.

El calendario que planteamos:

- Diciembre: os escribo para vernos y revisar el diseño de los procesos.
- Antes de fin de año: necesito de vosotros el grafo de procesos, el orden
  de elección de los alumnos y los criterios de prioridad. Es la parte que
  no puedo hacer yo.
- Enero: empezamos las pruebas con vuestro feedback.
- Mayo: contactamos con los centros para recoger la oferta de todo el año.
  Este año conviene adelantarlo: los que no responden a tiempo nos dejan
  medio año de trabajo detrás.
- Junio y julio: prematrículas y configuración de la oferta.
- Principios de septiembre de 2027: en marcha.

Dos cosas que quedan en el aire y que iré moviendo yo:

- Voy a consultar con Jesús si podemos leer automáticamente los metadatos
  de los certificados de delitos sexuales. Hoy el alumno los sube y la
  comprobación es manual, y es un problema que tenemos igual en Enfermería
  y en Educación, así que merece resolverse una sola vez.
- Hay que hablar con planificación académica para adelantar los plazos de
  matrícula, porque sin alumnos matriculados no podemos asignar.

Un saludo,
Pilar
```

## 🔗 Enlaces

- Transcripción cruda (Drive institucional, no sube a GitHub):
  `_secretos/Transcripciones/2026-09-09 - Automatizacion practicas - Fisioterapia.md`
- [[09-09-2026]] · [[Producto (Área)]]
- [[2026-09-10 - Prácticas Educación 26-27]] — **mismo proyecto, `GES-192`**, y comparten el
  problema del certificado de delitos sexuales
