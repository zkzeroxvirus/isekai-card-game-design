# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven combat, a soul-bound Divine Codex, Skills, modular Disciplines, location-based Jobs, hidden progression, equipment mastery, living-world consequences, narrative discovery, dungeons, town progression, and online co-op.

## Core design pillars

1. **Build a character, not just a deck.** Character identity comes from Origin, Background, Skills, Jobs, weapons, Disciplines, equipment, mastery, titles, knowledge, relationships, and world history.
2. **The deck defines capability; the player controls execution.** Movement, aiming, positioning, dodging, traversal, and interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**
4. **Cards are manifestations of the soul.** The Active Codex represents permitted interactions with the laws of the world.
5. **Skills are broader than cards.** They affect combat, crafting, survival, exploration, social interaction, class qualification, and perception.
6. **Jobs describe recognized roles; Disciplines describe combat frameworks.**
7. **Visible progression tells the player what they can pursue. Hidden progression rewards the person they accidentally became.**
8. **New places expand the character-build space.** Jobs are embedded in institutions, cultures, environments, activities, and secrets rather than a universal catalogue.
9. **Settlement growth increases depth before breadth.** A settlement gets better at what it already is rather than becoming a universal progression hub.
10. **The world remembers.** Choices, faction outcomes, settlement state, and consequences persist.
11. **Morality emerges from behavior.** The game supports heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths without a universal Good/Evil meter.
12. **Discovery is progression.** Hidden Jobs, Skills, Disciplines, manifestations, equipment evolutions, lore, and system information reward experimentation.
13. **Multiclassing should create integrated identities, not larger piles of unrelated abilities.**
14. **Magic should shape the battlefield, not merely replace arrows with colored projectiles.**
15. **Failure creates consequences and stories without deleting developed characters.**
16. **The gods do not necessarily own the system.** The Divine Codex, Transference, Dungeon Laws, and Authorities point toward deeper architecture.
17. **Isekai progression fantasy is the tone.** The player begins vulnerable, learns the world's hidden rules, and eventually becomes capable of exploiting them.

## Current design version

**v0.2.19 — Playable Demo Scope**

Broad feature expansion is now paused while the current systems are developed into one focused vertical slice.

The active implementation target is:

**The Stranded → Hearthcross → Greyfen March → The Buried Gate → Gatebound Hob → Gate Recognition → persistent return to Hearthcross**

The demo exists to prove that the project's major ideas work **together**, not merely as separate design documents.

See [`docs/PLAYABLE_DEMO_SCOPE.md`](docs/PLAYABLE_DEMO_SCOPE.md).

## Playable Demo Scope

The first vertical slice should let a player:

1. create a lightweight character and choose a Background
2. begin as **Accidental Transfer — The Stranded**
3. survive a low-information wilderness opening
4. acquire a first Skill through actual behavior
5. experience an adaptive first Codex manifestation
6. reach Hearthcross
7. learn one of three prototype combat Disciplines
8. discover and activate one frontier Job
9. resolve one Greyfen conflict with a persistent consequence
10. enter The Buried Gate
11. experience route choice, unsecured loot, securing/extraction, and Job/Skill interactions
12. defeat the Gatebound Hob
13. witness the first Gate recognition Story Revelation
14. return to a Hearthcross that acknowledges what happened

Target first complete playthrough: roughly **60–120 minutes**, with replay value from different Backgrounds, Disciplines, first manifestations, Jobs, choices, and dungeon routes.

## Demo Combat Triangle

### Guardian — Arming Sword & Shield

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

Tests active defense, positioning, protection, stagger, and melee timing.

### Arcanist — Channeling Staff & Arcane Focus

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

Tests ranged aim, ground targeting, magical geometry, control, and status interaction.

### Duelist — Twin Blades

**Read opening → Slipstep/angle change → build Flow → create or exploit vulnerability → commit finisher → disengage before greed is punished.**

Tests mobility, timing, Deflect, angle changes, opening creation, and offensive tempo.

