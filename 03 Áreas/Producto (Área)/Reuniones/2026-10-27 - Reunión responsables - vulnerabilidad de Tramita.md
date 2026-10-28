---
tipo: reunión
fecha: 2026-10-27
hora: 10:00–11:30
convoca: Miguel Ángel (Dirección TIC)
area: "[[Seguridad (Área)]]"
asistentes: [Pilar, Miguel Ángel, Luis Espiñeira, Adrián Cano, Sergio León, Antonio Pino, Ignacio Ros]
estado: preparación
jira: DT-308
tags: [reunión, responsables, dirección-tic, seguridad, tramita]
---
# 2026-10-27 · Reunión responsables — vulnerabilidad de Tramita

> **Estado:** **`preparación`** → `acta`
> Zoom + Sala TIC. Luis propuso dedicarla a la **vulnerabilidad de Sede/Tramita** y Pilar aceptó (26/10 10:48).
> ⚠️ **Regla de [[Seguridad (Área)]]:** aquí solo seguimiento. Nada de informes, versiones ni detalle explotable:
> el vault sube a GitHub. Los informes, en `C:\Varios\Dia a dia\`.

## 🎯 Objetivo
- Decidir **cómo se cierra el incidente** de Sede/Tramita (reportado por dos alumnos el sáb 24/10) y **qué se vuelve
  a abrir y cuándo**.
- Que **Miguel Ángel salga con la foto completa**: no está en el chat "UCAM Cliente" de Tangram, por donde ha ido todo.

### Dónde estamos (según Tangram, 26/10)
- El fallo es **del ET (Tramita), no de la Sede**. La Sede estaba parcheada; la **Sede PRO** *"la podéis tener operativa"*.
- **ET actualizado** a las 13:53.
- Piden que se les **reponga la VPN a PRE y PRO** para actualizar y probar.
- **Nadie de la UCAM lo ha verificado todavía.**

## 🚨 Bloque 1 · Vulnerabilidad (lo principal)
1. **Verificación independiente del parche** antes de dar nada por cerrado: que se repita la prueba de concepto de los
   alumnos **contra el ET parcheado** (Sistemas, o los alumnos con permiso). "Actualizado" no es "verificado".
2. ⚠️ **Discrepancia sobre los parches del servidor de Sede**: lo que dice Adrián (26/10 08:29) no cuadra con lo que dice
   Tangram. ¿Es el mismo servidor? **Que Adrián lo compruebe en la máquina.**
3. **VPN de Tangram a PRE y PRO**: es un cambio de seguridad pedido por correo en pleno incidente →
   - lo **decide la reunión**,
   - **alcance acotado** (solo PRE/PRO de Sede y ET),
   - lo **ejecuta Sistemas**, no se concede contestando al correo.
4. **Qué está cortado y qué deja de funcionar**: certificados, Tramita, certificado de delitos sexuales, B2, `ET-555`.
   Si se reabre la Sede PRO: **cuándo y con qué condición**.
5. **Foto completa para Miguel Ángel** (no está en el chat de Tangram).
6. **Cabos sueltos**:
   - Respuesta a los **alumnos que lo reportaron**: agradecer y pedir que paren las pruebas.
   - **Higiene**: el informe del exploit sigue adjunto en dos hilos de correo → que no se reenvíe más. Las convocatorias
     sobre el incidente llegan desde cuentas personales → pedir canal institucional.
7. **Deuda de plataforma sin dueño**: quién parchea el PHP de la Sede y las imágenes Java de Kubernetes. Necesita
   **responsable con nombre**.

## 🗂️ Bloque 2 · Si sobra tiempo (o a solas con Miguel Ángel)
- 🔐 **Laurea tras la segregación de UCAMSEGRE2 (26/10)**: pico de alumnos sin acceso y **noveno caso de SSO**
  (*"Attribute does not correspond"*). Lo lleva Alicia, pero es **un corte, no casos sueltos** → al CAU como incidencia única.
- 🔐 **Procedimiento de verificación de identidad en `laureaacademic`**: cuarta petición de reset desde Gmail (hoy, sin decir
  ni de qué cuenta). Que no dependa de quién conteste.
- 🗄️ **[[Cierre de Infucam]]**: dinero vivo sin cuadrar (saldos, reservas de plaza), depende de un
  [[Alfresco - nuevo repositorio|Alfresco que no existe]] y riesgo legal con doctorados y títulos propios antiguos no
  migrados → **no se puede comprometer fecha de apagado**.
- 📝 **[[Lectura y corrección de planillas|App de corrección de exámenes]]**: Almudena sigue esperando respuesta de Miguel Ángel.
- 🤖 **Reconocimientos**: cerrar la **fecha real de la IA** (se apuntó febrero) →
  [[2026-10-08 - Mejoras de la app de Reconocimientos]].
- ⚖️ **iText**: *"si no vamos a pagar, lo suyo sería verlo con SSJJ"* (Miguel Ángel, 15/10) → **quién lo lleva** →
  [[Licencias iText]].
- 🔗 **iMarina**: integración **parada por nosotros** desde el 25/09; el proveedor ya terminó su parte.

## ✅ Decisiones
- [ ] ¿Se da por bueno el parche del ET? ¿Quién lo verifica y cuándo?
- [ ] ¿Se repone la VPN a Tangram? ¿Con qué alcance?
- [ ] ¿Se reabre la Sede PRO? ¿Cuándo?
- [ ] Dueño del parcheo de plataforma (PHP de Sede, imágenes Java)

## 📋 Acciones (quién / cuándo)
- [ ] Comprobar en el servidor el estado de parches de la Sede — Adrián
- [ ] Verificación independiente del parche del ET — *por decidir*
- [ ] Respuesta a los alumnos que reportaron — *por decidir*
- [ ] Contarle a Miguel Ángel lo hablado en el chat de Tangram — *por decidir*

## 🔗 Enlaces
- [[27-10-2026]] · [[26-10-2026]] · [[Pendientes - Octubre 2026]] · [[Seguridad (Área)]]
- [[Segregación 26-10 - aplicaciones satélite]] · [[Cabina - Cartera]]
