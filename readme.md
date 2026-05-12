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
Survey the cosmos, develop warp drive theory, and assemble the Colony Ship across five construction phases (Hull, Engines, Life Support, Cargo & Cryo, Navigation Core). Once built and stocked with 10M of every resource, launch to a new planet — taking your hard-earned knowledge with you.

---

## Core Features

- **5 resources** across 3 layers: Energy, Minerals, Research, Population, Fuel
- **24 entries** spanning surface, orbital, deep space, and the 5-phase Colony Ship construction
- **19 upgrades** with layer-appropriate unlock conditions (4 of which are late-game Click Mastery upgrades)
- **Knowledge Tree** — a zoomable radial web of 26 nodes across 5 branches (Energy, Minerals, Research, Population, Fuel) plus cross-branch synthesis nodes. Ring-3 nodes are mutually exclusive, forcing meaningful specialization.
- **Click buttons** that unlock progressively — start with Energy, unlock Mining, Research, Habitat, and Fuel as you build
- **Prestige / Colony Ship Launch** — resets your run, carries cross-branch knowledge forward, and applies a permanent 1.5x production bonus. Each run lands on a new real exoplanet.
- **Legacy Points** accumulate across runs
- **Offline progress** capped at 8 hours with randomized Dream Events that apply bonuses or penalties
- **Story ticker** — narrative events trigger as you hit milestones, with ambient colony comms chatter in between. Click the **Log** button on any ticker to open the full transmission history.
- **Milestone cosmetics** — the UI accent color and header badges shift as you hit major milestones
- **Pause** — blurs the screen and freezes all timers and production
- **Time-to-afford** counters on all buildings and upgrades
- **Achievements** — 35 total (24 play-based + 11 rank collection), with milestone achievements marked with a star
- **Tab Badging** — `!` badge on tabs clears on visit and reappears only when a genuinely new item becomes available (not a permanent counter)
- **Hold to Generate Resources** — hold down any click button to continuously generate resources; touch-friendly for mobile play
- **Combined Resource Buildings** — multi-resource buildings are grouped in a dedicated section below the single-resource columns
- **Audio engine** — procedural SFX for clicks, purchases, achievements, knowledge unlocks, and prestige launch, plus a slow evolving ambient music pad. All generated in-browser via Web Audio API — no audio files.
- **Audio settings** — master, music, and SFX volume sliders accessible from the header; preferences persist across sessions
- **Click animations** — pulse + colored ring expand on every click, with particle burst, per-resource color
- **Layer transition cinematic** — full-screen reveal when you unlock Orbital or Deep Space
- **Patch Notes tab** — in-game changelog so returning players can see what changed
- **Hold to Buy / Sell** — press and hold any Buy or Sell button to repeat the action; matches the Hold to Generate pattern
- **Unified Upgrades tab** — all upgrades in one sorted grid, prioritized by what you can buy now, with resource accent colors
- **Building Prerequisites** — tier-2 and tier-3 buildings require specific other buildings; lock requirements display clearly on the card
- **Click Mastery upgrades** — four late-game upgrades that multiply click power 2×, 5×, 10×, 20× (up to 2000× stacked). Unlock after owning any tier-3 knowledge node.
- **Save / Load** — export the full save (XP, ranks, current run) as base64; copy to clipboard or download as .txt. Paste back in to restore.
- **Streamlined header** — utility buttons for audio, save, support+patch notes, and pause all live in the header. Two tabs freed up by moving Notes and Support behind icon buttons.
- **XP System** — earn XP from clicks, builds, upgrades, knowledge, achievements, layer transitions, story events, resource milestones, time played, daily streaks, and especially Colony Ship launches. First-time bonuses for new buildings, upgrades, layers, story events, and planets visited. Personal-best speed bonus for faster launches. XP gain decays slightly per prestige (8% per launch, floor 30%). Live floating popups in the top-right show every gain.
- **XP Store / Ranks** — spend XP on Ranks: persistent perks you own forever and can equip or swap freely. Only one Rank can be equipped at a time, but you keep them all once purchased. Currently 36 Ranks across Common, Uncommon, Rare, Legendary, Mythic, plus 3 Secret Ranks unlocked by play. Includes chaotic gems like Dave's Cousin (random building hiccups), The Intern (every 25th click fizzles), Beans McGraw, Esq. (100% sell refund), Heavyweight (+200% prod but click power = 0), Glass Cannon (+150% prod but halves a random building every 5 min), and The Lonely Astronaut (+500% prod, can't win — solo flight trophy). Ranks persist across launches.

