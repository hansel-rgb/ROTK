# Playable Prototype — Red Cliffs Vertical Slice

A self-contained, browser-based vertical slice of **Three Kingdoms: Mandate of
Heaven**, implementing the core strategic loop described in the design docs.

## Run it

Just open `game/index.html` in any modern browser. No build step, no server,
no dependencies — pure HTML/Canvas/JS.

## What it demonstrates (mapped to the GDD)

| Design doc | Implemented here |
|------------|------------------|
| `02` Setting & scenario | The 208 AD **Red Cliffs** start: Shu (you), Wei, Wu, and independents on a 13-city map of central China |
| `03` Officers | Historical roster (Guan Yu, Zhuge Liang, Cao Cao, Zhou Yu, Lü Bu-era heroes…) with the 5 ROTK stats (CMD/MGT/INT/POL/CHA), traits, recruitment, capture & defection |
| `04` Strategic layer | Turn/season loop, action points, economy (gold/food/order), develop / train / fortify / pacify / recruit / march, diplomacy (Shu-Wu alliance), AI factions, seasonal events, succession-style relocation |
| `05` Battle layer | **Real-time-with-pause tactical battles** on a stylized field: unit movement, troop-type counters (spears > cavalry > archers > …), terrain (forest / hill / river), **fire stratagems**, charge / volley / rally / heal / ambush abilities, cinematic **duels**, morale & routing, sieges — plus a one-click **auto-resolve** alternative |
| Aftermath | **Captured-officer decisions** after a won battle: **recruit / release / imprison / execute**, each with reputation (honor) and relationship (sworn-bond) consequences |
| `06` Art & UX | Ink-wash parchment map, lacquer/gold chrome, faction colors, click-the-map UX, alert log, modal events, battle HUD |

## How to play

1. Click a **city** to select it. Your cities are green (Shu).
2. Spend **Actions** (top bar) to Develop, Train, fortify, Pacify, or Recruit.
3. Ally with **Wu** (open Chaisang/Jianye) so you can focus on Cao Cao.
4. To attack: select one of *your* cities → **March Army** → click an adjacent
   enemy/neutral city, then choose **Fight on the field** (tactical battle) or
   **Auto-resolve**.
5. **In a tactical battle:** click your (green) units to select them, click the
   ground to move or an enemy to charge; use each officer's **stratagem**; press
   **Space** to pause; **Retreat** to withdraw. Rout or destroy the defenders to
   take the city. Win a battle and you'll **decide the fate of captured officers**.
6. **End Turn** to let the AI act and time advance.
7. **Win** by holding 60% of all cities; lose if you hold none.

This is a balance/feel prototype — the cheapest place to validate that the
strategic loop is fun before committing to engine (Unreal 5) work, exactly as
called out in `docs/07-tech-and-scope.md`.
