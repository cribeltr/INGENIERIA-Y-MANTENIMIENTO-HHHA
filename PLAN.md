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

## Fase 1 — Documentos del plan en la ficha del equipo ✅ (con reversión parcial)
**Objetivo:** resolver desde la ficha del equipo los documentos que faltan para
completar el plan (ej.: equipo 2-0166863, Reporte de Reprogramación C5 de abril
→ imprimir → entregar a Ignacio con delegación registrada → archivar).

- [x] Ficha del equipo: sección "📁 Documentos del plan" con lo que falta para la carpeta
- [x] Flujo por documento: 🖨 Imprimir (reporte individual) → ✍️ Entregado a [persona] → ✅ Archivar
- [x] Queda registrado a quién se entregó y cuándo (delegación con nombre y fecha)
- [x] Inventario vacío permite importar el .xlsm maestro y restaurar respaldo .json
- [x] ~~Ocultar todas las pestañas menos Inventario~~ → **revertido el 11-06-2026 por
      decisión del usuario ("no ocultes nada")**; todas las pestañas visibles de nuevo
- [x] Pruebas en Node: 44/44, incluyendo regresión de todas las vistas
- [ ] El usuario valida el flujo de documentos en la ficha con sus datos reales

## Fase 2 — Análisis y propuesta de programa 🔵
**Objetivo:** analizar el programa y los datos, y proponer la estructura del
programa definitivo. Detalle en **PROPUESTA.md** (5 pestañas: Mi día, Equipos,
Mes de trabajo, Servicio técnico, Datos).
**Criterio de terminado:** el usuario decide qué de la propuesta se hace.

- [x] Análisis del programa (11 pestañas, solapamientos, dos ejes: equipo y mes)
- [x] Escribir PROPUESTA.md con el programa propuesto y el camino por fases
- [ ] Recibir respaldo real del usuario (.json o .xlsm) para calibrar con sus datos
- [ ] El usuario decide: estructura de 5 pestañas, destino de Pendientes, nombre del hospital

## Fases siguientes (si la propuesta se aprueba) ⬜
- F2→F6 descritas en PROPUESTA.md: Mi día → Mes de trabajo (×2) → Pendientes → pulido.
- Otras ideas no comprometidas: gráfico de evolución mensual; % operativo por familia;
  recordatorio de respaldo semanal; acciones en lote.
