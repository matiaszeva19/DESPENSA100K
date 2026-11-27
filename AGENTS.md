# Sistema de Agentes — Contenido y Crecimiento Local (Fiambrería / Despensa · Campana)

Este workspace alberga el sistema operativo de contenido para redes sociales de **Chiche**, una **fiambrería / despensa en Campana, Buenos Aires**.
Su propósito es **posicionar el negocio en la zona centro de Campana** y **atraer visitas al local y leads para ventas** a partir de contenido grabado y editado por el creador.

---

## Arquitectura del Sistema (3 Capas)

### 1. El Cerebro Principal (`cerebro/`)
- **Rol:** Fuente única de verdad (*Single Source of Truth*) y memoria estratégica del negocio.
- **Función:** No redacta ni edita; almacena la identidad del local, productos, ofertas, perfil del cliente de Campana, metodología exacta de hooks/grabación/edición del creador y aprendizajes validados.
- **Regla obligatoria:** Ningún agente puede proponer guiones, precios, promos o estrategias sin consultar primero los archivos pertinentes en `cerebro/`. Si falta un dato clave, se pregunta o se marca como `[COMPLETAR]`; nunca se inventa.

| Archivo | Qué contiene |
| :--- | :--- |
| `cerebro/01-negocio-y-identidad.md` | Identidad de Chiche, ubicación en calle Perón al lado del Día, objetivos, tono y diferenciales. |
| `cerebro/02-productos-y-ofertas.md` | Catálogo, productos estrella (fiambres, quesos, picadas, despensa) y promos activas. |
| `cerebro/03-audiencia-campana.md` | Público objetivo local, hábitos en Campana centro, objeciones y disparadores. |
| `cerebro/04-estilo-y-formas-de-trabajar.md` | Metodología de hooks (4 ingredientes + 3 tipos), retención, equipamiento y flujo en CapCut. |
| `cerebro/05-registro-aprendizajes.md` | Bitácora de rendimiento, referentes analizados, skills adoptadas/descartadas. |

---

### 2. El Agente Maestro (`.agents/skills/agente-maestro/SKILL.md`)
- **Rol:** Director de Operaciones de Contenido y Orquestador (Nivel 3 — *Agent Team*).
- **Regla de Calidad No Negociable:** **Cero entregas vagas o superficiales.** Cada planificación debe bajar a calendario concreto, copys exactos dentro y fuera del video, descripción detallada toma por toma de qué hacer al grabar, overlays listos y edición exacta en CapCut.
- **Regla Obligatoria Previa a Nuevos Videos:** **Siempre ejecutar primero una pasada fresca del `subagente-investigador-competencia`** (competencia en Campana, tendencias de temporada y referentes virales del rubro) antes de guionar o armar cualquier tanda nueva de videos.
- **Checkpoint Humano Obligatorio:** Al planificar una semana o mes en lote, el Maestro investiga y propone primero la grilla de ideas, **se frena para que apruebes** y recién con tu *"OK / producir todo"* despacha en paralelo los guiones, guías de rodaje, edición/overlays, carruseles e historias.
- **Función:**
  1. Leer el estado actual del **Segundo Cerebro (`cerebro/`)**.
  2. Orquestar a los **Subagentes Especialistas** (cada uno definido en 3 capas: **Instrucción + Límites**, **Skills que invoca**, **Herramientas/MCPs**).
  3. Sistematizar toda la semana en una sola carpeta (`produccion/semanas/YYYY-semana-NN/`) y auditar con 6 filtros: **Campana real**, **Cero humo / Anti-IA**, **4 Ingredientes + 3 Ganchos (reglas estrictas de texto en pantalla)**, **Zona de Retención + Ancla de Confianza**, **Grabable con detalle en mostrador** y **CTA real a visita/lead**.
  4. Evaluar nuevas skills o metodologías que aporte el usuario y registrar la decisión en `cerebro/05-registro-aprendizajes.md`.

---

### 3. El Equipo Conectado: 1 Agente Maestro + 4 Subagentes Especializados

Distinción clave: **`cerebro/`** guarda la verdad única del negocio; **`produccion/oficina/estado-equipo.json`** es el **bus de estado compartido** para que ningún agente trabaje por inercia ni desconectado de los demás. **Regla obligatoria:** cada subagente debe ejecutar primero un **Análisis de Respaldo** (leyendo `cerebro/`, métricas previas y las entregas de sus pares) antes de producir y entregar su resultado concreto al **Agente Maestro**.

