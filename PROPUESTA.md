# PROPUESTA — Qué programa te propongo (11-06-2026)

> Estado: **esperando tu decisión**. Nada de esto se construye sin tu OK,
> y nada de lo que hoy funciona se elimina sin validar antes su reemplazo.

## Qué encontré al analizar el programa

El programa hace mucho y lo hace bien, pero **reparte tu trabajo en 11
pestañas que son caras distintas de las mismas dos cosas**:

1. **Todo nace de la planilla** (equipos + plan + resultados). Alertas,
   documentos, informes y cierre se calculan solos desde ahí. Lo único que
   tú registras a mano: ejecuciones, correctivos, asignaciones y estados
   de documentos.
2. Tu trabajo tiene **dos ejes**: el **equipo** (su expediente: historial,
   documentos, reparaciones) y el **mes** (asignar → ejecutar → documentar
   → informar → cerrar). Hoy esos ejes están cortados en pedazos:
   - Para cerrar un mes pasas por **5 pestañas**: Plan MP, Asignación,
     Documentos, Informes y el botón de Cierre.
   - **Hoy y Panel** repiten lo mismo (resumen + alertas) con distinto énfasis.
   - Las "cosas por hacer" viven en **3 lugares**: Pendientes, Documentos
     y la bitácora de Correctivos — cuando casi todas se generan solas.

## El programa que te propongo: 5 pestañas

| Hoy (11) | Propuesta (5) | Qué pasa |
|---|---|---|
| 🌅 Hoy + 📊 Panel | **🌅 Mi día** | Una sola pantalla de partida: arriba lo accionable (plazos, perseguir ST, papeles por mover, delegaciones por verificar, tareas sueltas), abajo los números para jefatura (cumplimiento, ST, no operativos). |
| 🗂 Inventario | **🗂 Equipos** | Igual que hoy: buscar → abrir ficha → resolver. La ficha ya es el expediente completo (plan, documentos, correctivos, historial). |
| 🗓 Plan MP + 👷 Asignación + 📁 Documentos + 📄 Informes | **🗓 Mes de trabajo** | El ciclo mensual completo, en orden, en una pestaña: ① asignar ejecutores (Excel con desplegable, subir de vuelta) → ② registrar ejecución y causales → ③ documentos del mes (imprimir lote → entregar → archivar) → ④ informes por servicio → ⑤ cierre con checklist. Incluye "imprimir protocolos del mes por técnico" (idea tuya pendiente). |
| 🛠 Correctivos | **🛠 Servicio técnico** | Igual que hoy: casos con hitos, días en estado y bitácora para perseguir. No es mensual: son casos abiertos hasta que se cierran. |
| ⚙️ Datos + 🧾 Reportes | **⚙️ Datos** | Importar maestro, respaldos, ejecutores. El generador de protocolos queda aquí como herramienta y como botón dentro de Mes de trabajo. |
| 📌 Pendientes | *(deja de ser pestaña)* | Las tareas sueltas (pocas, con fecha y delegado) se anotan y se ven en **Mi día**. Matriz Eisenhower, sapo y tablero se retiran: te generaron fatiga y los documentos ya se gestionan solos. |

## Qué NO cambia (tus decisiones firmes)

Un solo archivo que abre con doble clic, sin internet. El Excel oficial manda
(importación-fusión sin pérdida). El estado del equipo se deriva de eventos.
Filtros tipo Excel en todas las tablas. Todos los formularios e impresos
actuales se conservan tal cual.

## Cómo llegaríamos (sin retroceder nunca)

Cada fase: se construye lo nuevo **junto a** lo viejo → tú lo validas con tus
datos reales → recién ahí se retira lo viejo. Si algo no te gusta, se revierte.

- **F2** Mi día (fusión Hoy + Panel) → validar → retirar Panel
- **F3** Mes de trabajo, parte 1 (Plan + Asignación) → validar → retirar Asignación
- **F4** Mes de trabajo, parte 2 (+ Documentos + Informes + protocolos del mes) → validar → retirar ambas
- **F5** Pendientes como lista simple en Mi día → validar → retirar pestaña
- **F6** Pulido final (nombre del hospital unificado, recordatorio de respaldo semanal)

## Qué necesito de ti

1. **Tu respaldo real** (.json de la pestaña Datos, o el .xlsm maestro): para
   calibrar la propuesta con tus números reales y probar cada fase con ellos.
2. ¿La estructura de 5 pestañas te hace sentido? ¿Cuál no te calza?
3. Nombre a unificar en todo el programa: ¿"Hospital Regional de Temuco" o
   "Hospital Doctor Hernán Henríquez Aravena"?