---

## Progression Path

```
Solar Arrays x10           →  Mine click unlocks
Drill Rigs x10             →  Research click unlocks
Research Labs x10          →  Habitat click unlocks
Terraformer built          →  Layer 2 (Orbital) unlocks, Fuel added
Station Dock built         →  Layer 3 (Deep Space) unlocks
2× L3 upgrades + tier-3    →  Phase 1 (Hull Frame) unlocks
knowledge + L3 buildings
Phases 1 → 5 built          →  Launch readiness gate
10M of every resource held →  Launch button enabled
LAUNCH                      →  Win! Prestige to new planet
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

## Known Bugs

_(No open bugs.)_

---

## Backlog

Features planned for future runs:

### Progression & Depth
- **Bulk Buy (×10 / ×100)** — add buy-quantity toggles on building cards so mid/late-game players can scale up quickly without holding a button. Pairs well with tighter early-game pacing.
- **Construction Timer** — first build of any building type requires a timed construction phase (you're a person; only one thing at a time). Subsequent purchases of the same type are instant. Resources deducted immediately, building added on completion. Visual progress bar on the card.
- **Leaderboard** — fastest Colony Ship launch times by planet, submitted anonymously. Gives the "race" in Space Base Race real meaning.
- **Daily Challenge** — a fixed seed run with a specific planet and handicap condition, resetting every 24 hours. Shareable score at the end.
- **New Game Plus Modifiers** — after several prestiges, unlock optional run modifiers (e.g. "No Drills", "Double Fuel Cost") for challenge and replayability. *Depends on Story Enhancement — complete story arcs and effects before this.*

### Feel & Polish
- **Onboarding / First-Run Tutorial** — a lightweight tooltip sequence for brand-new players: highlight the first click button, explain resources, nudge toward the first building. Skippable, never shown again after run 1. Critical for itch.io discoverability where players have no context.
- **Keyboard Shortcuts** — number keys (1–5) to trigger resource clicks, hotkeys to switch tabs. Low-effort, high-reward for power users.
- **Tab Bar Redesign** — restyle the two-row tab bar to look like physical file tabs (raised active tab, recessed inactive, clear visual separation between rows and content panel) rather than plain text buttons on a strip.

### Accessibility & Platform
- **Mobile / Touchscreen Friendly** — responsive layout and touch-optimized controls so the game plays well on phones and tablets.
- **Multi-language Translation** — localization support for major languages, making the game accessible to a global audience.

### Meta & Community
- **User Registration** — account system so players can save progress server-side, appear on leaderboards, and carry stats across devices. Foundation for Daily Challenge, Leaderboard, and social features.
- **Referral / Share Link** — one-click share that opens itch.io, for word-of-mouth growth.

### Ranks & Achievements
- **Ranks in the Story** — make rank collecting feel meaningful through two layers: (1) **Rank lore** — story events and codex entries that explain what ranks *are* in-world: a mix of Earth HQ's official Colonial Designation System, Dave's own parallel classification framework, and the history of how the two systems diverged and occasionally conflict. Each rarity tier has a different origin (e.g. Common ranks are Earth-issued field designations; Legendary ranks were coined by Dave; secret ranks have no official record). (2) **Rank milestone story events** — specific story cards fire when the player collects their first rank of a given rarity, their first secret rank, or reaches a milestone count. Dave reacts to rank milestones in his own way. The narrative frames collecting ranks as the colony's growing reputation being observed — by Earth, by Dave, and possibly by something else.

### Story & World
- **Story Effects on Gameplay** — story events should trigger real mechanical effects: a solar flare temporarily doubles energy, antimatter incident locks an upgrade for 60 seconds, Dave's calculations award a fuel bonus. Ties narrative to simulation and rewards players paying attention.
- **Environmental Storylines** — planet-specific story arcs driven by the environment itself: weather events on a frozen world, volcanic eruptions on a magma planet, atmospheric storms on a gas giant moon, tidal cycles on an ocean world. Each biome gets 3–5 unique environmental events that fire across a run, building a sense of place beyond just stat modifiers.
- **Alien Signal Storyline** — the signal detected in the first story event develops across layers into a full mystery arc.

---

## Changelog

### v1.3
- ★ Rank Collection Achievements — 11 new achievements tied to the rank system: first of each rarity tier (Common through Mythic), milestone counts (5, 10, 20 ranks), Full Roster (all non-secret), and Classified Cleared (all 3 secret ranks). Rank collecting is now an explicit long-term goal.
- ✓ Tab Badge Behaviour — badges now clear when you visit a tab and reappear only when genuinely new items become available. Changed from a number counter to a single `!` indicator.
- ✓ Countdown Timer Layout Fix — building and upgrade cards now always reserve the timer line height. Shows `~Xs` while counting down, swaps to green "✓ Available" when ready. Cards no longer shift height.
- ✓ Readability & Contrast Pass — brighter text throughout: comms/log entries, story ticker, planet name, tab labels. Increased font weight on secondary labels.

### v1.2
- ★ Textbook / Codex tab — in-game reference for everything: Resources, Buildings, Upgrades, Knowledge nodes, Ranks, Biomes, Planets, and People. 130+ entries with lore, mechanics, and progressive discovery (locked entries shown as classified until seen in-game).
- Rank lore — narrative system explaining the Colonial Designation System, Dave's parallel classification, and the origin story of each rarity tier.

### v1.1
- ★ 30 Biomes — each prestige run lands on a uniquely flavoured world: Mushroom World, Sentient Fog, Dave World, Chaos World, Gerald's World, The Waiting Room, and 24 more. Biome shown as a badge in the header.
- ★ Biome weather events — the comms ticker pulls biome-specific events 40% of the time, grounding the run in its environment
- ★ Dave Arc — 6 new story events building a cross-layer mystery arc: Dave's Question → Dave in the Ore → Dave Knows the Planet → Dave's Calculations → The Signal Is Dave → Dave Chooses
- ★ 10 new story events filling narrative gaps across all three layers (Resonance, First Harvest, What the Ore Becomes, Patient Zero, Deep Cut, Margaret's Report, Sleeping Volunteers, The View From Here, Second Signal, The Weight of It)
- 25 new ambient colony chatter events (pool doubled from 12 to 37)

### v1.0
- ★ Two new buildings: Quarry (minerals tier 2, requires 5× Drill Rigs) and Nursery (population tier 2, requires 5× Habitat Domes)
- ★ Stats Tab — new tab showing this-run stats (time, clicks, buildings, knowledge, upgrades, resources) and all-time stats (launches, total XP, personal best, planets visited, ranks owned, daily streak)
- ★ Run Summary Screen — full-screen modal on Colony Ship launch showing run time, legacy points, clicks, buildings, knowledge nodes, and personal best flag; dismiss to embark
- Two-row tab bar — tabs split across two rows (Build / Upgrade / Knowledge / Achievements on top; Ranks / Stats / Launch on bottom), more breathing room at all screen sizes
- Early game pacing — tier-1 building production reduced from 0.5/s to 0.3/s; base cost raised from 12 to 18; first few buildings require more investment
- Version number shown in Support & Patch Notes modal header
- Bug fix — upgrade tab badge no longer counts exclusive upgrades that are blocked by a purchased sibling choice

### v0.9.1
- ★ Soft Choices / Branching Upgrades — three exclusive upgrade pairs (one per layer); pick one, lock the other forever
- ★ Animated Building Icons — idle animations on building cards when producing (spin, bounce, pulse, sway, float)
- ★ High Contrast Mode — 👁 header toggle; white-on-black theme for accessibility; persists across sessions
- Quieter XP Popups — smaller, lower opacity, shorter duration; rapid gains batch into one popup
- Colony Ship phase costs ×100 — endgame now requires serious resource accumulation
- Bug fix — passive production for non-clicked resources continued correctly while holding a click button
- Bug fix — in-game Patch Notes now in sync with readme changelog

### v0.9
- ★ Phased Colony Ship construction — five sequential build phases replacing the single buy button
- Phase 1 entry gates: tier-3 knowledge node, 2 of 3 Layer-3 upgrades, and building prereqs
- Launch requires holding 10M of every resource after all 5 phases complete
- Layer Skipper rank halves all phase costs

### v0.8
- ★ Click Mastery upgrades — four new upgrades multiplying click power 2×, 5×, 10×, 20× (up to 2000× stacked); unlock by owning any tier-3 knowledge node
- ★ Save / Load — export full save state to base64, copy or download as .txt, import to restore
- Moved Patch Notes into the Support modal; both now live behind a single ℹ button in the header
- Header gained 💾 save and ℹ support buttons; two tabs freed up

### v0.7
- ★ 16 new Ranks across Rare, Legendary, and Mythic tiers (including Pioneer, Industrialist, Atomic Scholar, Lucky Breaker, Layer Skipper, The Hoarder, Static Cling, Architect, Hivemind, Time Lord, Dyson Heir, Heavyweight, Glass Cannon, Stellar Council, The Architect Prime, The Lonely Astronaut)
- ★ 3 Secret Ranks unlocked through play: Dave (5 launches), The Naked Engineer (Running Naked achievement), Echo of the First Colony (10 unique planets)
- New Achievement: Running Naked — launch with no Rank equipped after a launch with one (milestone, gold star)
- Ranks like Pioneer and The Architect Prime now apply their starting state on every run including the first one after equipping
- Glass Cannon adds tense risk to long runs; Heavyweight rewards full idle play; The Lonely Astronaut is a trophy build with no win path

### v0.6
- ★ XP System — earn XP from nearly every action (clicks, builds, upgrades, knowledge, achievements, layer transitions, milestones, story events, time played, daily streaks, and Colony Ship launches)
- First-time bonuses, personal-best speed bonus, and a daily streak reward
- XP gain decays per prestige (8% per launch, 30% floor) to keep the meta layer meaningful
- Floating "+N XP" popups in the top-right
- ★ XP Store with 20 Ranks across Common and Uncommon tiers — equip one at a time, swap between any you own
- Chaotic Ranks added for flavor: Dave's Cousin, The Intern, Beans McGraw Esq., The Optimist, Coffee Addict
- Ranks persist across Colony Ship launches and apply to every run

### v0.5.1
- Bug fix — mobile taps on Buy / Sell were triggering hold-repeat after a single tap; touch and mouse events were both firing. Now suppressed.
- Bug fix — same issue on resource click buttons could leak repeating timers in rare cases
- Tuned hold-detection threshold to 350ms (was 280ms) for more reliable mobile taps

### v0.5
- Hold to Buy / Sell — press and hold any building's Buy or Sell button to repeat
- Particle burst on click — colored particles radiate outward from resource buttons
- Unified Upgrades tab — all upgrades in one sorted grid, prioritized by what you can buy now
- Building Prerequisites — tier-2 and tier-3 buildings require specific other buildings; lock requirements display clearly on the card
- Removed the X close button from the story ticker banner

### v0.4
- Audio engine — procedural SFX for clicks, purchases, achievements, knowledge unlocks, and prestige launch
- Ambient music — slow evolving synth pad, generated entirely in-browser
- Audio settings — master, music, and SFX volume sliders accessible from the header
- Click button animations — pulse + colored ring expand on every click
- Layer transition cinematic — full-screen reveal when you unlock Orbital or Deep Space
- Patch Notes tab — in-game changelog so returning players can see what changed

### v0.3
- Tab Badging — live badges on Upgrade, Knowledge, and Achievements tabs
- Hold to Generate — hold any click button to continuously produce resources
- Combined Resource Buildings — multi-resource buildings now grouped in their own section

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
