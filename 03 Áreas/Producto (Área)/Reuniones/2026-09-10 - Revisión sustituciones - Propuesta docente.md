---
tipo: reunión
fecha: 2026-09-10
hora: 11:41–13:14
proyecto: "[[Producto (Área)]]"
convoca: Pilar Campoy
asistentes: [Pilar Campoy, Francisco Javier Molina Sotomayor, José Alberto Moreno Moñino, Carmen Botía, Pablo Gallardo, jfpoma, pjulian]
estado: acta
transcripcion: "_secretos/Transcripciones/2026-09-10 - Revision sustituciones - Gestion propuesta docente.md"
confluence:
jira:
tags: [reunión, requisitos, propuesta-docente, sustituciones, laurea]
---
# Revisión de sustituciones — Gestión de propuesta docente

> **La convocas tú**, así que esto **sí es el acta oficial**. Sala de trabajo TIC + Meet, grabada
> en Zoom en paralelo.
>
> ⚠️ **La transcripción no distingue quién habla**: Zoom atribuyó las 499 intervenciones a Pilar.
> Lo que sigue va por **roles** (Ordenación de Profesorado / Recursos / TIC). Hay además tramos
> con errores de reconocimiento y algunos en otros idiomas, marcados donde afecta.

## 🎯 Objetivo

Revisar con los usuarios finales el **módulo de bajas y sustituciones** que ha desarrollado Pablo,
validar cómo se registran las horas y **cerrar qué columnas necesita el Excel de salida** para
poder calcular nóminas y los informes de ANECA.

## ✅ Decisiones

### Protección de la propuesta docente

1. **La propuesta docente no se toca. Bajo ningún concepto.** Se reafirma la norma y se pide que
   conste: si alguien la modifica, **hay rastreo y se sabe quién ha sido**.
2. Se pide **un nivel de protección por permisos**, no solo el acuerdo: que el sistema impida el
   error humano en vez de confiar en que nadie toque.
   - **El motivo es técnico, no de disciplina:** el servicio de actualizaciones de Laurea deja de
     funcionar si se ha tocado la propuesta por debajo. Un error humano rompe el volcado.

### Notificaciones de bajas

3. **Baja definitiva → correo a todos los coordinadores** de los planes afectados.
4. **Baja temporal → correo solo a los coordinadores del semestre afectado.** Se descartó avisar a
   todos: si a alguien se le sustituye un día y da clase en 15 titulaciones, mandar 15 correos hace
   que nadie los lea. *"Un exceso de correos no se le hace caso."*
   - Para saber el semestre se usa la **fecha de inicio del segundo cuatrimestre**, que debería
     estar en Laurea *(a confirmar con Almudena; si no, se mete a mano)*.
   - Regla práctica: el primer semestre acaba en diciembre, el segundo va de principios de febrero
     a finales de junio.
5. **Recordatorio periódico** a los coordinadores con sustituciones pendientes de revisar: **cada 3
   días o cada semana**.
6. Texto del correo: *"esta persona tiene un proceso de sustitución abierto, confirme o compruebe
   que no está afectado"* — puede que necesite sustituto o puede que no.
7. Se valoró que el coordinador **decida si notifica al resto** cuando el periodo es muy corto, y
   se dejó como opción a definir.

### Visibilidad de profesores de baja

8. **Baja temporal → el profesor sigue apareciendo** en las listas de asignación, con un símbolo
   que lo indique.
9. **Baja definitiva → deja de aparecer** a partir de la fecha en que es efectiva. Ya no se puede
   asignar.
10. **Al replicar la propuesta del año siguiente**, quien tuvo baja definitiva **no aparece**, salvo
    que tenga una **situación contractual activa en Laurea**. Si se le quiere meter como
    conferenciante, tiene que estar dado de alta con contrato.
11. **La excedencia es temporal, no definitiva.** Al incorporarse se abre una nueva asociación
    contractual.
