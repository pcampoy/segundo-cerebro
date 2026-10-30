---
tipo: dossier
fecha: 2026-11-02
hora: 09:00–10:00
proyecto: Gestión de la Docencia (GD)
convoca: María Mendoza
asistentes: [María Mendoza, Miguel Ángel, Pilar Campoy]
fuentes: Jira GD (consultado el 30/10/2026) · notas del vault desde el 04/09
tags: [dossier, gestion-docencia, propuesta-docente]
---
# Aplicativo docente — dossier para el lunes 2/11

> **Lunes 2/11, 09:00–10:00, Meet.** La convoca María Mendoza, con Miguel Ángel. **No hay acta posible**
> (no la convocas tú): al salir, dicta un resumen de 3 min por el canal `n:`.
>
> ⚠️ **Pisa el Seguimiento Sprint de las 09:15**, que además cierra el `2026/17`. Sigue sin moverse.
>
> Datos de Jira del **30/10/2026**. **Confluence no lo he vuelto a mirar** desde la revisión del 08/09.

## En una frase

**Desde septiembre se ha apagado el fuego y se ha cerrado Bajas y Sustituciones, pero los módulos nuevos
están parados**: Investigadores y Conferenciantes no se tocan desde el 06/10, y Ámbitos de conocimiento
sigue sin existir en Jira. Ámbitos es justo el que le importa a María (su cliente es RRHH).

## ✅ Lo que está hecho (desde el 08/09)

| Bloque | Qué se ha hecho | Estado |
|---|---|---|
| **Incidente del volcado** (las ~10.000 h perdidas) | Recuperadas las asignaciones perdidas del curso 2026, cortado el borrado masivo, auditoría y traza de borrados, reintentos y visibilidad de los rechazos de Laurea, volcado por estudio sin cruzar centros. Después, una tanda de planes atascados en pre-volcado resueltos uno a uno (Enfermería Cartagena, Psicología, Máster en Fisioterapia, Tecnología de los Alimentos…) | ✅ Épicas `GD-656` y `GD-657` **cerradas el 29/10** |
| **Bajas y sustituciones** | Lo que se decidió el 10/09 con Profesorado: horas de sustitución separadas, campo de asistencia retirado, acceso del coordinador solo a sustituciones, correos de baja registrada y recordatorio a coordinadores, modificar una baja ya validada, indicador de si la baja está volcada, nombre del sustituto en la gestión de horas | ✅ Épica `GD-596` **cerrada el 29/10** |
| **Reducciones** | Módulo terminado, más dos errores corregidos (editar y eliminar reducciones duplicadas) | ✅ Épica `GD-539` cerrada el 29/10 *(confirmado por Pablo el 30/10)* |
| **Rediseño visual** | Rediseño de la interfaz | ✅ Épica `GD-619` cerrada el 29/10 *(confirmado por Pablo el 30/10)* |
| **Pendientes del 10/09** | Protección por permisos de la propuesta docente · profesores con baja definitiva ocultos en las listas de asignación · control del error de Laurea con acta generada · dos Excel separados (Ordenación de Profesorado y Recursos) | ✅ *(confirmado por Pablo el 30/10)* |
| **Seguridad** | Migración completa al servicio central de seguridad (selector de rol, auditorías de sustituciones adaptadas a la identidad nueva), desplegada en desarrollo, preproducción y producción | ✅ Todas las tareas hechas |
| **Informes** | Listado de profesorado por facultad con créditos y % de dedicación (entregado a Miguel Ángel el 09/10) · servicio para exportar el Excel de horas por lista de planes · Excel de profesores corregido (reducciones y horas del módulo, sin solicitudes pendientes) | ✅ |
| **Demo** | Vídeo con todas las funcionalidades, en lugar de capturas | ✅ 29/10 |
| **Soporte** | Una docena de errores de producción resueltos (accesos de revisor y coordinador, propuesta del plan 869, Idiomas I/II…) | ✅ |

**El mensaje para María:** el núcleo está en producción, el incidente del verano está cerrado con
trazabilidad de borrados, Bajas y Sustituciones y Reducciones están terminados, y todo lo que se acordó
con Profesorado el 10/09 está hecho.

## 🔨 En curso ahora (sprint `2026/17`, acaba el lunes)

- `GD-763` — **un profesor que deja la universidad a mitad de curso deja su plan en pre-volcado** sin
  volcar sus horas. **Es lo único que le queda a Pablo** (30/10). Mejor que lo cuentes tú antes de que
  salga en la reunión.
