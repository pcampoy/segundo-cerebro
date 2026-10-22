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
- [ ] **A Alicia:** el **reparto plan a plan del centro 126** entre Medicina (147) y Farmacia y
      Nutrición (148). Sin ese mapa no se puede comprobar si el campus ha quedado bien.
- [ ] **Juanma avisado** de que el lunes mira el campus virtual, y **que busque hoy dónde están
      escritos los códigos 126 y 128** en el campus y su sincronización.
- [ ] **Línea base del campus:** nº de matrículas sincronizadas por plan y centro, sacado antes
      del lunes. Sin foto previa no se puede demostrar qué cambió.

### Lunes 26 y martes 27 — lo nuestro: **campus virtual**

| Aplicación | Jira | Quién | Qué comprobar |
|---|---|---|---|
| **Campus virtual / Canvas** | `CAN` | Juanma | **Los planes que salen del 126** (los que más riesgo tienen: se reparten entre 147 y 148) y **los que salen del 128** hacia el 153. Comprobar matrícula sincronizada y los **nodos de sincronización**. Si un alumno dice que no ve su campus, patrón de 3 niveles: (0) no matriculado en Laurea · (1) check del Partner · (2) nodo caído → [[Producto (Área)]] |

**Y nada más.** Lo que aparezca en otras aplicaciones se traslada a quien corresponda, no se asume.

### Después — no cerrar en caliente

- [ ] **Vigilar el campus hasta el viernes 30.** En 2025 los efectos de la segregación siguieron
      apareciendo más de una semana después.
- [ ] Dejar constancia en Jira (`CAN`) de lo que salga, para que la próxima segregación no haya
      que reconstruir esto del correo.

## 🏛️ Alcance: qué cambia el 26/10

*(Lo pasó Pilar el 22/10/2026.)*

| Centro actual | Qué le pasa | Centros destino |
|---|---|---|
| **126 · Facultad de Ciencias de la Salud** | **Se reparte** entre dos centros nuevos | **147 · Medicina** y **148 · Farmacia y Nutrición** |
| **128 · Facultad de Ciencias Jurídicas y de la Empresa** | **Se extingue** | **153 · Economía y Empresa** (traslado en bloque) |

### Lo que esto significa para el campus virtual

**Son dos casos de distinta dificultad, y conviene no tratarlos igual:**

- **126 → 147 / 148 es un reparto, no un renombrado.** No hay correspondencia 1:1: **cada plan va a
  uno de los dos centros nuevos** y alguien ha tenido que decidir a cuál. Es el caso frágil: si el
  campus deduce algo a partir del centro, un plan mal clasificado no da error, da un alumno en el
  sitio equivocado. 🔴 **Aquí es donde hay que mirar.**
- **128 → 153 es un traslado en bloque**, uno a uno. Más simple: o va todo o no va nada, y si falla
  se ve enseguida.

📌 **Lo concreto a revisar con Juanma antes del lunes:** dónde aparecen los códigos **126** y
**128** en el campus virtual y en su sincronización —reglas, filtros, tablas de mapeo, consultas,
configuraciones de Canvas—. **A partir del 26 ninguno de los dos existe como hoy.** Lo que esté
escrito a fuego con esos códigos deja de valer en silencio.

> 💡 **Engancha con otro proyecto:** el 26/10 **nace la Facultad de Medicina (147)**. Fisioterapia
> sale del 126 y Nutrición también. Tenerlo presente en
> [[Prácticas externas - Medicina, Fisioterapia y FP]], que arranca en 2027: la estructura de
> centros con la que se diseñe ya es la nueva, no la de hoy.

Referencia de volumen, **solo orientativa**: en el extracto *"Planes con alumnos estado A"* del
**2 de julio** (en tu carpeta de descargas), el **126 era el centro con más planes distintos** —
Fisioterapia, Nutrición, Terapia Ocupacional, Psicología, Ciencia y Tecnología de los Alimentos y
varios másteres sanitarios—, y el **128** agrupaba ADE, Derecho y el MBA. Es una consulta parcial
de julio, no el catálogo: sirve para hacerse una idea del tamaño, no para dar cifras.

## ❓ Lo que no sé

- **Qué plan concreto de los del 126 va a Medicina y cuál a Farmacia y Nutrición.** Es el dato que
  falta para poder comprobar nada. Está en el acta de consultoría del 01/10 (PDF), en el
  SharePoint `UCAMSEGRE2` → Documentos o se lo pides a Alicia.
- Si hay **titulaciones que se quedan fuera** del proceso. En 2025 fueron 7 y permanecieron en sus
  facultades antiguas → casuística mixta.
- Cuándo entra en **producción** la Q3/2026 de las tablas `I_...`.

## 🔗 Enlaces

- [[Cronograma de proyectos (hasta dic 2026)]] · [[Pendientes - Octubre 2026]]
- [[Producto (Área)]] · [[Proyectos y claves Jira]]
- [[Prácticas externas - Medicina, Fisioterapia y FP]]
