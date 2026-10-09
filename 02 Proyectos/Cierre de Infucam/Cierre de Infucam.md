---
tipo: proyecto
estado: en curso
inicio: 2026-09-30
fin: 
jira: 
confluence: "~5c7cfc943fb39d723db25676/1245806594"
tags: [proyecto, infucam, laurea, titulos, cierre, migracion]
---
# 🎯 Cierre de Infucam

> **Objetivo:** apagar Infucam conservando lo que cada departamento necesita, y sacar un **plan de
> cierre** acordado con Dirección TIC.
> **Estado:** en curso · **Horizonte: cierre de 2026 y principios de 2027**

**Por qué hay que apagarlo:** es una aplicación en **Visual Basic** contra un **SQL Server 2008**,
**sin actualizaciones ni mantenimiento**. Fuera de soporte, con lo que implica en seguridad.

> 💡 *"Creo que tiene bastante más implicaciones de las que pensamos"* — Pilar, 08/10/2026.

## 🧩 Las cuatro partes

El cierre no es un bloque único. Cada parte tiene su interlocutor y su casuística:

| Parte | Quién | Estado |
|---|---|---|
| **Gestión económica** | Gestión Económica y Administración | 🔴 Saldos **vivos y sin cuadrar**. **Reunión del 09/10 documentada** → [[2026-10-09 - Cierre de Infucam con Gestión Económica]]. Lo que manda es el **histórico de *Alta de pagos***. *Ya no se cobra nada por Infucam* |
| **Títulos** | Sección de Títulos (Loles) | Reunión del 30/09 y del 08/10 documentadas |
| **Expedientes** | Secretaría Central, Ordenación Académica, UCAM Laurea | Consulta de expedientes y documentos de preinscripción |
| **Títulos propios** | SIE — Postgrados y Títulos Propios (Pedro López) | No se migraron los de la etapa anterior |

## 🗓️ Reunión de Gestión Económica — viernes 09/10/2026

La segunda de las reuniones por partes. **Tema: los pagos pendientes y las contabilidades que se
llevan en Infucam.**

| Quién | Papel |
|---|---|
| **Gracia Paloma** | Jefa de Gestión Económica de **Murcia** |
| **Juan Ruiz** | Gestión económica en **Cartagena** |
| **Alberto Fernández** | Técnico de **Administración** |

⚠️ **No está en el calendario** (comprobado el 08/10). El viernes 09 solo figuran la **clase de
08:30 a 10:30** y el **Seguimiento megarepo de Dirección TIC de 13:00 a 14:00**: el hueco libre es
**de 10:30 a 13:00**.

**Qué llevar**, a partir de lo que ya sabemos:

- **Los saldos positivos y negativos pendientes de actualizar**: dónde están exactamente y con qué
  se relacionan. Hoy *"no sé dónde están las notas ni qué relación"* tienen.
- **Que por Infucam se cobran certificados** (confirmado por el SIE): qué pasa con ese flujo de
  cobro al apagar.
- **Los traspasos de saldo entre familiares** (entre hermanos).
- La pregunta de fondo: **¿los saldos se cuadran antes de apagar, se migran, o se trasladan a otro
  sistema?** Es lo que condiciona la fecha de apagado.
- Y el matiz técnico que importa aquí: **un saldo no se consulta, se concilia**. Un PDF no sirve;
  hace falta dato operable.

## 🔄 Cómo se está trabajando

Método fijado por Pilar:

1. **Reuniones particulares con cada parte**, por separado.
2. De cada una sale un **documento de requisitos en Confluence**.
3. Después, **una reunión con Miguel Ángel** con todo junto.
4. De ahí sale el **plan de cierre de Infucam**.

> Es deliberado: **primero se entiende cada parte, y luego se decide**. Por eso no se convocó una
> reunión conjunta.

## 📄 Dónde está la documentación de Infucam

*Precisado el 08/10/2026.* **Está en dos sitios**:

1. En los **propios directorios del sistema**.
2. En el **Alfresco antiguo**, que **ya no se utiliza** y cuyo contenido se migró al Alfresco
   posterior.

👉 **Las dos cosas entran en el trabajo de Jesús** → [[Alfresco - nuevo repositorio]]: pasar los dos
Alfrescos anteriores al nuevo, y **migrar también los directorios de Infucam** si los hubiera.

## 🔴 La dependencia que condiciona el calendario

**La solución documental del cierre es guardar los expedientes en Alfresco** — y ese Alfresco
**todavía hay que crearlo y migrarle los dos anteriores**. Es un proyecto de Jesús, **sin fecha**.

> **No se puede comprometer una fecha de apagado sin saber cuándo está el repositorio.**
> Y después del apagado, **Alfresco pasa a ser la única puerta a los expedientes históricos**.

## ✅ Pendientes

- [ ] Terminar las **reuniones particulares** de las cuatro partes.
- [ ] **Reunión con Miguel Ángel** y **sacar el plan de cierre**.
- [ ] 🔴 Resolver los **saldos económicos** antes de cualquier fecha de apagado.
- [ ] **Medir** en cuántos de los ~2.800 expedientes está mal la fecha de fin.
- [ ] Buscar en la base de datos si existe la **fecha de retirada del título**.
- [ ] **Copia actualizada de la base de datos** antes de cerrar.
- [ ] Reflejarlo en el **cronograma** → [[Cronograma de proyectos (hasta dic 2026)]]

## 📅 Cronología

| Fecha | Qué |
|---|---|
| **30/09/2026** | Correo a los departamentos preguntando quién usa Infucam. Reunión con la Sección de Títulos |
| **05/10/2026** | Censo de usuarios cerrado. Aparecen los **saldos de Gestión Económica** |
| **06/10/2026** | Miguel Ángel da luz verde a convocar a los departamentos |
| **08/10/2026** | Reunión de requisitos con Títulos. Se fija el método: **una reunión por parte → documento → reunión con Miguel Ángel → plan de cierre** |
| **09/10/2026** | Reunión con **Gestión Económica y Administración** → [[2026-10-09 - Cierre de Infucam con Gestión Económica]]. Actividad "Infucam" en Laurea para deudas; sesión pendiente delante de Infucam |

## 🔗 Enlaces

- **Confluence:** [Migración Infucam → Laurea (30/09)](https://ucam.atlassian.net/wiki/spaces/~5c7cfc943fb39d723db25676/pages/1245806594) ·
  [Requisitos del 08/10](https://ucam.atlassian.net/wiki/spaces/~5c7cfc943fb39d723db25676/pages/1267138562) ·
  [Gestión Económica del 09/10](https://ucam.atlassian.net/wiki/spaces/~5c7cfc943fb39d723db25676/pages/1270448129)
- [[Alfresco - nuevo repositorio]] — de él depende la solución documental
- [[Producto (Área)]] · [[Quién es quién (apodos e interlocutores)]] · [[Cronograma de proyectos (hasta dic 2026)]]
