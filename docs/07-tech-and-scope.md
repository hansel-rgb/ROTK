# 07 — Tech, Scope & Roadmap

## Engine & tech choices

- **Engine:** **Unreal Engine 5** or **Unity (HDRP)** — chosen for mature 3D
  pipelines, large-crowd rendering (battles), strong tooling, and console
  portability. Recommendation: **Unreal 5** for the cinematic/large-battle
  spectacle and Nanite/Lumen-friendly stylized art.
- **Language/architecture:** a **data-driven simulation core** (officers,
  cities, economy, AI) kept separate from rendering, so the strategy sim can be
  developed, tested, and balanced headlessly.
- **Data:** all officers, scenarios, buildings, traits, events, and units defined
  in **external data files** (JSON/database + designer tools), enabling rapid
  balancing and **modding/Steam Workshop** support from day one.
- **AI:** layered — a **strategic AI** (faction agendas, diplomacy, economy,
  campaign planning) and a **tactical AI** (battle command), plus **utility/
  behavior-tree** driven officer personalities so traits actually change play.
- **Saves:** robust serialization of the full sim state; autosave + cloud saves.

## Production scope (realistic framing)

This is an ambitious mid-to-large project. Scope is staged so a vertical slice
proves the fun before the full content build.

### Vertical slice (prove the loop)

- One scenario (**207–208, Red Cliffs**) on a reduced map (~10–15 cities).
- ~50 key officers fully implemented (stats, traits, a few abilities).
- Full turn loop: develop, recruit, diplomacy basics, one intrigue type.
- RTwP battles with 3–4 troop types, 3 stratagems, basic sieges, one duel.
- One difficulty preset, placeholder/early UI, temp audio.
- **Goal:** is the core loop fun for 2–3 hours? Balance and feel before scale.

### MVP / Early Access

- 3 scenarios, ~40 cities, ~250 officers.
- Full strategic layer (economy, diplomacy, intrigue, succession).
- Full battle layer (all troop types incl. navy, sieges, duels, stratagem set).
- Chronicle + Free modes; Story/Standard/Grand presets; advisor/delegation.
- Core UI complete; English VO for marquee events; dynamic music v1.
- Modding data hooks exposed.

### 1.0 / Full release

- All 7 scenarios + sandbox; full ~800 officer roster; complete China map.
- Full cinematic set-pieces; Mandarin + English VO; complete codex.
- Custom officer editor + Steam Workshop.
- Console builds (stretch).

## Content pipeline notes

- **Officer data** is the largest content task: 800 officers × (stats, traits,
  portrait, 3D model, relationships, historical death dates). Build a designer
  tooling/spreadsheet → data pipeline early; use shared modular 3D models with
  swappable parts to make 800 models feasible.
- **Events/story** authored in a branching-narrative format (e.g., Ink/Yarn) so
  writers work independently of engineers.

## Monetization

- **Premium base game** (no pay-to-win, no loot boxes — respects the strategy
  audience).
- **Expansions/DLC** in ROTK/Paradox tradition: new scenarios, mechanics
  (e.g., deeper court intrigue, naval expansion), and officer packs.
- **Free updates** + Workshop to sustain a long-tail community.

## Risks & mitigations

| Risk | Mitigation |
|------|------------|
| Scope/content volume (800 officers, full map) | Vertical slice → EA → 1.0 staging; modular asset pipeline; data-driven content |
| UI complexity overwhelming new players | Progressive disclosure, advisors, depth presets, vertical-slice UX testing |
| RTwP battles feeling shallow *or* fiddly | Prototype battles first; auto-resolve + speed controls; stratagem depth |
| AI not being a credible opponent | Invest early in layered AI; expose difficulty via behavior, not just stat buffs |
| Balancing a living-officer sim (defections/coups) | Headless sim harness for automated balance testing; telemetry in EA |
| Licensing/IP | Uses **public-domain history & the *Sanguo Yanyi* novel** (not Koei's assets); original art, names from history |

## High-level roadmap

1. **Pre-production:** sim core prototype, data schema, art style exploration.
2. **Vertical slice:** prove the loop (above). Greenlight gate.
3. **Production → Early Access:** MVP scope, community feedback loop.
4. **EA → 1.0:** full content, polish, localization, console.
5. **Post-launch:** expansions, Workshop curation, balance patches.

## A note on the repository

This repo currently contains the **design** for the game. A natural next step
is a prototype of the headless simulation core (turn loop + officer/economy
model) in this repo to validate the strategic layer before committing to engine
work — that core is engine-agnostic and the cheapest place to find the fun.
