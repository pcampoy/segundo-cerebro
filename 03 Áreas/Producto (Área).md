---
tipo: área
tags: [área, producto]
---
# 🧭 Producto (Área)

> Producto y aplicaciones de gestión integradas con el SIS (**LAUREA**): visión, roadmap, requisitos y decisiones.

## 🔗 Proyectos y notas
- [[Inicio de curso 2026-27 (MOC)]]

## 🗺️ Roadmap / prioridades
- 

## 📋 Requisitos y decisiones de producto
- 

## 🧩 Aplicaciones
- **Campus virtual · no se crean los usuarios de un curso** — *patrón de diagnóstico, de un caso real
  de **PGO** resuelto el 07/10/2026*. El fallo **puede ser doble, y hay que mirar las dos cosas**:

  0. **¿El alumno está dado de alta y matriculado en Laurea?** Si no existe en origen, no hay nada
     que sincronizar. *(Caso del 08/10/2026 con PGO: ~1,5 h para acabar en esto.)* **Comprobar esto
     primero: es lo más barato de descartar y lo que más tiempo hace perder.**
  1. **¿Ha marcado Partner el check** para que el curso se cree en el campus virtual? Si el curso no
     se crea, **los usuarios no se crean**. No es nuestra casilla.
  2. Si ya está marcado, **¿ha fallado algún nodo de sincronización?** En este caso se había marcado
     el check, pero **uno de los nodos falló** y las altas se quedaron sin hacer por nuestro lado.

  ⚠️ **Lo engañoso es que el síntoma es idéntico en los tres casos** —"no aparecen los alumnos"—,
  pero la causa 0 es de matrícula, la 1 es de Partner y la 2 es nuestra. **Ir en ese orden.**

  🔴 **Y no es un curso cualquiera:** **PGO** son los **másteres de Odontología**, que son **título
  propio** y los gestiona directamente **Enrique Palenzuela** (Director de Marketing Nacional).
  Es **el Partner más importante que tiene la UCAM** *(aclarado por Pilar el 07/10/2026)*. Una
  incidencia de altas en PGO no es una incidencia más: trátala con esa prioridad.
- **Prado y PradoJS — los dos entornos de la CARM** *(apuntado el 05/10/2026)*
  La **CARM** ofrece **dos entornos** para interactuar con **su aplicación de mapa docente, oferta de
  plazas y asignación**:

  | Entorno | Para qué |
  |---|---|
  | **PradoJS** | Titulaciones **sanitarias** |
  | **Prado** | Facultad de **Educación** |

  📌 **"La oferta" es el mapa docente**: son la misma cosa, no dos asuntos distintos.
  🟢 *05/10: contactado por fin con la CARM y **acceso concedido al entorno de pruebas**; resuelta la
  visualización del mapa docente de Prado.*
- **Gestión de permisos** — se accede por <https://gestionpermisos.ucam.edu/> *(apuntado el 22/09/2026)*
- **Tramita** — la **sede electrónica**. Proyecto de Jira `ET`, lo lleva **Jesús March**.
  📌 **Toda tarea de sede va a `ET` y a Jesús**, y su documentación al espacio `ESE` de
  Confluence → [[Proyectos y claves Jira]]
 
