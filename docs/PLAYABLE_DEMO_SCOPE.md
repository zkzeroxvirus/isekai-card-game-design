# Playable Demo Scope — Hearthcross Vertical Slice

**Design Version: v0.2.19**

## Purpose

Freeze broad feature expansion and convert the current design into a playable vertical slice centered on **The Stranded → Hearthcross → Greyfen March → The Buried Gate**.

The demo should prove the project's identity end-to-end:

**Isekai arrival → direct 3D action combat → Skills → Codex revelation → Hearthcross → Job discovery → one living-world choice → dungeon expedition → boss → Story Revelation → persistent consequences**

This is not a miniature version of the entire game. It is a focused demonstration that the foundational systems work together.

## Demo Target

### Primary Experience

A first-time player should be able to:

1. create a lightweight character
2. begin as **Accidental Transfer — The Stranded**
3. survive an opening wilderness sequence with limited HUD information
4. acquire or recognize a first Skill through actual behavior
5. discover their first Codex manifestation during danger
6. reach Hearthcross
7. choose one prototype combat Discipline package
8. discover and activate one frontier Job
9. complete one Greyfen contract with a persistent consequence
10. enter The Buried Gate
11. experience route choice, unsecured loot, securing/extraction, and party-compatible dungeon play
12. defeat the Gatebound Hob
13. witness the Buried Gate Story Revelation
14. return to a changed Hearthcross state

### Session Shape

Target first complete run: approximately **60–120 minutes** depending on exploration, dialogue, failure, and optional encounters.

The demo should support replay because Job discovery, combat Discipline, first manifestation, regional choice, and dungeon route can differ.

## Hard Scope Freeze

The playable demo includes only what is necessary to prove the vertical slice.

### Included

- third-person movement and camera
- keyboard/mouse baseline, controller-compatible input architecture
- one Origin prologue: **The Stranded**
- limited Background selection or a small preset set
- adaptive first Skill recognition
- adaptive first Codex manifestation from a small pool
- Hearthcross compact hub
- one Greyfen field route with optional branches
- three combat Disciplines:
  - Guardian — Arming Sword & Shield
  - Arcanist — Staff & Arcane Focus
  - Duelist — Twin Blades
- reliable Weapon Arts for each
- five prototype manifestations per Discipline
- one Active Job slot
- a reduced Job roster for demo implementation
- one or two hidden Job qualification paths
- The Buried Gate dungeon
- Gatebound Hob boss
- one secure/extraction checkpoint
- basic unsecured versus secured loot
- one equipment mastery/evolution teaser per Discipline
- one persistent Hearthcross world-state choice
- first Story Revelation
- save/load
- basic host-owned world persistence

### Deferred

Do not block the demo on:

- all five standard Origins
- System Anomaly Origin
- full 1–6 player production networking
- large companion system
- full town construction tree
- full Guild Rank ladder
- infinite dungeon generation
- deep crafting economy
- large Job roster
- full multiclass system
- advanced hybrid Disciplines
- Authorities
- large open world
- PvP
- dedicated servers
- endgame progression

These systems may be represented by hooks, data architecture, or teaser states, but they are not demo requirements.

## Multiplayer Scope

The demo should be built **server-authoritative from the start**, but networking scope should be staged.

### Demo Minimum

Prove stable host + one client first.

### Demo Stretch

Scale the same slice to 1–4 players before attempting the full 1–6 target.

### Production Compatibility

Data and gameplay authority should remain compatible with eventual 1–6 player sessions.

World state belongs to the host. Character progression belongs to each player.

## Demo Character Creation

Keep creation short enough that players reach gameplay quickly.

### Required

- body/appearance preset or modest customization
- Background choice from a small set
- one starting inclination/Skill choice where appropriate
- name

### Suggested Background Demo Set

- Civilian / Office Worker
- Athlete
- Medical Worker
- Hunter / Outdoorsperson
- MMO Player
- Academic / Researcher

Background affects starting Skill opportunities, dialogue, and System-perception flavor rather than large stat bonuses.

## Opening — The Stranded

### Goals

Teach:

- move
- camera
- sprint
- dodge
- interact
- pick up/equip weapon
- basic attacks
- first Weapon Art
- environmental observation
- danger
- first Skill recognition
- first manifestation reveal

### Structure

1. fragmented Threshold imagery
2. character wakes near a damaged roadside ruin / Greyfen edge
3. minimal HUD
4. scavenges basic equipment
5. environmental micro-choice creates early Skill tracking
6. weak creature encounter establishes vulnerability
7. escalating threat forces first manifestation condition
8. road/caravan/survivor encounter points toward Hearthcross
9. arrival at town gate unlocks stable interface layers and multiplayer-ready world state

## First Skill Recognition

