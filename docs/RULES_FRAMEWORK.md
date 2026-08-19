# Core Rules Framework

Version: **v0.2.21**

## 1. Game Structure

The game is a persistent 3D action-RPG/deckbuilder built around exploration, combat, discovery, civilian life, character development, and consequence.

The macro loop is:

**Explore / Accept Opportunity → Prepare Character & Party → Travel / Work / Enter Dangerous Space → Fight, Discover, Negotiate, Investigate, Trade, Build or Practice → Secure / Retreat / Complete Objective → Resolve Consequences → Develop Character & World → Continue**

Settlements are persistent places rather than abstract menu phases.

Dungeons are important expedition spaces, but the game is not limited to a strict Town → Dungeon → Town roguelite loop.

---

## 2. Player-Facing Progression Domains

The game organizes its many systems into six player-facing domains:

1. **Character** — Origin, Background, Attributes, Skills
2. **Combat Build** — Weapon, Discipline, Development Grid, Divine Codex
3. **Role** — Jobs
4. **Gear** — Equipment, mastery, evolution
5. **Discovery** — Knowledge, hidden qualifications, System Comprehension
6. **World** — relationships, reputation, factions, economy, citizenship, property, settlements, narrative consequences

New mechanics should fit one of these domains whenever possible.

See [`COHESIVE_PROGRESSION_ARCHITECTURE.md`](COHESIVE_PROGRESSION_ARCHITECTURE.md).

---

## 3. Character Structure

A character may contain:

- Origin
- Background
- Attributes
- Health and combat resources
- learned Skills
- known and active Jobs
- Primary and Secondary Disciplines where unlocked
- Discipline Development Grid investment
- equipped weapon set(s)
- Weapon Arts
- Divine Codex deck and current hand
- equipment and equipment mastery/evolution
- rare Treasures
- selected Titles / recognitions
- Knowledge records
- System Comprehension
- relationships
- professional history
- public / group reputation evidence
- legal identity/status where relevant
- persistent unlocks

### Prototype Attributes

- **Might** — physical power, heavy techniques, force
- **Finesse** — precision, agility, speed, ranged and dexterous techniques
- **Mind** — arcane reasoning, spell shaping, analysis
- **Spirit** — willpower, faith, supernatural resilience, soul-facing systems
- **Vitality** — health, endurance, recovery

Attributes should create direction without overpowering synergy, execution, equipment, or discovery.

---

## 4. Real-Time Combat Architecture

Combat is **real-time third-person action combat**.

The three principal action layers are:

### Foundation Actions

Reliable actions that do not depend on card draw:

- move
- camera / aim
- sprint
- dodge
- traversal where appropriate
- interact
- target / lock handling
- contextual universal actions

### Weapon Arts

Reliable combat actions shaped by:

**Weapon Family + Discipline + Equipment Mastery = Weapon Moveset**

### Codex Manifestations

The Divine Codex supplies rotating extraordinary abilities through a five-slot active hand.

Manifestations may include Techniques, Spells, Reactions, Stances, Summons, movement abilities, counters, transformations, buffs/debuffs, utility, miracles, and advanced rule-manipulation effects.

Cards should modify and expand the action combat already underway rather than cause the player to stop playing the action game.

See [`WEAPON_ARTS_COMBAT_LAYERS.md`](WEAPON_ARTS_COMBAT_LAYERS.md).

---

## 5. Discipline System

Disciplines are learned combat frameworks rather than permanent character identities.

A Discipline can provide:

- a combat mechanic or resource
- access to manifestations
- Weapon Art modifications
- specialization branches
- passive/behavioral rules
- mastery recognition
- multiclass bridges
- hidden qualifications

Prototype Disciplines:

- Guardian
- Arcanist
- Duelist

Prototype direction supports **Primary + Secondary Discipline** after multiclassing becomes available.

Multiclassing should create integrated identities rather than simply enlarging the ability pool.

---

## 6. Discipline Development Grid

Development Points are the main conventional point-spending progression currency.

