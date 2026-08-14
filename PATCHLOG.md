# Design Patch Log

This log records meaningful rules, system, terminology, and balance changes. Prototype defaults may change frequently; core-rule changes should explain the reason and expected design impact.

Version format follows semantic-style design versioning:

- **MAJOR** — foundational redesign or compatibility-breaking rules overhaul
- **MINOR** — new systems, mechanics, card families, classes, or substantial rule additions
- **PATCH** — clarifications, balance changes, wording fixes, and narrow mechanical adjustments

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

### Next Target

**v0.3.0 — Combat Prototype**

Planned focus:

- first 3 base classes
- distinct class resources/mechanics
- approximately 45 class cards
- neutral starter cards
- branching Skill Mastery examples
- equipment families and evolutions
- two companions and Support Decks
- enemy families and Bestiary progression
- elites and first boss
- first Guild advancement test
- complete short dungeon run with extraction and defeat consequences

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

### Known Open Areas

- Final draw model.
- Final Action economy.
- Bleed, Poison, and Stagger implementation.
- Exact defeat/extraction loss rules.
- Final dungeon scaling formula.
- Product format: physical, digital, or hybrid.
- Solo/party/co-op structure.

---

## Unreleased

### Added

### Changed

### Balance

### Fixed / Clarified

### Removed
