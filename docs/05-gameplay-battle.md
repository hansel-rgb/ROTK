# 05 — Battle Layer (Tactical Combat)

Battles are the dramatic climaxes of the strategy game. We modernize ROTK's
classic tactical battles into **real-time-with-pause (RTwP)** engagements on
3D battlefields, while preserving the officer-led, stratagem-driven flavor.

## When a battle happens

When an army attacks a city or two armies meet in the field, the player can:

- **Fight manually** on the tactical map (full control), or
- **Auto-resolve** with a previewed odds estimate (for trivial or tedious
  fights — respects the delegation philosophy).

## Battle structure

- **Units** are led by officers and composed of troop types. A unit's strength
  comes from troop count **and** its leader's stats (Command, Might, Intellect).
- **Troop types** with a rock-paper-scissors core:
  - **Spearmen** beat cavalry, lose to archers/infantry.
  - **Cavalry** beat archers & flanks, lose to spears.
  - **Archers / Crossbows** beat infantry at range, weak in melee.
  - **Infantry/Swordsmen** — durable generalists, siege.
  - **Siege engines** (rams, catapults, towers) — break walls/gates.
  - **Navy** (rams, fire ships, transports) for river/coastal battles —
    essential for Red Cliffs-style engagements.
- **Terrain & weather:** forests (ambush/fire), rivers (fords, naval), hills
  (high-ground bonus), weather (wind enables fire attacks, rain disables them).

## Real-time-with-pause flow

- Battle runs in real time; **pause any time** to issue orders, queue moves,
  and trigger abilities — preserving tactical depth without twitch demands.
- Adjustable speed (0.5×–3×); a "tactical pause" auto-triggers on key events
  (officer in danger, stratagem available, reinforcements arrive).

## Officer abilities & stratagems

The signature ROTK flavor: **stratagems** turn battles, not just numbers.

- **Active abilities** per officer, gated by Intellect and traits and on
  cooldown/resource (a "stratagem" gauge):
  - **Fire Attack** — devastating in forests / against ships with the right wind
    (the Red Cliffs fantasy).
  - **Ambush** — hidden units spring from terrain.
  - **Confuse / Taunt / Rumor** — disrupt enemy formations and morale.
  - **Rally / Inspire** — restore morale and ATK.
  - **Flood / Decoy / Feigned Retreat** — classic novel stratagems.
- **Counter-stratagems:** a clever enemy strategist can *see through* and negate
  your plan — an Intellect duel within the battle.

## Duels (single combat)

A beloved ROTK feature, modernized:

- When two officers clash, an optional **cinematic duel** can trigger — a
  motion-captured one-on-one decided by Might, traits, health, and a light
  timing/choice mini-interaction (attack/defend/feint).
- Outcomes ripple outward: winning a duel can rout the loser's whole unit;
  duels can capture, wound, or kill marquee officers. High drama, high stakes.

## Morale & the human factor

- Units have **morale**; routs cascade. Killing/capturing an enemy general
  collapses nearby morale. Heroic officers can hold a line against the odds.
- This makes battles feel like the novel: a single hero (Zhao Yun at Changban)
  can swing an engagement.

## Sieges

- Assault walls with siege engines, scale with ladders, or use spies to **open
  the gates from within** (ties intrigue → battle).
- Or **starve a city out** on the strategic layer — sieges aren't only assaults.

## Victory, retreat & consequences

- Win by routing/destroying the enemy army or taking the objective (city/gate).
- **Retreat** preserves troops at a cost; smart withdrawal is valid play.
- Casualties, captured officers, and captured cities carry back to the strategic
  layer — battles have weight beyond the battle screen.

## Scale & pacing

- Skirmishes (a few units) resolve in minutes; grand battles (full stacks,
  siege, naval) are set-piece encounters.
- Auto-resolve plus battle-speed controls keep a long campaign from drowning in
  tactical micro — the player chooses where to spend attention.
