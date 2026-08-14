# Isekai Card Game Design

Design repository for a progression-fantasy deckbuilding dungeon crawler built around customizable characters, multiclass card pools, skill and equipment mastery, infinitely scaling dungeon runs, persistent town development, companions, achievements, and legendary treasures.

## Design pillars

1. **Build a character, not just a deck.** Cards represent learned techniques, spells, reactions, equipment actions, summons, and other character capabilities.
2. **Classes are modular disciplines.** Characters combine class card pools rather than being permanently locked into one class identity.
3. **Mastery changes abilities.** Skills and equipment can improve, branch, and evolve through use, training, accomplishments, and discoveries.
4. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset, while mastery, treasures, achievements, town systems, companions, knowledge, and discoveries persist.
5. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
6. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, equipment evolutions, recipes, and dungeon phenomena reward experimentation.
7. **Knowledge is power.** Bestiary research and world knowledge reveal enemy behavior, weaknesses, loot, recipes, and hidden interactions.
8. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without erasing developed characters.
9. **The power curve escalates dramatically.** The intended arc moves from vulnerable adventurer to specialized veteran to legendary system-breaking build.
10. **Isekai progression fantasy is the tone.** The player should feel as though they are learning and eventually exploiting the hidden rules of a new fantasy world.

## Repository map

### Core Rules

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core game loop, character construction, combat, deck construction, party structure, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, card anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — core resources, damage, defense, statuses, keyword rules, triggers, and timing language.

### Progression Systems

- [`docs/PROGRESSION.md`](docs/PROGRESSION.md) — master progression model and long-term power arc.
- [`docs/SKILL_MASTERY.md`](docs/SKILL_MASTERY.md) — persistent skill use, mastery tiers, branching upgrades, and hidden evolutions.
- [`docs/EQUIPMENT_PROGRESSION.md`](docs/EQUIPMENT_PROGRESSION.md) — equipment mastery, learned techniques, affixes, crafting, and item evolution.
- [`docs/GUILD_AND_RANK.md`](docs/GUILD_AND_RANK.md) — Adventurer Guild contracts, reputation, certifications, and institutional rank.
- [`docs/COMPANIONS.md`](docs/COMPANIONS.md) — companion Support Decks, party roles, recruitment, progression, injuries, and solo alternatives.
- [`docs/KNOWLEDGE_AND_DEFEAT.md`](docs/KNOWLEDGE_AND_DEFEAT.md) — Bestiary progression, world knowledge, wounds, secured loot, extraction, and recovery runs.

### World Systems

- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) — versioned design changes.

## Current design version

**v0.2.0 — Isekai Progression Framework**

The project now has a formal progression architecture covering ability mastery, equipment growth, Guild status, companions, persistent knowledge, and meaningful-but-recoverable failure.

Numerical values marked **Prototype Default** remain testing assumptions rather than locked balance targets.

## Power Curve

The intended long-form character fantasy is:

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

Early enemies should be dangerous and resources meaningful. Midgame should open multiclassing, equipment evolution, crafting, companions, and increasingly elaborate engines. Endgame should reward extreme specialization, rare classes, legendary equipment, treasures, summons, unusual interactions, and mastery of hidden systems.

## Design status labels

- **Core Rule** — foundational unless deliberately changed in a patch.
- **Prototype Default** — chosen so the game can be tested; expected to change.
- **Content Guideline** — direction for future card/content design.
- **Open Question** — intentionally unresolved.

## Near-term prototype target — v0.3.0 Combat Prototype

The first vertical slice should support:

- 1 customizable player character
- 3 base classes with distinct class mechanics
- 2-class multiclassing
- approximately 15 cards per class
- branching mastery examples for several skills
- 1 neutral card pool
- 2 equipment families with mastery/evolution examples
- 2 prototype companions with Support Decks
- 3 normal enemy families with Bestiary discovery states
- 3 elites
- 1 boss
- 1 short dungeon run
- temporary card upgrades during a run
- 3 persistent treasures
- 1 hidden class unlock condition
- 1 Guild Rank advancement test
- wounds, equipment damage, secured/unsecured loot, and extraction
- a minimal town containing Guild, Training Hall, Blacksmith, Library, and Treasure Vault

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
