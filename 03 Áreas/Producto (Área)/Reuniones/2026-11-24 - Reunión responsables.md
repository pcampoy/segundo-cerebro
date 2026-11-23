---
tipo: reunión
fecha: 2026-11-24
hora: 10:00–11:30
convoca: Miguel Ángel (Dirección TIC)
area: "[[Equipo (Área)]]"
asistentes: [Pilar, Miguel Ángel, Luis Espiñeira, Adrián Cano, Sergio León, Antonio Pino, Ignacio Ros, Luis Martínez]
estado: preparación
jira: DT-311
tags: [reunión, responsables, dirección-tic, informe]
---
# 2026-11-24 · Reunión de responsables — informe de Desarrollo

> **Estado:** **`preparación`** → `acta`. Zoom + Sala de trabajo TIC, 10:00–11:30.
> Informe de situación del **equipo de Desarrollo** a 23/11. Datos: Jira (comprobado el 23/11 por la tarde),
> [[2026-11-23 - Seguimiento Sprint - Dev]] y [[23-11-2026]].
> ⚠️ **Limitaciones conocidas:** la [[Cabina - Cartera|cabina]] no se refresca desde el **30/10** (24 días) y la
> *Revisión de Sprint* de ayer **no tiene acta** — lo de abajo es lo que dice Jira, no lo que se habló.
> 🔐 Regla de [[Seguridad (Área)]]: aquí **solo seguimiento**. Ni versiones vulnerables, ni detalle explotable.

## 📌 En una línea

El sprint va bien de ejecución y **las dos incidencias de producción del 16/11 están resueltas**, pero hay **tres
cosas que no se arreglan dentro del equipo**: dos aplicaciones sin tarea para un aviso de seguridad de INCIBE, dos
fechas duras el **1 de diciembre** que no dependen de nosotros, y **una tercera app este otoño que nace fuera de
Desarrollo y aterriza aquí sin pasar por ningún sitio**.

---

## 1 · Dónde está el equipo (sprint `Desarrollo 2026/19`)

| | |
|---|---|
| Sprint | **2026/19**, del **17/11 al 30/11** (cierra el lunes a las 18:00) |
| Mañana | día hábil **6 de 10** → quedan **5** (24, 25, 26, 27 y 30) |
| Carga | **121 tareas**: 56 cerradas · 65 abiertas |
| Siguiente | `2026/20` arranca el **1/12** — y probablemente **con el puente del 7–8/12** dentro |

**Lo que ha salido:**
- 🟢 **Gestión Docente vuelve a sincronizar** (`GD-765`, 19/11), después de **22 días** parada.
- 🟢 **Resuelto el 503 al pasar lista en producción** (`AS-595`, 20/11) — Mi Docencia.
- 🟢 **Corrección de planillas en producción desde el 13/11**, con mejoras de rendimiento, impresión y
  estadísticas esta semana.

**Dónde no llegamos:** 7 requisitos de **Reconocimientos** (4 Urgentes) llevan **38 días sin dueño**, y el mapa
docente de Prado (`GES-254`) lleva **62 días en curso sin nadie asignado** — es la **séptima** vez que lo anoto.
No es falta de horas: es que el equipo está completo con lo que ya tiene.

---

## 2 · 🔐 Seguridad — lo que traigo a esta mesa

**Aviso de INCIBE del 20/11 (Spring Security).** Cinco aplicaciones nuestras con control de acceso por anotación
tienen que actualizarse. Situación a hoy:

| Aplicación | Tarea | Estado |
|---|---|---|
| Mis Notas · Mis Planillas | `IN-580` (Jesús) | 🟡 en curso desde ayer |
| Prácticas | `GES-294` (Alex) | ✅ hecha |
| **Mis Alumnos** | — | 🔴 **sin tarea** |
| **Docentia** | — | 🔴 **sin tarea** |
| Widgets | `WD-428` se quedó una versión por detrás | ❓ por confirmar si le afecta |

➡️ **Lo asigno hoy mismo**; lo traigo para que conste la foto, no para pedir nada.

**Además, cerrado por el equipo esta quincena:** imágenes Docker al día por el CVE, mitigación del fallo del
servidor de aplicaciones, informes de seguridad de tres aplicaciones, credenciales de prácticas sacadas a un
*secret* de Kubernetes y el servidor de Infucam actualizado.

**Lo que sigue abierto de la reunión del 27/10** (de aquella no hay acta, así que lo pregunto):
- ¿Se verificó de forma **independiente** el parche del ET, o seguimos con "actualizado" como única garantía?
- 🔴 **El parcheo de plataforma sigue sin dueño con nombre** — PHP de la Sede e imágenes Java de Kubernetes.
  Es el punto que más me preocupa de aquella reunión y el único que no ha avanzado.

---

## 3 · ⏰ Dos fechas duras el 1 de diciembre

Las dos caen **a mitad del cambio de sprint** y **ninguna de las dos la puede resolver mi equipo**:

1. 🧩 **Licencias de Atlassian.** Sngular deja de gestionar la modalidad **mensual** el 1/12 y propone pasar a
   anual; avisan de que sin regularizar *"podríais quedaros sin servicio"*. Adrián ya ha pedido reunión.
   **Jira y Confluence son la herramienta de trabajo diaria del equipo**: pido que esa reunión caiga **antes del 30**.
