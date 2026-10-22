---
tipo: proyecto
estado: abierto
cliente: Dirección TIC (interno) — el proyecto SEGRE lo lleva Alicia
prioridad: alta
inicio: 2026-10-22
fin_previsto: 2026-10-30
palabras_clave: [SEGRE, UCAMSEGRE2, segregación, aplicaciones satélite]
actualizado: 2026-10-22
tags: [proyecto, segre, laurea, sigma, aplicaciones-satelite]
---
# 🛰️ Segregación del 26/10 · comprobación de aplicaciones satélite

> **Esto NO es el proyecto SEGRE** —ese lo lleva Alicia y está marcado *fuera* en
> [[Cronograma de proyectos (hasta dic 2026)]]—. Esto es **lo nuestro**: las aplicaciones del área
> que leen datos de Laurea y que en 2025 se rompieron después de la segregación.
>
> **Fecha de ejecución en Explotación: lunes 26 de octubre de 2026.**
> Confirmada por Alicia el 30/09 ("Confirmamos entonces el Lunes 26 de octubre…") y ratificada por
> Kaloyan (Sigma) el 05/10 ("confirmado definitivamente"). Sin aplazamiento posterior a 22/10.

## ⚠️ Por qué esta nota existe: lo que pasó en 2025

La segregación de 2025 se ejecutó los **días 20 y 21 de octubre**. Lo que vino después, con fechas
y origen:

| Qué se rompió | Evidencia | Cuánto tardó |
|---|---|---|
| **Módulo de horarios y espacios de Laurea** | Pilar a Nuria Matiacci, 30/10/2025: *"falló el módulo de horarios y espacios y hasta este lunes no lo han solucionado"* | ~**1 semana** |
| **Control de asistencia** (depende del anterior) | Antonia Sánchez, 29/10 y 01/12/2025: profesores sin asistencia desde el 23/10 | Hasta **diciembre** en algún grupo |
| **Open Analytics / cubos (OASIG)** | Ref. Sigma `290257` *"Segregación de Facultades UCAM que está afectando a OA"*. Hubo que añadir la dimensión *Estado motivo expediente* a 6 cubos (Abandono, Cohortes, Graduación, Matrícula, Matrícula por asignatura, Rendimiento) | 23–27/10 + ajuste del filtro |
| **Planes duplicados 217 y 223** | Hilo *MIGHISTIT*, 28/10/2025. Se resolvió con fecha de baja y carencia | ~1 semana |
| **PAT · asignación de tutoras** | Hilo *Cuerpo de Tutoras*, 03/11 → 05/12/2025. Causa: el docente debe tener docencia en el centro seleccionado | **1 mes** |
| **Bloqueo de aplicaciones satélite** | Reunión urgente convocada por Sigma el **22/10/2025 a las 16:00** (Aitor Arjona; Alicia, Almudena, Toñi, Pilar). Alicia: *"La reunión es necesaria a pesar de esa respuesta"* | 2 días después de ejecutar |

**El patrón:** todo lo que se rompió está indexado por **centro/facultad + plan**. La segregación
cambia precisamente eso. Y hubo un agravante de calendario: la nueva versión de las **tablas
`I_...`** (interfaz de datos → DWH) se instaló el **mismo 22/10/2025**, con lo que no se podía
distinguir qué fallo venía de cada cosa.

> 📌 **Las quejas no entraron por soporte.** Antonia Sánchez, 29/10/2025: *"muchas veces la gente
> se va quejando con nosotras, con los secretarios técnicos y vete a saber dónde pero no pone el
> soporte"*. Si no se abre un canal explícito, el fallo se entera tarde.

## 🚨 El riesgo específico de este año: Educación

La segregación cae **dos días antes del lanzamiento de Prácticas de Educación**:

| Día | Qué |
|---|---|
| **lun 26** | 🔴 Segregación en Explotación |
| **mar 27** | Educación: pruebas · **descarga de Prado** |
| **mié 28** | 🚀 **Lanzamiento de Educación** (apertura a alumnos) |

Las prácticas se asignan **por titulación y centro**. Es exactamente el eje que mueve la
segregación. **Decisión a tomar antes del viernes 23:** si el lanzamiento del 28 se mantiene o se
protege con un día de margen. No es decisión de Alicia; es de Pilar con Juanma y Alex.

