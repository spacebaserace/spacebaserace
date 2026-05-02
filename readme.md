# 🚀 Space Base Race

A browser-based idle clicker game where you build a space colony, reach orbit, launch a deep space program, and ultimately send a Colony Ship to a new planet — then do it all again, faster.

**Play it on itch.io:** https://spacebaseracedev.itch.io/space-base-race

---

## Gameplay Overview

Space Base Race is structured across three layers of progression, each unlocking after hitting a milestone in the previous one.

### Layer 1 — Surface Colony 🌍
Establish your first colony on a new planet. Build Solar Arrays, Drill Rigs, Research Labs, and Habitat Domes to generate your four core resources: Energy, Minerals, Research, and Population. Progress through refineries, greenhouses, and ultimately the Terraformer, which reshapes the planet and unlocks orbital operations.

### Layer 2 — Orbital Station 🛸
Build a presence in orbit. A fifth resource — Fuel — powers your orbital ambitions. Construct Launch Pads, Orbital Labs, Solar Collectors, and a Command Module. The Station Dock completes your orbital infrastructure and opens the door to deep space.

### Layer 3 — Deep Space Program 🌌
Survey the cosmos, develop warp drive theory, and construct a Colony Ship. Building the Colony Ship wins the run and lets you launch to a new planet — taking your hard-earned knowledge with you.

---

## Core Features

- **5 resources** across 3 layers: Energy, Minerals, Research, Population, Fuel
- **20 buildings** spanning surface, orbital, and deep space tiers
- **15 upgrades** with layer-appropriate unlock conditions
- **Knowledge Tree** — a zoomable radial web of 26 nodes across 5 branches (Energy, Minerals, Research, Population, Fuel) plus cross-branch synthesis nodes. Ring-3 nodes are mutually exclusive, forcing meaningful specialization.
- **Click buttons** that unlock progressively — start with Energy, unlock Mining, Research, Habitat, and Fuel as you build
- **Prestige / Colony Ship Launch** — resets your run, carries cross-branch knowledge forward, and applies a permanent 1.5x production bonus. Each run lands on a new real exoplanet.
- **Legacy Points** accumulate across runs
- **Offline progress** capped at 8 hours with randomized Dream Events that apply bonuses or penalties
- **Story ticker** — narrative events trigger as you hit milestones, with ambient colony comms chatter in between. Click the **Log** button on any ticker to open the full transmission history.
- **Milestone cosmetics** — the UI accent color and header badges shift as you hit major milestones
- **Pause** — blurs the screen and freezes all timers and production
- **Time-to-afford** counters on all buildings and upgrades
- **Achievements** — 23 total, with milestone achievements marked with a star

---

## Progression Path

```
Solar Arrays x10  →  Mine click unlocks
Drill Rigs x10    →  Research click unlocks
Research Labs x10 →  Habitat click unlocks
Terraformer built →  Layer 2 (Orbital) unlocks, Fuel resource added
Station Dock built →  Layer 3 (Deep Space) unlocks
Colony Ship built  →  Win! Launch to new planet (Prestige)
```

---

## Knowledge Tree Branches

| Branch | Specialty | Ring-3 Effect |
|---|---|---|
| Energy | Solar power, plasma conduits | Dyson Fragment — Energy x4 |
| Minerals | Drilling, asteroid mining | Asteroid Siphon — Minerals x4 |
| Research | Peer review, quantum computing | Unified Field Theory — All prod x2.5 |
| Population | Ergonomics, cloning, hive mind | Hive Mind Protocol — Population x4 |
| Fuel | Combustion, antimatter, warp | Warp Bubble Theory — All fuel x3 |
| Cross-branch | Plasma Drill, Xenoarchaeology, Neural Colony, Bio-Reactors, Solar Sails + outer combos | Synergistic bonuses |

Ring-3 branch nodes are **mutually exclusive** — choosing one blocks the others, pushing players toward specialization or cross-branch builds.

---

## Prestige System

Completing a run by building the Colony Ship triggers a launch sequence. On launch:

- All buildings, upgrades, and resources reset
- **Cross-branch knowledge nodes survive** (the synthesis nodes between branches)
- A permanent **1.5x production multiplier** is applied (stacks each run)
- **Legacy Points** are awarded based on run time, knowledge unlocked, and layer reached
- The next run begins on a new planet drawn from a list of real exoplanet candidates

### Destination Planets
Kepler-442b, Proxima Centauri b, TRAPPIST-1e, Gliese 667Cc, HD 40307g, 55 Cancri f, Wolf 1061c, Ross 128b, Teegarden b, LHS 1140b

---

## Tech Stack

- **React 18** (loaded via CDN)
- **Babel Standalone** for JSX transpilation in-browser
- **Single file** — the entire game ships as one `index.html` with no build step required
- **localStorage** for offline time tracking

---

## Development

### Running Locally

No build step needed. Just open `index.html` in a browser.

```bash
# Optional: serve with a local server for localStorage to work correctly
npx serve .
# or
python -m http.server 8080
```

### Branch Strategy

| Branch | Purpose |
|---|---|
| `main` | Stable, deployed to itch.io |
| `dev` | Active development |
| `feature/*` | Optional feature branches |

Merge `dev` → `main` to trigger deployment.

---

## Backlog

Features planned for future runs:

- **Soft Choices / Branching Upgrades** — upgrade trees with meaningful tradeoffs (e.g. double gold but halve click power), giving players a strategic identity
- **Textbook / Codex** — a reference tab with full lore definitions for every building, upgrade, and knowledge node
- **Biomes** — each prestige destination planet has a unique biome (ice world, volcanic, gas giant moon, etc.) that modifies starting conditions, building costs, resource rates, and story flavor. Revealed on the launch screen before the new run begins.
- **Multi-language Translation** — localization support for major languages, making the game accessible to a global audience
- **Mobile / Touchscreen Friendly** — responsive layout and touch-optimized controls so the game plays well on phones and tablets
- **Hold to Generate Resources** — hold down a click button to continuously generate resources rather than clicking repeatedly. Essential for accessibility and mobile play.

---

## Changelog

### v0.2
- Log button now opens a modal overlay showing full comms and story history
- Tab labels corrected to full names (Knowledge, Achievements)
- Support email updated to spacebaserace@gmail.com

### v0.1
- Initial release

Found a bug or have a feature idea? Email us:

**spacebaserace@gmail.com**

Please use the subject line: `TICKET Space Base Race`

---

## License

All rights reserved. Not open source at this time.
