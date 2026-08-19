# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven combat, a soul-bound Divine Codex, Skills, modular Disciplines, location-based Jobs, hidden progression, equipment mastery, living-world consequences, civilian life, economy, reputation, settlement development, narrative discovery, dungeons, and online co-op.

## Core design pillars

1. **Build a character, not just a deck.** Character identity comes from Origin, Background, Skills, Jobs, weapons, Disciplines, equipment, mastery, titles, knowledge, relationships, reputation, and world history.
2. **The deck defines capability; the player controls execution.** Movement, aiming, positioning, dodging, traversal, and interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**
4. **Cards are manifestations of the soul.** The Active Codex represents permitted interactions with the laws of the world.
5. **Skills are broader than cards.** They affect combat, crafting, survival, exploration, social interaction, professions, qualification, and perception.
6. **Jobs describe recognized roles; Disciplines describe combat frameworks.**
7. **Visible progression tells the player what they can pursue. Hidden progression rewards the person they accidentally became.**
8. **New places expand the character-build space.** Jobs are embedded in institutions, cultures, environments, activities, professions, and secrets rather than a universal catalogue.
9. **Settlement growth increases depth before breadth.** A settlement gets better at what it already is rather than becoming a universal progression hub.
10. **The world remembers.** Choices, faction outcomes, settlement state, reputation evidence, legal status, and consequences persist.
11. **Reputation is not morality.** What happened, what people know, and what people believe can differ.
12. **The world should function without the player.** Economy, trade, work, construction, faction projects, and social networks continue to create opportunities and consequences.
13. **Every profession participates in the same world.** Crafting, medicine, trade, construction, and ordinary work should connect to shared resources, Skills, Jobs, NPCs, and settlements rather than isolated minigames.
14. **Morality emerges from behavior.** The game supports heroic, villainous, pragmatic, revolutionary, mercantile, civic, criminal, tyrannical, and mixed paths without a universal Good/Evil meter.
15. **Discovery is progression.** Hidden Jobs, Skills, Discipline nodes, manifestations, equipment evolutions, lore, and system information reward experimentation.
16. **Multiclassing should create integrated identities, not larger piles of unrelated abilities.**
17. **Magic should shape the battlefield, not merely replace arrows with colored projectiles.**
18. **Failure creates consequences and stories without deleting developed characters.**
19. **The gods do not necessarily own the system.** The Divine Codex, Transference, Dungeon Laws, and Authorities point toward deeper architecture.
20. **Isekai progression fantasy is the tone.** The player begins vulnerable, learns the world's hidden rules, establishes a place in society, and eventually becomes capable of exploiting rules that once constrained them.
21. **Complexity must remain legible.** New mechanics should fit existing player-facing systems unless they have a compelling reason to become a new major system.

## Current design version

**v0.2.21 — Society, Economy & Reputation Refactor**

The project still uses six player-facing domains:

1. **Character** — Origin, Background, Attributes, Skills
2. **Combat Build** — Weapon, Discipline, Development Grid, Divine Codex
3. **Role** — Jobs
4. **Gear** — Equipment, mastery, evolution
5. **Discovery** — Knowledge, hidden qualifications, System Comprehension
6. **World** — relationships, reputation, factions, economy, citizenship, property, settlements, narrative consequences

Civilian life is explicitly **not** a seventh progression domain. It is how the player participates in the World using Skills, Jobs, money, relationships, legal status, and choices.

See:

- [`docs/SOCIETY_ECONOMY_AND_REPUTATION.md`](docs/SOCIETY_ECONOMY_AND_REPUTATION.md)
- [`docs/COHESIVE_PROGRESSION_ARCHITECTURE.md`](docs/COHESIVE_PROGRESSION_ARCHITECTURE.md)
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md)
- [`docs/TOWN.md`](docs/TOWN.md)
- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md)

## Project Essence

The target experience is:

