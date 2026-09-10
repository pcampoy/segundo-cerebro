---
tipo: reunión
fecha: 2026-09-10
hora: 09:48–10:48
proyecto: "[[Producto (Área)]]"
convoca: María Dolores "Dolo" Saravia Alarcón (SOIL)
asistentes: [Dolo Saravia, Esther Puerto, Elena Cuevas, Cristina Hernández, Pilar Campoy, Alejandro Sánchez, Alex Aix, Juanma Mascarell, Paco Torrecillas]
estado: acta
transcripcion: "_secretos/Transcripciones/2026-09-10 - Reunion Practicas Educacion.md"
confluence:
jira: GES-192
tags: [reunión, requisitos, practicas, educacion, prado]
---
# Prácticas Educación 26-27 — configuración y restricciones de la aplicación

> **Convocada por Dolo (SOIL)**, presencial en *M_0_R01 Monast. S. Reuniones Planta Baja 1* + Meet,
> de 09:30 a 11:00. Pilar grabó en Zoom en paralelo para poder sacar los requisitos.
>
> ⚠️ **La transcripción no distingue quién habla.** Al ser presencial con un solo micro, Zoom
> atribuyó **las 254 intervenciones a Pilar**. Lo que sigue va por **roles** (Educación / SOIL /
> TIC): atribuir una frase a una persona concreta sería inventar. La transcripción automática
> además tiene errores de reconocimiento notables — los tramos dudosos están marcados.

## 🎯 Objetivo

Enseñar a Educación la aplicación nueva de **elección de centros de prácticas** —la que ya usa
Enfermería—, **incluida la vista del alumno**, que nunca habían visto, y cerrar la configuración y
las **restricciones de funcionamiento** para Grado y Máster antes de abrirla a los alumnos.

## 📅 Calendario acordado

| Fecha | Qué |
|---|---|
| **10 de octubre** | La **parte básica** tiene que estar terminada. Ese día "todos probando" |
| **25 de octubre** | Objetivo de poder conectar ya con los alumnos · pruebas terminadas |
| **27 de octubre** | **Descarga de Prado** |
| **28 de octubre** | **Apertura para los alumnos** |

Se hará **un acto/evento para confirmar las fechas definitivas**.

> ⚠️ **Ojo, aquí hay un desajuste sin resolver:** se habló del **25** como fecha de conexión con
> los alumnos y del **28** como apertura. Habría que fijar cuál es la buena.

Al margen: **Prado cierra el 29 de septiembre para grados y el 6 de octubre para el Máster de
Profesorado** (hasta esa fecha los tutores aún pueden darse de alta para ofertarse).

## ✅ Decisiones

### Criterios de asignación

1. **Grado: solo nota media.** No se pondera por créditos superados. *(Enfermería sí pondera nota
   y créditos; Educación expresamente no.)*
2. **Máster: nota media del expediente**, y además **fecha de preinscripción**, que va **separada
   por especialidades** porque son códigos distintos. El de un 9 va primero.
3. La matrícula ya viene filtrada por Secretaría General: sin los créditos mínimos no se puede
   matricular, así que no hace falta controlarlo en la aplicación.

### Certificado de delitos sexuales

4. **Sin el certificado subido, el alumno no puede seleccionar plaza.** Se le muestra un mensaje
   claro y grande explicando por qué.
5. La comprobación la sigue haciendo **Educación** contra la web del Ministerio con el código del
   certificado — proceso manual y arduo, igual que en Fisioterapia y en todo lo que implique
   contacto con menores.
6. Para no duplicar trabajo: **Educación pasa un fichero (CSV) con DNI o NIA y un sí/no**, y se
   carga de forma masiva. Cuanto más tarde suba el alumno el certificado, menos plazas le quedan.

### Elección de plazas

7. **Todos los alumnos pueden optar a cualquier plaza**, tengan Práctico 1 y 2 o solo uno. "Hay
   que ser justos": el orden lo pone la nota.
8. **El alumno mantiene el mismo centro en Práctico 1 y 2 durante todo el año.** Es la restricción
   principal: el centro del segundo tiene que ser el del primero.
9. **Rango de fechas de Prácticos 1 y 2: del 1 de noviembre al 31 de mayo.** Las ofertas fuera de
   ese rango no se visualizan ni se pueden seleccionar.
