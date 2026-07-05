# Playable Prototype — Three Kingdoms: Mandate of Heaven

A self-contained, browser-based prototype of **Three Kingdoms: Mandate of
Heaven**, implementing the core loop from the design docs across a full China
map with multiple scenarios, real-time-with-pause land **and naval** battles,
captured-officer decisions, and prisoner management.

## Run it

Open `game/index.html` in any modern browser. No build step, no server, no
dependencies — pure HTML/Canvas/JS. On launch you pick a **scenario** and the
**faction** you'll lead.

## What it demonstrates (mapped to the GDD)

| Design doc | Implemented here |
|------------|------------------|
| `02` Setting & scenarios | **4 playable scenarios** — *Contending Heroes* (194), *Guandu* (200), *Red Cliffs* (208), *Three Kingdoms* (220) — on a **24-city map of China** with rivers, passes, and regions. Pick your faction (Shu / Wei / Wu / Yuan Shao where historical). |
| `03` Officers | 31-officer historical roster (Liu Bei, Guan Yu, Zhuge Liang, Cao Cao, Sima Yi, Sun Quan, Zhou Yu, Lü Bu, Yuan Shao, Ma Chao…) with the 5 ROTK stats, traits, recruitment, capture, defection, and per-scenario placement |
| `04` Strategic layer | Turn/season loop, action points, economy (gold/food/order), develop / train / fortify / pacify / recruit / march, **alliances with any AI faction**, honor/reputation, seasonal events |
| `03` Living officers | **Loyalty drifts** each turn (with your momentum, honor, posts, ambition, and sworn bonds); neglected officers **defect** to rivals, and powerful ambitious ones **rebel** and seize their city. **Reward** officers to hold their allegiance. Officers **age and die**, and **next-generation heroes** (Jiang Wei, Deng Ai, Sima Zhao…) come of age over a long campaign. |
| Rulers & succession | Every faction has a **ruler** (Liu Bei, Cao Cao, Sun Quan…) whose politics/charisma give faction-wide bonuses. When a ruler dies, a **designated heir succeeds** (you can name yours) — a weak succession dents legitimacy and shakes loyalty. |
| Legitimacy / Mandate | A per-faction **legitimacy** score rising with territory, honor, and control of the **imperial seat (Luoyang)** — "commanding the lords." An alternate **Mandate victory** rewards holding the seat at high legitimacy. |
| Diplomacy | A full **Diplomacy screen**: relations per faction, **tribute**, **dynastic marriage**, and **alliances** gated by relations. Warm relations deter attacks; a **coalition** forms against any power (including you) that grows too dominant — a built-in anti-snowball. |
| Strategic AI | Opponents **reward their own restless officers**, **reinforce threatened borders**, respect **relations/alliances**, **pile onto the coalition target**, and **attack the highest-value city they can beat** — they genuinely expand across the map |
| `05` Battle layer — land | **Real-time-with-pause tactical battles**: unit movement, troop-type counters, terrain (forest / hill / river), fire stratagems, charge / volley / rally / heal / ambush, cinematic **duels**, morale & routing, sieges |
| `05` Battle layer — naval | **Naval battles** on river crossings: ships instead of troops, water battlefield, cavalry weakened, **Navy-trait officers** (Gan Ning) strengthened, and **fire attacks that leap between ships** — the Red Cliffs fantasy |
| Aftermath | **Captured-officer decisions** (recruit / release / imprison / execute) and a **prisoner-management screen** to recruit, release, or execute held captives later — all with honor and sworn-bond consequences |
| `06` Art & UX | Ink-wash parchment map, lacquer/gold chrome, faction colors, click-the-map UX, alert log, modal events, battle HUD, scenario/faction select |

## How to play

1. **Choose a scenario and faction** on the start screen.
2. Click a **city** to select it (your cities glow when selected).
3. Spend **Actions** to Develop, Train, fortify, Pacify, or Recruit.
4. **Alliances:** open a rival faction's city and *Propose Alliance* to secure a
   front (e.g., Shu + Wu vs. Cao Cao at Red Cliffs).
5. **Attack:** select your city → **March Army** → click an adjacent enemy /
   neutral city, then **Fight** (tactical) or **Auto-resolve**. River crossings
   are fought as **naval battles**.
6. **In battle:** click your units to select; click the ground to move or an
   enemy to charge; use each officer's **stratagem**; **Space** pauses; **Retreat**
   withdraws. Rout the defenders to take the city, then decide the fate of any
   **captured officers**.
7. **Prisoners:** the **⛓ button** (top bar) opens the prisoner screen to recruit,
   release, or execute captives you're holding.
8. **Keep your officers loyal:** watch the *Restless officers* count in the realm
   panel and **Reward** officers (in the city panel) before neglect turns them —
   a disloyal officer may defect, and an ambitious one may rebel and take his city.
9. **Rule & succeed:** name an **heir** (realm panel) so your cause survives your
   ruler's death; a strong heir softens the succession shock.
10. **Diplomacy** (⚑ top bar): send **tribute**, arrange a **marriage**, or form an
    **alliance** to warm relations and deter attacks — but beware the **coalition**
    that forms if you grow too dominant.
11. **End Turn** to let the AI act. **Win** by holding 60% of all cities, or by
    holding the imperial seat at high **legitimacy** (the Mandate of Heaven).

This remains a balance/feel prototype — the engine-agnostic place to validate
that the loop is fun before committing to a 3D engine, as `docs/07` describes.