They are primarily used on compact Discipline Development Grids.

A mature Discipline may contain roughly **20–35 meaningful nodes**, though the vertical slice should prototype far fewer.

Node families include Connector, Behavior, Build, Keystone, Bridge, and Hidden Nodes.

Most nodes should alter play or reinforce a strategy rather than only add percentages.

Development Points are not a universal currency for Skills, Jobs, professions, reputation, citizenship, or settlement progression.

---

## 7. Skills

Skills are broad persistent capabilities, not cards and not another giant passive tree.

Examples include:

- Swordsmanship
- Appraisal
- Tracking
- Medicine
- Smithing
- Cooking
- Mana Perception
- Deception
- Fieldcraft

Skills improve primarily through meaningful use, training, study, teachers, discoveries, accomplishments, professional work, and hidden conditions.

Different Skills may branch or evolve, but they should share a consistent mastery language.

---

## 8. Jobs and Professions

Jobs represent roles or identities the world/system recognizes the character as fulfilling.

Jobs are separate from combat Disciplines.

Jobs may provide:

- contextual effects
- Job-related Skills
- permissions
- institutional or social recognition
- professional opportunities
- evolution routes
- hidden qualification access

Jobs are rooted in places, cultures, institutions, activities, environments, professions, and secrets.

The rule is:

**Locations create opportunities. Actions create qualifications. The Codex recognizes the result.**

Characters may know multiple Jobs but benefit fully from only a limited number of Active Jobs at once.

A profession-oriented Job should eventually allow the player to perform recognizable work from that profession.

No separate universal profession skill tree or profession-point currency is added.

---

## 9. Divine Codex and Deck Construction

The character may know many manifestations while equipping a smaller combat deck.

Current prototype direction:

- combat deck target: roughly **15–25 manifestations**
- active hand: **5 manifested slots**
- keyboard can map slots to `1–5`
- controller uses fast mapped access with optional radial support

When a manifestation is used, it normally leaves the active slot and a replacement manifests according to deck-cycle rules.

Deck cycling should be tested as a primary source of extraordinary-ability tempo, reducing reliance on traditional cooldown bars.

The Codex is a build-construction system; it does not require a separate giant passive tree.

---

## 10. Card / Manifestation Zones

Keep zones as simple as possible.

Core zones:

- **Deck** — manifestations waiting to enter the active hand
- **Active Hand** — the five currently available manifestations
- **Discard / Memory** — used manifestations waiting to circulate back
- **Exhaust / Sealed** — manifestations temporarily inaccessible under explicit rules

Additional zones should only be added when a mechanic genuinely requires them.

---

## 11. Manifestation Resolution

A manifestation generally resolves through real-time gameplay:

1. Player activates a hand slot.
2. Targeting mode is established if required.
3. Legality, cost, state, and interruption rules are checked.
4. Animation / cast / movement commitment begins.
5. Gameplay effects resolve at defined timing points.
6. Reactions, statuses, damage, movement, summons, or world interactions resolve server-authoritatively.
7. The manifestation moves to its destination state and the hand slot updates.

Supported targeting families should remain standardized where possible:

- Instant
- Current Target
- Aim / Projectile
- Ground Target
- Directional
- Area Around Self
- Channel
- Contextual Reaction

---

## 12. Discipline Resources

Prototype Disciplines currently use distinct combat resources or rhythm mechanics:

- Guardian — **Resolve**
- Arcanist — **Attunement**
- Duelist — **Flow**

These resources should reinforce each Discipline's playstyle rather than exist simply because every class needs a meter.

---

## 13. Equipment

Equipment is active progression, not only a stat container.

Equipment may:

- alter Weapon Arts
- grant or modify manifestations
- gain familiarity/mastery
- gain or modify affixes
- evolve through thematic conditions
- interact with Skills, Jobs, Disciplines, professions, and hidden progression

Equipment progression should share a consistent player-facing mastery language rather than proliferating unrelated XP systems.

---

## 14. Knowledge and System Comprehension