10. **Selección mínima y máxima configurable por práctico.** Se manejó *"entre 5 y 30"* y también
    *"mínimo 25"*. El máximo no obliga: si eliges 20 de 60 y te quedas sin plaza, es tu problema.
    **El mínimo sí se puede imponer.**
11. **Al confirmar no hay marcha atrás.** Como en Enfermería: el alumno puede volver a entrar solo
    a consultar. Se recomienda hacerlo desde navegador, no desde el móvil.
12. Se mantiene la **geolocalización** de los centros y la ordenación por prioridad arrastrando.

### Especialidades

13. **Hay que crear 18 especialidades de Máster + 4 de Grado.**
14. **Las especialidades dobles tienen que verse SEPARADAS**, no juntas. Afecta a:
    **Matemáticas / Informática**, **Idiomas** (Inglés, Francés, Alemán), **Administración y
    Comercio / Marketing** y **Biología-Geología / Historia** *(este último, por confirmar: en la
    transcripción queda dudoso)*.
    - **Causa del problema del año pasado:** en el plan de estudios la asignatura va junta con un
      solo código, pero a Prado se le pidió que separase por especialidad. Resultado: **había
      alumnos que no veían sus ofertas**.
    - **Solución:** trabajar con **alias sobre la asignatura**, como ya se hace en Enfermería. Es
      lo mismo que pasó con *Socio-sanitarias* y *Socio-comunitarias*, que se arregló con alias.
15. **Grado y Máster van separados en la aplicación**, filtrando por códigos de título. No se
    mezclan: "como si fuera una aplicación diferente".

### Máster de Enseñanza Bilingüe

16. Este año **duplica plazas y periodos**, con unos **45 alumnos** en centros, y **coincide con la
    especialidad de Inglés de Grado Primaria**.
17. **Educación bloquea nominativamente las plazas de Bilingüe ANTES de que se saque la oferta**, y
    esas plazas **no se publican a los alumnos de Grado Primaria**. Es lo que se viene haciendo
    desde hace un par de años.
18. El bloqueo se hace **a mano por DNI**: son 45, es asumible. Se descartó escalonar por fechas
    (primero Grado, luego Máster) porque **los de Máster se matriculan más tarde**.

### Plazas y periodos

19. **La misma plaza con fechas distintas cuenta como dos plazas.** Si además tiene dos tutores y
    cubre todo el año, la misma oferta sale **cuatro veces** (2 para el periodo A + 2 para el B).
20. **Máster: el periodo prescriptivo es el A**, y el alumno **solo puede elegir una especialidad
    entre A y B**, no ambas.
21. Hay que definir **por cada práctico**: fecha inicial, fecha fin, **grupo** (Murcia / Cartagena)
    y la **descripción de la asignatura del aula virtual**, que va siempre unida al nombre del
    periodo rotatorio. Las horas vienen por defecto de la asignatura.
22. Educación tiene **dos periodos**, no rotatorios como Enfermería: hay que adaptar la
    configuración. TIC ayuda a configurarlo también en Infantil, Primaria y sede de Cartagena.

### Interfaz

23. **Se elimina el turno (mañana/tarde) de la vista del alumno.** Viene de Prado pero **no es
    fiable**, y como el 80 % de los alumnos trabaja, todos pedirían tarde y se genera un problema.
    Se descartó dejarlo visible solo para gestores: **se elimina directamente**.

### Ofertas privadas y asignaciones manuales

24. **La plantilla oficial de Prado no es modificable**, así que se adapta la de la aplicación para
    cargar la **oferta privada**: centros privados, concertados y públicos de otras comunidades que
    no salen en Prado.
25. Esas ofertas llevan un **sello o indicador** que distinga **con convenio / sin convenio**, y
    las que no se seleccionan no tienen por qué aparecer en la oferta del alumno.
26. **Asignaciones manuales:** se podrá **crear una oferta privada y asignarla directamente a un
    alumno**. Es el caso de los ~50-100 alumnos que se buscan el centro por su cuenta y firman
    convenio.
27. Carga por **Excel con plantilla** o centro por centro. **Ahora mismo el límite es de 5
    registros** — hay que ampliarlo para poder subir listas de 20 y más.
28. Los ficheros de carga (alumnos y centros externos) **tienen que venir en el formato CSV
    concreto** de la aplicación. El de Enfermería sirve de ejemplo. **Las columnas no obligatorias
    pueden ir vacías, no pasa nada.**

