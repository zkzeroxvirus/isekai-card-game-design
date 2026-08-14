# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, multiclass card pools, skill and equipment mastery, narrative exploration, infinitely scaling dungeon runs, persistent town development, companions, achievements, legendary treasures, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards represent learned techniques, spells, reactions, equipment actions, summons, and other character capabilities.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and environmental interaction happen directly in 3D space; cards determine which abilities are available.
3. **Classes are modular disciplines.** Characters combine class card pools rather than being permanently locked into one class identity.
4. **Mastery changes abilities.** Skills and equipment can improve, branch, and evolve through use, training, accomplishments, and discoveries.
5. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset, while mastery, treasures, achievements, town systems, companions, knowledge, and discoveries persist.
6. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
7. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, equipment evolutions, recipes, and dungeon phenomena reward experimentation.
8. **Knowledge is power.** Bestiary research and world knowledge reveal enemy behavior, weaknesses, loot, recipes, and hidden interactions.
9. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without erasing developed characters.
10. **Multiplayer should feel like visiting another adventurer's world.** World persistence belongs to the host; persistent characters belong to individual players.
11. **The power curve escalates dramatically.** The intended arc moves from vulnerable adventurer to specialized veteran to legendary system-breaking build.
12. **Isekai progression fantasy is the tone.** The player should feel as though they are learning and eventually exploiting the hidden rules of a new fantasy world.

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

### World & Technical Systems

- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine direction, 1–6 player listen-server co-op, world/character ownership, 3D card abilities, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) — versioned design changes.

## Current design version

**v0.2.5 — Digital World & Multiplayer Direction**

The game is now provisionally defined as a **third-person 3D PC action-RPG/deckbuilder** with narrative travel, player-hosted 1–6 player cooperative worlds, server-authoritative gameplay, and persistent player characters.

**Unreal Engine 5** is the provisional engine choice pending a small networking/combat validation prototype.

Numerical values marked **Prototype Default** remain testing assumptions rather than locked balance targets.

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their persistent world and up to five other players may join with their own characters. Visiting players participate in the host's narrative and dungeon state without replacing their own world state. Secured character rewards and personal progression travel back with them.

Initial multiplayer uses player-hosted listen servers. The architecture should remain compatible with dedicated servers later.

## Power Curve

The intended long-form character fantasy is:

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

Early enemies should be dangerous and resources meaningful. Midgame should open multiclassing, equipment evolution, crafting, companions, and increasingly elaborate engines. Endgame should reward extreme specialization, rare classes, legendary equipment, treasures, summons, unusual interactions, and mastery of hidden systems.

## Design status labels

- **Core Rule** — foundational unless deliberately changed in a patch.
- **Prototype Default** — chosen so the game can be tested; expected to change.
- **Content Guideline** — direction for future card/content design.
- **Technical Direction** — intended implementation architecture that remains subject to prototype validation.
- **Open Question** — intentionally unresolved.

## Next prototype target — Technical Proof of Concept

Before the full combat-content vertical slice, validate the central digital premise with a small Unreal prototype containing:

- third-person movement
- listen-server hosting
- 1–6 player connection support
- one replicated enemy type
- one combat arena
- five test cards
- replicated hand/deck/discard state
- one melee Technique
- one projectile Spell
- one defensive Reaction
- one status effect
- one cross-player combo
- one loot pickup
- one secure/extract checkpoint
- save/reload
- join-in-progress

The goal is to prove that **3D action, deck constraints, replication, persistence, and co-op are coherent together** before scaling content production.

## Following gameplay target — v0.3.0 Combat Prototype

Once the technical proof is sound, the first content vertical slice should support:

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
