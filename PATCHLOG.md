# Design Patch Log

This log records meaningful rules, system, terminology, technical-direction, and balance changes. Prototype defaults may change frequently; core-rule changes should explain the reason and expected design impact.

Version format follows semantic-style design versioning:

- **MAJOR** — foundational redesign or compatibility-breaking rules overhaul
- **MINOR** — new systems, mechanics, card families, classes, or substantial rule additions
- **PATCH / interim milestone** — clarifications, technical direction, balance changes, wording fixes, and narrow mechanical adjustments

---

## v0.2.5 — Digital World & Multiplayer Direction — 2026-08-13

### Product Direction

- Reframed the project as a **third-person 3D PC action-RPG/deckbuilder** rather than a purely card/tabletop-style game.
- Established narrative exploration, travel events, instanced dungeons, persistent host worlds, and online cooperative play as core digital-product goals.
- Added the principle: **The deck defines capability; the player controls execution.**
- Basic movement, positioning, aiming, traversal, dodging, and environmental interaction are direct 3D actions rather than card-driven movement.

### Engine Direction

- Selected **Unreal Engine 5** as the provisional engine choice pending technical prototype validation.
- Established a hybrid architecture using C++ for authoritative gameplay/state systems and Blueprint/data-driven content for presentation and rapid content iteration.
- Identified Unreal's Gameplay Ability System as a candidate execution layer for replicated card abilities, effects, tags, costs, statuses, and activation rules.

### Added — Multiplayer Architecture

- Established **1–6 players per world session** as the target multiplayer range.
- Initial topology uses a **player-hosted listen server**.
- The host acts as the authoritative simulation while also playing.
- Architecture should remain compatible with a future dedicated-server mode.
- Solo play remains first-class and should use the same authoritative gameplay rules path where practical.

### Added — Ownership Model

Established the persistence rule:

**World persistence belongs to the host. Character persistence belongs to each player.**

Host-owned state includes:

- narrative decisions
- faction outcomes
- town upgrades
- region unlocks
- NPC state
- host-world quests
- world discoveries
- persistent environmental consequences

Player-owned state includes:

- character progression
- classes
- skill mastery
- cards
- equipment
- equipment mastery
- treasures
- titles
- achievements
- portable companion progression where allowed

Joining another player's world does not overwrite the visitor's personal world state.

### Added — Drop-In / Drop-Out Sessions

- Added join-in-progress as a design goal.
- Defined prototype safe join points: Town, Guild Hall, Camp, Dungeon Staging Area, and completed encounter boundaries.
- Sensitive boss phases and narrative cinematics may temporarily restrict joining.
- Secured personal progression should save at authoritative checkpoints.
- Unsecured expedition rewards remain governed by extraction rules.

### Added — Host Loss Policy

- Seamless host migration is not required for the first implementation.
- If the host leaves or the session is lost, the active world session ends.
- Players keep already-secured progression.
- Unsecured expedition state may revert to the latest valid checkpoint.
- Future options include resumable session snapshots, elected-host migration, cloud hosting, and dedicated persistent worlds.

### Added — Server Authority Rules

Gameplay-critical state is server authoritative, including:

- card zones and hand state
- resources
- damage/healing
- statuses
- inventory mutations
- loot ownership
- mastery gains
- enemy state
- dungeon objectives
- narrative/world flags

Clients request actions; the authority validates and executes them.

### Added — Card-to-3D Ability Model

Separated card data from executable 3D abilities.

Cards define:

- identity
- class/source
- tags
- resource costs
- targeting
- range
- timing
- deck behavior
- mastery/evolution links
- ability reference

Executable gameplay abilities define:

- animation
- movement commitment
- targeting execution
- projectiles/traces/areas
- gameplay effects
- replication
- interrupts
- combo windows
- world interaction

### Added — Real-Time Cooperative Combat Direction

- Combat uses direct 3D movement with tactical restrictions created by the player's current hand/deck state.
- Cross-player synergies are encouraged.
- Standard content should not require strict MMO Tank/Healer/DPS compositions.
- Encounter scaling across 1–6 players should use enemy composition, mechanics, reinforcement timing, hazards, and target pressure rather than relying primarily on HP multiplication.

### Added — Narrative & Travel Integration

- Persistent narrative state belongs to the host world.
- Character builds may act as narrative keys through Origins, Classes, Skills, Equipment, Treasures, Titles, Guild Rank, Bestiary Knowledge, Companions, factions, and prior decisions.
- Added travel events as active content including ambushes, weather, wounded travelers, monster tracks, faction patrols, shrines, caravans, companion scenes, rare merchants, anomalies, temporary dungeons, discoveries, and narrative choices.

### Added — Instancing Strategy

Preferred world structure:

- persistent host-owned world state
- explorable towns/hubs
- overworld/travel regions
- instanced dungeons
- instanced major narrative encounters
- maximum six-player party/session

The project is explicitly **not dependent on MMO-scale persistent servers**.

### Added — Save Data Boundaries

