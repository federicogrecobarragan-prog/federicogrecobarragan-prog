# Federico Greco Barragán

**Chief Officer IA Manager & KAM en CDA** · Buenos Aires, Argentina.

Construyo sistemas multiagente autónomos, automatización con IA y herramientas para Claude Code y agentes de codificación.

Este perfil está organizado con **topics**. Podés filtrar cualquier categoría desde la búsqueda de GitHub, por ejemplo:

```
user:federicogrecobarragan-prog topic:harness
```

---

## 🚀 ¿Arrancás un proyecto nuevo? — Matriz de capacidades

> **Este README es el REPOSITORIO MADRE.** Antes de empezar cualquier proyecto, mirá acá qué tenés ya disponible para potenciarlo. Buscá el tipo de proyecto y combiná las piezas. Casi todo es reutilizable entre dominios.

| Si el proyecto es de… | Qué tenés para potenciarlo | Repos clave |
|---|---|---|
| **Ventas · Outreach · Captación** | Mapear decisores de una cuenta, sourcing de leads, secuencias de outbench (LinkedIn/email/social), CRM y casos de éxito para cerrar. | `linkedin-orgchart`, `recluta-os`, `OpenOutreach`, `growchief`, `crm-colmena`, `cda-casos-exito`, `n8n` + `n8n-nodes-instantly`, `oficina-de-jhonson-agencia` |
| **Diseño · UI · Branding** | Generar UIs/landings premium, design systems, componentes, creativos con IA, video desde HTML, edición de imagen. | `open-design`, `open-codesign`, `emil-design-eng`, `ui-ux-pro-max-skill`, `claude-creative-work`, `hyperframes`, `Fooocus`, `PhotoGIMP` |
| **Programación · Harness · Agentes** | Spec-driven dev, orquestación de sub-agentes, meta-prompting, skills, safety hooks, code review, memoria. Arranque de proyecto cargando contexto del ecosistema desde la LLM Wiki. **Catálogo + sync de skills propias entre PC local y VPS (`skills-ecosistema`)**. | `arrancar-proyecto` (skill), **`skills-ecosistema`** (catálogo + sync de skills local↔VPS, mapeo por objetivo), `gstack`, `cc-sdd`, `get-shit-done`, `agent-teams-lite`, `open-agents`, `hermes-agent`, `caveman`, `claude-code-safety-hooks`, `gentleman-guardian-angel`, `pskoett-ai-skills`, `awesome-claude-code`, `awesome-agent-skills` |
| **Web · Landing · Sitios** | **Framework build+deploy end-to-end (`montar-web`)**: 2 stacks (SPA React+CDN sin build / HTML vanilla), backend Supabase (leads/blog/noticias/panel funnel), chat agéntico, lead-magnets, e-commerce con IA, GEO/AEO, deploy Hostinger/Vercel/nginx + verificación 360. Más: plantillas de referencia, clonar referencias, SEO, analytics, agenda embebida. | `montar-web`, `decretando-disney-web`, `oficinadejhonson-web`, `Syncro-WEB`, `lightingyoga-web`, `open-design`, `goclone` / `Website-Cloner`, `claude-seo`, `analytics`, `cal.diy` |
| **Marketing · SEO · Contenido** | Auditoría/generación SEO, intel de búsqueda (SerpApi), agencia de marketing IA, funnels, creativos, distribución, **cockpit de marketing (funnel de leads + ads/email/social/contenido)**. | `claude-seo`, `serpapi-claude-plugin` / `serpapi-cursor-plugin`, `ai-marketing-claude`, `colmena-digital`, `command-center` (módulo Marketing), `Fooocus`, `n8n` |
| **Scraping · Datos · Intel** | Scraping adaptativo, scraping por LLM, crawling, organigramas LinkedIn, media→texto, consola de resultados. | `Scrapling`, `Scrapegraph-ai`, `firecrawl`, `linkedin-orgchart`, `scraping-dashboard`, `Webwright`, `yt-dlp` + `whisper`, `obsidian-clipper` |
| **Automatización · Mensajería** | Motor de workflows, nodos a medida, WhatsApp self-hosted, agendamiento, alertas a Telegram. | `n8n`, `n8n-nodes-instantly`, `OpenWA`, `wa-automate-nodejs`, `wa-avd-docker`, `cal.diy`, `notify-admin-telegram`, `growchief` |
| **Infra IA · Memoria · Modelos** | Router local-first (ahorro de tokens), memoria persistente, índice vectorial, transcripción, workspace IA, MCP. | `llm-local-router`, `engram`, `turbovec`, `whisper`, `gentle-ai`, `odysseus`, `AppFlowy-Cloud`, `inspector`, `mcp-for-beginners`, `playwright` |
| **Seguridad · Supply-chain** | Escaneo de vulnerabilidades, auditoría de paquetes npm pre-install, hooks de seguridad, deploy hardened. | `nuclei`, `npq`, `npm-security-best-practices`, `claude-code-safety-hooks`, `openclaw-safe-update`, `infra-deploy`, `vw_web_builds` |
| **Apps mobile · Play Store · iOS** | Framework completo Expo → Play Store (build, Hermes, Edge Function LLM, data safety, closed testing 12×14d, legales). Apps de referencia listas, incluida una **local-first sin backend con cifrado en reposo + biometría real**. | `mobile-playbook`, `folio-os`, `alimentando-a-popa`, `mishizen`, `la-boveda`, `pinta-pinta` |
| **Fintech · Pagos** | Integración de pagos generada, agente autónomo que cobra. | `agente-pagokit`, `cashclaw` |

> **Proyectos combinados:** la mayoría de los proyectos reales mezclan dominios. Ej.: una **web de captación** = `open-design` (diseño) + `claude-seo` (marketing) + `cal.diy` (agenda) + `analytics` (medición) + `linkedin-orgchart`/`OpenOutreach` (outreach del lead). El **harness** (`gstack`/`cc-sdd`/`caveman`/safety-hooks) aplica como capa transversal a cualquier proyecto de código.

---

---

## 🧠 Las 4D en el ecosistema agéntico

El harness de La Colmena opera sobre el **AI Fluency Framework de Anthropic** (Rick Dakan & Joseph Feller): cuatro competencias que convierten el uso casual de IA en ingeniería de sistemas.

| D | Competencia | Cómo vive en el harness |
|---|---|---|
| **Delegation** | ¿Qué le delego al agente? ¿Qué queda en juicio humano? | Volumen + repetición → agente. Estrategia, ética y criterio → humano. El COMMAND CENTER define los límites de cada rol. |
| **Description** | Describir el objetivo con precisión que genera output útil, no plausible. | Specs EARS antes de codear. Output anchors en el system prompt. Anti-narración: el agente produce, no explica. |
| **Discernment** | Evaluar críticamente el output: errores, sesgo, off-brief. | Gate del Reviewer (`cc-sdd`): único que cierra tareas. Pre-fetch verificado: la IA sintetiza datos reales, nunca inventa. Si no hay dato, dice `«sin dato»`. |
| **Diligence** | Responsabilizarte de lo que hacés con la IA y cómo. | R0-R12: 13 reglas vinculantes. Auditoría Jhonson cada 15 min. Dead-letter queue. Vaultwarden para secretos. |

> **Por qué importa:** un sistema donde el operador mantiene control real (Delegation + Diligence) mientras la IA maximiza throughput (Description + Discernment). No es ChatGPT; es ingeniería de agentes.

---

## 🔐 Seguridad: Reglas R0–R12 (13 reglas vinculantes)

> **Namespace:** estas **R0-R12** son los **controles de seguridad de producto**. La higiene de **credenciales/secretos** (Vaultwarden, rotación de tokens, scope validation) es un marco separado: **K0-K12** (vault `seguridad-r0-r12`). No confundir.

