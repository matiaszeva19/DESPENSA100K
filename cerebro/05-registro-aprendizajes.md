# 05 — Registro de Aprendizajes, Referentes y Criterio de Skills (Cerebro Principal)

> **Propósito:** Memoria evolutiva del sistema. Registra skills evaluadas, los 15 referentes/competidores analizados y los resultados reales de los videos publicados.

---

## Criterio de Evaluación de Nuevas Skills / Ideas

| Filtro | Pregunta clave |
| :--- | :--- |
| **1. Encaje local** | ¿Funciona para Chiche en Campana Centro (calle Perón al lado del Día)? |
| **2. Viabilidad operativa** | ¿Se puede grabar con celular y editar en CapCut con detalle claro? |
| **3. Impacto en retención/visitas** | ¿Mejora los 4 ingredientes del gancho, la zona de retención o atrae clientes al local? |
| **4. Simplicidad** | ¿Suma estructura accionable sin burocracia vacía? |

---

## Registro de Skills y Metodologías Evaluadas

| Fecha | Skill / Fuente | Decisión | Motivo / Cómo se integró |
| :--- | :--- | :--- | :--- |
| 2026-11-18 | Arquitectura Base + HyperFrames | **Adoptada** | Base modular inicial; HyperFrames queda como apoyo puntual si se necesitan placas/overlays complejos. |
| 2026-11-18 | `blacktwist/social-media-skills` | **Adaptada / Consolidada / Descartada** | Se integraron patrones de hooks, corte de caption y planificación flexible; se consolidó analítica en `subagente-analista-mejora`; se descartó texto B2B (LinkedIn/X/Bluesky) y MCP externo. |
| 2026-11-18 | `coreyhaines31/marketingskills/marketing-psychology` | **Adaptada (Selectiva)** | Extraídos 14 principios útiles en mostrador (JTBD, Zeigarnik, Pratfall, Mere Exposure, Contabilidad Mental, Ley de Hick, Prueba Social) e integrados sin subagente extra. |
| 2026-11-18 | `louisblythe/Sales-Skills` | **Adaptada (3 de 122)** | Extraído LAER para objeciones, cross-sell natural y arco narrativo en 4 tiempos; descartado todo lo de bots SDR/B2B. |
| 2026-11-18 | `Varnan-Tech/opendirectory` | **Adaptada (3 de 65)** | Integrado filtro anti-IA (`human-tone`), Openverse/audio mono (`openverse-sfx`) y mapa de ritmo; descartados scrapers dev y `meta-tribeV2`. |
| 2026-11-18 | `karanb192/awesome-claude-skills` | **Descartada como paquete** | Es un índice de enlaces externos; evaluar solo links puntuales si hacen falta. |
| 2026-11-18 | **Metodología Propia del Creador + Subagente Investigador** | **Adoptada al 100%** | Se incorporaron los 4 ingredientes del gancho, 3 tipos de gancho (con las 6 reglas estrictas del texto en pantalla), zona de retención + 4 pilares de confianza y se creó `subagente-investigador-competencia`. |
| 2026-11-18 | `adelaidasofia/instagram-mcp` | **Adoptada para Fase 2** | MCP oficial de Instagram Graph API (insights por post, guardados/compartidos, ciudad de audiencia, comentarios y `business_discovery` de cuentas públicas). Queda en espera hasta crear el Instagram Business de Chiche. |
| 2026-11-18 | `Panniantong/agent-reach` (v1.6.1 ya instalada en el sistema) | **Adoptada (Selectiva y con resguardo)** | Aporta búsqueda/lectura web y YouTube (títulos/subtítulos de Shorts) en `subagente-investigador-competencia`. IG y Facebook son canales **experimentales** que requieren login (usar solo cuenta secundaria si el usuario decide activarlos). **No soporta TikTok.** |
| 2026-11-19 | Metodología Kallaway — *How to Master Storytelling* (`WluuZB_ck9Q`) | **Adoptada y Adaptada** | **Adoptado en `cerebro/04`, `subagente-guionista-hooks` y `subagente-editor-video`:** planificar desde el remate, arranque sin "W" lentas, fricción *"pero / por eso"* (solo en cuerpo hablado, nunca en Gancho de Texto para no violar las 6 reglas), *Dopamine Ladder* (estimulación 0–2s → curiosidad → anticipación → validación → afecto con Cristina → firma Pavloviana), rehooks en >18s, Héroe vs. Obstáculo, pintura sensorial y micro-clímax visual cada 2–3s. **Descartado:** formato largo YouTube (~60min) y plataformas/herramientas pagas mencionadas (*Sandcastles*, *Skool*, software pago). |
| 2026-11-19 | Canal `@kallawaymarketing` — Top 3 videos más vistos (`8cQidXgtGmU`, `2byPP_9F0-Q`, `LmXpbP7dD48`) | **Adoptada y Adaptada** | **Adoptado en `cerebro/04`, `subagente-estratega-local`, `subagente-guionista-hooks`, `subagente-investigador-competencia` y `subagente-editor-video`:** *Audience Matching* y disciplina de muestra inicial (~200 no seguidores sin virales fuera de avatar); *4 Jinetes del Engagement* + 5 disparadores de comentarios con postura firme; los 4 errores fatales del gancho (*Delay, Confusion, Irrelevance, Disinterest* + Test de Aislamiento 6º grado + *"vos/tu"* + Contraste A vs. B); fórmula hablada en 3 pasos (*Context Lean → Scroll Stop Interjection → Contrarian Snapback*, solo en audio hablado), oraciones *staccato* (0–4s), *Cult Hopping* local, texto visual de 3–5 palabras grandes + movimiento calibrado, ventana crítica ≤4s (*Value Loop*) y análisis por *Outlier Score*. **Descartado:** *Sandcastles AI*, *Short Form Academy*, funnels B2B/SaaS pagos y clickbait vacío. |
| 2026-11-19 | Andrea Estratega — *Equipo de Marketing con Agentes IA* (`lITYzb6Rn8k`) | **Adoptada y Adaptada (Arquitectura Nivel 3)** | **Adoptado en `AGENTS.md`, `agente-maestro`, `subagente-distribucion-leads`, `subagente-editor-video`, `subagente-analista-mejora` y `produccion/semanas/`:** distinción explícita *Segundo Cerebro (`cerebro/`) + Skills + Agentes en 3 capas* (Instrucción/Límites, Skills, Herramientas); mapeo a 5 roles (**Maestro, Radar, Aria, Cali, Nova**); **Checkpoint Humano obligatorio** (proponer 7 piezas → pausa para OK humano → recién producir en paralelo); carpeta única semanal; **overlays/placas listas** + **Carruseles sin cámara** + **Secuencias de Venta por Historias (IG/WA)** y bucle de auditoría semanal de Aria al equipo. **Descartado:** suscripción paga a *Skool Fórmula 100k* (USD 47/mes) y generación artificial de persona/producto con herramientas pagas tipo *Higgsfield* (Chiche filma real en mostrador con Cristina). |
| 2026-11-18 | `ZJU-REAL/Easel` (113 skills) | **Adaptada (3 mecánicas) / Descartado el resto** | Se integró la **autopsia por capas** y **minería de preguntas en comentarios** en `subagente-analista-mejora`, más el **filtro de viabilidad de ideas** en `subagente-estratega-local`. Se descartaron ~110 skills/scripts de redes chinas (Douyin, Xiaohongshu, WeChat, Bilibili). |
| 2026-11-18 | `Shaitrish/37studio` | **Descartada (Redundante)** | App de escritorio con HyperFrames + publicación; ya cubierto nativamente con Antigravity + HyperFrames + celular/CapCut. |
| 2026-11-18 | `trypostit/trypost`, `cbsshekhawat18-lab/social-stats-social-media-manager`, `GkhanKINAY/postqueen-app` | **Descartadas** | Plataformas completas de scheduling tipo Buffer/Hootsuite (PHP/Django/TS + Docker). Infraestructura innecesaria hoy para 3 videos semanales y cuentas aún sin abrir. |
| 2026-11-18 | `soxoj/maigret` y `benedekrozemberczki/awesome-community-detection` | **Descartadas (Fuera de rubro)** | `maigret` es OSINT para investigar usernames de personas; `awesome-community-detection` es una lista académica de papers de grafos/ML. Cero utilidad para Chiche. |
| 2026-11-25 | **Canva MCP + Flujo de Carrusel 4:5 (`DAHb8saf5sE`)** | **Adoptada** | Validado para subir fotos reales del local previamente enderezadas (EXIF aplicado) y generar carruseles editables `1080×1350` directo en la cuenta del creador (`Matias Zevallos`). |