Defined three persistence domains:

- **Player-Owned Data** — character progression and portable possessions
- **World-Owned Data** — host narrative/world state
- **Session-Owned Data** — temporary run/combat state and unsecured loot

Session data becomes persistent only when explicitly promoted through secure/extract/save rules.

### Technical Risks to Prototype Early

- six-player replicated combat
- deck/hand synchronization under latency
- join/rejoin state transfer
- host save reliability
- ability prediction and perceived latency
- projectile/AoE replication
- high enemy-count performance
- multiplayer companion AI
- dungeon instance transitions
- world-state synchronization
- secured/unsecured reward integrity
- online-service choice such as Steam or EOS

### New Technical Proof-of-Concept Target

Before large-scale card/content production, build a small Unreal multiplayer test containing:

- third-person movement
- listen-server hosting
- 1–6 player connectivity
- one replicated enemy
- one arena
- five cards
- replicated draw/hand/discard state
- one melee Technique
- one projectile Spell
- one defensive Reaction
- one status effect
- one cross-player combo
- one loot pickup
- one extraction checkpoint
- save/reload
- join-in-progress

Success condition: **3D action, card constraints, replication, persistence, and cooperative play feel coherent together.**

### Open Technical Areas

- combat pacing and possible solo time-slow/pause behavior
- baseline dodge/block rules independent of cards
- mouse/keyboard and controller targeting model
- exact travel topology
- Steam vs EOS vs alternative online layer
- anti-cheat and character-save trust model for peer-hosted worlds
- reconnect grace rules
- whether companions consume the six-player party cap
- visitor quest-reward transfer rules
- cross-platform goals
- mod-support goals
- PvP is assumed out of scope unless deliberately added later

---

## v0.2.0 — Isekai Progression Framework — 2026-08-13

### Design Direction

Established the intended long-form power arc:

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

Early progression should emphasize danger, scarcity, learning, and meaningful party/equipment decisions. Midgame should expand skill evolution, equipment growth, crafting, multiclassing, companions, and build engines. Endgame should reward extreme specialization, rare classes, legendary equipment, Treasures, summons, and unusual rule interactions.

### Added — Skill Mastery & Evolution

- Added persistent Skill Mastery distinct from Class Mastery.
- Defined Known Skills versus Mastered Skills.
- Added prototype mastery stages: Learned, Practiced, Refined, Mastered, and Evolved.
- Added branching skill evolution as a primary form of vertical ability progression.
- Added Skill Families for related disciplines and techniques.
- Added thematic evolution conditions referencing combat behavior, achievements, classes, equipment, bosses, materials, and hidden events.
- Added hidden skill evolutions.
- Added anti-grind guardrails so advanced mastery rewards meaningful use rather than trivial repetition.

### Added — Equipment Progression

- Defined equipment as an active progression system rather than a stat container.
- Added Equipment Mastery.
- Added the ability for equipment to teach cards, proficiencies, and permanent skill knowledge.
- Added evolving equipment with thematic conditions and branching outcomes.
- Added weapon families and technique compatibility.
- Added equipment affixes intended to modify build behavior rather than only provide flat stats.
- Added crafting support for repair, sockets, affixes, monster-material binding, awakening, and evolution.
- Established damaged equipment as a normal defeat consequence rather than permanent item destruction.
- Clarified Equipment versus Treasure identity.

### Added — Adventurer Guild & Rank

- Added Guild Rank as persistent institutional progression separate from Character Level.
- Added prototype rank ladder: Tin, Copper, Iron, Steel, Silver, Gold, Mythril, Adamant, Astral.
- Added advancement requirements based on contracts, evaluations, reputation, dungeon accomplishments, certifications, and recommendations.
- Added contract categories including Hunt, Extermination, Escort, Rescue, Exploration, Recovery, Investigation, Suppression, Gathering, Emergency, and Raid.
- Added reputation axes and certifications.
- Established that Guild Rank should primarily unlock opportunities rather than raw combat stats.

### Added — Companions & Party Structure

- Added persistent companions with compact Support Decks.
- Added prototype 0–2 active companion structure.
- Added prototype 4–8 card Support Deck size.
- Added party role vocabulary including Vanguard, Defender, Striker, Healer, Controller, Support, Scout, and Summoner.
- Added companion recruitment, personal progression, equipment, relationships, personal quests, and injury states.
- Established that companions should not require control of multiple full-sized decks.
- Preserved solo builds as a supported alternative through dedicated solo benefits and build paths.
- Clarified Companion versus Summon terminology.

### Added — Knowledge & Bestiary

- Added persistent Knowledge as a progression layer.
- Added Bestiary discovery stages: Unknown, Observed, Studied, Researched.
- Added progressive revelation of enemy health, behavior, weaknesses, resistances, loot, abilities, and hidden interactions.
- Connected Guild reports, Library research, Cartography, scouting, classes, achievements, and combat observation to knowledge gain.
- Added the principle that information precision may improve as enemy knowledge increases.

