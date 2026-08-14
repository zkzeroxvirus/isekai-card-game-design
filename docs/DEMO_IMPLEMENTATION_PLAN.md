# Playable Demo Implementation Plan

**Production Phase: Vertical Slice Implementation**

## Goal

Turn the existing Hearthcross / Greyfen / Buried Gate design into a playable third-person demo that proves the project’s core identity end-to-end.

The demo is not intended to prove content breadth. It must prove that the existing systems are enjoyable together.

## Demo Spine

**The Stranded → first Skill → first Codex manifestation → Hearthcross → Discipline + Job discovery → Greyfen consequence → Buried Gate → Gatebound Hob → Gate recognition → persistent return state**

## Development Rule

**Do not add a new major system until the vertical slice demonstrates that the existing systems are fun together.**

Every implementation task should answer one of three questions:

1. Does the player control feel good?
2. Do the game systems interact coherently?
3. Does the demo communicate the intended isekai progression fantasy?

If a task does not materially help answer one of those questions, it is outside the current demo scope.

---

# Milestone 0 — Project Skeleton

## Objective

Establish the Unreal project structure and authoritative gameplay foundation before content work expands.

## Deliverables

- Unreal Engine 5 project created and bootable
- source-control-safe project organization
- gameplay module structure
- Enhanced Input enabled
- Gameplay Ability System evaluated/initialized for the prototype
- basic networked character spawning
- server-authoritative health/damage skeleton
- gameplay tags/data asset conventions
- debug map for rapid combat iteration

## Exit Criteria

- host and one client can join a test map
- both can move independently
- server owns health and validates damage
- debug logging can identify ability, status, card, and combat events

---

# Milestone 1 — Movement, Camera & Guardian Combat Sandbox

## Objective

Prove the basic third-person action game before implementing the Codex.

## Player Controls

Prototype actions:

- move
- camera
- sprint
- dodge
- interact
- lock-on / target assist if retained after testing
- light attack
- heavy attack
- weapon action
- Weapon Art inputs

## First Weapon Package

Implement **Guardian + Arming Sword & Shield** first because it tests the largest number of foundational action-combat requirements.

Baseline actions:

- Sword Cut
- Driving Cut
- Guard

Weapon Arts:

- Advancing Slash
- Shield Bash
- Intercept
- Counterstep

## Guard Outcomes

Implement the qualitative prototype:

- Weak Guard
- Solid Guard
- Perfect Guard

Do not tune final frame windows yet. The first implementation should make the three outcomes obvious and instrumentable.

## First Enemy

Create one simple Greyfen melee enemy capable of:

- approach
- basic attack
- clearly telegraphed heavy attack
- stagger response
- target switching
- death

This enemy is a combat test instrument before it is finished content.

## Exit Criteria

- movement and camera feel stable
- attacks have readable commitment
- dodge can avoid threats
- Guard direction matters
- Perfect Guard is understandable
- Shield Bash can interrupt the heavy attack
- combat works for host and client
- basic enemy remains readable with two players

---

# Milestone 2 — Codex Runtime

## Objective

Add the system that makes this game different from a conventional action RPG.

## Runtime Model

Implement a five-slot Active Codex hand.

Each card should contain data sufficient to describe:

- identity
- source / Discipline
- category
- tags
- targeting family
- costs
- deck behavior
- executable ability reference
- mastery/evolution metadata hooks

Executable gameplay remains separate from card definition.

## Required Zone Flow

Prototype only what the demo needs:

- Deck
- Hand
- Discard
- Exhaust
- Prepared / transformed-in-place support where required

## First Card Set

Guardian starter manifestations:

1. Brace → Perfect Guard
2. Shield Counter
3. Guardian’s Advance
4. Hold Fast
5. Severing Riposte

## Required System Features

- slot activation independent of card identity
- replacement card enters emptied slot
- server validates card use
- same-slot transformation
- card targeting families
- discard / redraw loop
- debug deck inspector

## Exit Criteria

- five cards can be used while moving
- using cards does not require opening menus
- Brace can transform in the same slot
- Guardian’s Advance can modify Advancing Slash
- server and client agree on card zones and effects
- deck cycling creates understandable combat tempo

---