### Notificaciones

29. **Correo automático al alumno** cuando se hace la asignación: sí, es sencillo.
30. **Al tutor, no** — "ya entramos en protección de datos".

## 📌 Acciones

### Educación / SOIL

- [ ] **Mandar por escrito todas las restricciones y criterios** acordados: criterios de Grado y
      Máster, delitos sexuales, reglas de bloqueo del Máster Bilingüe. *Es la petición expresa de
      Pilar al cerrar: "sobre todo me interesa que estemos todos en consonancia con las
      restricciones".*
- [ ] **Bloquear nominativamente las plazas de Bilingüe** antes de que se saque la oferta de Prado
- [ ] **Adaptar sus ficheros** de carga de alumnos y de centros externos al formato CSV requerido
- [ ] **Pasar el fichero de certificados** de delitos sexuales (DNI/NIA + cumple sí/no)
- [ ] **Definir cada práctico**: fechas, grupos de Murcia y Cartagena, y descripción de asignatura
- [ ] Confirmar el **listado de especialidades** (18 de Máster + 4 de Grado) y las dobles
- [ ] Facilitar el **primer listado de orden de alumnos** (nota media y fecha de preinscripción por
      especialidad) para cruzarlo con el que saque TIC

### TIC (nuestro equipo)

- [ ] **Pasar la plantilla de oferta privada** y el formato de los ficheros de carga
- [ ] **Descargar la oferta de Prado del año pasado de Educación** para adelantarse al problema de
      las especialidades dobles → enlaza con el pendiente ya abierto en
      [[Pendientes - Septiembre 2026]]
- [ ] **Crear las asignaturas prácticas**: 18 especialidades de Máster + 4 de Grado, con grupos,
      descripciones y horas
- [ ] **Configurar periodos y rotatorios** adaptados a los dos periodos de Educación
- [ ] **Configurar selección mínima y máxima** por práctico
- [ ] **Ampliar el límite de 5 registros** en la carga por Excel de asignaciones manuales
- [ ] **Quitar el turno** de la vista del alumno
- [ ] **Implementar el correo automático de asignación** al alumno (no al tutor)
- [ ] **Pruebas con datos del año pasado** antes del 25 de octubre: tirar asignaciones (50/50/50) y
      verificar que las restricciones y la lógica dan el resultado esperado
- [ ] **Sesiones de trabajo conjuntas** en cuanto haya los primeros códigos cargados, para verificar
      pantallas y datos con Educación delante

## 🖥️ Lo que nos toca a nosotros, en una línea

El **10 de octubre** es la fecha que manda: ese día la parte básica tiene que estar en pie para
poder probar. Y de todo lo hablado, **lo único que bloquea de verdad es que Educación mande las
restricciones por escrito**: sin eso, cualquier configuración que hagamos es una interpretación.

## 🕓 Para tener en cuenta más adelante

- **El módulo de tutores es el siguiente frente, y es grande:** hay que asignar **50 tutores a 500
  alumnos**, unos 10 por profesor, publicárselo, y que luego cada tutor **evalúe mediante un
  formulario** casado con la aplicación para tener las notas. **A medio o largo plazo**, y aplica
  también al resto de titulaciones.
- **Pantalla de asignaciones para el alumno:** poder ver a qué centro le han asignado. "No nos va a
  dar tiempo ahora, pero en cuanto podamos lo queremos poner."
- **Descarga de la oferta y de la presentación en PDF** para publicarla, ya que va en varias fases.
- **Notas y certificados dentro de la aplicación**, conectando con la aplicación de notas
  existente y con la Sede Electrónica. *"Esa es la siguiente parte del proyecto."*
- **Banco de datos histórico de centros privados**, que pidió Educación. Haría falta algún dato más
  (fecha desde / fecha hasta, validez).
- **Fisioterapia pidió algo parecido** para evaluación: que el tutor externo entre, evalúe y firme
  con certificado.
- Lo que se vuelca a **Laurea** va automático; lo que no es centro queda por trabajar.

## ❓ Puntos abiertos

- **Las restricciones por escrito** siguen sin llegar. Es el punto crítico.
- **¿25 o 28 de octubre** para abrir a los alumnos? Se dijeron las dos.
- **Biología-Geología / Historia** como especialidad doble: la transcripción es confusa ahí, hay
  que confirmarlo.
