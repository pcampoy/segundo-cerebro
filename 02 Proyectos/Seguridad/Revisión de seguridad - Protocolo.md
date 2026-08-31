---
tipo: nota
estado: en remediación
fecha: 2026-08-31
tags: [seguridad, protocolo, reunión]
---
# 🔐 Revisión de seguridad – Protocolo (31/08/2026)

> ⚠️ **Informe completo (con el detalle) — fuera del vault, NO versionado:**
> - `C:\Varios\Dia a dia\Informe-seguridad-protocolo-2026-08-31.pdf`
> - `C:\Varios\Dia a dia\Informe de Seguridad - Protocolo.md`
>
> Aquí solo el seguimiento, **sin detalles explotables**.

**Revisado por:** Pilar · **Hallazgos:** 2 críticos · 1 alto · 1 medio

## ✅ Acciones (orden: rotar → limpiar → reescribir historial)
- [ ] **H-1 · Certificado TLS** — reemitir con par de claves NUEVO (no reutilizar el CSR) + revocar el actual · *CRÍTICO*
- [ ] **H-2 · Secreto de sesión** — regenerar largo y moverlo a variable de entorno · *CRÍTICO*
- [ ] **H-3 · Contraseñas de BD (pre/test)** — rotar · *ALTO*
- [ ] **H-4 · Autologin (entorno dev)** — comprobar si el usuario existe fuera de local y cambiar si aplica · *MEDIO*
- [ ] Dejar de versionar `.env` y `.pem`, ampliar `.gitignore`, añadir plantillas `.example`
- [ ] Limpiar el historial del repositorio (coordinar ventana con el equipo)

## 🗣️ A decidir en la reunión con Alejandro
- [ ] ¿Se trata como **incidente** o como **mantenimiento**? (la renovación de octubre da margen)
- [ ] ¿Quién **tramita la reemisión** del certificado? (es lo de más plazo → arrancar primero)
- [ ] ¿Quién **verifica** que la reemisión lleva claves nuevas?
- [ ] ¿**Cuándo** se reescribe el historial? (ventana con todo el equipo avisado)
- [ ] ¿Se **revisan los otros repos** del equipo?

## 🔗 Enlaces
- Proyecto: [[Seguridad (Proyecto)]]
- Reunión con Alejandro: *(crear nota con la Plantilla - Reunión cuando la agendéis)*