# Milestone 3 — Stranded Opening & First Manifestation

## Objective

Prove that progression systems can be introduced through narrative rather than exposed as a complete game UI immediately.

## Opening Slice

Implement only **Accidental Transfer — The Stranded**.

Sequence:

1. Threshold fragments
2. wake in dangerous Greyfen outskirts
3. limited HUD
4. movement and interaction
5. improvised/basic weapon access
6. first physical threat
7. behavior tracking
8. first Skill recognition
9. crisis event
10. adaptive first manifestation
11. route toward Hearthcross

## Adaptive First Manifestation

Prototype candidates may be reduced to three:

- Desperate Parry
- Instinctive Step
- Focused Strike

Selection should respond to player behavior rather than a dialogue menu.

## Exit Criteria

- player can reach first combat without tutorial popup overload
- at least one Skill can be recognized through behavior
- first manifestation feels like the system noticed the player
- Active Codex UI appears as a narrative reveal
- save data retains the recognized Skill and first manifestation

---

# Milestone 4 — Hearthcross Hub & Job Discovery

## Objective

Create the smallest version of Hearthcross that proves towns are character-building spaces rather than vendor menus.

## Required Locations

Block out and implement:

- town gate / arrival
- Adventurer Guild Hall
- Split Anvil
- Lantern House
- Survey Office / Archive Annex
- limited Shrine presence
- limited Underbridge access

## Demo Job Scope

Do not implement the full v0.2.18 roster.

Initial playable Jobs:

- Adventurer
- Scout
- Smith
- Survey Assistant

One semi-hidden Job:

- Smuggler **or** Acolyte, chosen based on production cost

One hidden Job signal:

- Gate Listener qualification progress

## Job Runtime Requirements

- qualification predicates
- qualification progress events
- one Active Job slot
- Job effects
- Job Skills/permissions hooks
- System Comprehension visibility level

## Exit Criteria

- player can qualify for at least two different Jobs through different activities
- active Job changes at least one interaction or passive system result
- Job qualification is not a universal character-creation menu
- hidden qualification feedback can appear without revealing its identity

---

# Milestone 5 — Greyfen Field Slice

## Objective

Connect Hearthcross to meaningful field gameplay and demonstrate world-state consequence.

## Required Content

One compact traversal route containing:

- road
- marsh/forest edge
- optional side path
- one small ruin or abandoned structure
- one goblin encounter area
- Buried Gate staging entrance

## Enemy Scope

Implement only the minimum set needed to demonstrate varied combat:

- Greyfen Goblin Skirmisher
- Goblin Bruiser
- Mirehound

Dungeon vermin may be added only if required for encounter pacing.

## Regional Choice

The goblin scavenger situation must support at least two materially different outcomes, preferably three:

- violence
- negotiation/trade
- withdrawal/alternative resolution

Result changes a small Hearthcross or Greyfen state flag.

## Exit Criteria

- travel feels purposeful rather than empty
- Guardian, Arcanist, and Duelist can all complete the route
- at least one noncombat resolution exists
- world state changes persist after returning to Hearthcross
- one later interaction reflects the decision

---

# Milestone 6 — Three-Discipline Combat Benchmark

## Objective

Add Arcanist and Duelist once the basic runtime has proven Guardian.

## Arcanist

Implement:

- Arc Bolt
- Focused Lance
- Focus Guard
- Sigil Cast
- Arc Step
- Disrupting Pulse
- Threaded Shot
- Attunement

Starter manifestations:

- Ember Rune
- Detonate Sigil
- Mana Thread
- Gravitic Snare
- Arc Lance

## Duelist

Implement:

- Alternating Cuts
- Cross Sever
- Deflect
- Passing Cut
- Rising Fang
- Slipstep
- Reversal Cut
- Flow

Starter manifestations:

- Pursuit
- Perfect Tempo → Tempo Break
- Open Vein
- Echoing Steel
- Sever the Moment

## Exit Criteria

- all three disciplines feel distinct before card use
- all three remain viable solo
- shared states create optional party synergy
- no discipline requires MMO trinity assumptions
- controller and keyboard/mouse remain usable with five-slot Codex

---

# Milestone 7 — The Buried Gate

## Objective