Use a small behavior-driven pool:

- Observation I
- Endurance I
- Combat Awareness I
- Medicine I
- Tracking I
- Improvised Tools I

The player should not select this directly from a menu during the opening.

## First Manifestation Pool

Use the existing adaptive candidates:

- Desperate Parry
- Instinctive Step
- Focused Strike
- Protective Impulse
- Mana Spark
- Predator's Mark

The chosen manifestation should reflect actual qualifying behavior whenever possible.

## Hearthcross Demo Hub

Implement a compact readable town rather than a large city.

### Required Spaces

- town gate / Warden checkpoint
- Adventurer Guild Hall
- Split Anvil
- Lantern House
- Survey Office / Archive Annex
- Shrine of the Returning Flame
- Underbridge access point

Not every interior needs a full separate level. Efficient connected spaces are acceptable.

## Demo Job Roster

Implement only enough Jobs to prove location-based discovery.

### Openly Available

1. **Adventurer**
2. **Scout**
3. **Smith**
4. **Field Medic**
5. **Survey Assistant**

### Semi-Hidden

6. **Smuggler**

### Dungeon / Activity Discovery

7. **Dungeon Surveyor**

### Hidden Demo Job

8. **Oathbearer** or **Gate Listener**

Only one hidden Job needs to be fully attainable in the first demo build; the other can provide visible hidden-progress feedback as a teaser.

## Job Demo Requirements

Each implemented Job needs only:

- one meaningful active effect or contextual benefit
- 1–3 associated Skills
- at least one permission or interaction
- at least one NPC/world recognition change
- visible qualification logic where appropriate

The demo is proving **Job discovery**, not full Job endgame progression.

## Combat Discipline Selection

Hearthcross should provide plausible onboarding into one of the three prototype Disciplines.

The choice should not feel like selecting an MMO class from a menu.

Possible framing:

- Guild evaluation
- training yard
- mentor recommendation based on Skills/behavior
- player chooses which discipline to pursue after trying basic packages

### Guardian

Tests timing, blocking, interception, Resolve, frontline control.

### Arcanist

Tests ranged aim, Sigils, Attunement, ground targeting, battlefield control.

### Duelist

Tests mobility, Deflect, Slipstep, Flow, angle-based pressure.

## Codex Demo Deck

After Discipline training, provide a compact deck that produces a five-card manifested hand.

For the demo, prioritize reliability over deckbuilding breadth.

### Prototype Deck Size

Use a small curated deck, likely **8–12 manifestations**, with five active hand slots.

This is deliberately below the eventual broader deck target if needed for usability testing.

### Demo Questions

- Is five-card hand management readable during action combat?
- Does draw/cycle create useful tempo?
- Do cards enhance weapon combat rather than replace it?
- Are transformed slots understandable?
- Does controller access remain comfortable?

## Greyfen Contract

The first shared field contract should create a persistent choice before the dungeon.

### Recommended Scenario

A trade/patrol route is being disrupted by a Greyfen goblin scavenger group.

Possible outcomes:

- kill or drive them out
- negotiate passage
- trade supplies
- expose a third-party cause of escalation
- secretly cooperate with them

### Persistent Effects

Track a reduced set:

- Warden Trust
- Underbridge Influence
- Goblin Relations
- Road Safety

These values change dialogue, one or two Job opportunities, and later dungeon/town details.

The demo does not need a huge simulation. It needs to prove that the world remembers.

## The Buried Gate Demo Dungeon

### Required Structure

- entry / staging
- first combat
- route split
- hazard or observation room
- optional goblin/scavenger interaction callback
- secure/extraction point
- anomaly room
- elite or pressure encounter
- Gatebound Hob boss arena
- true Gate chamber

### Dungeon Goals

Teach:

- route choice
- encounter composition
- basic Knowledge progression
- unsecured loot
- securing/extraction
- Job/Skill interactions
- combat Discipline strengths
- world-state callback
- environmental mystery

## Gatebound Hob

The boss remains the shared combat benchmark.

It must include:

- clearly blockable heavy attack
- attack best answered through dodge/repositioning
- interruptible action
- add or spatial-pressure phase
- exposed/recovery window
- one Buried Gate anomaly interaction

Each Discipline should have a satisfying answer without one being mandatory.

## First Story Revelation

After the boss:

**The Buried Gate recognizes the character/party, but does not fully open.**

The demo should show at least two perception layers:

### Low System Comprehension

Strange geometry, pressure, resonance, partial symbols, uncertain meaning.

### Higher System Comprehension

A more explicit but incomplete classification/recognition event.

Do not explain the central mystery.

## Persistence Demo

After returning to Hearthcross, persist:

- chosen Background
- Skills acquired
- Discipline
- equipment/mastery progress
- Codex manifestations
- active/known Jobs
- Greyfen contract outcome
- faction/world-state variables
- Buried Gate completion
- Story Revelation flag
- secured loot

On reload, Hearthcross should visibly acknowledge at least one earlier decision.

## Equipment Progression Teasers

The demo should show one evolution path per prototype package, but full evolution need not complete in the first run.

- Guardian → Hearthcross Militia Shield → **Gatewarden Shield**
- Arcanist → Hearthcross Survey Staff → **Gate-Echo Staff**
- Duelist → starter twin blades → **Gate-Split Blades**

A player should be able to see that equipment is beginning to remember how it was used.

## Art Scope

Target the established visual direction:

**stylized anime fantasy + softly stylized PBR + grounded frontier environments + restrained early supernatural effects**.

### Priorities

1. readable player silhouettes
2. strong combat animation timing
3. clear enemy telegraphs
4. convincing Hearthcross mood
5. Buried Gate visual transition from frontier ruin to impossible architecture
6. readable Codex manifestations
7. spectacle only where it supports hierarchy

Do not spend demo scope on massive environment acreage.

## Enemy Scope

Recommended minimum:

- Greyfen Goblin Skirmisher
- Greyfen Goblin Bruiser
- Mirehound
- Dungeon-Altered Vermin
- one elite variant
- Gatebound Hob

Reuse skeletons and behavior modules intelligently where production requires it.

## UI Scope

Required:

- health / defensive or relevant resource
- five manifested hand slots after reveal
- current Discipline resource: Resolve, Attunement, or Flow
- minimal status indicators
- interaction prompts
- inventory/equipment minimum viable screens
- Skills / Jobs summary screen
- sparse System messages
- secure/unsecured loot distinction

System Comprehension should visibly alter information presentation where feasible.

## Demo Technical Milestones

### Milestone A — Movement & Combat Sandbox

- third-person movement/camera
- one enemy
- all three basic weapon packages
- Weapon Arts
- basic hit/defense/network authority architecture

### Milestone B — Codex Combat

- five hand slots
- draw/use/discard/cycle
- one transformed card flow
- Guardian Resolve
- Arcanist Attunement/Sigil
- Duelist Flow

### Milestone C — Opening + Hearthcross

- Stranded prologue
- first Skill recognition
- first manifestation
- town traversal/dialogue
- Discipline onboarding
- Job qualification framework

### Milestone D — Greyfen Field Slice

- travel route
- goblin choice encounter
- persistent world-state consequence
- Job/Skill interactions

### Milestone E — Buried Gate

- route split
- extraction checkpoint
- dungeon encounters
- Gatebound Hob
- Story Revelation

### Milestone F — Persistence + Multiplayer Proof

- save/reload
- host world state
- visitor character state
- host + one client through Hearthcross and dungeon

### Milestone G — Demo Polish

- onboarding clarity
- controller pass
- VFX readability
- sound/music pass
- performance
- bug fixing
- replay hooks

## Demo Success Criteria

The vertical slice succeeds if testers can answer yes to most of these:

1. Does the game feel like an action RPG even when the Codex hand is awkward?
2. Do cards materially change combat decisions?
3. Do Guardian, Arcanist, and Duelist feel genuinely different?
4. Does discovering a Skill feel connected to player behavior?
5. Does discovering a Job make the world feel systemic rather than menu-driven?
6. Does Hearthcross feel like a place rather than a services screen?
7. Does at least one choice visibly change later content?
8. Is The Buried Gate interesting before infinite procedural systems exist?
9. Does the Gate revelation create curiosity without dumping lore?
10. Is there a reason to replay with a different Discipline/Job/choice?
11. Can the same architecture plausibly scale toward 1–6 players and deeper progression?

## Production Rule

**Do not add a new major system until the vertical slice demonstrates that the existing systems are fun together.**

New design ideas can be recorded as backlog material, but implementation priority remains the Hearthcross demo until the slice is playable and evaluated.

## Locked Demo Principles

1. The first playable demo centers on The Stranded, Hearthcross, the Greyfen March, and The Buried Gate.
2. The demo is a vertical slice, not a content-complete miniature game.
3. One Origin is enough for the first implementation pass.
4. Guardian, Arcanist, and Duelist remain the three combat benchmarks.
5. Job implementation is deliberately reduced to a small roster proving location-based discovery.
6. At least one hidden progression path must be attainable without being explicitly advertised.
7. One persistent regional choice must visibly affect later content.
8. The Buried Gate must demonstrate combat, exploration, extraction, Knowledge, Job interaction, and narrative mystery in one dungeon.
9. Persistence and server authority are architectural requirements even if full six-player networking comes later.
10. Feature expansion pauses until this slice proves the game's core identity.