---

## Radar de Competencia (Campana) y Top 15 Referentes del Rubro

> Mantenido por `subagente-investigador-competencia`. Informe completo en `produccion/ideas/2026-11-investigacion-competencia-referentes.md`.

| # | Cuenta / Referente | Ámbito | Qué hace bien (Gancho / Visual / Ancla) | Cómo lo potenciamos en Chiche |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Supermercado Día (`Av. Perón 531`) | Campana (Pegado a Chiche) | Tráfico peatonal masivo (8–22hs) y promos Club Día. | Atacar sus fricciones reales: filas, un solo empleado y fiambre envasado; mostrar corte vivo sin espera. |
| 2 | El Parmegiano (`@elparmegiano` — 47k seg. · San Martín 397) | Campana (Cadena 11 suc.) | Reels prolijos de aperturas y lifestyle con música. | **Cierra 20:30**, casi no publica contenido específico de Campana, **cero voz/ganchos de texto ni precios**. Chiche atiende hasta las **21:00** y habla directo al centro de Campana. |
| 3 | Mauro Fiambres (`@maurofiambres` — 1.763 seg.) & Locos por el Queso (`@locosporelqueso19` — 644 seg.) | Campana (Locales) | En Mauro rinde la prueba social/charla (35–126 likes); en Locos rindió mostrar una persona real del equipo (59 likes). | Mauro no tiene local fijo ni precios y sus posts diarios caen a 0–5 likes por copy repetitivo; Locos casi no publica y solo usa placas estáticas de mañana. Chiche domina con Reels constantes, precios/rinde claros y cara/voz humana. |
| 4 | La Cañada (`Av. Mitre 1155`), LA TABA (`Lavalle 521`), Santa Germina (IG caído) | Campana (Locales) | La Cañada en tablas por WhatsApp; La Taba en Facebook tradicional (cierra 20:30). | Terreno de Reels locales prácticamente vacío en Campana para compra espontánea en Perón 500 hasta las 21hs. |
| 5 | `@almacenlodeadri` (El Jagüel — 155,8k seg. verif.) | Referente Indirecto Despensa (IG) | 100% Reels en el local real; debate de heladera con precios a mano (*"Alfajores fríos?"*) = **5,3k likes / 439 com.**; backstage reposición = **1,2k likes**. | **Referente #1 para Despensa:** replicar debates cotidianos con precios visibles + backstage antes del cierre (21hs) + bio con ubicación/horario completo. |
| 6 | `@elpeladodelossandwiches` (Villa María — 274,6k seg. verif.) | Referente Indirecto Fiambrería (IG) | Cara real + micrófono corbatero detrás del mostrador (**7,8k–24,5k likes**); POV de balanza `0.265` + comanda a mano = **1,5k likes**. | **Referente #1 para Fiambrería:** armar producto en vivo mientras se habla a cámara; en planos sin cara usar POV de balanza + cortadora. |
| 7 | `@piccadely` (52,1k seg.) y `@mercadito.fiambreria` (59 seg.) | Anti-patrones verificados (IG) | Piccadely oculta precios, sin cara y cierra comentarios (**12–94 likes**); Mercadito solo fotos estáticas genéricas (**6–17 likes**). | **Validado qué evitar:** nunca usar fotos mudas de catálogo ni ocultar precios/ubicación; en barrio gana la cercanía humana y Reels con gancho. |
| 8 | `@maritolaurens` (TikTok) y `@elpicaderomg` | Referentes Arg | Balanza como ancla de confianza contra engaños + gancho de ahorro/ocasión local. | Replicar prueba de balanza y frescura real en Chiche (cero ASMR, voz directa). |