Aplicables a todo proyecto del ecosistema. Stack: [`claude-code-safety-hooks`](https://github.com/federicogrecobarragan-prog/claude-code-safety-hooks) · [`nuclei`](https://github.com/federicogrecobarragan-prog/nuclei) · [`npq`](https://github.com/federicogrecobarragan-prog/npq) · [`infra-deploy`](https://github.com/federicogrecobarragan-prog/infra-deploy) · [`vw_web_builds`](https://github.com/federicogrecobarragan-prog/vw_web_builds).

| # | Regla |
|---|---|
| R0 | Secretos nunca en código, logs ni pantallas. Solo en Vaultwarden cifrada. |
| R1 | `SUPABASE_SERVICE_KEY` solo en scripts locales del VPS — nunca en Docker expose ni en logs. |
| R2 | RLS activo en **todas** las tablas de Supabase. Cada dato solo lo ve quien debe verlo. |
| R3 | Anti-inyección: ningún input externo va a SQL/shell sin sanitizar. |
| R4 | Webhooks firmados con HMAC. Sin firma válida = rechazado automático. |
| R5 | Rate-limiting en todos los endpoints públicos. |
| R6 | Operaciones destructivas requieren confirmación humana explícita. Gate obligatorio. |
| R7 | Supply-chain: `npq` audita paquetes npm antes del install. No hay paquete nuevo sin auditoría. |
| R8 | Escaneo de vulnerabilidades con `nuclei` antes de cada deploy. |
| R9 | Backup cifrado GPG AES256 (`openclaw-backup-madre`). Passphrase solo en la bóveda. |
| R10 | Notas del vault: secretos marcados `[REDACTADO — ver Vaultwarden]`. Nunca texto plano. |
| R11 | Apps mobile: `FLAG_SECURE` + blur en app-switcher + clipboard auto-clear (ver `la-boveda`). |
| R12 | Deploys hardened: Traefik + Vaultwarden, secretos vía `.env` no versionado (`infra-deploy`). |

---

## 🏗️ El Arnés: 9 pilares de ingeniería de agentes

El harness hace al modelo **intercambiable** y al sistema **robusto**. Cambia el LLM debajo; el sistema sigue funcionando.

| Pilar | Descripción | Repo / Patrón |
|---|---|---|
| **Pre-fetch pattern** | Un script junta datos reales ANTES de llamar al modelo. La IA sintetiza; nunca inventa. | Cualquier agente de producción |
| **Output anchors** | El tipo de salida está declarado en el system prompt. Sin sorpresas de formato. | `cc-sdd`, system prompts |
| **Anti-narración** | El agente produce output directo. No explica lo que hace. ~65% menos tokens. | `caveman` |
| **Anti-alucinación** | Si no hay dato, dice `«sin dato»`. Confianza falsa = bug de producción. | Gate del Reviewer |
| **Auditoría Jhonson** | Un agente vigila a todos los demás cada 15 minutos. SLA en producción. | `la-colmena` |
| **Dead-letter queue** | Mensajes sin procesar no se pierden. Cola de reintentos con log. | `la-colmena` |
| **SessionStart hook** | Al iniciar: lee contexto, carga memoria, ejecuta pre-flight checks. | `claude-code-safety-hooks` |
| **Estado en disco** | El sistema sobrevive reinicios. Estado externalizado a Supabase, nunca solo en RAM. | `la-colmena`, `engram` |
| **Memoria semántica** | Engram + vault: el agente recuerda entre sesiones. No empieza de cero. | `engram`, `vault-colmena` |

---

## 📋 SDD/LTR: Spec-Driven Development + Code Review

Antes de código, existe el spec. Roles separados garantizan calidad sin revisión arbitraria.

```
Leader      → diseña el spec (EARS) y define criterios de aceptación
Implementer → ejecuta contra el spec, sin tomar decisiones de diseño
Reviewer    → ÚNICO que puede cerrar la tarea (gate de calidad)
```

**Doble loop (pskoett):**
- **Inner loop:** verify-gate + self-healing + context-surfing — recupera fallas durante la sesión.
- **Outer loop:** learning-aggregator + harness-updater + eval-creator — cierra brechas entre sesiones.

**Handoff multi-modelo:** modelo económico (DeepSeek V3.2) produce volumen; modelo premium (Sonnet 4.6) revisa criterio. El Reviewer es siempre el tier superior.

Repos: [`cc-sdd`](https://github.com/federicogrecobarragan-prog/cc-sdd) · [`agent-teams-lite`](https://github.com/federicogrecobarragan-prog/agent-teams-lite) · [`gentleman-guardian-angel`](https://github.com/federicogrecobarragan-prog/gentleman-guardian-angel) · [`pskoett-ai-skills`](https://github.com/federicogrecobarragan-prog/pskoett-ai-skills).

---

## 🧭 Estándar de Desarrollo de 7 Etapas

> **Estándar universal para TODO desarrollo nuevo del ecosistema.** Toda skill de deployment/build/ejecución debe embeber este checklist. Ninguna etapa avanza sin pasar su gate.

| # | Etapa | Qué exige | Vive en |
|---|-------|-----------|---------|
| 1 | **DEFINE** | Definición del problema + plan acordado con el orquestador ANTES de tocar código. | `arrancar-proyecto` (skill) |
| 2 | **SPECIFY (SDD)** | Spec formal de caso de uso: composición del equipo, nº de agentes, tipos de especialización, contratos I/O e inter-agente. | `cc-sdd`, `metodologia-sdd-ltr` |
| 3 | **PLAN AT SCALE** | Arquitectura escalable desde el día 1. Sin atajos que bloqueen el crecimiento. Cada componente reemplazable de forma independiente. | Diseño dockerizado aislado (suite-precios/life-hub) |
| 4 | **BUILD IN STAGES** | Desarrollo incremental con QA automatizada + code review en cada stage gate. Nada avanza sin pasar el test de etapa. | `tasks.json` (pending→review-pending→done) + Reviewer gate |
| 5 | **TEST & VERIFY** | Suite automatizada: uso funcional, edge cases, estabilidad bajo carga, stress y benchmarks de escalabilidad. Resultados documentados. | REGLAS-DE-ORO Regla 13 (4 capas) + `gstack /qa` + `verify` |
| 6 | **DEPLOY SAFE** | Checklist de validación completo + verificación de capa de seguridad antes de producción. Cero excepciones. | R0-R12 + `nuclei` pre-deploy + `deploy-playstore` |
| 7 | **OPERATE & IMPROVE** | Monitoreo post-launch + ciclos de evaluación programados. Backlog alimentado por uso real. | Self-improving loop + Auditoría Jhonson (15 min) + `patterns.md` |

**Embebido en:** `arrancar-proyecto`, `montar-web`, `deploy-playstore`, `team-setup`. Doc canónico: `estandar-7-etapas` (vault `10-ecosistema`).

---

## 🌙 Dreams System — goal-tracking de largo plazo *(Phase 1 buildeada)*

> Capa de seguimiento de **metas de largo plazo / north-stars** de los agentes, persistente a través de sesiones. **NO confundir con `GR00T-Dreams`** (ese es DreamGen de Nvidia, generación de datos de robótica vía world models — referencia ML, no goal-tracking).

**Problema que resuelve:** hoy `/dame` persigue **una** meta verificable por run (efímero), y `dream-review` del Command Center es solo un cron-reporte. No existía una capa que persiga aspiraciones/objetivos de horizonte largo a través del tiempo.

**Arquitectura (reusa lo que ya existe):**
- **`dreams` (tabla Supabase)** — north-star, KPIs, deadline, agente-owner, status, progreso % · pilar *Estado en disco*.
- **`engram`** — persistencia semántica del contexto del dream entre sesiones.
- **`/dame`** — motor de loop ya existente: cada dream se descompone en sub-metas verificables que corren como runs DAME.
- **`dream-review` (cron semanal)** — consolida progreso, re-prioriza, alerta desvíos.
- **skill `dream`** — análoga a `dame` pero con horizonte multi-sesión/multi-run y revisión periódica.
- **Dashboard** — vista de progreso en `command-center` / Latido.

Repo: 🔒 [`dreams-system`](https://github.com/federicogrecobarragan-prog/dreams-system) (privado) · doc de diseño `dreams-system-design` (vault `00-inbox`). **Estado: Phase 1 buildeada** (SDD 28 req EARS + `0001_dreams.sql` + cron `dream-review` + skill `/dream`); **Phase 2 staged** (aplicar SQL a Supabase + cron VPS + vista command-center + seed). `/dame` = músculo (un loop por milestone), `dream` = cerebro (muchos loops en el tiempo, gate humano para cerrar).

---

## Proyectos propios

> 🔒 = repo **privado**: el nombre es visible, pero el contenido es de acceso restringido (solo el owner).

| Repo | Descripción |
|---|---|
| 🔒 [metrik](https://github.com/federicogrecobarragan-prog/metrik) | Metrik — panel de marketing contenedorizado (Docker: postgres+postgrest+Node cero-deps). Mide campañas/funnel/ads/email/redes multi-tenant. Producto VibeMarketing OdJ. |
| 🔒 [scraper-precios-competencia](https://github.com/federicogrecobarragan-prog/scraper-precios-competencia) | **Scraper de precios de competencia** (motor BLACK CODE, Python + Playwright headless) para Vinoteca/Segunda Copa: scrapea precios y alimenta el pipeline de publicación IG/FB vía n8n. Pieza de scraping del legacy IMPERIO DIGITAL. |
| 🔒 [suite-precios](https://github.com/federicogrecobarragan-prog/suite-precios) | **Suite de Inteligencia de Precios** — CompetitorBot (B2B) + PriceGhost (B2C) sobre **un motor**, backend de monitoreo de precios/competencia. Motor de scraping multi-método + **votación de precio** (JSON-LD / site-specific / CSS / IA-fallback, con confidence y desambiguación de tachados→`posible_descuento`), **API async** (POST 202 + Supabase Realtime), Supabase **16+ tablas con RLS multitenant** (CMP-05 aislamiento cross-tenant **validado en vivo**), Edge Function `llm-proxy` (OpenRouter/Haiku, **probada en vivo**), scheduler por-producto. SDD 262 req EARS · 169 tests · smoke 10/10 contra DB real. Diseño 3 superficies por Claude Design (web B2B + companion mobile + B2C mobile) en `handoff/`. Stack Node/TS + Puppeteer-stealth/Scrapling. Deploy VPS dockerizado aislado (handoff BAKUGO pendiente). Familia OdJ. |
| 🔒 [colmena-kit](https://github.com/federicogrecobarragan-prog/colmena-kit) | Colmena Kit — equipo de agentes IA gestionado para PyMEs (productización de La Colmena) |
| 🔒 [cda-os](https://github.com/federicogrecobarragan-prog/cda-os) | **CDA-OS** — sistema operativo multiagente enterprise (CORE) que orquesta todo el entorno: ejecutivos C-Level, agentes especializados, workflows y bitácora de proyectos/skills. |
| 🔒 [la-colmena](https://github.com/federicogrecobarragan-prog/la-colmena) | **La Colmena** — ecosistema multiagente en producción sobre OpenClaw (12 agentes, Supabase fuente de verdad, scheduler cron, 9 pilares del harness). Incluye **COMMAND CENTER** (cockpit.oficinadejhonson.com — panel único del ecosistema, `cockpit/` + collector) y motor VibeMarketing (leadgen Places 2 segmentos/día + Instantly). Export scrubbeado scripts+docs+harness. |
| 🔒 [openclaw-to-hermes-migration](https://github.com/federicogrecobarragan-prog/openclaw-to-hermes-migration) | **Migración OpenClaw → Hermes** (feature #15) — del ecosistema La Colmena (11 agentes + crons) al arnés Hermes. SDD completo (EARS R1-R18 + design §1-10) + helper `hermes_migrate_agent.py` (setup/port-cron/tick-lines) + `cutover_discord.sh`. Auto-fire híbrido (gateway always-on + system-cron tick por profile) + tick selectivo para split-migration. KIRA graduada + 7 crons internos en Hermes; dev-pipeline + cutover client-facing pendientes. Sin big-bang, todo reversible. |
| 🔒 [hermes-platform](https://github.com/federicogrecobarragan-prog/hermes-platform) | **Hermes Platform** — gestión de la plataforma Hermes Agent (Nous Research) en todas nuestras implementaciones (La Colmena + OdJ/VibeMarketing + productos = 1 install, N profiles). Monitor recurrente (`hermes_update_check.py`, cron lunes): valida vs el upstream oficial — versión core (commits behind), skills hub (updates), inventario de skills/profiles. Doctrina de update (gateado, backup, rollback) + skills-management + deployments. Status auto-pusheado + alertas Telegram. |
| 🔒 [genesis](https://github.com/federicogrecobarragan-prog/genesis) | **GÉNESIS** — producto enlatado: agente IA premium auto-capacitado sobre Hermes. Install rápido (PC/VPS/servidor) + knowledge-pack curado + onboarding agéntico (nombrar agente → entrevista objetivos → auto-capacitación → operar real-time) + mission-packs. 1er caso de éxito: CDA → desplegar SONAR (recluta-os). Reusa hermes-platform/installer + patrones colmena-kit + skill desplegar-producto-vps. Frontend por Claude Design (One-Shot). Familia OdJ. |
| 🔒 [dreams-system](https://github.com/federicogrecobarragan-prog/dreams-system) | **Dreams System** — goal-tracking de largo plazo (north-stars de semanas/meses) sobre `/dame` + `engram` + Supabase. Un dream se descompone en milestones verificables; cada milestone = un run `/dame` real; `progress_pct` lo recalcula el cron `dream-review`; `achieved` solo por gate humano. Phase 1 buildeada (SDD 28 req EARS, `0001_dreams.sql`, cron, skill `/dream`); Phase 2 staged (SQL+cron VPS+command-center+seed). NO confundir con GR00T-Dreams (Nvidia ML). Ver sección "🌙 Dreams System". |
| 🔒 [command-center](https://github.com/federicogrecobarragan-prog/command-center) | **COMMAND CENTER v2 / Motor Único** — cockpit unificado del ecosistema (Node.js cero-deps + frontend vanilla sin build + Supabase como bus, snapshot de **21 claves**). Monitoreo (agentes/crons/servicios/consumo IA/vencimientos) + **vista Marketing**: funnel real (HUNTER `hunter_prospects`/`opportunities`/`activities`) + ingest de ads/email/social/campañas/contenido vía tablas `marketing_*` (productores n8n / cron Claude+MCP). Patrón: productores escriben a Supabase, el builder solo lee. Productizable como **Latido** (observabilidad agéntica self-host, MIT). |
| 🔒 [colmena-vault](https://github.com/federicogrecobarragan-prog/colmena-vault) | **COLMENA VAULT** — knowledge graph 360 del ecosistema (24 scopes: VPS + repos externos) generado por Graphify: AST tree-sitter local ($0) + semántica de docs DeepSeek + bridger cross-scope (40 hubs de concepto que conectan tablas/agentes/productos/libs). ~13,4k nodos · ~15,9k links. Vault Obsidian (nota por nodo + wikilinks + nav por proyecto), wiki, GRAPH_REPORT y visor web (cockpit). Auto-sync determinístico con secret-scan pre-push. Fuente de verdad del MAPA (Supabase = datos). |
| 🔒 [vault-colmena](https://github.com/federicogrecobarragan-prog/vault-colmena) | **Vault compartido PC↔VPS** — LLM Wiki curada del ecosistema (patrón Karpathy): conocimiento, proyectos, infra, agentes, negocio + resúmenes de grafos de código de 11 repos. Sync git cada 15 min con la PC de Federico. Distinto de `colmena-vault` (ese es el grafo de código auto-generado; éste es la wiki curada compartida). |
| 🔒 [aria-agent](https://github.com/federicogrecobarragan-prog/aria-agent) | **Aria** — copiloto IA de voz para reuniones comerciales (KAM en CDA), self-hosted (cerebro + RAG propios: Pipecat + Deepgram + ElevenLabs + Supabase pgvector + embeddings locales e5). **App unificada con selector de modos validada en vivo:** 🎙️ conversación (asesora interna por voz) + 🎧 coaching (escucha al cliente en la reunión y sopla qué responder, "Solo voz" o "Voz+Texto") + robustez WebRTC (mixer keepalive anti-silencio, auto-reconexión). Incluye `HANDOFF-VPS.md` para montarla productiva en la VPS. Próximo: modo "Aria presente" con avatar (HeyGen LiveAvatar Lite, decisión tomada). Parte del ecosistema La Colmena. |
| 🔒 [oficina-de-jhonson-agencia](https://github.com/federicogrecobarragan-prog/oficina-de-jhonson-agencia) | **Agencia Autónoma OFICINA DE JHONSON + ESTUDIO DE JHONSON** — repo paraguas de **VibeMarketing**: motor de captación 100% autónomo. Engine diario (rotación por rubro): Google Places → leads → qualify → email-enrich → WhatsApp (Meta Cloud API) + Email (Instantly). Tracking de entregas/respuestas. Dashboard de leads ([vibe.oficinadejhonson.net](https://vibe.oficinadejhonson.net)). Operado autónomo por **Hermes Agent**. Specs SDD + scripts del motor. |
| 🔒 [colmena-digital](https://github.com/federicogrecobarragan-prog/colmena-digital) | **La Colmena Digital / OFICINA DE JHONSON** — consultora de automatización IA: web pública, ChatJhonson (widget agéntico), funnels WhatsApp, pipeline outbound. Export scrubbeado (sin material de clientes). |
| 🔒 [cda-casos-exito](https://github.com/federicogrecobarragan-prog/cda-casos-exito) | **Armador de Casos de Éxito** — visor web Azure + harness anti-alucinación para portfolio comercial KAM. Sistema activo con 136 antecedentes + 27 casos curados (datos locales, privados). |
| 🔒 [agencia-autonoma](https://github.com/federicogrecobarragan-prog/agencia-autonoma) | **Agencia Autónoma** — sistema personal para diseñar, crear y vender productos digitales (Printables, Ebooks, Templates, SVG, Presets, Prompt Packs) en Etsy, Gumroad y web directa. Outreach + SEO + tracker de ingresos. Objetivo ≥ 1.000 USD/mes. |
| 🔒 [crm-colmena](https://github.com/federicogrecobarragan-prog/crm-colmena) | **CRM La Colmena** — CRM interno KAM (cuentas, contactos, CNs, tareas, actividades) sobre Supabase + Edge Functions. Pieza CRM del ecosistema La Colmena. Estructura sanitizada (sin datos sensibles). |
| 🔒 [recluta-os](https://github.com/federicogrecobarragan-prog/recluta-os) | **Recluta-OS** — ATS de sourcing: creás vacantes, definís criterios y disparás un scrape on-demand; el motor LinkedIn del VPS (reusa `linkedin-orgchart`) devuelve perfiles a Supabase y movés candidatos por el pipeline. **Dos modos:** búsqueda por parámetros + **refresh por URL (ingeniería inversa)** — visita el perfil y sobrescribe selectivo la info vieja (empresa/cargo/ubicación/skills) sin pisar datos del reclutador (salario/motivo/interés). Incorpora **modelo de evaluación**: doble score técnico/hunting, 6 factores ponderados, **Firewall Comercial** (cero-contacto a clientes activos), triaje A/B/C y "radiografía" por candidato. Demo validándose primero sobre Excel antes de migrar a Supabase (handoff a BAKUGO/VPS). Next.js (Vercel) + Supabase (Auth/Realtime) + Edge Function firmada. El repo no contiene lógica de scraping, solo el contrato. |
| 🔒 [colmena-dashboard](https://github.com/federicogrecobarragan-prog/colmena-dashboard) | **Dashboard La Colmena** — UI web de una sola página (sin build) para el estado vivo del ecosistema: heartbeats vs cadencia, crons, pipeline HUNTER + quick-entry a Supabase. Export scrubbeado. |
| 🔒 [openclaw-backup-madre](https://github.com/federicogrecobarragan-prog/openclaw-backup-madre) | **BACKUP MADRE** — backup cifrado (GPG AES256) de todo el ecosistema OpenClaw/La Colmena (config, scripts, harness, credentials, secrets, memorias, SOULs de 12 agentes). Disaster recovery; passphrase en LA BÓVEDA. Excluye reproducibles. |
| 🔒 [imperio](https://github.com/federicogrecobarragan-prog/imperio) | **IMPERIO DIGITAL** (legacy) — sub-ecosistema operado por NEXUS para el cliente Vinoteca/Segunda Copa: scrape de precios → copy DeepSeek → preview → publicación IG/FB vía n8n. Export scrubbeado. |
| 🔒 [mobile-playbook](https://github.com/federicogrecobarragan-prog/mobile-playbook) | **Mobile Playbook** — fuente de verdad para construir y publicar apps mobile (React Native + Expo → Play Store → iOS) con agente LLM adentro. Consolida buenas prácticas de POPA + Folio.OS: playbook 11 secciones, checklists (data safety tilde por tilde), templates (eas.json, Edge Function, gitignore-fix) y legales. Punto de partida de toda app nueva. |
| 🔒 [alimentando-a-popa](https://github.com/federicogrecobarragan-prog/alimentando-a-popa) | **Alimentando a POPA** — app móvil de dieta personalizada (React Native + Expo, Supabase, local-first + sync nube por usuario). Motor nutricional con evidencia (Mifflin-St Jeor, macros, ajuste adaptativo por peso real), recetas validadas + swap, **"Mis comidas"** (armá tu comida y calcula kcal), registro de deslices fuera del plan, IMC/composición, horarios de comida, **Modo Aceleración** y **POPA IA** (coach nutricional vía Edge Function → OpenRouter). Entitlements Free/Basic/Premium + seam RevenueCat. **En closed testing Play Store** (v1.3.0). |
| 🔒 [folio-os](https://github.com/federicogrecobarragan-prog/folio-os) | **Folio.OS** — app móvil de finanzas personales para Argentina (React Native + Expo, local-first). Dashboard caja+proyección, carga de gastos ARS/USD (categorías a medida + date picker), objetivos de ahorro con aportes, USD Radar (dolarapi con histórico real), Contador IA (Edge Function → OpenRouter), racha de carga, backup/export JSON+CSV. **Carga inteligente de gastos: escaneo de ticket con cámara (visión IA) + compartir un mail/mensaje a la app (share intent → LLM extrae el gasto).** **Publicada en closed testing Play Store** (v1.3.0 disponible para verificadores, Edge Function deployada y validada). |
| 🔒 [mishizen](https://github.com/federicogrecobarragan-prog/mishizen) | **MishiZen** — app móvil de bienestar (React Native + Expo SDK 56, local-first). Meditaciones con paisajes sonoros reales, respiración guiada (orbe animado + inhalar/exhalar reales), hábitos con rachas, **diario de reflexión** (free 3/día · premium ilimitado), progreso/logros, despertar suave (notificaciones locales) y **Mishi IA** (gato calico compañero; cerebro local + seam Edge Function → OpenRouter free). Mascota anime, copy es-AR, modo oscuro. AAB con AD_ID/RECORD_AUDIO bloqueados. **LIVE en closed testing Play Store** (v1.0.0 publicada — link opt-in activo, invitación a verificadores enviada; com.mishizen.app). |
| 🔒 [la-boveda](https://github.com/federicogrecobarragan-prog/la-boveda) | **La Bóveda** — app móvil **gestor de contraseñas 100% local** (React Native + Expo SDK 56, offline-first, **sin backend de datos**). Estética cyberpunk/anime (mascota candado "Bovi" + llave guardián "Llavín"). Categorías/campos a medida, **generador de contraseñas CSPRNG** + medidor de fuerza, **Gestor IA "Llavín" on-device** (rule-based, cero red) y **desbloqueo biométrico**. **Seguridad endurecida (auditoría adversarial 4 bloqueantes resueltos):** Android Keystore DEK con `requireAuthentication` + **AES-256-CBC + HMAC** (IV CSPRNG, encrypt-then-MAC), FLAG_SECURE + blur en app-switcher, auto-lock con purga de memoria, clipboard auto-clear. **Data Safety = no recopila / no comparte** (todo cifrado solo en el teléfono). Monetización USD 5 INAPP (seam Premium en beta + guard anti-release). **Enviada a closed testing Play Store** (v1.0.0 / versionCode 2, `com.bovedalabs.laboveda`, lista Testers POPA = 10, 177 países; opt-in pendiente de aprobación de Google). Patrón nuevo reutilizable: vault local cifrado + biometría como **barrera criptográfica** (no cosmética). |
| 🔒 [pinta-pinta](https://github.com/federicogrecobarragan-prog/pinta-pinta) | **Pinta Pinta** — app móvil infantil para **colorear libros** (React Native + Expo SDK 56, local-first). **Lienzo Skia**: balde flood-fill por luminancia (line-art con blendMode multiply), pincel/goma vectoriales, estado = comandos serializables (undo/redo por reproducción), guardar a "Mis dibujos". 8 libros gratis (rasterizados de PDF con **mupdf wasm**), onboarding sin lectura. **Generador IA** (receta por chips → Edge Function Supabase → **Pollinations gratis** / SD Forge / Replicate, **post-proceso de cierre de líneas** porque ningún modelo cierra solo, cuota mensual atómica). Monetización mock (parental gate matemático + Zona de Grandes + Tienda + Paywall, seam RevenueCat). **Mascota 3D "Pincelín"** (GLB rigueado headless en Blender, clips Saludo/Baile/Giro). Spec SDD en `harness/`. **v1.0.0 GRATIS APROBADA y LIVE en prueba cerrada (14 testers + 177 países, lanzada 22-jun-2026); 13 testers invitados por mail. Declaraciones Play completas: IARC=Todos, Data Safety sin datos, Diseñado para familias, categoría Educación, ID publicidad No, política de privacidad.** `com.oficinadejhonson.pintapinta`. Patrón nuevo: pipeline PDF→PNG + flood-fill Skia + generación de imagen gratis con cierre server-side. |
| 🔒 [maki-backend](https://github.com/federicogrecobarragan-prog/maki-backend) | **MAKI** — Sistema Omnicanal de despacho para gastronomía (NestJS + Prisma + WebSocket): **integración WhatsApp Cloud API (Meta) en vivo** — webhook inbound → consola, recepción de imágenes (comprobantes), control de alérgenos, priorización VIP, round-robin de operadores. Consolas web: inbox omnicanal, KDS cocina, tracking de pedidos, clientes, métricas y auditoría. Carga manual de pedidos. Cliente: Masaca Sushi (Pilar). |
| 🔒 [life-hub](https://github.com/federicogrecobarragan-prog/life-hub) | **Life Hub** — Middleware de inteligencia comercial inmobiliaria para **Life Desarrollos** (Gran Rosario), clon/rebrand de `maki-backend`. Consola comercial: cola de leads, **chat IA que califica y auto-completa la ficha** (nombre/barrio/uso/presupuesto/financiación CAC/canje), **alerta de stock anti doble-venta** con sugerencia de alternativa, **filtro de no calificados**, **round-robin por zona** y derivación a comercializadoras vía **broker link tokenizado sin login** con estados en tiempo real (Contactado/Visita/Perdido+motivo) y **alertas de inacción >2h**. **Tablero de gerencia (BI):** embudo, leads recuperados 24/7, rendición de cuentas de brokers, KPIs (lead-to-contact, broker engagement, caducidad, CPL, horas-hombre, **torta de objeciones**). **Pre-alta Odoo** (JSON account.receivable). **IA real** OpenRouter (deepseek-v3.2/claude-haiku) vía proxy local + Edge Function Supabase. Demo browser self-contained (React CDN sin build, rebrand verde foresta/arena/terracota) + **modo LIVE verificado end-to-end** (7 Edge Functions Deno + Supabase DB/Realtime + IA real OpenRouter; escrituras solo service-role). **Hardenizado** (escape de filtros PostgREST, rate-limit, tokens cripto, RLS anon read-only). **Scaffold Docker aislado** (subdominio propio) listo para montar en VPS. Próximo: deploy VPS (BAKUGO) + WhatsApp Cloud API + **Hermes Agent** (voz + consultor interno). |
| 🔒 [oficinadejhonson-web](https://github.com/federicogrecobarragan-prog/oficinadejhonson-web) | Sitio público **OFICINA DE JHONSON** — [www.oficinadejhonson.com](https://www.oficinadejhonson.com). HTML estático (Black Code design system) + widget de chat. Catálogo de 15 productos en 3 tiers desde `products.json` (single source of truth que también re-entrena ChatJhonson) + **6 herramientas gratis como lead magnets** (AgendaBot, ReseñaBot, FacturaBot, AnuncioBot, PresupuestoBot, LocalBot) + blog SEO + `llms.txt` (GEO/AEO). Frontend deploy en Vercel; backends en VPS (chat + webhooks n8n). |
| 🔒 [Syncro-WEB](https://github.com/federicogrecobarragan-prog/Syncro-WEB) | **Syncro+** — sitio de plataforma de IA empresarial. HTML estático (HandOff de diseño). Deploy en Vercel ([syncro-plus.vercel.app](https://syncro-plus.vercel.app)). |
| 🔒 [lightingyoga-web](https://github.com/federicogrecobarragan-prog/lightingyoga-web) | **LightingYoga** — diseño web para un estudio de yoga (programa Raíz / MSC Mindfulness). Material fuente del prototipo: HTML de referencia para cloning, briefs, meditaciones guiadas, videos e imágenes. Web final en construcción. |
| 🔒 [decretando-disney-web](https://github.com/federicogrecobarragan-prog/decretando-disney-web) | **Decretando Disney** — web de **agentes de viaje** (Martín & Mica): Disney, Universal, cruceros y Caribe. SPA estática (React 18 por CDN + JSX/Babel en navegador, **sin build**): aurora canvas, **Mickey 3D** (model-viewer + GLB), 8 categorías, video-cards, **cursor guante de Mickey**, navegación con **History API** (el back de Android navega in-app, no cierra), **cache-busting + Error Boundary** (anti pantalla-blanca). **Fase 2 backend Supabase** (Edge Functions Deno, RLS, secretos en env): captura de **leads** (contacto/reserva/newsletter/blog) → aviso por email a los agentes vía **Brevo** + **panel comercial privado** (`#panel` + clave, fail-closed): funnel de ventas, prospectos calientes con follow-up 1-toque (WhatsApp/llamar/Gmail), KPIs, tendencia 14d, top destinos. **Blog-comunidad** (Supabase Auth: registro/login/comentarios/emojis), **newsletter** (Brevo) y **noticias automáticas** (cron Lun/Mié/Vie → OpenRouter + Google News RSS) + **editor de autoservicio en el panel** (el cliente carga/pausa/borra **promociones**, **temas de blog** y **noticias/novedades a mano**, **modera reseñas de pasajeros** y **sube imágenes** sin tocar código ni SQL — Edge Function `panel-write` fail-closed + imagen canvas→base64 en la fila, sin bucket de Storage). **Reseñas con moderación** (tabla `resenas`, RLS: anon lee aprobadas, inserta pendientes). **Newsletter automático** (Brevo): al crear una promo avisa a los suscriptores y la bienvenida incluye las 3 promos vigentes; noticias con pool de imágenes variado. Emails de la web abren **Gmail compose**. **En vivo:** [decretandodisney.com](https://decretandodisney.com) (Hostinger Premium, SSL), validado **360** (desktop/iPhone/Android, 0 errores/404/overflow). **Pipeline de assets local (reutilizable):** Mixamo → **Blender headless** (`fbx2glb.py`: FBX→GLB texturizado) + videos **ffmpeg 2-pass** comprimidos. |
| [decretando-disney-preview](https://github.com/federicogrecobarragan-prog/decretando-disney-preview) | **Decretando Disney — preview** (público): repo de preview/staging de la SPA Decretando Disney (gemelo del repo de producción privado `decretando-disney-web`). React 18 por CDN sin build. |
| 🔒 [Creaciones-de-im-genes-y-Post-para-redes](https://github.com/federicogrecobarragan-prog/Creaciones-de-im-genes-y-Post-para-redes) | Repositorio de assets del ecosistema: imágenes y posts para redes sociales (creativos y publicaciones). |
| [CEFALU-Sistema-de-Gestion-ERP](https://github.com/federicogrecobarragan-prog/CEFALU-Sistema-de-Gestion-ERP) | Sistema de gestión (ERP) construido desde cero con Claude Code. |
| [CV_FedericoGrecoBarragan.github.io](https://github.com/federicogrecobarragan-prog/CV_FedericoGrecoBarragan.github.io) | Sitio de CV / portfolio personal. |
| [Banco-Nacional-de-Cordoba-Presentacion](https://github.com/federicogrecobarragan-prog/Banco-Nacional-de-Cordoba-Presentacion) | Presentación web institucional. |

---

## Stack por categoría

### Harness · Agentes · Claude Code — [`topic:harness`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aharness&type=repositories)

| Repo | Descripción |
|---|---|
| [gstack](https://github.com/federicogrecobarragan-prog/gstack) | El setup de Claude Code de Garry Tan: 23 herramientas (CEO, diseñador, eng manager, QA, release). |
| [cc-sdd](https://github.com/federicogrecobarragan-prog/cc-sdd) | Harness mínimo de Spec-Driven Development para Claude Code, Codex, Cursor y más. |
| [get-shit-done](https://github.com/federicogrecobarragan-prog/get-shit-done) | Sistema de meta-prompting y context engineering para Claude Code. |
| [agent-teams-lite](https://github.com/federicogrecobarragan-prog/agent-teams-lite) | Orquestador + 9 sub-agentes para desarrollo dirigido por specs. Sin dependencias. |
| [hermes-agent](https://github.com/federicogrecobarragan-prog/hermes-agent) | Agente de NousResearch "que crece con vos": framework de agente con memoria/aprendizaje continuo. Referencia para agentes long-running. |
| [open-agents](https://github.com/federicogrecobarragan-prog/open-agents) | Template open source para construir agentes en la nube. |
| [learn-harness-engineering](https://github.com/federicogrecobarragan-prog/learn-harness-engineering) | Tutorial de harness engineering de 0 a 1. |
| [harness-engineering-guide](https://github.com/federicogrecobarragan-prog/harness-engineering-guide) | Guía abierta de harness engineering: conceptos, tutoriales, papers, herramientas. |
| [awesome-claude-code](https://github.com/federicogrecobarragan-prog/awesome-claude-code) | Lista curada de skills, hooks, slash-commands y plugins para Claude Code. |
| [awesome-agent-skills](https://github.com/federicogrecobarragan-prog/awesome-agent-skills) | Fork de VoltAgent: 1424+ agent skills curadas de equipos oficiales (Anthropic, Google, Vercel, Stripe, Cloudflare, Supabase, Figma, OpenAI…) + comunidad. Claude Code/Codex/Gemini CLI/Cursor. |
| [Gentleman-Skills](https://github.com/federicogrecobarragan-prog/Gentleman-Skills) | Skills comunitarias para Claude Code, OpenCode y otros asistentes. |
| [pskoett-ai-skills](https://github.com/federicogrecobarragan-prog/pskoett-ai-skills) | Skills para agentes con filosofía de **doble loop**: el *inner loop* (verify-gate, self-healing, context-surfing) recupera fallas durante la sesión; el *outer loop* (learning-aggregator, harness-updater, eval-creator, pre-flight-check) cierra brechas entre sesiones. Plugin Claude Code / Codex / Copilot. |
| [caveman](https://github.com/federicogrecobarragan-prog/caveman) | Skill que recorta ~65% de tokens "hablando como cavernícola". |
| [graphify](https://github.com/federicogrecobarragan-prog/graphify) | Skill de coding-assistant (Claude Code/Codex/OpenCode) que construye el **knowledge graph** de un codebase: AST tree-sitter local + semántica de docs. Motor detrás de `colmena-vault` (mapa 360 del ecosistema). |
| [superpowers](https://github.com/federicogrecobarragan-prog/superpowers) | Framework de agentic skills + metodología de desarrollo de software para agentes. Referencia de harness. |
| [miniverse](https://github.com/federicogrecobarragan-prog/miniverse) | Mundo pixel-art en miniatura para agentes (sandbox/visualización). Referencia. |
| 🔒 [montar-web](https://github.com/federicogrecobarragan-prog/montar-web) | **Skill build+deploy de webs end-to-end**, destilado de las webs reales del ecosistema (Disney, Oficina de Jhonson, Syncro+, ChemX/Card-Detailing, Lighthouse Yala). 2 stacks (SPA React+CDN sin build / HTML vanilla), mobile-first dvh+safe-area, assets (ffmpeg/3D Mixamo-GLB/cursor/Web-Audio), backend Supabase (leads+RLS/Brevo/blog/noticias-cron-IA/**panel funnel de ventas**/**editor de autoservicio CMS-lite** — el cliente carga promos+temas y sube imágenes sin Storage), features de captación (**chat agéntico**, lead-magnets IA, products.json-única-fuente-que-alimenta-la-IA, GEO/AEO llms.txt), **e-commerce con IA vendedora** (MercadoPago+stock por trigger), design systems, micro-interacciones. Deploy a Hostinger/Vercel/Netlify/nginx/Apache-cPanel. Verificación 360 headless (puppeteer+esbuild) + ~20 gotchas resueltos. `/montar-web`. |
| [claude-code-safety-hooks](https://github.com/federicogrecobarragan-prog/claude-code-safety-hooks) | Hooks PreToolUse config-driven: backup de archivos críticos, bloqueo de JSON malformado, aviso en archivos de alto impacto. Sin dependencias. |
| 🔒 [openclaw-safe-update](https://github.com/federicogrecobarragan-prog/openclaw-safe-update) | Updater seguro del binario OpenClaw: backup + age gate supply-chain + reinstala plugins críticos + verifica canales. Privado. |
| [gentleman-guardian-angel](https://github.com/federicogrecobarragan-prog/gentleman-guardian-angel) | Code review con IA, agnóstico de proveedor (Claude, Gemini, Codex, Ollama). |
| 🔒 [skills-main](https://github.com/federicogrecobarragan-prog/skills-main) | Gestor del ecosistema de skills y agentes (privado). |
| 🔒 [skills-propias](https://github.com/federicogrecobarragan-prog/skills-propias) | Skills propias de Federico para Claude Code (autoría local). Primera: `registrar-avance` (bitácora Obsidian + grafo Graphiti). Privado. |
| 🔒 [ejemplo-harness](https://github.com/federicogrecobarragan-prog/ejemplo-harness) | Ejemplo de referencia de harness con subagentes (privado). |

### Diseño · UI — [`topic:design`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Adesign&type=repositories)

| Repo | Descripción |
|---|---|
| [open-design](https://github.com/federicogrecobarragan-prog/open-design) | Alternativa local y open-source a Claude Design: 19 skills, 71 design systems, export HTML/PDF/PPTX/MP4. |
| [claude-creative-work](https://github.com/federicogrecobarragan-prog/claude-creative-work) | Guía de Claude for Creative Work (9 conectores Adobe/Affinity/Blender…, 3 demos, 6 workflows, plan 5 días) + prompt master de batch processing de fotos. |
| [ui-ux-pro-max-skill](https://github.com/federicogrecobarragan-prog/ui-ux-pro-max-skill) | Skill de IA con inteligencia de diseño UI/UX multiplataforma. |
| [PhotoGIMP](https://github.com/federicogrecobarragan-prog/PhotoGIMP) | Patch para GIMP 3+ que lo adapta a usuarios de Photoshop. |
| [hyperframes](https://github.com/federicogrecobarragan-prog/hyperframes) | Escribís HTML, renderiza video. Pensado para agentes. |
| [Fooocus](https://github.com/federicogrecobarragan-prog/Fooocus) | Generador de imágenes IA (Stable Diffusion) enfocado en prompting. Uso en La Colmena (evaluación/condicional, requiere GPU): creativos para posts de Tokio, ads de funnels y contenido Vinoteca. |
| 🔒 [emil-design-eng](https://github.com/federicogrecobarragan-prog/emil-design-eng) | Skill de ingeniería de diseño / componentes UI front (privado). |
| 🔒 [open-codesign](https://github.com/federicogrecobarragan-prog/open-codesign) | Agente de diseño local, open codesign (privado). |

### Marketing · SEO — [`topic:marketing`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Amarketing&type=repositories)

| Repo | Descripción |
|---|---|
| [claude-seo](https://github.com/federicogrecobarragan-prog/claude-seo) | Skill universal de SEO para Claude Code: 25 sub-skills + 18 sub-agentes. |
| [serpapi-claude-plugin](https://github.com/federicogrecobarragan-prog/serpapi-claude-plugin) | Plugin de Claude para la API de SerpApi. |
| [serpapi-cursor-plugin](https://github.com/federicogrecobarragan-prog/serpapi-cursor-plugin) | Plugin de Cursor para la API de SerpApi. |
| 🔒 [ai-marketing-claude](https://github.com/federicogrecobarragan-prog/ai-marketing-claude) | Agencia de marketing con IA para Claude (privado). |
| [marketingskills](https://github.com/federicogrecobarragan-prog/marketingskills) | 45 marketing skills + 65 CLIs (Corey Haines) para Claude Code/agentes: CRO, copy, SEO, funnels, email, social. Operados por **Hermes Agent** en VibeMarketing. |

### Scraping · Extracción web — [`topic:scraping`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Ascraping&type=repositories)

| Repo | Descripción |
|---|---|
| [Scrapling](https://github.com/federicogrecobarragan-prog/Scrapling) | Framework de web scraping adaptativo, de un request a un crawl completo. |
| [Scrapegraph-ai](https://github.com/federicogrecobarragan-prog/Scrapegraph-ai) | Scraper en Python basado en IA: extracción de datos web mediante grafos y LLMs. |
| 🔒 [linkedin-orgchart](https://github.com/federicogrecobarragan-prog/linkedin-orgchart) | Motor LinkedIn completo: scraping v2 (deep mode: años exp, contactos, actividad reciente, email), account pool multi-cuenta (jhonson + sacrificiales Mora/Tokio), proxy residencial vía Tailscale, anti-fingerprint patchright. Genera organigrama jerárquico (.drawio) por área y jerarquía. Privado. |
| 🔒 [scraping-dashboard](https://github.com/federicogrecobarragan-prog/scraping-dashboard) | Consola web privada (Flask) para el ecosistema de RRHH/Intel de La Colmena. Módulos: noticias de tendencias IA (Mora), organigramas LinkedIn viewer (app.diagrams.net integrado), Recluta con búsqueda inteligente (score doble: firewall comercial + técnico + hunting, pipeline fresh/stale desde Supabase), contextos de búsqueda personalizados (CRUD), motor de scraping LinkedIn v2. SPA + API JSON proxy Supabase server-side, nginx Basic Auth. |
| [firecrawl](https://github.com/federicogrecobarragan-prog/firecrawl) | Buscá, scrapeá y limpiá la web para agentes de IA. |
| [goclone](https://github.com/federicogrecobarragan-prog/goclone) | Clonador de sitios web con goroutines de Go (clona en segundos). |
| [Website-Cloner](https://github.com/federicogrecobarragan-prog/Website-Cloner) | Descarga recursiva de un sitio (HTML, imágenes, archivos) a local. |
| [ai-website-cloner-template](https://github.com/federicogrecobarragan-prog/ai-website-cloner-template) | Cloná cualquier sitio con un comando usando agentes de IA. |
| [Webwright](https://github.com/federicogrecobarragan-prog/Webwright) | Framework de agente-navegador para tareas web de horizonte largo. |
| [yt-dlp](https://github.com/federicogrecobarragan-prog/yt-dlp) | Descargador CLI de audio/video con mil opciones. Uso en La Colmena: ingesta de media → Whisper (transcripción), captura de contenido para Mora/análisis y assets Vinoteca/IG. |
| [obsidian-clipper](https://github.com/federicogrecobarragan-prog/obsidian-clipper) | Fork oficial: Web Clipper de Obsidian — captura/resalta páginas web → Markdown durable (templates, variables, filtros). Chrome/Firefox/Safari/Edge. |
| [PriceGhostScarappper](https://github.com/federicogrecobarragan-prog/PriceGhostScarappper) | App self-hosted de tracking de precios de productos desde cualquier web. Referencia/insumo para la suite de precios (`suite-precios` / PriceGhost B2C). |
| [obsidian-api](https://github.com/federicogrecobarragan-prog/obsidian-api) | Fork oficial: type definitions TS de la API de Obsidian para desarrollar plugins. |
| [obsidian-releases](https://github.com/federicogrecobarragan-prog/obsidian-releases) | Fork oficial: catálogo de community plugins + themes + releases de Obsidian. |

### Automatización · WhatsApp · Outreach — [`topic:automation`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aautomation&type=repositories)

| Repo | Descripción |
|---|---|
| [n8n](https://github.com/federicogrecobarragan-prog/n8n) | Plataforma de automatización de workflows fair-code con IA nativa (400+ integraciones). |
| [n8n-nodes-instantly](https://github.com/federicogrecobarragan-prog/n8n-nodes-instantly) | Nodo community de n8n para integrar la API de Instantly (email outbound en frío). Directo para los funnels outbound de La Colmena Digital. |
| [notify-admin-telegram](https://github.com/federicogrecobarragan-prog/notify-admin-telegram) | Notificador Telegram sin dependencias para alertas de infra/tooling (cuotas, billing, tokens, licencias). Env-driven, con severidades. |
| [OpenOutreach](https://github.com/federicogrecobarragan-prog/OpenOutreach) | Herramienta de outreach LinkedIn con IA: describís producto + mercado objetivo y el motor encuentra los leads. Referencia/alternativa para el pipeline HUNTER. |
| [growchief](https://github.com/federicogrecobarragan-prog/growchief) | Tool all-in-one de automatización de outreach en redes sociales. Candidato para escalar el outreach multicanal. |
| [OpenWA](https://github.com/federicogrecobarragan-prog/OpenWA) | API Gateway de WhatsApp gratuito, open source y self-hosted. |
| [wa-automate-nodejs](https://github.com/federicogrecobarragan-prog/wa-automate-nodejs) | Herramienta para chatbots de WhatsApp con features avanzadas. |
| [wa-avd-docker](https://github.com/federicogrecobarragan-prog/wa-avd-docker) | Imagen Docker con Android virtual + WhatsApp preinstalado (VNC/noVNC). |
| [cal.diy](https://github.com/federicogrecobarragan-prog/cal.diy) | **Cal.com** — infraestructura de agendamiento self-hosted (alternativa a Calendly). Uso en La Colmena: funnel AgendaBot, booking KAM/Aria, widget de agenda embebido en oficinadejhonson.com. |

### MCP · Testing — [`topic:mcp`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Amcp&type=repositories)

| Repo | Descripción |
|---|---|
| [mcp-for-beginners](https://github.com/federicogrecobarragan-prog/mcp-for-beginners) | Currículum open-source de Model Context Protocol (MCP) multi-lenguaje. |
| [inspector](https://github.com/federicogrecobarragan-prog/inspector) | Herramienta de testing visual para servidores MCP. |
| [playwright](https://github.com/federicogrecobarragan-prog/playwright) | Framework de testing y automatización web (Chromium, Firefox, WebKit). |

**Recursos para descubrir MCPs** — consultar ANTES de automatizar/configurar a mano (¿existe un MCP para delegárselo a un agente?): [mcpservers.org](https://mcpservers.org/) · [composio.dev](https://composio.dev/) · [pulsemcp.com](https://www.pulsemcp.com/).

### Infraestructura de IA — [`topic:ai-infra`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aai-infra&type=repositories)

| Repo | Descripción |
|---|---|
| 🔒 [llm-local-router](https://github.com/federicogrecobarragan-prog/llm-local-router) | **Router LLM local-first** (zero deps): intenta un modelo local (Ollama, OpenAI-compatible) y cae a un proveedor cloud (OpenRouter) ante OFF/timeout/output inválido. Probe fail-fast + patrón validate-or-fallback + ledger de ahorro. Pensado para offloadear tareas simples (clasificar/resumir) y ahorrar tokens. Usado en La Colmena (VPS ↔ Ollama de desktop vía Tailscale). |
| [engram](https://github.com/federicogrecobarragan-prog/engram) | Memoria persistente para agentes de codificación (Go + SQLite/FTS5, MCP, CLI, TUI). |
| [turbovec](https://github.com/federicogrecobarragan-prog/turbovec) | Índice vectorial sobre TurboQuant (Rust con bindings de Python). |
| [odysseus](https://github.com/federicogrecobarragan-prog/odysseus) | Workspace de IA self-hosted (todo-en-uno). Candidato a evaluar como cockpit local de agentes. |
| [AppFlowy-Cloud](https://github.com/federicogrecobarragan-prog/AppFlowy-Cloud) | Backend de AppFlowy — workspace colaborativo con IA (alternativa open-source a Notion). Proyectos, wikis y equipos con tus datos bajo control. |
| [gentle-ai](https://github.com/federicogrecobarragan-prog/gentle-ai) | Utilidades de IA en Go: building blocks ligeros para agentes/servicios IA. |
| [whisper](https://github.com/federicogrecobarragan-prog/whisper) | Speech-to-text robusto de OpenAI (transcripción/traducción). Uso en La Colmena: Aria transcribe reuniones Meet/Zoom y llamadas de venta → log a CRM/Supabase. |

### Otros — Seguridad · Fintech · ML · Self-hosting

| Repo | Categoría | Descripción |
|---|---|---|
| [nuclei](https://github.com/federicogrecobarragan-prog/nuclei) | [`security`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Asecurity&type=repositories) | Escáner de vulnerabilidades rápido y customizable (DSL en YAML). |
| [npq](https://github.com/federicogrecobarragan-prog/npq) | [`security`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Asecurity&type=repositories) | Instala paquetes npm de forma segura auditándolos en etapa pre-install. Capa supply-chain. |
| [npm-security-best-practices](https://github.com/federicogrecobarragan-prog/npm-security-best-practices) | [`security`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Asecurity&type=repositories) | Colección de buenas prácticas de seguridad para el package manager npm. |
| [agente-pagokit](https://github.com/federicogrecobarragan-prog/agente-pagokit) | [`fintech`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Afintech&type=repositories) | Plugin de Claude Code que genera integración de pagos completa (Stripe, Mercado Pago, Wompi, Lemon Squeezy). |
| [cashclaw](https://github.com/federicogrecobarragan-prog/cashclaw) | [`fintech`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Afintech&type=repositories) | Agente autónomo que toma trabajo, lo hace, cobra y mejora. |
| [nn-zero-to-hero](https://github.com/federicogrecobarragan-prog/nn-zero-to-hero) | [`ml`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aml&type=repositories) | Redes neuronales: de cero a héroe (curso). |
| [GR00T-Dreams](https://github.com/federicogrecobarragan-prog/GR00T-Dreams) | [`ml`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aml&type=repositories) | DreamGen (Nvidia GEAR Lab) — generación de datos de robótica vía world models. Referencia de investigación. |
| [vw_web_builds](https://github.com/federicogrecobarragan-prog/vw_web_builds) | [`self-hosting`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aself-hosting&type=repositories) | Fork de Bitwarden para compilar solo el web-vault de Vaultwarden. |
| 🔒 [infra-deploy](https://github.com/federicogrecobarragan-prog/infra-deploy) | [`self-hosting`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aself-hosting&type=repositories) | Configs de deploy scrubbeadas (solo compose) de infra self-hosted de La Colmena: Vaultwarden (LA BÓVEDA) + Traefik. Secretos vía `.env` no versionado. |
| [analytics](https://github.com/federicogrecobarragan-prog/analytics) | [`self-hosting`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Aself-hosting&type=repositories) | **Plausible** — analytics web self-hosted, privacy-first, sin cookies (alternativa a GA). Uso en La Colmena: medición de oficinadejhonson.com + conversión de funnels (AgendaBot/FacturaBot/ReseñaBot) y landings. |
| [twentyCRM](https://github.com/federicogrecobarragan-prog/twentyCRM) | [`crm`](https://github.com/search?q=user%3Afedericogrecobarragan-prog+topic%3Acrm&type=repositories) | Fork de **Twenty** — alternativa open-source a Salesforce diseñada para IA. Referencia/evaluación CRM frente a `crm-colmena` (decisión pendiente: reemplazar o quedar solo como referencia). |