> **A choose-your-adventure life inside a complex fantasy world where the player arrives vulnerable, discovers how the world works, builds an identity through actions, establishes relationships and a place in society, and eventually becomes capable of exploiting rules that once constrained them.**

The game should capture the emotional progression of isekai fantasy without requiring a rigid hero narrative.

The player may become an adventurer, specialist, merchant, scholar, criminal, protector, artisan, physician, landholder, tyrant, explorer, religious figure, system researcher, or something the world has no ordinary name for.

Character history should emerge from what the player does rather than only from what they select during character creation.

## Cohesive Progression Architecture

The principal conventional point-spending system is the **Discipline Development Grid**.

Character Levels and selected major accomplishments grant **Development Points**, which are primarily spent on compact Discipline specialization grids. Mature grids may contain roughly 20–35 meaningful nodes; the vertical slice should test only about 6–10 nodes per Discipline.

Skills, Jobs, Gear, civilian reputation, legal status, property, and hidden progression do not duplicate the Development Point system.

Key model:

> **Skills determine capability. Jobs recognize role. Reputation records track record. The World provides opportunity.**

## Living Society Model

Settlements may track compact world-state categories such as:

- Food
- Raw Materials
- Crafted Goods
- Medicine
- Labor
- Housing
- Trade Access
- Security
- Prosperity

These variables can affect shop stock, prices, work opportunities, construction, migration, faction projects, shortages, and narrative events.

The economy exists to generate understandable stories and consequences rather than exhaustive commodity simulation.

### Reputation

Reputation has three primary scales:

- **Personal Reputation** — what individual NPCs know and remember
- **Group Reputation** — what factions, settlements, guilds, professions, churches, clans, and networks think
- **Public Reputation** — what broader society has heard or believes

The world distinguishes **what happened** from **what people know or believe happened**.

Witnesses, evidence, records, rumors, social networks, factions, merchants, clergy, and criminal contacts can propagate information.

### Citizenship and Property

Characters can progress socially from outsider toward recognized resident, citizen, licensed professional, landholder, or business owner where local law allows.

Legal status can affect property rights, training, guild access, licenses, taxes, civic participation, weapon rights, Jobs, and legal protections.

Construction uses defined plots, renovations, civic projects, or frontier claims by default rather than unrestricted survival-game free-building.

### Professions

Profession-oriented Jobs should eventually support recognizable work.

Examples:

- Smiths repair and forge equipment for customers.
- Medics treat patients and work clinics.
- Merchants procure goods and organize trade.
- Surveyors map routes and sell information.
- Hunters supply meat, hides, and monster materials.
- Cooks work kitchens, inns, camps, and catering.

Ordinary work can lead to money, Skills, Job qualification, relationships, rumors, reputation, hidden progression, and adventure hooks.

## Playable Demo Scope

Broad feature expansion remains paused while the current systems are developed into one focused vertical slice.

The active implementation target is:

**The Stranded → Hearthcross → Greyfen March → The Buried Gate → Gatebound Hob → Gate Recognition → persistent return to Hearthcross**

The first vertical slice should let a player:

1. create a lightweight character and choose a Background
2. begin as **Accidental Transfer — The Stranded**
3. survive a low-information wilderness opening
4. acquire a first Skill through actual behavior
5. experience an adaptive first Codex manifestation
6. reach Hearthcross
7. interact with at least two distinct businesses
8. take one small civilian work opportunity
9. gain one legal-status step or registration outcome
10. learn one of three prototype combat Disciplines
11. make a small number of meaningful Discipline Development Grid choices
12. discover and activate one frontier Job
13. experience one reputation consequence based on reliability, professionalism, or social behavior
14. resolve one Greyfen conflict with a persistent consequence
15. enter The Buried Gate
16. experience route choice, unsecured loot, securing/extraction, and Job/Skill interactions
17. defeat the Gatebound Hob
18. witness the first Gate recognition Story Revelation
19. return to a Hearthcross that acknowledges what happened

