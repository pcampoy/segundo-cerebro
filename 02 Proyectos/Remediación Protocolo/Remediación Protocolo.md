---
tipo: proyecto
estado: en curso
cliente: TIC
prioridad: Alta
inicio: 2026-08-31
fin_previsto: 2027-12-31
jira: [ED-1915, ED-1916]
confluence: 
palabras_clave: [Protocolo]
semaforo: rojo
avance: 0
historias_total: 2
historias_hechas: 0
puntos_total: 2
puntos_hechos: 0
ultima_actividad: 2026-05-25
proxima_reunion: 
actualizado: 2026-10-30T14:49
componente: "Seguridad"
alerta: rojo
alerta_desde: 2026-10-26
tags: [proyecto, seguridad, protocolo]
---
# 🔐 Remediación Protocolo

> **Objetivo:** cerrar los cuatro hallazgos de la revisión de seguridad de Protocolo del 31/08/2026
> (H-1 a H-4) y dejar el repositorio sin secretos versionados.
> **Estado:** en curso · **Fin previsto:** por fijar (la renovación del certificado era en octubre)

<!-- cabina:inicio estado -->
> 🔴 **Rojo** — 111 días hábiles sin actividad (Jira, actas y correo).
> *Calculado por `/cabina` el 30/10/2026 14:49.*
<!-- cabina:fin estado -->

## 📈 Avance
<!-- cabina:inicio avance -->
**0 %** por número de tareas · _1 pendientes sin estimar: por puntos no sería fiable_ · 0 de 2 tareas hechas.

_Nada de este proyecto en el sprint activo._
<!-- cabina:fin avance -->

## 👀 Lo que pide atención

**Tareas quietas** (7 días hábiles o más sin moverse)
<!-- cabina:inicio quietas -->
_Ninguna._
<!-- cabina:fin quietas -->

**Bloqueos** — quién espera a quién

| Desde | Qué está parado | Espera a |
|---|---|---|

**Espero de otros** — lo que yo espero, con su fecha

| Desde | De quién | Qué |
|---|---|---|

## 📝 Requisitos
<!-- cabina:inicio requisitos -->
_Ninguna acta de captura de requisitos asociada a este proyecto._
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
**Próxima reunión:** _ninguna en los próximos 30 días con las palabras clave de la ficha._

**Últimas actas:** _ninguna asociada._

**Correo reciente:** _ningún asunto con las palabras clave en los últimos 30 días._
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