Knowledge records what the character has learned about the world.

System Comprehension controls how clearly deeper system information can be perceived.

Knowledge can reveal creature behavior, materials, factions, laws, markets, dungeon structures, recipes, profession information, and anomaly patterns.

System Comprehension can reveal status information, hidden qualification feedback, compatibility tags, hidden Grid structures, Dungeon Law wording, deeper Codex metadata, and Authority signatures.

These belong to one broader player-facing **Discovery** domain.

---

## 15. Hidden Progression

The game tracks meaningful patterns in player behavior and history.

Hidden qualifications may reference:

- repeated behavior
- mastery
- professional history
- reliability
- narrative decisions
- faction relationships
- reputation
- world state
- equipment use/evolution
- failures and recovery
- system combinations
- deliberate refusals or negative conditions

Hidden progression may reveal Skills, Jobs, Discipline branches, Grid Nodes, Hybrid Manifestations, equipment evolutions, Titles, Treasures, narrative states, and eventually Authorities.

Hidden content should be surprising but interpretable in hindsight.

---

## 16. Achievements, Titles and Treasures

### Achievements

Primarily records of accomplishment and discovery hooks. They are not a central stat ladder.

### Titles

In-world recognitions that may affect presentation, social reactions, events, or hidden qualifications. Only selected Titles should have mechanical effects.

### Treasures

Rare, limited, major rewards.

**Equipment primarily modifies the character. Treasures may modify rules.**

---

## 17. Exploration, Contracts and World Interaction

The player can pursue:

- contracts
- faction requests
- personal opportunities
- exploration
- dungeon expeditions
- crafting/training
- social relationships
- trade
- employment
- profession work
- investigation
- construction
- property
- business
- hidden content

Quests should not be the only source of meaningful play.

Jobs, Skills, relationships, Knowledge, reputation, economy, legal status, and world state should create alternate interactions and outcomes.

---

## 18. Society, Economy and Civilian Life

Civilian life belongs primarily to the **World** domain and reuses existing systems rather than becoming a disconnected life-sim layer.

See [`SOCIETY_ECONOMY_AND_REPUTATION.md`](SOCIETY_ECONOMY_AND_REPUTATION.md).

### Economy

Settlements may track compact economic categories such as Food, Materials, Crafted Goods, Medicine, Labor, Housing, Trade Access, Security, and Prosperity.

Economic state may affect stock, prices, work opportunities, construction, migration, faction projects, shortages, and narrative events.

### Stores

Stores react to supply, demand, proprietor wealth, relationships, legality, faction control, production knowledge, and world state rather than functioning as infinite static inventories.

### Work

Accepted work can create deadlines, quality expectations, supplied materials, and social obligations.

Repeated reliability, efficiency, carelessness, abandonment, discretion, or professionalism contributes to reputation.

### Citizenship and Legal Identity

Legal status can affect property rights, licenses, guild access, legal protection, taxes, training, civic participation, and Jobs.

### Property and Construction

Property and construction use defined places, legal permission, materials, labor, money, Skills, Jobs, and time rather than unrestricted free-building by default.

### Business

Advanced civilian progression may allow shops, workshops, clinics, taverns, warehouses, farms, caravan companies, and other ventures where they fit the setting.

Business ownership should create meaningful decisions while supporting delegation.

---

## 19. Reputation and NPC Memory

Reputation is not one global score and is not morality.

Primary scales:

- **Personal Reputation** — what individual NPCs think and remember
- **Group Reputation** — how institutions, factions, settlements, guilds, professions, clans, and networks regard the player
- **Public Reputation** — what broader society has heard or believes

Reputation derives from evidence such as completed work, missed commitments, crimes, generosity, rudeness, competence, collateral damage, discretion, mercy, brutality, promises, and betrayal.

The game distinguishes **what happened** from **what people know or believe happened**.

Information may propagate through witnesses, official reports, guilds, merchants, family, rumor, faction networks, clergy, criminal contacts, or other setting-appropriate channels.