| Agente | Skills que utiliza | Rol y Tarea Única | Análisis de Respaldo Obligatorio | Conexión y Entrega al Maestro |
| :--- | :--- | :--- | :--- | :--- |
| **Maestro Orquestador** | `agente-maestro` | Coordina la mesa, aprueba el checkpoint semanal, exige análisis previo, audita los 6 filtros y consolida el paquete final. | Verifica `cerebro/01..05` y coherencia global antes de aprobar. | Recibe los 4 reportes y arma `produccion/semanas/YYYY-semana-NN/`. |
| **1. Guionista de Hooks y Calendarizador** | `subagente-guionista-hooks` + `subagente-estratega-local` | Define la **calendarización** (qué se graba cada día) y redacta **guiones + 3 ganchos** (Texto ≤2 líneas 0 puntuación, Hablado Kallaway 3 pasos, Visual, CTA). | Analiza audiencia de Campana, referentes locales y el informe de **Métricas (Subagente 4)**. | Pasa calendario y guiones a **Carruseles (2)** y **Ayudante Editor (3)**; reporta al Maestro. |
| **2. Diseñador de Carruseles y Placas** | `subagente-editor-video` (Carruseles/Nova) + `subagente-distribucion-leads` | Crea los **carruseles de mostrador** (5–7 placas), portadas, textos de overlays y **secuencias de Historias (IG/WA)**. | Analiza calendario/ganchos del **Subagente 1**, ofertas de `cerebro/02` y guardados/compartidos de **Métricas (4)**. | Coordina estética con **Ayudante Editor (3)** y entrega carruseles + portadas + copies al Maestro. |
| **3. Ayudante Editor y Director de Rodaje** | `subagente-director-grabacion` + `subagente-editor-video` | Te guía **qué grabar y cómo moverte en cuadro** con Cristina en Av. Perón 525, y arma el **mapa CapCut segundo a segundo**. | Analiza guiones del **Subagente 1**, portadas del **Subagente 2** y reglas de ritmo/cero ASMR de `cerebro/04`. | Entrega hoja de rodaje + timeline CapCut al Maestro y marca puntos de retención para **Métricas (4)**. |
| **4. Analista de Métricas y Resultados** | `subagente-analista-mejora` | Estudia **vistas, retención 3s, guardados, compartidos y leads WhatsApp** de cada video publicado; detecta qué funciona y qué no. | Compara cada video contra el promedio del local y mina preguntas reales de comentarios/DMs. | Emite informe de respaldo y directivas a los **Subagentes 1, 2 y 3** y al Maestro en `cerebro/05`. |

---

## Flujo Operativo Conectado (Bus Compartido)

```text
                  ┌──────────────────────────────────────┐
                  │  4. ANALISTA DE MÉTRICAS (Subagente) │
                  │  Estudia qué funcionó y qué no       │
                  └──────────────────┬───────────────────┘
                                     │ Informe de respaldo + directivas
                                     ▼
 [Agente Maestro] ◄──► [1. GUIONISTA & CALENDARIZADOR] ──► (Qué grabar + Hooks)
        ▲                            │                              │
        │                            ▼                              ▼
        │             [2. CARRUSELES & PLACAS] ◄──────► [3. AYUDANTE EDITOR & RODAJE]
        │              (Carruseles + Portadas)           (Cómo grabar + CapCut)
        │                            │                              │
        └────────────────────────────┴──────────────────────────────┘
               Todo conectado en `produccion/oficina/estado-equipo.json`
```

---

## Carpeta de Producción

- `produccion/semanas/YYYY-semana-NN/` — **Carpeta única por semana aprobada** (calendario maestro en tabla, guiones, plan de grabación en tanda, textos de overlays/portadas, carrusel e historias).
- `produccion/ideas/` — Investigaciones de competencia, referentes, perfiles y planificación mensual base.
- `produccion/guiones/` — Guiones individuales sueltos con los 3 ganchos, shot list detallada y copy completo.
- `produccion/crudos/` — Notas sobre videos grabados, duración y tomas disponibles.
- `produccion/edicion/` — Mapas de edición en CapCut, overlays, composiciones HyperFrames y entregables finales.
