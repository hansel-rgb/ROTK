# Three Kingdoms: Mandate of Heaven

A modern reimagining of Koei's *Romance of the Three Kingdoms* — the grand
turn-based strategy series set in the collapse of Han-dynasty China (184–280 AD).
This repository holds the **Game Design Document (GDD)** for a contemporary
remake that keeps the historical characters, the *Sanguo Yanyi* storyline, and
the deep "rule a kingdom, unify China" gameplay loop, while modernizing the
graphics, presentation, UX, and systems.

> Working title: **Three Kingdoms: Mandate of Heaven** (3K:MoH)

## Pitch in one line

> *Lead a warlord's faction from a single contested province to the unification
> of all China — balancing economy, diplomacy, intrigue, and dramatic
> real-time-with-pause battles, dramatized by hundreds of historical heroes who
> live, age, scheme, and die.*

## Design documents

| Doc | Contents |
|-----|----------|
| [`docs/01-vision.md`](docs/01-vision.md) | Vision, pillars, target audience, references, platforms |
| [`docs/02-setting-and-story.md`](docs/02-setting-and-story.md) | Historical setting, narrative scenarios, campaign structure |
| [`docs/03-characters.md`](docs/03-characters.md) | Officer system, stats, traits, lifecycle, relationships |
| [`docs/04-gameplay-strategic.md`](docs/04-gameplay-strategic.md) | The grand strategy layer (the "kingdom" turn loop) |
| [`docs/05-gameplay-battle.md`](docs/05-gameplay-battle.md) | Tactical battle layer (real-time-with-pause) |
| [`docs/06-art-and-audio.md`](docs/06-art-and-audio.md) | Visual direction, UI/UX, audio direction |
| [`docs/07-tech-and-scope.md`](docs/07-tech-and-scope.md) | Engine, architecture, data, monetization, roadmap, MVP |

## What "modernized" means here

- **Presentation:** stylized 3D realm map and battlefields (think *Total War*
  meets ink-wash painting), fully voiced key story beats, motion-captured
  duels, dynamic music.
- **UX:** no more dense spreadsheet menus by default — a clean, layered
  interface with progressive disclosure, smart advisors, and one-click
  delegation for players who want the high-level fantasy.
- **Systems:** a living-officer simulation (ambition, loyalty, factions inside
  your own court), emergent diplomacy, and battles that blend ROTK's classic
  unit-vs-unit tactics with modern real-time-with-pause control.
- **Accessibility & scope:** scalable difficulty, "advisor auto-pilot" for
  micro-management, and three play depths (Story / Standard / Grand).