## ✅ Lista de comprobación

### Antes del viernes 23 — preguntar y repartir

- [ ] **A Alicia:** ventana horaria exacta del 26, si hay **parada de servicio**, si hay **punto de
      retorno** (copia previa) y **hasta cuándo** se puede revertir.
- [ ] **A Alicia / Sigma:** quién es el **contacto de guardia** el 26 y el 27, y por qué vía.
- [ ] **A Sigma:** ¿se instala algo más esa semana (versión de tablas `I_...`, parches)? En 2025
      coincidió y enturbió el diagnóstico. **Pedir que no coincida.**
- [ ] **¿Hay titulaciones que no entran?** En 2025 fueron 7 y se quedaron en sus facultades
      antiguas → casuística mixta en todas las apps. Pedir el listado equivalente de 2026.
- [ ] **Guardia del equipo:** quién mira qué el lunes 26 y el martes 27.
- [ ] **Canal de incidencias:** decir por escrito a secretarías técnicas y coordinadores que lo que
      salga raro va a soporte, no al pasillo. Es el fallo de 2025.
- [ ] **Línea base:** sacar **hoy o mañana** las cifras de control de cada app (nº de expedientes
      por centro, grupos con horario, matrículas sincronizadas). Sin foto previa no se puede
      demostrar qué cambió.

### Lunes 26 y martes 27 — comprobar app por app

| # | Aplicación | Jira | Quién | Qué comprobar |
|---|---|---|---|---|
| 1 | **Asistencia** | `AS` | Paco / José Ángel | Que **horarios y espacios** estén poblados y que **un profesor real pueda pasar lista**. 🔴 Es lo que falló en 2025 |
| 2 | **Gestión de prácticas** | `GES` | Juanma · Alex | Titulación y centro de las plazas de Educación. 🔴 Lanza el 28 |
| 3 | **Campus virtual / Canvas** | `CAN` | Juanma | Nodos de sincronización + matrícula por plan y centro *(ver el patrón de 3 niveles en [[Producto (Área)]])* |
| 4 | **Gestión Docencia** | `GD` | Pablo | Profesor ↔ unidad de plantilla ↔ **facultad**. Es justo lo de `GD-706` |
| 5 | **DWH Vertica + cubos** | `MDDD` | Alejandro | Tablas `I_...` y las **tasas** de los 6 cubos de OASIG. 🔴 Falló en 2025 |
| 6 | **Reconocimientos** | `RDC` · `RDCO` | Juanma | Expedientes segregados: que no se dupliquen ni pierdan el centro |
| 7 | **TFG/TFM** | `TFGTFM` | Alejandro | Centro del expediente y tribunales |
| 8 | **Sede electrónica / certificados** | `ET` · `GESTDOC` | Jesús | Certificados que imprimen **facultad y titulación** |
| 9 | **MyUCAM / Portal del alumno** | `IN` · `SUCAM` | Paco · Jesús | Que el alumno se vea su expediente con el centro nuevo |

### Después — no cerrar en caliente

- [ ] **Mantener la vigilancia hasta el viernes 30.** En 2025 el PAT no se detectó hasta el 3 de
      noviembre, once días después.
- [ ] Dejar constancia de cada incidencia en Jira con la etiqueta de la segregación, para que el
      año que viene esta lista no haya que reconstruirla del correo.

## ❓ Lo que no sé y hay que confirmar

- Si el equipo tiene ya asignado algo para esa semana que choque con la guardia.
- Si **Prado** (descarga del 27) depende de códigos de centro — si depende, es el eslabón más
  frágil, porque además es un sistema externo (CARM).
- Si alguien del equipo participó en las pruebas del Excel de censo en PRE que Alicia pidió el
  20/10 y recordó el 22/10. **Nadie había contestado en el hilo a 22/10.**

## 🔗 Enlaces

- [[Cronograma de proyectos (hasta dic 2026)]] · [[Pendientes - Octubre 2026]]
- [[Producto (Área)]] · [[Proyectos y claves Jira]]
- [[Prácticas externas - Medicina, Fisioterapia y FP]]
