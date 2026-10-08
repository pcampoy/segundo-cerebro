---
tipo: proyecto
estado: en curso
inicio: 2026-10-08
fin: 
jira: 
confluence: 
tags: [proyecto, alfresco, gestor-documental, migracion, dpo]
---
# 🎯 Alfresco · nuevo repositorio y migración de los antiguos

> **Objetivo:** crear un **nuevo repositorio de Alfresco** y **migrar a él los Alfrescos antiguos**.
> **Estado:** en curso · **Abierto en el vault el** 08/10/2026

**Alfresco es el gestor documental** de la universidad. **Tiene entidad de proyecto por sí mismo**,
no es una pieza de otro proyecto *(criterio de Pilar, 08/10/2026)*.

## 📌 Por qué está en la DPO de Jesús

Va **en la DPO de Jesús**, y entró **replanteando lo que había**: las DPO estaban fijadas **desde
enero** y **las necesidades reales no se corresponden con aquello**. Este proyecto es parte de esa
corrección.

## 🗺️ El mapa de Alfrescos

*Precisado por Pilar el 08/10/2026.* **Hay tres**, y conviene no confundirlos:

| Cuál | Estado |
|---|---|
| **Alfresco antiguo** | **Ya no se utiliza.** Su contenido se migró en su momento al posterior. Aquí hay **documentación de Infucam** |
| **Alfresco posterior** | El intermedio, el que vino después del antiguo |
| **🆕 Alfresco nuevo** | El que está montando **Jesús**. Es donde van a estar las **planillas de los exámenes** |

## 🧩 Alcance — las tareas de Jesús

1. **Coger los dos Alfrescos anteriores** (el antiguo y el posterior) **con todos los documentos que
   existan** y **pasarlos al Alfresco nuevo**, el de las planillas.
2. **Migrar también los directorios de Infucam** al nuevo, **en el caso de que los hubiera**.
3. **Salesforce → Alfresco:** pasar a Alfresco la **parte documental** de lo que **Adrián Cano**
   tiene en **Salesforce**.

### ❓ Duda abierta: ¿dónde va lo de Salesforce?

**Sin decidir.** Las dos opciones sobre la mesa:

- **En el Alfresco nuevo** que está haciendo Jesús, el mismo de las planillas.
- **En otro Alfresco distinto**, que Jesús crearía, **para no mezclar los datos**.

> Es una decisión de arquitectura documental, no de capacidad: tiene que ver con **si conviene
> mezclar los documentos de Salesforce con los académicos**. Conviene cerrarla antes de que Jesús
> empiece la tercera tarea, porque condiciona el diseño del repositorio.

## 🔗 De qué depende quién — y esto es lo importante

**Alfresco no es un proyecto aislado: hay al menos dos proyectos esperándolo.**

### 1. Lectura y corrección de planillas → [[Lectura y corrección de planillas]]

**Las planillas que se van a corregir tienen que estar almacenadas en ese Alfresco.** Es una
dependencia dura: sin el repositorio, la aplicación de planillas no tiene dónde leerlas.

> Las dos cosas están en la **DPO de Jesús**, y una depende de la otra. **El orden importa.**

### 2. 🔴 Cierre de Infucam → [[Pendientes - Octubre 2026]]

La propuesta de Dirección TIC para apagar Infucam es **exportar los expedientes a PDF y guardarlos
en Alfresco**, con una carpeta por alumno. En la reunión del 30/09 con la Sección de Títulos se
advirtió *"cuidado con el Alfresco, que no funciona"* y se aclaró que **se usaría el nuevo**.

**Ese "Alfresco nuevo" es este proyecto.** Es decir:

> ⚠️ **El cierre de Infucam depende de un repositorio que todavía hay que crear y migrar.**
> Y en el análisis de Infucam ya está escrito que, tras el apagado, **Alfresco pasa a ser la única
> puerta a los expedientes históricos**: si falla, no se pierde un documento, se pierde el acceso a
> la única copia.

Esto **no estaba conectado** hasta hoy. Conviene que lo sepan los dos lados antes de comprometer
fechas de apagado.

## ✅ Pendientes

- [ ] ❓ **Decidir dónde va lo de Salesforce**: Alfresco nuevo o uno aparte. **Bloquea la tarea 3.**
- [ ] **Inventariar el volumen** de los dos Alfrescos anteriores y de los directorios de Infucam.
- [ ] Definir el **plan de migración** y qué pasa con los documentos durante el proceso.
- [ ] **Ordenar la secuencia con planillas**: el repositorio tiene que estar antes.
- [ ] 🔴 **Avisar en el expediente de Infucam** de que su solución documental depende de este
      proyecto, y que **no hay fecha**.
- [ ] Dimensionar **fiabilidad y respaldo**: si va a ser archivo único de expedientes académicos,
      su disponibilidad deja de ser un asunto de conveniencia.
- [ ] Reflejarlo en el **cronograma** → [[Cronograma de proyectos (hasta dic 2026)]]

## 📅 Cronología

| Fecha | Qué |
|---|---|
| **Enero 2026** | Se fijan las DPO del año. Lo de Alfresco **no estaba** como está planteado ahora |
| **30/09/2026** | En la reunión de Infucam se habla de guardar los expedientes en Alfresco, *"el nuevo"* |
| **08/10/2026** | Pilar lo fija como proyecto con entidad propia y en la DPO de Jesús, replanteando lo de enero |

## 🔗 Enlaces

- [[Producto (Área)]] · [[08-10-2026]] · [[Cronograma de proyectos (hasta dic 2026)]]
- [[Lectura y corrección de planillas]] — depende de este proyecto
- Expediente de Infucam: documentos en Confluence, espacio personal de Pilar