Target first complete playthrough remains roughly **60–120 minutes**. Civilian systems must remain lightweight enough that they enrich the slice rather than delay the first dungeon excessively.

## Demo Combat Triangle

### Guardian — Arming Sword & Shield

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

Prototype Development Grid directions:

- Bulwark
- Vanguard
- Oathkeeper

### Arcanist — Channeling Staff & Arcane Focus

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

Prototype Development Grid directions:

- Sigilcraft
- Threading
- Battle Focus

### Duelist — Twin Blades

**Read opening → Slipstep/angle change → build Flow → create or exploit vulnerability → commit finisher → disengage before greed is punished.**

Prototype Development Grid directions:

- Tempo
- Predation
- Reversal

## Demo Jobs

Openly discoverable:

- **Adventurer**
- **Scout**
- **Smith**
- **Field Medic**
- **Survey Assistant**

Semi-hidden:

- **Smuggler**

Dungeon/activity discovery:

- **Dungeon Surveyor**

Hidden progression:

- one fully attainable hidden Job, likely **Oathbearer** or **Gate Listener**
- the other may appear only as hidden qualification feedback in the first build

The rule remains:

**Locations create opportunities. Actions create qualifications. The Codex recognizes the result.**

## Hearthcross

Hearthcross is a compact frontier settlement, not a city-sized content map.

Required demo spaces:

- town gate / Warden checkpoint
- Adventurer Guild Hall
- Split Anvil
- Lantern House
- Survey Office / Archive Annex
- Shrine of the Returning Flame
- Underbridge access point

Its growth remains governed by:

**Settlement growth increases depth before breadth.**

Civilian proof for the first build should be intentionally small:

- two distinct shops
- one ordinary work opportunity
- one reliability or quality consequence
- one named NPC memory
- one propagated reputation event
- one legal-status step
- one economic variable affecting stock, price, or work
- one Job/Skill changing a civilian interaction

Full property ownership, business management, taxation, and large-scale economic simulation remain deferred.

## Greyfen March

The demo includes one dense field route rather than a large open world.

The principal regional choice centers on a Greyfen goblin scavenger conflict. The player may kill, displace, negotiate, trade, investigate the actual cause, or cooperate covertly depending on circumstances.

A reduced world-state set should track consequences such as:

- Warden Trust
- Underbridge Influence
- Goblin Relations
- Road Safety
- one economy-facing variable such as Medicine Supply or Trade Access if useful

At least one later interaction must visibly change because of the player's decision.

## The Buried Gate

The demo dungeon should include:

- entry/staging
- first combat
- route split
- hazard or observation space
- world-state/goblin callback
- secure/extraction checkpoint
- anomaly room
- pressure or elite encounter
- Gatebound Hob
- true Gate chamber

The dungeon must prove combat, exploration, Knowledge, extraction, Jobs, world-state callbacks, and narrative mystery in the same space.

## Persistence

The demo should save at minimum:

- Background
- acquired Skills
- chosen Discipline
- Discipline Development Grid investment
- Codex manifestations
- equipment/mastery progress
- known and active Jobs
- at least one relevant NPC memory / reputation result
- legal registration/status result
- Greyfen contract outcome
- reduced faction/world-state variables
- Buried Gate completion
- Story Revelation flag
- secured loot

## Multiplayer Direction

The final game target remains **1–6 player online co-op**, with host-owned world state and player-owned character state.

Host-world state includes local NPC memories, economy, citizenship, property, businesses, legal investigations, and settlement development.

Player-owned portable state includes Skills, Jobs, Gear, Codex, and appropriate broader recognitions where fictionally valid.

## Demo Production Rule

**Do not add a new major system until the vertical slice demonstrates that the existing systems are fun together.**

New ideas can be recorded as backlog material, but implementation priority remains the Hearthcross vertical slice.

## Repository map

### Demo & Evaluation

- [`docs/PLAYABLE_DEMO_SCOPE.md`](docs/PLAYABLE_DEMO_SCOPE.md)
- [`docs/ISEKAI_GAME_QUALITY_CHECKLIST.md`](docs/ISEKAI_GAME_QUALITY_CHECKLIST.md)

