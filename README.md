# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, multiclass card pools, skill and equipment mastery, narrative exploration, a persistent living world, infinitely scaling dungeon runs, town development, companions, achievements, legendary treasures, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards represent learned techniques, spells, reactions, equipment actions, summons, and other character capabilities.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and environmental interaction happen directly in 3D space; cards determine which abilities are available.
3. **Cards are manifestations of the soul.** The card interface represents the character's permitted interactions with the laws of the world through a soul-bound Active Codex.
4. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later in the campaign.
5. **Morality emerges from behavior.** The game supports heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths without reducing them to one Good/Evil meter.
6. **The story is discovered, not merely followed.** A central mystery exists, but players uncover it through revelations, exploration, factions, companions, and world state rather than a rigid main-quest chain.
7. **Classes are modular disciplines.** Characters combine class card pools rather than being permanently locked into one class identity.
8. **Mastery changes abilities.** Skills and equipment can improve, branch, and evolve through use, training, accomplishments, and discoveries.
9. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset, while mastery, treasures, achievements, town systems, companions, knowledge, relationships, and discoveries persist.
10. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
11. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, equipment evolutions, recipes, divine permissions, and dungeon phenomena reward experimentation.
12. **Knowledge is power.** Bestiary research and world knowledge reveal enemy behavior, weaknesses, loot, recipes, hidden interactions, and eventually the true nature of game systems.
13. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without erasing developed characters.
14. **Multiplayer should feel like visiting another adventurer's world.** World persistence and timeline belong to the host; persistent characters belong to individual players.
15. **The power curve escalates dramatically.** The intended arc moves from vulnerable adventurer to specialized veteran to legendary system-breaking build.
16. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper metaphysical infrastructure behind the Divine Codex and Transference.
17. **Isekai progression fantasy is the tone.** The player should feel as though they are learning and eventually exploiting the hidden rules of a new fantasy world.

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

### Lore, Narrative & World Systems

- [`docs/DIVINE_CODEX_LORE.md`](docs/DIVINE_CODEX_LORE.md) — Divine Codex, Transference, soul manifestations, gods, Authorities, native/otherworlder perception, and the central metaphysical mystery.
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md) — world time, faction reputation, behavioral tendencies, consequence records, faction projects, evolving settlements, world eras, and hero/villain paths.
- [`docs/NARRATIVE_STRUCTURE.md`](docs/NARRATIVE_STRUCTURE.md) — Core Mystery, regional storylines, companion arcs, emergent world stories, player campaign history, Story Revelations, and era-based narrative escalation.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.

### Technical Systems

- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine direction, 1–6 player listen-server co-op, world/character ownership, 3D card abilities, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) — versioned design changes.

## Current design version

**v0.2.8 — Narrative Structure**

The project now uses a **sandbox-first living world with a discoverable core mystery**.

Narrative is organized into five layers:

1. **Core Mystery** — the truth behind Transference, the Divine Codex, Authorities, Dungeon Laws, the gods, and the Endless Dungeon.
2. **Regional Storylines** — political, social, religious, monster, economic, and magical conflicts that can resolve differently or continue without the player.
3. **Character & Companion Arcs** — persistent personal stories shaped by relationships, world state, behavior, factions, and time.
4. **Emergent World Stories** — consequences created by simulation and interacting world-state systems.
5. **Player Campaign History** — the unique combination of all of the above plus the player's own goals and decisions.

The Core Mystery advances primarily through **Story Revelations** rather than a rigid main-quest chain. The player should feel that they are discovering the plot.

There is no permanent global apocalypse timer forcing continuous main-story engagement. Regional crises and faction projects may advance or resolve with time, while the deeper Core Mystery escalates through World Era, discoveries, major world transitions, and deliberate engagement.

## Narrative Escalation

The provisional campaign eras are:

**Arrival → Adventurer → Heroic → Sovereign → Mythic**

Narrative scale rises with the player's influence:

**Personal survival → regional conflicts → major faction/divine attention → nations and system control → gods, Authorities, Transference, and world laws.**

The Core Mystery does not assume a heroic protagonist. Characters may seek the truth to protect the world, gain power, overthrow gods, preserve divine authority, seize the system, stop Transference, exploit it, or pursue other emergent goals.

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

Faction reputation remains independent by organization, and morality emerges from persistent behavior and concrete consequences rather than a universal Good/Evil meter.

## Central Lore Mystery

The intended progression of understanding is:

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

Mechanics should increasingly become lore as the player gains knowledge.

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their persistent timeline and up to five other players may join with their own characters. Visitors participate in the host's current narrative reality without replacing their own world state. Visiting characters may provide narrative keys based on their Origins, Classes, Skills, Titles, Authorities, Knowledge, or faction histories where appropriate.

Initial multiplayer uses player-hosted listen servers. The architecture should remain compatible with dedicated servers later.

## Power Curve

The intended long-form character fantasy is:

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

Early enemies should be dangerous and resources meaningful. Midgame should open multiclassing, equipment evolution, crafting, companions, faction influence, and increasingly elaborate engines. Endgame should reward extreme specialization, rare classes, legendary equipment, treasures, summons, political influence, unusual interactions, Authorities, and mastery of hidden systems.

## Design status labels

- **Core Rule** — foundational unless deliberately changed in a patch.
- **Canon Lore** — current setting truth unless deliberately retconned in a later patch.
- **Narrative Rule** — foundational structure for authored and emergent story content.
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
- five test cards represented as Active Codex manifestations
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

The goal is to prove that **3D action, deck constraints, replication, persistence, lore presentation, and co-op are coherent together** before scaling content production.

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