## Demo Jobs

The full Hearthcross ecosystem is larger, but the demo intentionally implements a reduced roster.

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

Hearthcross is a compact frontier hub, not a city-sized content map.

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

## Greyfen March

The demo includes one dense field route rather than a large open world.

The principal regional choice centers on a Greyfen goblin scavenger conflict. The player may kill, displace, negotiate, trade, investigate the actual cause, or cooperate covertly depending on circumstances.

A reduced world-state set should track consequences such as:

- Warden Trust
- Underbridge Influence
- Goblin Relations
- Road Safety

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

## First Story Revelation

After the Gatebound Hob:

**The Buried Gate recognizes the character or party, but does not fully open.**

Different System Comprehension levels should present different amounts of information without explaining the central mystery.

## Persistence

The demo should save at minimum:

- Background
- acquired Skills
- chosen Discipline
- Codex manifestations
- equipment/mastery progress
- known and active Jobs
- Greyfen contract outcome
- reduced faction/world-state variables
- Buried Gate completion
- Story Revelation flag
- secured loot

Returning to Hearthcross after reload should visibly acknowledge at least one earlier decision.

## Multiplayer Direction

The final game target remains **1–6 player online co-op**, with host-owned world state and player-owned character state.

For the first demo implementation:

1. build server-authoritative gameplay from the start
2. prove host + one client first
3. scale the same slice toward 1–4 players as a stretch target
4. preserve architecture compatible with eventual 1–6 play

Full multiplayer scale must not block getting the single-player/host experience fun.

## Demo Production Rule

**Do not add a new major system until the vertical slice demonstrates that the existing systems are fun together.**

New ideas can be recorded as backlog material, but implementation priority remains the Hearthcross vertical slice.

## Repository map

### Demo

- [`docs/PLAYABLE_DEMO_SCOPE.md`](docs/PLAYABLE_DEMO_SCOPE.md) — frozen vertical-slice scope, milestones, content requirements, deferred systems, and success criteria.

### Core Rules & Combat

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md)
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md)
- [`docs/MECHANICS.md`](docs/MECHANICS.md)
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md)
- [`docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md`](docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md)
- [`docs/SECOND_COMBAT_PACKAGE_ARCANIST.md`](docs/SECOND_COMBAT_PACKAGE_ARCANIST.md)
- [`docs/THIRD_COMBAT_PACKAGE_DUELIST.md`](docs/THIRD_COMBAT_PACKAGE_DUELIST.md)

### Character & Progression

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

### Lore, World & Narrative

- [`docs/DIVINE_CODEX_LORE.md`](docs/DIVINE_CODEX_LORE.md)
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md)
- [`docs/NARRATIVE_STRUCTURE.md`](docs/NARRATIVE_STRUCTURE.md)
- [`docs/FIRST_REGION_AND_DUNGEON.md`](docs/FIRST_REGION_AND_DUNGEON.md)
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md)
- [`docs/TOWN.md`](docs/TOWN.md)

### Visual & Technical

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md)
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md)
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md)
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md)
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/)

## Immediate implementation milestones

1. **Movement & Combat Sandbox** — third-person controller, one enemy, all three weapon packages, Weapon Arts, hit/defense authority.
2. **Codex Combat** — five hand slots, draw/use/discard/cycle, Resolve/Attunement/Flow, Sigils, transformed-card flow.
3. **Opening + Hearthcross** — Stranded prologue, first Skill, first manifestation, compact hub, Discipline and Job onboarding.
4. **Greyfen Field Slice** — route, goblin choice, persistent consequence, Job/Skill interactions.
5. **Buried Gate** — route split, extraction checkpoint, encounters, Gatebound Hob, Gate revelation.
6. **Persistence + Multiplayer Proof** — save/reload, host state, player state, host + one client.
7. **Demo Polish** — onboarding, controller pass, VFX readability, audio, performance, bugs, replay hooks.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

The demo covers only the earliest portion of that curve while clearly showing the systems that can later support the rest.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.