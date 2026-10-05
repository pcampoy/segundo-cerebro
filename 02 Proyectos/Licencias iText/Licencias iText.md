---
tipo: proyecto
estado: en curso
inicio: 2026-09-02
fin: 
jira: 
confluence: 
tags: [proyecto, licencias, itext, apryse, juridica]
---
# 🎯 Licencias iText

> **Objetivo:** cerrar la situación de licencia de **iText (AGPLv3)** en las aplicaciones de la
> UCAM, decidir por aplicación si se migra o se licencia, y dejar fijada la postura frente al
> fabricante.
> **Estado:** en curso · **Abierto el** 02/09/2026

> ⚠️ **Nota interna de trabajo.** Recoge análisis propio y posiciones aún no cerradas con Asesoría
> Jurídica. No es un documento para compartir fuera del equipo tal cual.

## 📄 De qué va

El **2 de septiembre de 2026 Apryse** —propietaria de iText desde 2021, cuando era PDFTron—
comunica a la UCAM que usa iText bajo licencia dual y le recuerda las obligaciones de la **AGPLv3**.
No hay excepción académica: el uso universitario no exime.

En Compras hay que buscar contratos por **cuatro nombres**: Apryse, PDFTron, iText Group NV e
iText Software.

## 🧩 Inventario de aplicaciones

Obtenido primero por búsqueda de código en Bitbucket y **corregido después leyendo los metadatos
`Producer` de documentos reales**:

| Aplicación | Versión en el repositorio | Versión real emitida | Nota |
|---|---|---|---|
| `certificadosws` | 7.1.1 | **iText Core 8.0.2 (AGPL)** | En producción. API kernel/layout: migrar es reescribir |
| `tfgtfm` | 5.5.8 | **iText Core 7.2.5 (AGPL)** | Desmiente al repositorio |
| `cuadernodoctorado` | 5.0.6 | *sin verificar* | Pendiente de leer el Producer |
| `documentacion-secretaria` | 5.5.8 | *sin verificar* | Pendiente de leer el Producer |

> 🔴 **Las versiones de Bitbucket no son fuente fiable.** Las **dos** aplicaciones verificadas
> desmienten a su repositorio, y en las dos la versión real es **más moderna**. El inventario se
> cierra leyendo metadatos de documentos emitidos, no el código. Hipótesis por comprobar: la
> búsqueda de Bitbucket solo indexa la rama principal y el despliegue sale de otra.

**Verificado en las cuatro:** no se usa ningún add-on de pago (pdfCalligraph/`typography`,
pdfOptimizer, DITO) ni existe clave `itextkey`. No hay licencia comercial previa detectada.

**Hay al menos tres ramas de iText en producción** —5.5.13.2, 7.2.5 y 8.0.2—, todas AGPL. Una
salida por licencia tendría que cubrir las tres, no una.

## 🔄 El circuito mixto — el dato que lo complica

El gestor académico es **SaaS de Sigma**, y **la sede electrónica también está subcontratada**.
El circuito del certificado de expediente es:

> Sigma genera el PDF → lo envía a la **sede electrónica de la UCAM** → la sede lo sella (CSV +
> pie de firma) → vuelve a Sigma → lo descarga el usuario.

**Ninguno de los dos pasos lo ejecuta software propio**: son dos proveedores distintos usando la
misma versión AGPL.

- **Criterio de reparto:** la AGPLv3 obliga a quien **opera** el software y lo ofrece por red, no a
  quien lo encarga. La pregunta clave sobre la sede es **quién la opera y sobre qué
  infraestructura**.
- **Matiz para Jurídica:** la sede se presenta al ciudadano como sede de la UCAM y bajo nuestro
  dominio. No dar por descontado que la subcontratación nos saca del artículo 13.
- **Exposición propia** = las cuatro aplicaciones internas. Los informes de
  JasperReports/OpenPDF no generan obligación.

### Cómo leer los metadatos

iText **no sustituye** el `Producer` al modificar: le **añade** *"; modified using iText…"*.
Primera mitad = quién generó, segunda = quién modificó.

- ⚠️ Un PDF que pasa por Adobe Acrobat lleva el `Producer` sobrescrito: **la ausencia de iText en un
  documento no prueba que la aplicación no lo use**.
- Un documento de **matrícula** trae `Producer(null)`: algo sobrescribe el aviso del fabricante.
  Hay que localizar en el código quién escribe ese metadato.

## 💶 Lo que ofrece el fabricante

Tras la primera reunión, Apryse ofrece licencia comercial **de iText 5**, por suscripción anual y
tramos de volumen:

| Tramo | Precio |
|---|---|
| Hasta 30.000 documentos | **4.109 €/año** |
| Hasta 60.000 documentos | **7.396 €/año** |

**No cubre `certificadosws` (8.x)**, que es justo la que no se puede migrar fácil.

## 🧭 Recomendación vigente

> La primera recomendación —*"migrar tres a OpenPDF y licenciar solo `certificadosws`"*— **queda
> sin efecto** al descubrirse que las versiones reales son más modernas.