2. 🚋 **BONO CAMPUS** deja de recargarse el 1/12 y **hay que quitarlo de las peticiones online**. En Jira no hay
   ninguna tarea; **la creo yo esta semana**, pero necesito saber si hay más sitios donde aparezca fuera de lo nuestro.

---

## 4 · 🛰️ El punto de fondo: aplicaciones que entran por la puerta de atrás

**Tres casos este otoño**, y van:

| Caso | De dónde viene | Qué pide |
|---|---|---|
| **Academicship** | Tomás (Rankings), para la encuesta de QS | Alojamiento externo, dominio UCAM, OAuth, acceso a datos |
| **Stock del Preclínico Odontológico** | Acuerdo con la clínica | Entrar en nuestra arquitectura |
| *(y antes)* otras satélite | — | Mantenimiento |

El patrón es siempre el mismo: **se decide fuera, se construye fuera y llega a Desarrollo cuando ya hay compromiso
y prisa**. En Academicship, además, hay **datos personales de 91 investigadores** (nombres, correos y fotos) fuera
de la infraestructura UCAM y una base de datos que tendría que aceptar conexiones desde fuera: **eso lo tiene que
ver el DPD antes, no después**.

### 💡 Lo que propongo: una regla de entrada, en tres preguntas

Antes de que una aplicación de otra unidad entre en nuestra infraestructura:

1. **¿Lo ha visto el DPD?** Si hay datos personales, informe antes de desplegar nada.
2. **¿Lo ha visto Sistemas?** Dominio, OAuth, repositorio y red son suyos, no se conceden por correo.
3. **¿Quién la mantiene cuando el que la hizo no esté?** Con nombre y con equipo.

Y, si entra, **que entre con tarea, proyecto y sprint** — no como favor.

➡️ **Lo que pido a la reunión:** que esto se acuerde como procedimiento, y **quién lo aplica** (¿Responsables?
¿el inventario de Adrián?). No pido que se paren los proyectos: pido que no lleguen terminados.

---

## 5 · 🚦 Cartera — proyectos en rojo

> Semáforo de la cabina del **30/10**, corregido con lo que dice Jira hoy. **Toca refrescarla.**

| | Proyecto | Por qué sigue en rojo | Qué desbloquearía |
|---|---|---|---|
| 🔴 | [[Reconocimientos]] | 7 requisitos sin dueño, 4 Urgentes, 38 días | Que se repartan — el análisis del flujo ya está hecho |
| 🔴 | [[Alfresco - nuevo repositorio]] | El Gestor Documental lleva 20 días quieto | Prioridad y una persona estable |
| 🔴 | [[Cierre de Infucam]] | Depende del Alfresco que no existe; dinero vivo sin cuadrar y títulos antiguos sin migrar | **No se puede comprometer fecha de apagado**, y conviene decirlo aquí |
| 🔴 | [[Remediación Protocolo]] | Sin tareas en este sprint; la cabina ya marcaba 111 días sin actividad el 30/10 | Decidir si sigue vivo o se cierra |
| 🔴➡️🟢 | [[Lectura y corrección de planillas]] | **En producción desde el 13/11** | **Propongo bajarlo de rojo** |

---

## 6 · ❓ Lo que llevo a preguntar

- [ ] **Regla de entrada** para aplicaciones de otras unidades: ¿se acuerda? ¿quién la aplica?
- [ ] **Dueño del parcheo de plataforma** (PHP de Sede, imágenes Java) — pendiente desde el 27/10
- [ ] **Licencias Atlassian**: ¿reunión antes del 30?
- [ ] **BONO CAMPUS**: ¿aparece en algún sitio más fuera de nuestras aplicaciones?
- [ ] **Infucam**: ¿se asume que no hay fecha de apagado mientras no haya Alfresco?
- [ ] **Remediación Protocolo**: ¿sigue vivo?
- [ ] **Reconocimientos**: la fecha real de la IA se apuntó en febrero — ¿se mantiene?

## 📋 Acciones mías, salga lo que salga

- [ ] Crear las tareas de **Spring Security** de **Mis Alumnos** y **Docentia** (hoy)
- [ ] Repartir **`RDCO-182`…`188`** — cuarta vez que lo anoto
- [ ] Tarea para quitar el **BONO CAMPUS** antes del 1/12
- [ ] **`/inicio-sprint`** el 30 y genéricas de diciembre
- [ ] Refrescar la **cabina** (lleva 24 días)

## 🔗 Enlaces

- [[2026-11-23 - Seguimiento Sprint - Dev]] · [[23-11-2026]] · [[Cabina - Cartera]]
- [[2026-10-27 - Reunión responsables - vulnerabilidad de Tramita]] *(sin acta)*
- [[Reconocimientos]] · [[Alfresco - nuevo repositorio]] · [[Cierre de Infucam]] · [[Lectura y corrección de planillas]]
- [[Equipo (Área)]] · [[Seguridad (Área)]] · [DT-311](https://ucam.atlassian.net/browse/DT-311)
