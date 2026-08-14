# Isekai Card Game Design

Design repository for a progression-fantasy deckbuilding dungeon crawler built around customizable characters, multiclass card pools, infinitely scaling dungeon runs, persistent town development, achievements, and legendary treasures.

## Design pillars

1. **Build a character, not just a deck.** Cards represent learned techniques, spells, reactions, equipment actions, summons, and other character capabilities.
2. **Classes are modular disciplines.** Characters combine class card pools rather than being permanently locked into one class identity.
3. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset, while class mastery, treasures, achievements, town systems, and discoveries persist.
4. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
5. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, treasures, recipes, and dungeon phenomena reward experimentation.
6. **Isekai progression fantasy is the tone.** The player should feel as though they are learning and eventually exploiting the hidden rules of a new fantasy world.

## Repository map

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core game loop, character construction, combat, deck construction, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, card anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — core resources, damage, defense, statuses, keyword rules, triggers, and timing language.
- [`docs/PROGRESSION.md`](docs/PROGRESSION.md) — run, character, class mastery, achievement, treasure, and account progression layers.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) — versioned design changes.

## Current design version

**v0.1.0 — Foundation**

This version establishes a playable rules skeleton. Numerical values marked **Prototype Default** are testing assumptions, not locked balance targets.

## Design status labels

- **Core Rule** — foundational unless deliberately changed in a patch.
- **Prototype Default** — chosen so the game can be tested; expected to change.
- **Content Guideline** — direction for future card/content design.
- **Open Question** — intentionally unresolved.

## Near-term prototype target

The first vertical slice should support:

- 1 customizable player character
- 3 base classes
- 2-class multiclassing
- approximately 15 cards per class
- 1 neutral card pool
- 3 normal enemy families
- 3 elites
- 1 boss
- 1 short dungeon run
- temporary card upgrades during a run
- 3 persistent treasures
- 1 hidden class unlock condition
- a minimal town containing Guild, Training Hall, Blacksmith, and Treasure Vault

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
