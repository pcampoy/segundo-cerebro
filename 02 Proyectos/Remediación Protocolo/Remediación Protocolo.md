---
tipo: proyecto
estado: en curso
cliente: 
prioridad: 
inicio: 2026-08-31
fin_previsto: 
jira: 
confluence: 
palabras_clave: [Protocolo]
semaforo: incompleta
avance: 
historias_total: 
historias_hechas: 
puntos_total: 
puntos_hechos: 
ultima_actividad: 
proxima_reunion: 
actualizado: 2026-10-22T15:57
tags: [proyecto, seguridad, protocolo]
---
# 🔐 Remediación Protocolo

> **Objetivo:** cerrar los cuatro hallazgos de la revisión de seguridad de Protocolo del 31/08/2026
> (H-1 a H-4) y dejar el repositorio sin secretos versionados.
> **Estado:** en curso · **Fin previsto:** por fijar (la renovación del certificado era en octubre)

<!-- cabina:inicio estado -->
> ⚪ **Ficha incompleta** — falta fin previsto, prioridad · sin claves de Jira en la ficha.
> *Calculado por `/cabina` el 22/10/2026 15:57.*
<!-- cabina:fin estado -->

## 📈 Avance
<!-- cabina:inicio avance -->
_Sin datos de Jira: añade claves en `jira:` (proyecto, épica o incidencia) para medir el avance._
<!-- cabina:fin avance -->

## 👀 Lo que pide atención

**Tareas quietas** (7 días hábiles o más sin moverse)
<!-- cabina:inicio quietas -->
_Sin datos de Jira._
<!-- cabina:fin quietas -->

**Bloqueos** — quién espera a quién

| Desde | Qué está parado | Espera a |
|---|---|---|

**Espero de otros** — lo que yo espero, con su fecha

| Desde | De quién | Qué |
|---|---|---|

## 📝 Requisitos
<!-- cabina:inicio requisitos -->
_Pendiente del primer `/cabina`: actas de captura con su `estado:` y los días que llevan en él._
<!-- cabina:fin requisitos -->

## ⚖️ Decisiones
| Fecha | Decisión | Quién | Acta |
|---|---|---|---|

## 🔀 Cambios de alcance
| Fecha | Entra | Sale o se retrasa | Lo pide | Decisión |
|---|---|---|---|---|

## ⚠️ Riesgos
| Riesgo | Impacto | Plan B |
|---|---|---|
| H-1 exige reemitir el certificado con claves nuevas | Si se renueva reutilizando el CSR, H-1 sigue abierto | Tramitar la reemisión lo primero: es lo de más plazo |

## 📅 Agenda y correo
<!-- cabina:inicio agenda -->
_Pendiente del primer `/cabina`: próxima reunión, últimas 5 actas y últimos 5 hilos de correo._
<!-- cabina:fin agenda -->

---

> 🗒️ **Notas del proyecto** — de aquí abajo es todo tuyo: `/cabina` no lo toca nunca.

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