### Added — Defeat, Extraction & Recovery

- Defined defeat as meaningful loss without normal-mode character deletion.
- Added temporary persistent Wounds.
- Added companion Injuries.
- Added equipment damage.
- Added **Secured** versus **Unsecured** dungeon loot.
- Added extraction as a push-your-luck decision.
- Added retreat as preferable to defeat but less rewarding than successful completion.
- Added Recovery Contracts / Lost Cache events that can turn failed expeditions into future content.
- Reserved permanent character/companion death and destructive loss systems for explicit challenge modes.

### Changed — Core Rules

- Expanded the macro loop to include contracts, parties, knowledge acquisition, extraction, and consequences.
- Character structure now includes Skill Mastery, Equipment Mastery, Guild Rank/certifications, Bestiary knowledge, and companion relationships.
- Classes now explicitly include a class mechanic in addition to cards and passives.
- Equipment may now directly participate in card access and evolution rules.
- Enemy Intent can interact with Bestiary Knowledge.
- Persistent progression now explicitly includes knowledge, companion growth, certifications, and equipment mastery.
- Rules priority now includes Equipment and Treasure passives alongside Character/Class passives.

### New Core Progression Principle

**Levels expand capability. Mastery deepens identity. Knowledge reveals possibilities. Synergies create power.**

### Prototype Defaults Added

- Active companions: 0–2.
- Companion Support Deck: 4–8 cards.
- Skill Mastery prototype stages: 5.
- Bestiary discovery prototype stages: 4.
- Equipment quality vocabulary: Common, Fine, Rare, Epic, Legendary, Mythic.
- Guild Rank names are placeholders pending setting-specific terminology.

---

## v0.1.0 — Foundation — 2026-08-13

### Added

- Established the Town → Character Build → Dungeon Run → Reward → Town macro loop.
- Defined characters as customizable containers for Origins, Attributes, Classes, Decks, Equipment, Treasures, Titles, and persistent unlocks.
- Established classes as modular disciplines rather than permanent character identities.
- Added prototype Primary + Secondary class multiclass structure.
- Added Known Card, Equipped Card, and Run Card distinction.
- Added prototype 15-card minimum deck size and 15–25 card target range.
- Added primary card types: Technique, Spell, Reaction, Stance, Summon, Skill, Item, Ultimate, Curse, Blessing, and Event Card.
- Added card source categories: Class, Hybrid, Neutral, Origin, Equipment, Treasure, Dungeon, Achievement, Title, Monster, Town, and Unique.
- Added functional card taxonomy for offense, defense, control, economy, deck manipulation, engines, summoning, and exploration.
- Established branching card upgrades as a preferred design direction.
- Added card zones: Deck, Hand, Discard, Exhaust, Prepared, In Play, and Sealed.
- Added prototype Action economy, hand-size rules, Guard, and damage-resolution framework.
- Added initial keyword vocabulary including Exhaust, Retain, Prepared, Fleeting, Ethereal, Innate, Generate, Discover, Scry, Draw, Discard, Recycle, Seal, Copy, and Transform.
- Added initial status framework and prototype Burn, Bleed, Poison, Stagger, Weak, Vulnerable, Taunt, Silence, and Root concepts.
- Added standardized trigger vocabulary for future card templating.
- Added secondary-resource design rules and generator/converter/multiplier/payoff/finisher engine framework.
- Established persistent progression layers for character growth, class mastery, equipment, treasures, achievements, titles, town systems, and dungeon depth.
- Defined Treasures as limited-slot persistent rule-changing rewards distinct from normal equipment.
- Added Hidden Class discovery framework.
- Added infinitely scalable dungeon framework based on biomes, enemy families, affixes, boss mutations, hazards, modifiers, and Dungeon Laws.
- Established principle that deep-dungeon difficulty should increasingly come from rules complexity rather than raw numerical inflation.
- Added initial Town building framework including Guild, Training Hall, Blacksmith, Arcanist Tower, Alchemist, Temple, Tavern, Cartographer, Treasure Vault, Marketplace, Monument/Hall of Records, and Library.
- Added controlled terminology glossary.
- Added tracked Open Design Questions for prototype testing.

### Prototype Defaults

- Starting hand: 5 cards.
- Primary turn resource: 3 Action.
- Maximum hand size: 10 cards.
- Deck minimum: 15 cards.
- Recommended deck range: 15–25 cards.
- Maximum normal duplicate count: 2.
- Starting class structure: 1 Primary + 1 Secondary.
- Guard normally expires at the start of its owner's next turn.
- Burn currently deals damage equal to its stacks at its trigger, then loses 1 stack.

### Design Principles Locked for Initial Prototype

- **Build a character, not just a deck.**
- **Classes are modular disciplines.**
- **Runs create temporary power; persistent progression creates possibility.**
- **Depth changes rules, not only numbers.**
- **Discovery is progression.**
- **Levels expand options; synergies create power.**

---

## Unreleased

### Added

### Changed

### Balance

### Fixed / Clarified

### Removed