- `GD-762` — un grupo de examen creado en GD que no existe en Laurea (plan 869). Jira lo da en curso; no
  se le preguntó a Pablo.
- *(Bajo el paraguas de GD, pero no es GD: la migración y mejoras de Reconocimientos previos, `GD-748/749`.)*

## ⏳ Lo que queda pendiente

### Módulos nuevos — el punto flojo

| Módulo | Para quién | Situación |
|---|---|---|
| **Investigadores** | RRHH, Investigación, Profesorado | 21 historias: **0 terminadas**, 4 en pruebas, 3 en curso, 14 sin empezar. **Sin movimiento desde el 06/10** y fuera de los sprints `2026/16` y `2026/17`. Comprometido "hasta diciembre" |
| **Conferenciantes** | Profesorado | **Avance desde septiembre:** ya tiene épica (`GD-682`, 28/09) y 7 historias. Solo el análisis está empezado, también **parado desde el 06/10** |
| **Ámbitos de conocimiento** | **RRHH**, coordinadores, dirección académica | 🔴 **Sigue sin épica ni historias.** PRD y prototipos validados en marzo; el lanzamiento estaba previsto para el 31/05. Es el más delicado con María |

### Lo que quedó del 10/09 (sustituciones)

- La parte de Pablo está **hecha** (ver arriba). Queda **apuntar en Jira** esos cambios, que no tienen tarea.
- **Tuyo:** redefinir el **proceso de solicitudes de contratación** con Alex — *"el melón de octubre"* — y
  octubre se acaba hoy. **Tuyo:** confirmar con Almudena la fecha del segundo cuatrimestre en Laurea.

### Arrastrados

- **Almacén de datos de RRHH** (`GD-493…499`): 7 tareas creadas en mayo, sin tocar.
- **Plantillas de planificación** (`GD-25`, desde julio de 2024) y las **fotos de usuarios** (`GD-214`):
  candidatas a cerrarse.
- **Confluence:** en septiembre el Home era la plantilla por defecto y el cronograma estaba congelado
  en febrero. Sin revisar desde entonces.

### Dependencias externas

- **Laurea**: el servicio no distingue por plan de estudios (99,9 % resuelto, y *"un 0,1 puede suponer
  una contratación"*). A la espera del **servicio de Baleares**, sin fecha.
- **Ediciones de plan en Laurea**, para el curso 27-28: decisión de cartera con Miguel Ángel.

## ❓ Dudas que aclarar antes o durante

1. ~~¿Por qué se cerraron el 29/10 las épicas de Reducciones y de Rediseño visual?~~ **Resuelto:**
   están terminadas (Pablo, 30/10).
2. **Higiene de Jira:** hay épicas cerradas con hijas abiertas (`GD-763` en Bajas, `GD-762` en Integridad)
   y la épica de seguridad sigue "por hacer" con todo terminado. No es para la reunión.
3. **¿Francisco está fuera de Investigadores a propósito?** Si se le ha llevado a otra cosa, el
   "hasta diciembre" ya no vale y hay que decirlo en la reunión.

## 🎯 Lo que yo llevaría a la reunión

- **Lo bueno, primero:** incidente cerrado, sustituciones y reducciones terminadas, rediseño hecho,
  propuesta docente protegida por permisos, seguridad migrada, y el vídeo para enseñarlo.
- **Lo único abierto de Pablo:** las bajas de profesores que dejan la universidad a mitad de curso. Cuéntalo
  tú, con fecha si la tienes.
- **Ámbitos de conocimiento, sin esconderlo:** o se retoma (con épica, sprint y fecha) o se aparca y se
  le dice a RRHH. María es la persona a quien decírselo.
- **Investigadores:** fecha realista, no "diciembre" por inercia, con 0 de 21 historias cerradas.
- **Pídeles lo que es suyo:** el criterio de ordenación de ámbitos (Profesorado) y quién redefine las
  solicitudes de contratación.
- El **summary para María** sigue bloqueado desde el 08/09 (faltan los pasos de repasar Jira y etiquetar):
  esta reunión puede sustituirlo, o servir para comprometer una fecha de entrega.

## 🔗 Enlaces

- [[2026-09-08 - Revisión del proyecto Gestión de la Docencia]] · [[2026-09-08 - Summary Gestión de la Docencia (María Mendoza)]]
- [[2026-09-10 - Revisión sustituciones - Propuesta docente]] · [[2026-09-04 - Criterios de implantación de modificaciones de planes]]
- [[Cronograma de proyectos (hasta dic 2026)]] · [[Producto (Área)]]