1. **Cerrar el inventario con metadatos**, no con el repositorio.
2. **Decidir después, aplicación por aplicación.**
3. OpenPDF solo sirve para la **rama 5**, donde hoy no hay ninguna confirmada. Para 7 y 8 no hay
   atajo: o licencia del producto correcto, o rehacer con Apache PDFBox.
4. 🟢 **Hay precedente interno**: `resumenReconocimiento` ya usa **JasperReports sobre OpenPDF 1.3.32**
   en producción. La migración no es un experimento y hay gente que sabe hacerla.

**Es previsible que el coste sea mayor de lo estimado al principio.**

## ✅ Pendientes

- [ ] 🧾 **Documento de renuncia**: pedido a Tangram su **documento tipo** en su ticket
      `Tarea #41293` *(29/09)*. **Esperando que lo manden.** Luego lo adaptan con nuestros datos
- [ ] 🧾 **Ticket nuevo a Tangram** *(05/10, tras la reunión con Apryse)*: preguntarles **si se les ha
      dado el caso de que a alguno de sus clientes se le haya podido reclamar el uso "a toro pasado"
      de la librería de iText**. ⚠️ *Falta el número de ticket y quién lo abrió*
- [ ] ⚖️ **Adrián escribe a Servicios Jurídicos** sobre esto mismo *(05/10)* — la reclamación
      retroactiva. Es lo que hay que llevar resuelto a la reunión de la semana que viene
- [ ] 🗓️ **Nueva reunión con Apryse la semana del 12/10** — *nos emplazan en la del 05/10*. ⚠️ *Sin
      día ni hora todavía; ojo que el **lunes 12 es festivo***
- [ ] ✍️ **Firma**: la firma **la presidenta**, decidido el 22/09. Miguel Ángel pasó la pelota a
      **Luis Espiñeira**, que prepara el documento
- [ ] 🔍 **Cerrar el inventario**: leer el `Producer` de documentos generados por
      `cuadernodoctorado` y `documentacion-secretaria`
- [ ] 🔍 **Atribuir la versión 5.5.13.2**, localizada en una carta de admisión y en una copia
      auténtica con CSV. Aplicación de origen sin identificar
- [ ] 🔍 **Capturar el PDF tal y como entra en la sede** y leer su `Producer`. Es la prueba que
      reparte responsabilidad entre Sigma, la sede y nosotros
- [ ] 🔍 Localizar **quién escribe `Producer(null)`** en los documentos de matrícula
- [ ] ⚖️ **Asesoría Jurídica**: fijar la posición sobre el artículo 13 y sobre el reparto con los
      dos proveedores
- [x] 🗓️ **Reunión con Apryse del lunes 5/10, 12:00** *(convocada por Adrián)* — **celebrada**.
      Salen de ella los tres puntos de arriba y una **nueva reunión la semana que viene**
- [ ] 🧾 **Sigma Ref. 306886** — cerrada por nuestra parte el 28/09

## 🛑 Postura acordada

**No responder al fabricante ni enviarle inventarios, versiones ni número de usuarios** antes de
que Asesoría Jurídica fije la posición.

💡 **Palanca a favor:** el metadato `(AGPL-version)` acredita que **los proveedores** usan la
compilación libre en un servicio que **comercializan**. Su posición frente a Apryse es peor que la
nuestra.

💡 **Matiz favorable:** la copia auténtica **no lleva firma incrustada** (sin `/Sig` ni
`/ByteRange`), solo pie visible y CSV. Migrar la sede **no exige reimplementar criptografía**.

## 📅 Cronología

| Fecha | Qué |
|---|---|
| **02/09/2026** | Apryse comunica el uso de iText y recuerda la AGPLv3. Inventario inicial por Bitbucket y primeras lecturas de `Producer` |
| **Septiembre** | Primera reunión con Apryse. Oferta de licencia de iText 5 por tramos |
| **22/09** | Reunión de Apryse pospuesta por Adrián |
| **22/09** | Decidido **quién firma**: la presidenta, vía Luis Espiñeira |
| **28/09** | Luis pregunta si Tangram tiene un **documento tipo** que podamos adaptar |
| **29/09** | **Pedido a Tangram** en su ticket `Tarea #41293` |
| **05/10** | **Reunión con Apryse/iText, 12:00** (celebrada). Se abre **ticket a Tangram** para saber si a algún cliente suyo le han reclamado el uso **"a toro pasado"** de iText; **Adrián escribirá a Servicios Jurídicos**; **nos emplazan a una nueva reunión la semana que viene** |

## 🔗 Enlaces

- Herramientas propias: `C:\Users\pcampoy\Desktop\Carpeta de Trabajo Claude\iText-Inventario\`
  *(rastreador de iText y clonador de Bitbucket)* y `Buscar-Producer-PDF.ps1` *(lee el Producer de
  PDF locales y publicados, en lote)*
- Informe publicado: https://claude.ai/code/artifact/c57a40c6-6c1f-4b44-aea0-87df7a886545
- [[Producto (Área)]] · [[Cronograma de proyectos (hasta dic 2026)]] · [[Seguridad (Proyecto)]]
- [[29-09-2026]] · [[Pendientes - Septiembre 2026]]