- **Si Prado no cierra a tiempo** (29/09 grados, 06/10 máster), habrá que trabajar con la oferta
  del año pasado. Se aceptó explícitamente: *"con la del año pasado me vale"*.
- **Riesgo reconocido:** que los datos de Prado no cuadren con los registros internos. De ahí las
  pruebas comparativas con el año pasado.
- Un tramo sobre **infantil y alumnos que convalidan el Práctico 1 por venir de FP** quedó a medias:
  tendrían que ofertarse de manera distinta, pero no se cerró cómo.

## ✉️ Borrador de correo a los asistentes

> ⚠️ **No convocaste tú esta reunión** — la convocó Dolo. Esto **no es el acta oficial**: son *tus*
> notas, y va redactado como tal. **Borrador: no se envía hasta que le des a enviar.**

**Para:** Dolo Saravia, Esther Puerto, Elena Cuevas, Cristina Hernández, Alejandro Sánchez, Alex Aix, Juanma Mascarell, Paco Torrecillas
**Asunto:** Mis notas de la reunión de Prácticas Educación 26-27 — y las restricciones que necesito por escrito

```
Hola a todos,

Os paso mis notas de la reunión de esta mañana, sobre todo para que
validemos las restricciones antes de que empecemos a configurar. Si me he
dejado algo o he entendido mal alguna cosa, decídmelo y lo corrijo.

Calendario que apunté:

- 10 de octubre: la parte básica tiene que estar terminada, y ese día
  probamos todos.
- 27 de octubre: descarga de Prado.
- 28 de octubre: apertura para los alumnos.

Una duda: hablamos también del 25 como fecha para conectar con los
alumnos. ¿Nos quedamos con el 25 o con el 28?

Restricciones y criterios que entendí, y que es lo que necesito que me
confirméis por escrito:

- Grado: la asignación va solo por nota media, sin ponderar créditos.
- Máster: nota media del expediente y fecha de preinscripción, separada
  por especialidades.
- Sin el certificado de delitos sexuales subido, el alumno no puede
  seleccionar plaza. Vosotros lo comprobáis en la web del Ministerio y nos
  pasáis un fichero con DNI o NIA y un sí/no para cargarlo de golpe.
- Todos los alumnos pueden optar a cualquier plaza, tengan uno o dos
  prácticos. La restricción es que mantengan el mismo centro en el
  Práctico 1 y en el 2 durante todo el año.
- Los prácticos van del 1 de noviembre al 31 de mayo. Lo que caiga fuera
  de ese rango no se les muestra.
- Las especialidades dobles (matemáticas/informática, idiomas,
  administración y comercio) tienen que verse separadas. Lo resolvemos con
  alias sobre la asignatura, como en Enfermería, para que no vuelva a
  pasar lo del año pasado.
- Máster de Enseñanza Bilingüe: bloqueáis las plazas de forma nominativa
  antes de que saquemos la oferta, y no se publican a los alumnos de Grado
  Primaria.
- Quitamos el turno de mañana/tarde de la vista del alumno.
- Al confirmar la selección no hay marcha atrás.

Lo que necesito de vosotros:

- Las restricciones de arriba confirmadas por escrito. Es lo que de verdad
  nos desbloquea.
- El listado de especialidades: 18 de máster más las 4 de grado.
- La definición de cada práctico: fechas, grupos de Murcia y Cartagena, y
  la descripción de la asignatura del aula virtual.
- El fichero de certificados.
- El primer listado de orden de alumnos, para cruzarlo con el que saquemos
  nosotros y comprobar que coincide.

Por nuestra parte os pasamos la plantilla de oferta privada y el formato de
los ficheros de carga, y nos bajamos la oferta de Prado del año pasado para
adelantarnos al tema de las especialidades dobles.

Y como dijimos, en cuanto tengamos los primeros códigos cargados nos
sentamos juntos a revisar pantallas y datos, y hacemos selecciones de
prueba antes de abrir a los alumnos.

Un saludo,
Pilar
```

## 🔗 Enlaces

- Transcripción cruda (Drive institucional, no sube a GitHub):
  `_secretos/Transcripciones/2026-09-10 - Reunion Practicas Educacion.md`
- [[10-09-2026]] · [[Producto (Área)]] · [[Quién es quién (apodos e interlocutores)]]
- [[Pendientes - Septiembre 2026]] · [[Cronograma de proyectos (hasta dic 2026)]]
