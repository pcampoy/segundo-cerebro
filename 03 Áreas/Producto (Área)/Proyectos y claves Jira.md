---
tipo: referencia
tags: [referencia, producto, jira, equipo]
actualizado: 2026-09-08
estado: BORRADOR — pendiente de que Pilar corrija
---
# 🗂️ Proyectos de Desarrollo y sus claves de Jira

> **Para qué sirve:** que Claude sepa de qué se habla cuando se dice un nombre de proyecto, sin
> confundir unos con otros. Lo consultan `/apunta`, `/semanal` y `/daily`.
>
> ⚠️ **BORRADOR.** Las columnas *Clave*, *Nombre en Jira* y *Categoría* salen de Jira y son
> fiables. **Las columnas *Alias* y *Quién lo lleva* son inferencias mías** — corrígelas.

## ⚠️ Lo primero: dos proyectos que se confunden

| | Clave | Nombre en Jira | Alias que usa Pilar |
|---|---|---|---|
| ❶ | **`DOC`** | Docentia | **Docentia** |
| ❷ | **`GD`** | Gestión Docencia | **Gestión de la Docencia** · **Docencia** · **propuesta docente** |

**Son proyectos DIFERENTES.** `GD` tiene tres nombres para lo mismo; `DOC` es otra cosa. Ante la
palabra "docencia" a secas, es **`GD`**. "Docentia" siempre es **`DOC`**.

## Proyectos de la categoría *Desarrollo* en Jira

| Clave | Nombre en Jira | Alias / cómo lo llama Pilar | Quién lo lleva *(por confirmar)* |
|---|---|---|---|
| `GD` | Gestión Docencia | Gestión de la Docencia · Docencia · propuesta docente | Pablo |
| `DOC` | Docentia | Docentia | Pablo |
| `GES` | Gestión de prácticas | Prácticas · gestor de prácticas | Juanma |
| `MIG` | Migraciones SIGMA | Migraciones | Jesús |
| `CAN` | Canvas | Campus Virtual · Canvas Data 2 | Juanma |
| `FAC` | Facturas | UCAM Facturas | Juanma |
| `LA` | Learning agreement | | Juanma |
| `GDP` | Personas | | Juanma |
| `PW` | Personas Web | | Juanma |
| `TM` | Talleres MEI | | Juanma |
| `TB` | Tranvía-Bus | | Juanma |
| `EVT` | Eventos | | Alejandro |
| `CF` | Cuadro financiero | | Alejandro |
| `MDDD` | Modelo de datos - Datawarehouse | DWH · Vertica | Alejandro |
| `TFGTFM` | TFG/TFM | | Alejandro |
| `VDP` | Visor de procesados | | Alejandro |
| `TOOL` | Toolbox | | Pablo |
| `ET` | Tramita | | Jesús |
| `GESTDOC` | Gestor documental | | Jesús |
| `RDC` | Reconocimiento de créditos previos | Recos | |
| `RDCO` | Reconocimiento de créditos Oficiales | Recos | |
| `ED` | Equipo Desarrollo | el tablero del sprint · imputación | Pilar (coordinación) |

## Proyectos de OTRAS categorías donde también trabaja el equipo

Esto importa: **filtrar por categoría "Desarrollo" dejaría fuera trabajo real.** Por eso el filtro
bueno es por **`assignee`**, no por categoría.

| Clave | Nombre en Jira | Categoría | Visto asignado a |
|---|---|---|---|
| `AS` | Asistencia | Web | Paco (`AS-546`, `AS-549` — AsistenciaDatio) |
| `IN` | MyUCAM | Web | Paco (`IN-505`), Jesús (`IN-541`, `IN-562`) |
| `TICAM` | Portal del trabajador UCAM | *(service desk)* | Pilar y equipo → van por `/tickets` |
| `SUCAM` | Portal del alumno UCAM | *(service desk)* | Pilar y equipo → van por `/tickets` |
| `DT` | Dirección TIC | Dirección TIC | Paco (`DT-306`, publicación LinkedIn) |

## Fuera del alcance del equipo

Categorías **Sistemas** (`EQPSIS`, `GC`, `GS`, `KUB`), **Comunicaciones** (`EC`, `RYC`, `SP`),
**Seguridad de la información** (`SDLI`, `SGSI`, `GDD`, `LUCAM`), **Web** (`W1N`, `AP`, `EVP`,
`GI`, `IJIRA`, `ONBO`, `PRPA`, `SFC`, `UPAY`), **Técnica** (`ETEC`) y **Dirección TIC** (`SIG`,
`DPO`). Si aparece una tarea de estas asignada a alguien del equipo, **es la excepción**: hay que
mirarla, no darla por suya.

## 🔗 Enlaces

- [[Producto (Área)]] · [[Equipo (Área)]] · [[Cronograma de proyectos (hasta dic 2026)]]
- Tablero del sprint: https://ucam.atlassian.net/jira/software/c/projects/ED/boards/3