---

## Bitácora de Rendimiento en Redes (Métricas Reales Verificadas)

> **Nivel de confianza actual:** **Señales tempranas** (3 publicaciones auditadas en `@chichefiambres` en TikTok Studio al 26/11/2026; cuenta con **75 seguidores** y **2.6K Me gusta totales**). Todavía no sacar reglas rígidas hasta completar 5–15 videos, pero ya hay hallazgos claros de qué retiene y genera conversación.

| Fecha | Pieza / Video (TikTok `@chichefiambres`) | Duración / Formato | Vistas | Retención (`3s` / Promedio / Completo) | Interacción (`Likes` / `Com.` / `Comp.` / `Guard.`) | Hallazgo Clave |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 2026-11-24 20:37 | Video 1 — Presentación *"¡Hola Campana! Te esperamos todos los días..."* | `00:32` · Video | **4.9K** (`4,902`) | `59%` a 3s · `7.08s` prom · `1.8%` completo | `96` / `2` / `0` / `8` (`14` seg.) | El arranque institucional cae fuerte al seg 10 (`21%`). Muy bajo completado (`1.8%`) frente a un video con situación real. |
| 2026-11-25 15:21 | **Video 2 — *"¿Saliste tarde de trabajar en Campana..."* (Abierto hasta 21hs)** | `00:29` · Video Cristina | **34K** (`34,000`) | `64%` a 3s · **`13.32s` prom** · **`13.9%` completo** | **`2,459` / `53` / `31` / `66`** (`69` seg.) | **Ganador x7 en retención completa:** espontaneidad de Cristina creó el apodo viral *"Señora Exitosa / 90+5 / Que Resuelve"* + debate humorístico por el horario `21hs` disparó 53 comentarios y `171h` de watch time (`99.3% Para ti`, `94%` Argentina, `81%` edad 18–34). |
| 2026-11-25 17:20 | Post 3 — Carrusel fotos (`No hay descripción`) | Carrusel estático | **276** | `6.37s` prom · `27.3%` completo | `10` / `0` / `0` / `0` (`1` seg.) | Subido **sin caption ni keywords de Campana**; `59.9%` vino solo del perfil (`36.8% Para ti`). Los carruseles mudos sin copy rinden muy poco en TikTok. |

