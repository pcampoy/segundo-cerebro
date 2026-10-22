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
> [[Cronograma de proyectos (hasta dic 2026)]]—.
>
> 🎯 **REGLA DE PILAR (22/10/2026): en una segregación, la única línea de actuación nuestra es el
> CAMPUS VIRTUAL.** Todo lo demás —cubos, PAT, planes, mantenimientos de la dupla Centro-Plan— es
> de otros departamentos o de Sigma. No montamos un operativo de revisión de media docena de
> aplicaciones. **Vale también para futuras segregaciones.**
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

✅ **Todo esto quedó resuelto en su momento.** La tabla es **histórico**, no hay nada abierto de
2025. Sirve para dimensionar lo que puede venir, no como lista de pendientes *(confirmado por
Pilar, 22/10/2026)*.

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

La segregación no es nuestra, pero **el lanzamiento del 28 sí**. Es un dato de calendario a tener
presente: si el lunes hay parada de servicio o ruido en Laurea, el martes de pruebas se come el
margen. No obliga a revisar nada de `GES` por la segregación —eso queda fuera por la regla de
arriba—, solo a no planificar el martes como si fuera un día normal.

## ✅ Lista de comprobación

### Antes del viernes 23

- [ ] **A Alicia:** ventana horaria exacta del 26 y si hay **parada de servicio** (para saber
      cuándo el campus puede quedar descolgado).
- [ ] **A Cristina Ríos (Sigma):** ¿cuándo entra en **producción** la versión Q3/2026 de las tablas
      `I_...`? Entró en preproducción el **19/10**. En 2025 coincidió con la segregación y no se
      podía distinguir qué fallo venía de cada cosa. **Pedir que no caiga en la semana del 26.**
- [ ] **Juanma avisado** de que el lunes mira el campus virtual.
- [ ] **Línea base del campus:** nº de matrículas sincronizadas por plan y centro, sacado antes
      del lunes. Sin foto previa no se puede demostrar qué cambió.

### Lunes 26 y martes 27 — lo nuestro: **campus virtual**

| Aplicación | Jira | Quién | Qué comprobar |
|---|---|---|---|
| **Campus virtual / Canvas** | `CAN` | Juanma | **Matrícula sincronizada por plan y centro** y los **nodos de sincronización**. Si un alumno dice que no ve su campus, aplicar el patrón de 3 niveles: (0) alumno no matriculado en Laurea · (1) check del Partner · (2) nodo caído → [[Producto (Área)]] |

**Y nada más.** Lo que aparezca en otras aplicaciones se traslada a quien corresponda, no se asume.

### Después — no cerrar en caliente

- [ ] **Vigilar el campus hasta el viernes 30.** En 2025 los efectos de la segregación siguieron
      apareciendo más de una semana después.
- [ ] Dejar constancia en Jira (`CAN`) de lo que salga, para que la próxima segregación no haya
      que reconstruir esto del correo.

## ❓ Lo que no sé

- **Qué facultades entran** (22/10). No está en el texto de ningún correo: viaja en el acta de
  consultoría del 01/10 (PDF), en el SharePoint `UCAMSEGRE2` → Documentos y en el Excel del censo
  de pruebas del 20/10. En 2025, 7 titulaciones **no** entraron y se quedaron en sus facultades
  antiguas; si este año pasa lo mismo, el campus se encuentra con casuística mixta.
- Cuándo entra en **producción** la Q3/2026 de las tablas `I_...`.

## 🔗 Enlaces

- [[Cronograma de proyectos (hasta dic 2026)]] · [[Pendientes - Octubre 2026]]
- [[Producto (Área)]] · [[Proyectos y claves Jira]]
- [[Prácticas externas - Medicina, Fisioterapia y FP]]