### Core Rules & Combat

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md)
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md)
- [`docs/MECHANICS.md`](docs/MECHANICS.md)
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md)
- [`docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md`](docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md)
- [`docs/SECOND_COMBAT_PACKAGE_ARCANIST.md`](docs/SECOND_COMBAT_PACKAGE_ARCANIST.md)
- [`docs/THIRD_COMBAT_PACKAGE_DUELIST.md`](docs/THIRD_COMBAT_PACKAGE_DUELIST.md)

### Character & Progression

- [`docs/COHESIVE_PROGRESSION_ARCHITECTURE.md`](docs/COHESIVE_PROGRESSION_ARCHITECTURE.md)
- [`docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md`](docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md)
- [`docs/STARTING_ORIGINS_AND_OPENINGS.md`](docs/STARTING_ORIGINS_AND_OPENINGS.md)
- [`docs/JOBS_MULTICLASS_AND_HIDDEN_PROGRESSION.md`](docs/JOBS_MULTICLASS_AND_HIDDEN_PROGRESSION.md)
- [`docs/HEARTHCROSS_JOB_ECOSYSTEM.md`](docs/HEARTHCROSS_JOB_ECOSYSTEM.md)
- [`docs/PROGRESSION.md`](docs/PROGRESSION.md)
- [`docs/SKILL_MASTERY.md`](docs/SKILL_MASTERY.md)
- [`docs/EQUIPMENT_PROGRESSION.md`](docs/EQUIPMENT_PROGRESSION.md)
- [`docs/GUILD_AND_RANK.md`](docs/GUILD_AND_RANK.md)
- [`docs/COMPANIONS.md`](docs/COMPANIONS.md)
- [`docs/KNOWLEDGE_AND_DEFEAT.md`](docs/KNOWLEDGE_AND_DEFEAT.md)

### Society, World & Narrative

- [`docs/SOCIETY_ECONOMY_AND_REPUTATION.md`](docs/SOCIETY_ECONOMY_AND_REPUTATION.md)
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md)
- [`docs/TOWN.md`](docs/TOWN.md)
- [`docs/DIVINE_CODEX_LORE.md`](docs/DIVINE_CODEX_LORE.md)
- [`docs/NARRATIVE_STRUCTURE.md`](docs/NARRATIVE_STRUCTURE.md)
- [`docs/FIRST_REGION_AND_DUNGEON.md`](docs/FIRST_REGION_AND_DUNGEON.md)
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md)

### Visual & Technical

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md)
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md)
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md)
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md)
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/)

## Immediate implementation milestones

1. **Movement & Combat Sandbox** — third-person controller, one enemy, all three weapon packages, Weapon Arts, hit/defense authority.
2. **Codex Combat** — five hand slots, draw/use/discard/cycle, Resolve/Attunement/Flow, Sigils, transformed-card flow.
3. **Opening + Hearthcross** — Stranded prologue, first Skill, first manifestation, compact hub, basic commerce, one work opportunity, legal registration, one reputation memory, Discipline, small Development Grid, and Job onboarding.
4. **Greyfen Field Slice** — route, goblin choice, persistent consequence, Job/Skill interactions, one world/economy callback.
5. **Buried Gate** — route split, extraction checkpoint, encounters, Gatebound Hob, Gate revelation.
6. **Persistence + Multiplayer Proof** — save/reload, host state, player state, host + one client.
7. **Demo Polish & Checklist Pass** — onboarding, controller pass, VFX readability, audio, performance, bugs, replay hooks, and evaluation against the isekai quality checklist.

## Power Curve

**Vulnerable Outsider → Competent Resident / Adventurer → Synergy-Driven Specialist → Influential World Actor → System-Breaking Legendary Build**

Combat power, social belonging, professional identity, wealth, reputation, and world influence need not increase at the same rate.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