### Auditoría de Comentarios & Directivas para Semana 2 (`Subagente 4 → Equipo`)

1. **Minería de comentarios reales (Video 2 — 34K):**
   - **Meme / Identidad ganadora (Cristina):** *"señora existosa"* (136 likes), *"gracias señora 90+5"* (96 likes), *"Gracias señora último momento"* (72 likes), *"Señora que resuelve"* (33 likes), *"una cara de buena esta mujer"* → **Cristina espontánea (incluso saliéndose del libreto) es el mayor activo de confianza y viralidad.**
   - **Fricción / Objeción de horario (10+ comentarios):** *"pensé que se iba a estirar hasta las 23"* (33 likes), *"pense q cerraba alas 00"*, *"Todos los chinos cierran a las 9..."* → El contraste de *"abierto hasta las 21"* generó debate sano y retención en loop mientras leían comentarios.
   - **Objeción de precio y stock (2 comentarios):** *"Si el pan está re caro, no me quiero imaginar lo demassss"*, *"Encontrás de todo, pero pan ya no"* → Señal directa para responder con **transparencia de precios reales al corte** (sin pelear).
   - **Fuga geográfica por viralidad:** Aparecieron comentarios de Tigre y La Rioja (`94%` Argentina). Hay que reforzar visual y verbalmente **"Campana · Av. Perón 525 (al lado del Día)"** para convertir alcance en visitas locales.

2. **3 Directivas concretas para el equipo (Semana 2):**
   - **Para `subagente-estratega-local` (Calendario):** Pasar los **carruseles de fotos solo a Instagram** y en **TikTok subir 100% videos con Cristina**; incluir **2 videos de Respuesta a Comentario** del hit de 34K (uno con guiño a *"la señora 90+5 / cierre 21hs"* y otro respondiendo a la duda de precios con corte en balanza y precio real a mano).
   - **Para `subagente-guionista-hooks` (Guiones):** **Nunca volver a guionar "presentaciones institucionales" genéricas** como el Video 1 (`1.8%` completo). Abrir siempre en `0–2s` con una situación cotidiana urgente (*saliste tarde / cena rápida / cuánto te sale*) y **no forzar a Cristina a recitar de memoria**: darle 3 ideas clave para que hable con su tono natural que ya enamoró al público. Anclar **"Campana / Perón 525"** en texto y cierre.
   - **Para `subagente-editor-video` (Edición y Copys):** **Prohibido publicar sin descripción (`No hay descripción`)**: todo post debe llevar caption SEO con `Campana` y `Av. Perón 525`. Seguir acortando los primeros `0–2s` (mayor caída actual en `0:01` con `84%`) con movimiento inmediato + texto grande arriba de 2 líneas.

3. **Ajustes aprobados tras auditoría y producción (`26–27/11/2026`):**
   - **Bio oficial simplificada:** Arrancar siempre con **`🧀 Fiambrería y Despensa`** + ubicación **`Av. Perón 525 (al lado del Día)`** + teléfono **`3489 55-7613`** visible directo en la bio.
   - **Hooks cortos de lectura fácil para Cristina:** Priorizar frases cortas que salgan de una sola toma sin trabarse y abrir nueva línea de video combinando **salame + quesos** de las canastas del mostrador.
