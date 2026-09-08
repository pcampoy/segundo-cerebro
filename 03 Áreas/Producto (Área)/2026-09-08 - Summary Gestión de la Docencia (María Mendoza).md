---
tipo: entregable
fecha: 2026-09-08
destinatario: María Mendoza García
proyecto: Gestión de la Docencia (GD)
estado: borrador — pendiente de revisión de Pilar
tags: [producto, gestion-docencia, summary]
---
# Summary para María Mendoza — Gestión de la Docencia

> **Registro:** ejecutivo. Sin claves de Jira, sin nombres de tecnologías, sin carga de trabajo
> del equipo. Una página. Ver `_privado\Gerencia UCAM - quien es quien.md`.
>
> ⚠️ **Borrador.** Lo que sale de Jira y Confluence es fiable; **la descripción funcional la he
> reconstruido de la documentación y de tus notas**, así que revisa sobre todo el bloque
> *"Qué es"* y el estado de cada módulo.

---

## GESTIÓN DE LA DOCENCIA — Estado del proyecto
**Septiembre de 2026**

### Qué es

La aplicación con la que la Universidad **planifica y asigna la docencia de cada curso**: qué
asignatura imparte cada profesor, con cuántas horas, y con qué criterios de reparto. Una vez
cerrada la propuesta, la traslada automáticamente al sistema académico (Laurea).

Sustituye un proceso que se sostenía sobre hojas de cálculo y un proceso automático heredado, con
poca trazabilidad y sin control de los límites de carga de cada docente.

### Dónde estamos

El **núcleo está en producción** y se ha usado para construir la propuesta docente del curso
26/27. Sobre esa base, el proyecto avanza por módulos, cada uno con sus requisitos definidos y
documentados junto a los departamentos implicados.

| Módulo | Para qué sirve | Estado |
|---|---|---|
| **Propuesta docente** | El núcleo: planificación y asignación de la docencia del curso | ✅ En producción |
| **Volcado al sistema académico** | Lleva la propuesta cerrada a Laurea | ✅ En producción · ⚠️ con una incidencia abierta *(ver abajo)* |
| **Ámbitos de conocimiento** | Que cada profesor tenga asociada su área, para que el reparto de docencia sea coherente con su especialidad | 📋 Requisitos definidos · **esperando criterio de Profesorado** |
| **Reducciones horarias** | Descargar de docencia a profesores con carga justificada | 📋 Definido |
| **Bajas y sustituciones** | Cubrir bajas temporales y permanentes sin rehacer la propuesta a mano | 🔨 En desarrollo · sesión de revisión el **jueves 10** |
| **Investigadores** | Que el personal investigador pueda computar para docencia, con control de las horas máximas que permite cada tipo de contrato | 🔨 Requisitos cerrados y en desarrollo |
| **Conferenciantes** | Centralizar su gestión, hoy dispersa | 📋 Definido |
| **Rediseño de la interfaz** | Usabilidad | ⏳ Pendiente de planificar |

### Lo que conviene saber

**1. Incidencia en el volcado al sistema académico.** Durante el verano se detectó la pérdida de
unas **10.000 horas de docencia** ya asignadas en la propuesta del curso 26/27. La causa está
identificada: el proceso que traslada la propuesta a Laurea podía eliminar asignaciones ya
existentes. El trabajo de corrección está analizado y desglosado, y organizado en dos líneas:
recuperar lo perdido y **garantizar que no vuelva a ocurrir**, con trazabilidad de cualquier
borrado. **Todavía no está cerrado**, y es la prioridad técnica del proyecto.

**2. Los ámbitos de conocimiento siguen pendientes.** Los requisitos están definidos y validados
desde abril. Lo que falta no es desarrollo: es el **criterio de Profesorado para ordenar los
ámbitos**. Sin esa clasificación, el reparto por especialidad no puede completarse, y también
condiciona la asignación docente del módulo de Investigadores.

### Qué necesitamos

- **El criterio de ordenación de los ámbitos de conocimiento** por parte de Profesorado. Es hoy
  la única dependencia externa que bloquea avance.

### Próximos hitos

- **Jueves 10 de septiembre** — revisión del módulo de Bajas y Sustituciones con Profesorado.
- **Hasta diciembre** — cierre del módulo de Investigadores e integración de las solicitudes
  docentes con el sistema de tickets.

---

## Notas para mí (no van en el envío)

- **Lo que he dejado fuera a propósito:** claves de Jira, nombres de tecnologías, el detalle
  técnico del incidente (borrados en cascada, timeouts), y cualquier cosa sobre la carga de
  trabajo o el reparto del equipo. María Mendoza supervisa contrataciones: meter nombres del
  equipo con valoraciones en un informe de proyecto sería meterlos en una conversación que no les
  toca.
- **Las 10.000 horas van dentro y creo que deben ir.** Es un proceso transversal y ella lo es
  también; si le llega por otro lado y no estaba en tu informe, quedas peor. Está redactado como
  problema gestionado —causa identificada, trabajo desglosado, sin cerrar— que es la verdad.
- **Los ámbitos son delicados.** Está redactado como dependencia, no como reproche: *"lo que falta
  no es desarrollo, es el criterio de Profesorado"*. Ella habló contigo de esto en su momento, así
  que sabe de qué va.
- **Por confirmar antes de enviar:** que el núcleo esté realmente "en producción" y se haya usado
  para el curso 26/27; que Conferenciantes y Reducciones estén solo "definidos" y no en marcha;
  y si el rediseño visual conviene mencionarlo o sobra.

## 🔗 Enlaces

- Documentación del proyecto: espacio **Gestión Docente** en Confluence
- [[Producto (Área)]] · [[2026-09-04 - Criterios de implantación de modificaciones de planes]]
