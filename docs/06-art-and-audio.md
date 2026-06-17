# 06 — Art, UI/UX & Audio

## Visual direction

A blend of **historical Chinese aesthetics** and clean modern game art —
"ink-wash painting meets stylized 3D." We avoid both photoreal grit and anime
excess; the look is painterly, readable, and timeless.

- **Realm map:** a stylized 3D diorama of China — terrain you can zoom from a
  scroll-painting "strategic" view down to bustling city streets. Seasons
  visibly change (snow in the north, flooding rivers, autumn harvests).
- **Cities:** each region has distinct architecture (northern fortress towns,
  southern river cities, Sichuan mountain strongholds) that visibly grows as
  you develop it.
- **Battlefields:** 3D terrain with hundreds-to-thousands of soldiers, banners,
  dust, and weather; camera free to sweep from tactical-overview to a
  cinematic ground-level "hero cam."
- **Character art:** every officer has a **hand-painted portrait** (the ROTK
  signature) **and** a stylized 3D model for battles, duels, and cutscenes.
  Portraits update with age and status (wounded, promoted, ruler).

## Cinematics & set-pieces

- Marquee story beats (Peach Garden Oath, Three Visits, Red Cliffs, deaths of
  major heroes) play as **directed, voiced cinematics** using in-engine models.
- **Duels** are motion-captured cinematic exchanges.
- Lighter events use **illustrated vignettes** (painted scene + portraits +
  voiced lines) — cheaper to produce at scale than full cinematics.

## UI / UX philosophy (the big modernization)

Older ROTK games are notoriously menu-dense. Our north star is **progressive
disclosure**: surface what matters, hide depth until summoned.

- **Layered interface:** a clean top-level dashboard (realm status, alerts,
  recommendations) → drill into city / officer / army / diplomacy panels only
  as needed.
- **Map-as-UI:** most actions start by clicking the thing on the map (a city,
  an army, an officer), with a radial/context menu — not by hunting through
  nested menus.
- **Advisor & alert system:** the game proactively flags what needs attention
  ("loyalty falling," "famine risk," "army idle") with one-click resolutions.
- **Tooltips & "why" transparency:** every number explains its modifiers on
  hover (why is order dropping? why did this battle prediction shift?). No
  hidden math.
- **Encyclopedia / codex:** in-game wiki of officers, factions, history, and
  mechanics for onboarding and lore.
- **Three depth presets:** Story / Standard / Grand reconfigure UI density and
  automation defaults.
- **Scalable to controller/touch:** the layered, click-the-map model adapts to
  console and tablet without a redesign.

## Audio direction

- **Music:** an orchestral score fusing a Western symphony with traditional
  Chinese instruments (guzheng, erhu, dizi, pipa, drums). **Dynamic** —
  intensity tracks state (peaceful development → tense intrigue → battle).
- **SFX:** weighty, layered battle audio (clashing steel, hooves, war drums,
  fire-attack roars, naval combat); ambient city/season soundscapes.
- **Voice:** key story beats and duels fully voiced. Offer **Mandarin** and
  **English** voice tracks (and ideally Japanese/Korean) for authenticity and
  reach; full subtitle localization.
- **Audio accessibility:** separate volume sliders, subtitles with speaker
  tags, and visual cues paired with important audio alerts.

## Accessibility (cross-cutting)

- Colorblind-safe palettes for the rock-paper-scissors unit colors and faction
  colors.
- Scalable UI/text, remappable controls, pause-anytime combat, adjustable game
  speed, and the delegation system itself as a difficulty/accessibility lever.