Crime should require witnesses, evidence, investigation, or information flow rather than omniscient reputation loss.

NPCs may simultaneously fear, respect, trust, dislike, owe, or professionally rely on the player.

---

## 20. Dungeons and Dangerous Spaces

Dungeons support combat, route choice, hazards, discoveries, hidden interactions, extraction decisions, anomalous rules, enemies, bosses, Story Revelations, and sometimes economically valuable resources or profession opportunities.

Scaling should emphasize new combinations, behaviors, rules, and Dungeon Laws rather than pure HP inflation.

---

## 21. Temporary vs Persistent Progression

Persistent character growth is the main progression fantasy.

Temporary expedition effects may include consumables, blessings, anomaly effects, situational modifications, and unsecured loot.

The player should not rebuild an entire temporary character during every expedition.

Persistent systems include Skills, Discipline investment, known manifestations, Jobs, equipment/mastery/evolution, Knowledge, System Comprehension, relationships, reputation evidence, legal/social history, faction/world state, settlement development, and rare Treasures.

---

## 22. Defeat, Retreat and Extraction

Failure should matter without deleting a developed character.

Consequences may include:

- loss of unsecured rewards
- Wounds
- equipment damage
- companion injuries
- contract outcomes
- missed work or deadlines
- reputation consequences
- legal consequences
- faction consequences
- world-state changes

Knowledge, major permanent unlocks, and previously secured progression normally survive.

Retreat should sometimes be a valid strategic decision.

---

## 23. Multiplayer

Target: **1–6 player online co-op**.

Core architecture:

- server-authoritative gameplay
- host-owned world state
- player-owned character progression
- visiting players participate in the host timeline
- host departure ends the initial listen-server session rather than attempting full host migration

Host-world state includes local NPC memories, economy, citizenship, property, business ownership, legal investigations, and settlement development.

Portable character state includes appropriate personal progression such as Skills, Jobs, Gear, Codex, and cross-world recognitions where fictionally valid.

---

## 24. Advanced Rule Manipulation

Covenants / Clauses, Compound Manifestations, Domains / Local Laws, and similar ideas are advanced **Codex Manifestation families**, not new base progression systems.

Authorities sit above ordinary manifestations and represent rare direct permissions over deeper world laws.

---

## 25. Rule Priority

When explicit game rules conflict, use this general hierarchy:

1. Authority or explicitly superior world-law override
2. Explicit encounter / Dungeon Law
3. Explicit manifestation / equipment / Treasure effect
4. Character, Discipline, Job, Skill, legal/world-state passive
5. Keyword rule
6. Core rule

Specific rules override general rules unless a higher-order rule explicitly prevents that override.

---

## 26. Simulation Guardrail

The game aims for a believable reactive world, not exhaustive simulation.

Simulate detail when it creates meaningful player-facing consequence.

Prefer category-level settlement economy, event-driven prices, generated shop stock, named-NPC memory, abstract background populations, visible construction, and profession activities with decisions.

Avoid mandatory daily chores, excessive appointment micromanagement, dozens of currencies, individual budgets for every NPC, and deep business spreadsheets unless a future feature proves they are fun.

---

## 27. Golden Design Rules

**Build a character, not just a deck.**

**The deck defines capability; the player controls execution.**

**Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**

**Locations create opportunities. Actions create qualifications. The Codex recognizes the result.**

**Skills determine capability. Jobs recognize role. Reputation records track record. The World provides opportunity.**

**Levels expand capability. Mastery deepens identity. Knowledge reveals possibilities. Synergies create power.**

**Visible progression tells the player what they can pursue. Hidden progression rewards the person they accidentally became.**

**The world remembers what happened, but people only react to what they know or believe.**

**Every profession participates in the same world rather than existing in its own minigame bubble.**

**Simulate causes deeply enough that consequences feel earned; abstract everything the player does not need to meaningfully understand or influence.**

**Do not add a new major system until the vertical slice demonstrates that the existing systems are fun together.**
