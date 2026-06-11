# CONTEXTO — Lo que sé del usuario y del proyecto

> Complementa a `CLAUDE.md` (contexto heredado de la sesión original, sigue vigente).
> Este archivo acumula lo aprendido sesión a sesión. Leerlo SIEMPRE al inicio, junto a `PLAN.md`.

## El usuario y su trabajo
- Ingeniero responsable administrativo de ~966 equipos biomédicos críticos del
  Hospital Regional de Temuco / HHHA (Hospital Dr. Hernán Henríquez Aravena).
- No repara equipos: **delega y persigue que se cumpla**. Necesita registro fechado
  de a quién preguntó y qué le respondieron.
- El documento oficial por resolución es el Excel `Programación MP 2026.xlsm`;
  GEB es su herramienta de control diaria. **El Excel manda**.
- Su mes "se cierra" cuando la carpeta física de cada equipo tiene todos los
  documentos firmados (corazón de la pestaña Documentos).
- Repositorio GitHub: `cribeltr/ingenieria-y-mantenimiento-hhha`.

## Preferencias de trabajo (firmes)
- Siempre en español; respuestas cortas y al grano, sin tecnicismos.
- Minimalista: prefiere filtrar antes que anotar; quiere podar vistas que no usa
  (la matriz Eisenhower le generó fatiga visual; Pendientes abre en vista lista).
- Preguntar el "¿para qué?" cuando pida algo y el fin no sea evidente; diseñar
  para su fin real, no para la petición literal. La decisión final es suya.
- Lo que ya funciona es intocable salvo acuerdo explícito.
- Tras cada cambio validado: commit + push + entregarle `index.html`.
- Trabajo por fases pequeñas; él valida cada fase antes de avanzar.

## Decisiones técnicas firmes (resumen; detalle en CLAUDE.md)
- Un solo archivo `index.html`: sin servidor, sin internet, sin librerías externas.
  Datos en localStorage (clave `geb_hrt_v3`); respaldo/restauración JSON en Datos.
- La app parte VACÍA; todo entra importando el `.xlsm` oficial con fusión sin
  pérdida (columnas Q-Observación y S-Responsable excluidas).
- El estado del equipo NUNCA se edita a mano: deriva de eventos.
- Lector y generador de Excel propios (sin librerías); filtros tipo Excel
  genéricos (`fcCfg`/`thFC`/`dropFC`) obligatorios para toda tabla nueva.
- `render()` restaura el foco del input activo: no romper (búsqueda en vivo).
- Probar con los respaldos JSON reales del usuario antes de entregar.

## Preguntas abiertas (esperando respuesta del usuario)
1. Nombre correcto del hospital para unificar (GEB dice "Hospital Regional de
   Temuco"; los reportes técnicos dicen "Hospital Doctor Hernán Henríquez Aravena").
2. Destino de las pestañas ocultas: cuáles se reactivan, cuáles se podan definitivamente.

## Bitácora de aprendizajes
- 11-06-2026 · Inicio de esta etapa: se recibe el zip con el proyecto completo
  (index.html + documentación) y se incorpora al repositorio nuevo sin cambios.
- 11-06-2026 · El usuario dirige el trabajo con instrucciones concretas y valida
  pasando a lo siguiente (no espera ceremonias). Decidió: **trabajar en una sola
  vista a la vez, partiendo por Inventario** (las demás ocultas con `TABS_VISIBLES`,
  código intacto).
- 11-06-2026 · Se refiere a los equipos por su **N° de inventario** (ej. "2-0166863"),
  no por el ID interno del Excel.
- 11-06-2026 · Su flujo documental real, contado con su ejemplo: en la ficha del
  equipo quiere VER qué documento falta para completar el plan (abril con causal
  C5 ⇒ falta el Reporte de Reprogramación con fecha fin de mes, 30-04) y desde ahí
  **imprimir → entregarlo a una persona (ej. Ignacio Berner Bergara) dejando la
  delegación registrada → archivar** cuando vuelve firmado. Eso reemplaza anotarlo
  como pendiente manual.
- 11-06-2026 · "Ignacio" = Ignacio Berner Bergara (de la lista de ejecutores).
