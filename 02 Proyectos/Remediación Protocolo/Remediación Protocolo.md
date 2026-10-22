---
tipo: proyecto
estado: en curso
inicio: 2026-08-31
fin:
prioridad:
jira:
confluence:
tags: [proyecto, seguridad, protocolo]
---
# 🔐 Remediación Protocolo

> **Objetivo:** cerrar los cuatro hallazgos de la revisión de seguridad de Protocolo del 31/08/2026
> (H-1 a H-4) y dejar el repositorio sin secretos versionados.
> **Estado:** en curso · **Fin previsto:** por fijar (la renovación del certificado era en octubre)

Se separó de [[Seguridad (Área)]] el 21/10/2026: esto **tiene fin** (cuando H-1…H-4 estén cerrados);
las revisiones y campañas que no paran viven en el área.

## 📄 Notas del proyecto
- [[Revisión de seguridad - Protocolo]] — hallazgos y acciones, **sin detalle explotable**

## ✅ Se cierra cuando…
- [ ] H-1 · certificado TLS reemitido con claves nuevas y el anterior revocado
- [ ] H-2 · secreto de sesión regenerado y fuera del código
- [ ] H-3 · contraseñas de BD de pre/test rotadas
- [ ] H-4 · usuario de autologin comprobado
- [ ] `.env` y `.pem` fuera del repositorio e historial limpio

## ⚠️ Regla de esta carpeta
Los informes con **detalle explotable NO se guardan aquí** (esto se sincroniza a GitHub).
Viven fuera del vault, en `C:\Varios\Dia a dia\`. Aquí solo **seguimiento**.

## 🔗 Enlaces
- Área: [[Seguridad (Área)]]
- Nota anterior (antes de dividir): [[Seguridad (Proyecto)]]
