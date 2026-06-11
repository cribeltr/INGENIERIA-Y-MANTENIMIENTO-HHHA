# PLAN — Proyecto GEB (Gestión de Equipos Biomédicos · HHHA)

Trabajo por fases: una a la vez, y ninguna se da por terminada sin validación del usuario.
Estados: ⬜ pendiente · 🔵 en curso · ✅ terminada

## Fase 0 — Contexto y comprensión ✅
**Objetivo:** entender el programa GEB y el día a día del usuario antes de tocar nada.
**Cierre:** el usuario validó pasando directo a dirigir el trabajo (11-06-2026).

- [x] Descomprimir el zip y leer todo su contenido (index.html, README, CLAUDE.md, HISTORIAL)
- [x] Incorporar el programa al repositorio git **sin modificarlo**
- [x] Crear PLAN.md y CONTEXTO.md
- [x] Entregar resumen y preguntas al usuario

## Fase 1 — Solo Inventario + documentos del plan en la ficha 🔵
**Objetivo:** trabajar enfocados en una sola vista (Inventario, las demás ocultas
sin eliminar código) y resolver desde la ficha del equipo los documentos que
faltan para completar el plan (ej.: equipo 2-0166863, Reporte de Reprogramación
C5 de abril → imprimir → entregar a Ignacio con delegación registrada → archivar).
**Criterio de terminado:** el usuario prueba el flujo con sus datos reales y lo valida.

- [x] Ocultar todas las pestañas menos Inventario (constante `TABS_VISIBLES`, código intacto)
- [x] Inventario vacío permite importar el .xlsm maestro y restaurar respaldo .json
- [x] Ficha del equipo: sección "📁 Documentos del plan" con lo que falta para la carpeta
- [x] Flujo por documento: 🖨 Imprimir (reporte individual) → ✍️ Entregado a [persona] → ✅ Archivar
- [x] Queda registrado a quién se entregó y cuándo (delegación con nombre y fecha)
- [x] Pruebas en Node: 44/44, incluyendo regresión de todas las vistas ocultas
- [ ] El usuario valida con sus datos reales

## Fases siguientes ⬜
Se definirán con el usuario. Candidatas mencionadas (no comprometidas, requieren su OK):

- Decidir el destino de las demás pestañas (reactivar, fusionar o podar)
- Unificar el nombre del hospital en toda la aplicación
- Gráfico de evolución mensual de cumplimiento
- % operativo por familia (disponibilidad)
- Imprimir protocolos del mes por técnico desde el Plan
- Recordatorio de respaldo semanal
- Acciones en lote (varios equipos a la vez)