Create the complete dungeon loop and first Story Revelation.

## Dungeon Scope

One short hand-authored dungeon with modest route variation:

- entry / expedition staging
- early combat
- environmental clue
- route choice
- hazard or anomaly
- secure/extract point
- deeper chamber
- Gatebound Hob boss
- true Buried Gate chamber

## Dungeon Systems

Required:

- unsecured loot state
- secure/extract checkpoint
- dungeon Knowledge discovery
- one survey interaction
- one relic/anomaly interaction
- persistent completion state

## Gatebound Hob

Must test:

- blockable heavy attack
- interruptible action
- dodge-required attack
- movement/charge pressure
- vulnerability window
- small add/control moment
- readable co-op telegraphs

## Story Revelation

After victory:

**The Gate recognizes the party in some way, but does not fully open.**

Different System Comprehension levels can receive different presentation detail, but the underlying event remains authoritative.

## Exit Criteria

- dungeon can be entered, completed, extracted from, and revisited
- boss tests all three disciplines without hard countering any one
- secured/unsecured loot distinction is understood
- Gate revelation creates intrigue without explaining the central mystery

---

# Milestone 8 — Persistence & Multiplayer Proof

## Objective

Prove the vertical slice survives session boundaries and basic co-op.

## Character Persistence

Save:

- Origin
- Background subset used by demo
- Skills
- Discipline
- Job unlocks / Active Job
- Codex cards
- equipment
- mastery hooks
- secured rewards
- System Comprehension

## Host World Persistence

Save:

- Hearthcross flags
- Greyfen regional choice
- Buried Gate state
- faction/relationship subset
- local Job opportunity changes required by demo

## Multiplayer Rule

**World persistence belongs to the host. Character persistence belongs to each player.**

First shipping proof only requires host + one client.

Architecture must avoid choices that make future 1–6 support impossible.

## Exit Criteria

- two players can enter Hearthcross and Buried Gate together
- host world state determines local reality
- client retains their own persistent character rewards
- leaving and rejoining does not corrupt card zones or inventory
- secured progression survives session termination

---

# Milestone 9 — Demo Polish

## Objective

Turn the functional slice into something external players can understand and evaluate.

## Required Polish

- animation timing pass
- hit reactions
- camera collision
- target readability
- combat VFX readability
- audio feedback
- Codex UI legibility
- damage/status feedback
- interact prompts
- basic settings
- controller support
- save/load UX
- restart/recovery behavior
- performance profiling
- basic accessibility pass

## Explicitly Not Required

Do not block the demo on:

- six-player certification
- all Origins
- full character creator
- companion system
- large town evolution tree
- full crafting
- deep procedural dungeon generation
- final economy
- all Hearthcross Jobs
- advanced multiclassing
- Authorities
- endgame content

---

# Immediate Work Queue

The first implementation sprint should complete tasks in this order:

1. Create UE5 project skeleton and test map.
2. Implement third-person movement/camera/Enhanced Input.
3. Implement server-authoritative health, damage, and basic replication.
4. Implement Guardian Sword/Shield light, heavy, Guard, dodge interaction.
5. Implement one Greyfen melee test enemy.
6. Implement Weak/Solid/Perfect Guard instrumentation.
7. Implement Shield Bash interruption.
8. Implement remaining Guardian Weapon Arts.
9. Establish gameplay tags/data assets needed for Codex work.
10. Begin five-slot Active Codex runtime.

## First Playable Checkpoint

The first checkpoint is deliberately small:

> A host and one client spawn in a greybox arena, move correctly, fight one readable enemy using Sword/Shield, distinguish Guard timing outcomes, interrupt a heavy attack with Shield Bash, take authoritative damage, die/reset, and repeat without desynchronization.

If this is not fun and stable, do not proceed to content production.

## Production Definition of Done

A feature is not complete because its code exists.

For the demo, a feature is complete when:

- it works in normal play
- it works after respawn/reload where relevant
- it works for host and client where relevant
- it communicates its state clearly
- it has basic debug visibility
- it has a known tuning owner/location
- it does not require design knowledge to understand during play

## Scope Gate

Any proposed feature must answer:

**Which current demo milestone requires this?**

If there is no clear answer, backlog it for after the vertical slice.