---
tipo: proyecto
estado: en curso
inicio: 2026-10-08
fin: 
jira: 
confluence: 
tags: [proyecto, planillas, examenes, actas, alfresco, dpo]
---
# 🎯 Lectura y corrección de planillas de exámenes

> **Objetivo:** que las planillas de examen se lean y corrijan desde la aplicación, y que la nota
> llegue al acta.
> **Estado:** en curso · **Abierto en el vault el** 08/10/2026 *(el trabajo venía de antes)*

## 📌 Por qué importa

- Es **uno de los proyectos importantes del año** *(criterio de Pilar, 08/10/2026)*.
- Va **en la DPO de Jesús**: es objetivo suyo del año, no un encargo suelto.
- Lo está **trabajando Jesús** ahora mismo.
- Está **vinculado al proyecto de Alfresco** → [[Alfresco - nuevo repositorio]].
  **La dependencia es dura:** las planillas que se van a corregir **tienen que estar almacenadas en
  el Alfresco nuevo**, que **todavía hay que crear y al que hay que migrar los antiguos**.
  ⚠️ **Las dos cosas están en la DPO de Jesús y una depende de la otra: el orden importa.** Sin
  repositorio, la aplicación no tiene de dónde leer las planillas.

## ⚠️ Lo que está abierto: los roles que acceden a la aplicación

**Hay discrepancias sin resolver sobre el ámbito de cada rol.** Es el punto que hay que cerrar antes
de avanzar, porque cambia el diseño.

Se contemplan **dos perfiles docentes distintos**:

| Rol | Qué puede hacer hoy |
|---|---|
| **Docente responsable de la asignatura** | Corregir planillas, subir nota y **volcar el acta** |
| **Docente que imparte la asignatura** | Corrige, pero **NO tiene permiso de escritura en acta** |

### Cómo surgió

- **Jesús** lo tenía enfocado a que **solo el responsable de la asignatura** pudiera corregir
  planillas y subir nota.
- Tras hablar con **Almudena** (Ordenación Académica), se reconsideró por la **docencia compartida**:
  - En una asignatura compartida, **varios profesores pueden hacer dos exámenes**.
  - **Quien corrige no tiene por qué ser el responsable**: puede ser cualquiera de los docentes
    compartidos.
  - Pero esos docentes **no tienen acceso como responsables de actas**, así que **no pueden
    volcarlas**. ⚠️ *(Falta concretar dónde se vuelca: Laurea o el aula virtual.)*

> **El fondo del asunto:** quien corrige y quien puede volcar el acta **no son necesariamente la
> misma persona**, y la aplicación hoy asume que sí.

## ✅ Decisiones pendientes

- [ ] ¿La aplicación permite corregir a **cualquier docente de la asignatura** o solo al responsable?
- [ ] Si corrige un docente compartido, **¿quién vuelca el acta?** ¿Se le amplía el permiso, o el
      volcado lo hace siempre el responsable con lo que han corregido otros?
- [ ] ¿El permiso de **responsable de actas** se puede ampliar y **quién lo autoriza**? Apunta a
      Ordenación Académica, **sin confirmar**.
- [ ] ¿Cómo queda la **trazabilidad de quién puso cada nota**? En un acta no es un detalle menor.
- [ ] **Secuenciar con Alfresco**: el repositorio nuevo tiene que estar antes de que la aplicación
      pueda leer las planillas → [[Alfresco - nuevo repositorio]].

## 📅 Cronología

| Fecha | Qué |
|---|---|
| **08/10/2026** | Pilar habla con Jesús por la mañana sobre el enfoque. Antes había hablado con Almudena. Se reconsidera el modelo de roles por la docencia compartida. **Sin decisión tomada** |

## 🔗 Enlaces

- [[Producto (Área)]] · [[08-10-2026]]
- **Alfresco** — proyecto vinculado, sin nota propia en el vault todavía
- 📂 Los repositorios de corrección de planillas están en **Bitbucket**. *Desde el 08/10/2026* se
  pueden **consultar en solo lectura cuando Pilar lo pida**, para detectar errores. **Los hallazgos
  se le dicen a ella**, que es quien los propone y los comunica a quien lleve el proyecto. **Nunca
  escribir en ellos, ni entrar por iniciativa propia, ni avisar directamente a nadie.**
