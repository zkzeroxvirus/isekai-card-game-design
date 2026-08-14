# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven combat, a soul-bound Divine Codex, Skills, modular disciplines, equipment mastery, living-world consequences, narrative discovery, infinitely scaling dungeons, town progression, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards are exceptional manifestations inside a larger build made from Skills, weapons, disciplines, equipment, mastery, titles, knowledge, relationships, and world history.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**
4. **Cards are manifestations of the soul.** The Active Codex represents permitted interactions with the laws of the world.
5. **Origins change both history and perception.** Arrival method, Background, Skills, divine involvement, combat experience, and System Comprehension can alter onboarding and narrative access.
6. **Skills are broader than cards.** Skills affect combat, crafting, survival, exploration, social interaction, class qualification, and perception.
7. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later.
8. **Morality emerges from behavior.** Heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths are supported without a single Good/Evil meter.
9. **The story is discovered, not merely followed.** The Core Mystery advances through Story Revelations, exploration, factions, companions, and world state.
10. **Visual progression mirrors character progression.** The world begins grounded and becomes increasingly supernatural as power rises.
11. **Classes are modular disciplines.** Characters qualify for and combine disciplines rather than being permanently locked into one identity.
12. **Mastery changes abilities.** Skills and equipment branch and evolve through meaningful use, training, accomplishments, and discoveries.
13. **Depth changes rules, not only numbers.** Infinite dungeon scaling uses enemy affixes, hazards, mutations, and Dungeon Laws alongside controlled stat growth.
14. **Discovery is progression.** Hidden classes, titles, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
15. **Knowledge is power.** Bestiary research and System Comprehension eventually expose deeper world rules.
16. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without deleting developed characters.
17. **Multiplayer should feel like visiting another adventurer's world.** World persistence belongs to the host; character persistence belongs to each player.
18. **The power curve escalates dramatically.** Vulnerable outsider becomes a specialized veteran and eventually a system-breaking legendary build.
19. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
20. **Isekai progression fantasy is the tone.** The player gradually learns, masters, and eventually exploits the hidden rules of a new fantasy world.

## Repository map

### Core Rules

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core loop, character construction, combat, deck construction, party structure, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — resources, damage, defense, statuses, keywords, triggers, and timing language.
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md) — Foundation Actions, Weapon Arts, Codex Manifestations, weapon sets, five-slot hand, targeting families, and combat-tempo rules.
- [`docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md`](docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md) — first complete playable combat package: Guardian, Arming Sword & Shield, Resolve, Guard timing, Weapon Arts, starter manifestations, mastery, and equipment evolution.

### Character & Progression Systems

- [`docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md`](docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md) — multiple Origin paths, the Threshold, Skills, System Comprehension, perception lenses, starting vulnerability, and gradual Codex discovery.
- [`docs/STARTING_ORIGINS_AND_OPENINGS.md`](docs/STARTING_ORIGINS_AND_OPENINGS.md) — playable Origin set, Background layer, Threshold scenes, adaptive first manifestations, and opening convergence.
- [`docs/PROGRESSION.md`](docs/PROGRESSION.md) — master progression model and long-term power arc.
- [`docs/SKILL_MASTERY.md`](docs/SKILL_MASTERY.md) — persistent skill use, mastery tiers, branching upgrades, and hidden evolutions.
- [`docs/EQUIPMENT_PROGRESSION.md`](docs/EQUIPMENT_PROGRESSION.md) — equipment mastery, learned techniques, affixes, crafting, and item evolution.
- [`docs/GUILD_AND_RANK.md`](docs/GUILD_AND_RANK.md) — Adventurer Guild contracts, reputation, certifications, and rank.
- [`docs/COMPANIONS.md`](docs/COMPANIONS.md) — companion progression, roles, recruitment, injuries, and Support Decks.
- [`docs/KNOWLEDGE_AND_DEFEAT.md`](docs/KNOWLEDGE_AND_DEFEAT.md) — Bestiary progression, world knowledge, wounds, secured loot, extraction, and recovery.

### Lore, Narrative & World Systems

- [`docs/DIVINE_CODEX_LORE.md`](docs/DIVINE_CODEX_LORE.md) — Divine Codex, Transference, gods, Authorities, perception, and the central metaphysical mystery.
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md) — world time, faction reputation, behavioral tendencies, consequences, projects, settlements, and hero/villain paths.
- [`docs/NARRATIVE_STRUCTURE.md`](docs/NARRATIVE_STRUCTURE.md) — Core Mystery, regional storylines, companion arcs, emergent stories, campaign history, and Story Revelations.
- [`docs/FIRST_REGION_AND_DUNGEON.md`](docs/FIRST_REGION_AND_DUNGEON.md) — Greyfen March, Hearthcross, first factions, regional state, The Buried Gate, Gatebound Hob, and the first shared Story Revelation.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — infinite dungeon framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town progression framework.

### Visual & Technical Systems

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md) — stylized anime-fantasy rendering, character direction, equipment evolution, VFX hierarchy, Divine Codex UI, factions, monsters, and camera.
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine 5 direction, listen-server co-op, ownership, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/) — versioned design changes.

## Current design version

**v0.2.14 — First Combat Package**

The first fully specified playable discipline is **Guardian**, paired with **Arming Sword & Shield**.

Guardian is an active-defense discipline rather than a passive MMO tank. Its core resource, **Resolve**, is earned primarily through correctly answering danger: timed blocks, interrupts, physical interception, protecting allies, and surviving heavy pressure with good positioning.

### First Weapon Art package

Reliable, non-random actions:

- **Advancing Slash** — short gap-closing attack; Guardian gains Resolve when pressuring enemies targeting allies.
- **Shield Bash** — compact interrupt/stagger tool; successful attack interruption generates extra Resolve.
- **Intercept** — quickly reposition toward an ally or protected point while raising the shield; successful rescue blocks are a major Resolve source.
- **Counterstep** — mobile defensive footwork that rewards causing an attack to miss or be deflected.

### Prototype Guard outcomes

- **Weak Guard** — mistimed or poorly angled; high defensive strain and no special reward.
- **Solid Guard** — correctly faced defense; normal cost and possible Resolve.
- **Perfect Guard** — narrow impact timing; lower cost, stronger Resolve, and counter opportunities.

Guard is deliberately not the answer to every attack. The first boss must include attacks that should be dodged or repositioned around.

### First five Guardian manifestations

1. **Brace → Perfect Guard** — same-slot Reaction transformation testing.
2. **Shield Counter** — spends Resolve to convert defensive setup into stagger/offense.
3. **Guardian's Advance** — modifies Advancing Slash and protects allies along the movement path.
4. **Hold Fast** — short active frontline Stance that converts good defense into nearby ally protection.
5. **Severing Riposte** — finisher that rewards Exposed/Staggered targets and cross-player status setup.

The key combat principle remains:

**Reliable weapon play must already feel good before the Codex appears; manifestations then deepen, transform, and exploit that combat vocabulary.**

## First Region

The first shared region is **the Greyfen March**, centered on **Hearthcross**. It is intentionally compact and reactive rather than open-world-scale.

Hearthcross includes the Adventurer Guild Hall, Split Anvil blacksmith, Lantern House, Shrine of the Returning Flame, Survey Office / Archive Annex, and Underbridge Market.

The first dungeon is **The Buried Gate**. Its first boss, the **Gatebound Hob**, now doubles as the primary Guardian test encounter: heavy telegraphs reward Perfect Guard, pressure moments reward Intercept and Hold Fast, and unblockable or unsuitable attacks force dodging.

After the boss, the party reaches the true Buried Gate and receives the first shared Story Revelation:

**The Gate recognizes the party in some way, but does not fully open.**

## Origins & Opening Experience

Origin and Background are separate concepts:

- **Origin:** how did you enter this world?
- **Background:** who were you before that happened?

The first two complete opening paths are:

1. **Accidental Transfer — The Stranded**
2. **Ritual Summon — The Invited**

Both converge on Hearthcross while retaining different Skills, social circumstances, perception lenses, and narrative flags.

Guardian can emerge differently by Origin: The Stranded may discover protection/interception behavior organically, while The Invited can be formally evaluated and trained.

## Combat Architecture

Combat uses three formal layers:

1. **Foundation Actions** — movement, dodge, interaction, traversal, camera/aim, and other reliable non-random actions.
2. **Weapon Arts** — reliable combat actions defined by weapon family, discipline, Skills, equipment mastery, and item evolution.
3. **Codex Manifestations** — rotating exceptional options such as Techniques, Spells, Reactions, Stances, Summons, Miracles, and Authorities.

Prototype formula:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

## Visual Direction

**Ground the world before breaking it.**

Visual target: **stylized anime fantasy with softly stylized PBR environments and increasingly supernatural escalation**.

**Practical fantasy → refined supernatural craft → legendary manifestations → divine intervention → Authority-driven reality distortion.**

## Narrative Structure

The game uses a **sandbox-first living world with a discoverable core mystery**.

Narrative layers:

1. Core Mystery
2. Regional Storylines
3. Character & Companion Arcs
4. Emergent World Stories
5. Player Campaign History

The Core Mystery advances mainly through Story Revelations rather than a rigid quest chain.

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

Faction reputation is organization-specific, and morality emerges through persistent behavior and consequences rather than a universal meter.

## Central Lore Mystery

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their timeline and up to five visitors join with their own characters. Visitors retain Origin, Skills, perception lens, progression, and secured rewards.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

## Design status labels

- **Core Rule** — foundational unless deliberately changed.
- **Canon Lore** — current setting truth unless deliberately retconned.
- **Narrative Rule** — foundational structure for authored and emergent story content.
- **Visual Direction** — production-facing target subject to prototype validation where noted.
- **Prototype Default** — chosen for testing; expected to change.
- **Content Guideline** — direction for future content design.
- **Technical Direction** — intended implementation architecture subject to prototype validation.
- **Open Question** — intentionally unresolved.

## Next prototype target — Guardian in the Buried Gate

Validate the end-to-end early-game combat chain:

- The Stranded or The Invited opening
- Hearthcross convergence
- Sword/Shield baseline combat before Codex access
- Swordsmanship, Shield Handling, and Combat Awareness Skills
- adaptive first manifestation
- Guardian qualification/training
- Resolve generation
- Weak/Solid/Perfect Guard distinction
- Advancing Slash, Shield Bash, Intercept, and Counterstep
- five-slot Active Codex hand
- Brace → Perfect Guard transformation
- co-op Guardian's Advance and Hold Fast behavior
- ally status → Severing Riposte synergy
- Gatebound Hob boss
- Hearthcross Militia Shield mastery
- first equipment evolution toward **Gatewarden Shield**
- 1–6 player readability and responsiveness

If this package feels good without relying on the Codex for basic functionality, it becomes the production template for the next prototype disciplines.

## Following gameplay target — v0.3.0 Combat Prototype

After validating Guardian, expand to three prototype disciplines, multiple weapon families, multiclass interactions, broader class card pools, equipment families, companions, enemy families, elites, the Buried Gate content slice, treasures, hidden qualifications, Guild advancement, wounds, extraction, and expanded town progression.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