12. Los **conferenciantes se dan de baja por año**. *(Salió a colación un aviso de Protección de
    Datos por una ficha con fecha de fin de contrato en 2099 que hacía aparecer a la persona en
    todas partes.)*

### Cómo se registran las horas de una sustitución

13. **Dos registros por sustitución**, sobre la misma asignatura:
    - **El sustituido**, con las **horas reales** que ha impartido (ej. 28)
    - **El sustituto**, con las **horas asumidas** (ej. 2)
14. **El total de horas del plan no se toca.** No se resta ni se duplica: si eran 30, siguen siendo
    30 entre los dos registros.
15. **Las horas de sustitución van en su propia fila y columna**, separadas de las reducciones.
    - **El motivo es de dinero:** si no se distinguen, al tirar las horas de un plan salen más horas
      impartidas de las reales, y eso desvirtúa los informes de **ANECA** y el cálculo de pagos.
16. **Se elimina el campo de horas de asistencia / "impartida fuera".** Era solo informativo, lo
    rellenaban los profesores a su criterio y **no era fiable**. *"No nos fiamos de que fuera un
    dato real."*
17. Se añade un **check** para el caso de que la asignatura ya se haya dado y no haga falta
    sustituto: se queda quien está.
18. **Una sustitución ya registrada se puede modificar**: si la baja se alarga, se reabre la misma
    solicitud y se cambian fechas, horas o incluso el sustituto. Puede haber más de uno.
19. Al entrar al plan docente, la asignatura afectada muestra un **icono de información** con el
    estado y **las fechas de la baja y el nombre del sustituto**.
20. La baja se puede generar **desde varios sitios**: desde el módulo y también desde la gestión de
    docentes, buscando al profesor. *"Todos los sitios donde aparezcan los profesores."*

### El Excel de salida — columnas nuevas

21. Se añaden estas columnas, y el motivo es que **cada hora se paga a un precio distinto**:
    | Columna | Para qué |
    |---|---|
    | **Idioma** (inglés / español / …) | La docencia en inglés se paga a otro precio |
    | **Ubicación / sede** | Madrid y Andalucía van a otro precio |
    | **Modalidad** (presencial / semipresencial) | Precio distinto |
    | **Sustitución (sí/no)** | Para poder filtrar y no duplicar el cómputo de horas |
    | **Cabecera de primer / segundo semestre** | La mayoría de profesores solo dan en uno |
22. **Poder filtrar por "sustituido" y "sustituto"** por separado, no solo por sustitución.
23. **Dos Excel distintos**, no uno: uno para **Ordenación de Profesorado** y otro para
    **Recursos**, cada uno con las columnas que necesite. Ahora los macrogrupos salen en un solo
    fichero y no sirve para nadie.
    - TIC manda una **propuesta de columnas** antes de tocar nada, porque quien tiene el Excel
      enchufado a sus cálculos se lo rompe si se cambia el orden.
    - Se pregunta también **qué columnas actuales NO se usan** (p. ej. la de reducciones), para
      poder quitarlas.

## ⚠️ Riesgos y problemas abiertos

### La dependencia de Laurea (el de fondo)

- **Los códigos de asignatura y de grupo se repiten entre planes** en la UCAM: "Cálculo" tiene el
  mismo código en 4 o 5 planes, y "Grupo 1" es el mismo en toda la universidad. **El servicio de
  Laurea no distingue a nivel de plan de estudios**, así que si se modifica el Grupo 1 de una
  asignatura en Murcia y en Cartagena, se pisan entre sí.
- Está **resuelto al 99,9 %**, pero se dejó claro que **99,9 no basta**: *"un 0,1 puede suponer una
  contratación o una no contratación"*.
- Ese servicio **está hecho para la estructura de otra universidad**, no para la de la UCAM, y se
  advirtió al contratar. Los casos que fallan son excepciones que allí no se dan.
- **Se está esperando un servicio de Baleares** para tener control propio sobre la gestión de datos.
  Llegará *"cuando Laurea quiera"*: la UCAM no es cliente preferente, aunque pague.
- Síntoma real: **unos usuarios ven datos que otros no ven** (caso de los grupos 40 en asignaturas
  de Ciencias Religiosas, con macrogrupos y plan propietario).

### El error silencioso de volcado

- **Caso concreto del plan 8/6/9:** se quitó un profesor y se puso otro. **La aplicación dice que
  se ha volcado a Laurea, pero en Laurea el cambio no está.** La sospecha es que **tiene acta
  generada**, igual que pasaba con el BOE.
- **El problema es que Laurea no devuelve un error**, así que TIC no puede avisar. Hay que
  comprobar si el servicio devuelve algo que se pueda categorizar.
- Si lo devuelve: mostrar un aviso del tipo *"póngase en contacto con el Servicio de Actas"*, que
  es quien lo resuelve a mano. Si no lo devuelve, habrá que consultar actas directamente.
- Hay un **segundo caso** en el mismo plan: en vez de quitar al profesor añadieron uno más, y **no
  se puso el check de acta**, así que el acta no se generó.

## 📌 Acciones

### Pablo

- [ ] **Investigar si Laurea devuelve error** cuando no puede hacer la sustitución por tener acta
      generada, y si se puede **categorizar** ese error
- [ ] **Añadir el nuevo tipo de fallo al listado de errores** controlados
- [ ] Corregir el caso del **plan 8/6/9** *(hay que abrir el plan también para el otro cambio, el de
      la asignatura a la que no se puso el check de acta)*
- [ ] Implementar la **fila y columna de sustituciones**, separada de reducciones
- [ ] **Quitar el campo de horas de asistencia**
- [ ] **Recordatorio periódico** a coordinadores y **filtro de correo por semestre**
- [ ] **Ocultar a los profesores con baja definitiva** en las listas de asignación

### TIC / equipo

- [ ] **Mandar la propuesta de columnas del Excel** a Ordenación de Profesorado y a Recursos, para
      que cada uno diga qué quita y qué pone
- [ ] Preparar **dos Excel diferenciados** en vez del macro actual

### Pilar

- [ ] **Coger a Alex y redefinir el proceso de solicitudes de contratación**, con quien lo va a
      usar. Hoy es un **cuello de botella**: *"una solicitud se genera y nadie se entera"*.
      **Se aborda en octubre.**
- [ ] Confirmar con **Almudena** si la fecha de inicio del segundo cuatrimestre está en Laurea

### Ordenación de Profesorado / Recursos

- [ ] Decir **qué columnas necesitan y cuáles no usan** del Excel actual
- [ ] Recordar a los **secretarios técnicos** que la propuesta docente no se toca

## 🕓 Para tener en cuenta más adelante

- **El proceso de solicitudes de contratación es el melón de octubre.** Pilar lo dijo claro: *"el
  proceso entre medias me da igual; lo que quiero es que al final la solicitud aprobada aparezca en
  tu lista"*. Redefinirlo con quien lo usa, no inventárselo.
- **Rol de visualización para los coordinadores del departamento de Idiomas transversales**: quedó
  aparcado, "eso ya llegará en el futuro".
- **Permisos de los secretarios técnicos**: se pidió uno y quedó a medias.
- **Queda pendiente definir cuántas horas son un crédito** en cada caso — se mencionó y no se cerró.
- Cuando llegue el **servicio de Baleares**, habrá que replantear cuánto de esto se puede gestionar
  en casa en vez de depender del servicio de Laurea.

## ❓ Puntos abiertos

- ¿**Laurea devuelve error** o no cuando hay acta generada? De la respuesta depende si se puede
  avisar al usuario o hay que ir a mirar actas a mano.
- **Cómo identificar las horas de sustitución en el Excel** de forma que se puedan filtrar sin
  romper los cálculos de quien ya lo tiene montado.
- Si el coordinador debe poder **decidir a quién notifica** cuando el periodo de baja es muy corto.
- Un tramo sobre **activar/desactivar asignaturas** al crear la sustitución (si un profesor tiene 15
  asignaturas y solo se sustituye una) quedó sin cerrar: se concluyó que **cuanto menos haya que
  tocar, mejor**, pero no se decidió el comportamiento por defecto.

## ✉️ Borrador de correo a los asistentes

> **Convocaste tú**, así que esto sí es el acta. **Borrador: no se envía hasta que le des a enviar.**

**Para:** Francisco Javier Molina, José Alberto Moreno, Carmen Botía, Pablo Gallardo, y el resto de asistentes
**Asunto:** Acta de la reunión de sustituciones — y las columnas del Excel que necesito que me confirméis

```
Hola a todos,

Os paso el acta de la reunión de esta mañana sobre el módulo de bajas y
sustituciones. Si algo no está como lo entendisteis, decídmelo.

Lo que decidimos:

- La propuesta docente no se toca. Vamos a añadir además una protección por
  permisos, para que no dependa de que nadie se equivoque: si se toca por
  debajo, el servicio de actualizaciones de Laurea deja de funcionar.
- Bajas definitivas: correo a todos los coordinadores afectados.
- Bajas temporales: correo solo a los coordinadores del semestre afectado.
  Si a alguien se le sustituye un día y da clase en quince titulaciones, no
  tiene sentido mandar quince correos.
- Añadimos un recordatorio periódico, cada tres días o cada semana, a los
  coordinadores que tengan sustituciones pendientes de revisar.
- Un profesor con baja definitiva deja de aparecer para nuevas asignaciones
  desde la fecha de efecto. Con baja temporal sigue apareciendo, marcado.
- Al replicar la propuesta del año siguiente, quien tuvo baja definitiva no
  aparece salvo que tenga contrato activo en Laurea.
- Cada sustitución genera dos registros sobre la misma asignatura: el
  sustituido con sus horas reales y el sustituto con las que asume. El total
  del plan no se toca.
- Las horas de sustitución van en su propia fila, separadas de las
  reducciones, para que al tirar las horas de un plan no salgan más de las
  reales. Esto es lo que estaba desvirtuando los informes.
- Quitamos el campo de horas de asistencia: era informativo y no era fiable.

Lo que necesito de vosotros:

Vamos a preparar dos Excel distintos, uno para Ordenación de Profesorado y
otro para Recursos, en vez del macro actual que no le sirve del todo a
nadie. Os mandaremos una propuesta de columnas antes de tocar nada, porque
sé que hay gente que lo tiene enchufado a sus cálculos y un cambio de orden
se lo rompe.

Las columnas nuevas que apunté son: idioma, ubicación o sede, modalidad
presencial/semipresencial, una que marque si el registro es una sustitución,
y cabecera de primer y segundo semestre. El motivo es que cada hora se paga
a un precio distinto y ahora mismo no hay forma de distinguirlas.

Cuando os llegue la propuesta, decidme qué falta y también qué columnas de
las actuales no usáis, para poder quitarlas.

Un caso que dejamos abierto: en el plan 8/6/9 hicimos un cambio de profesor
que la aplicación da por volcado y en Laurea no está. Sospechamos que es por
tener acta generada. Pablo va a mirar si Laurea nos devuelve algún error que
podamos capturar; si no, habrá que avisar de que se contacte con el Servicio
de Actas. Mientras tanto, Fran lo corrige a mano.

Y lo de las solicitudes de contratación lo abordamos en octubre: quiero
sentarme con quien lo usa y redefinir el proceso, porque hoy es un cuello de
botella y se generan solicitudes de las que nadie se entera.

Un saludo,
Pilar
```

## 🔗 Enlaces

- Transcripción cruda (Drive institucional, no sube a GitHub):
  `_secretos/Transcripciones/2026-09-10 - Revision sustituciones - Gestion propuesta docente.md`
- [[10-09-2026]] · [[Producto (Área)]] · [[Equipo (Área)]]
- [[2026-09-10 - Prácticas Educación 26-27]] · [[Pendientes - Septiembre 2026]]
