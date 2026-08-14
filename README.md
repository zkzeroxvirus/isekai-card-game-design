# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven action combat, a soul-bound Divine Codex, multiclass progression, Skills, equipment mastery, narrative exploration, a persistent living world, infinitely scaling dungeons, town development, companions, achievements, legendary treasures, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards represent exceptional manifestations of a larger character build made from Skills, weapons, classes, equipment, mastery, titles, knowledge, and relationships.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and environmental interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.** Reliable Weapon Arts form the combat backbone while the Active Codex creates tactical variation and supernatural escalation.
4. **Cards are manifestations of the soul.** The card interface represents the character's permitted interactions with the laws of the world through a soul-bound Active Codex.
5. **Origins change both history and perception.** Arrival method, previous-world experience, Skills, divine involvement, combat experience, and System Comprehension can change how the game initially presents itself.
6. **Every Origin teaches the same world through a different lens.** Origin prologues can vary dramatically while converging into the same underlying world and multiplayer simulation.
7. **Skills are broader than cards.** Persistent Skills can affect combat, crafting, survival, exploration, social interaction, perception, class qualification, and narrative access.
8. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later in the campaign.
9. **Morality emerges from behavior.** Heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths are supported without a single Good/Evil meter.
10. **The story is discovered, not merely followed.** A central mystery exists, but players uncover it through revelations, exploration, factions, companions, and world state rather than a rigid main-quest chain.
11. **Visual progression mirrors character progression.** The world begins grounded and readable while equipment, magic, dungeons, divine phenomena, and Authorities become increasingly supernatural.
12. **Classes are modular disciplines.** Characters combine disciplines and qualifications rather than being permanently locked into one class identity.
13. **Mastery changes abilities.** Skills and equipment can improve, branch, and evolve through meaningful use, training, accomplishments, and discoveries.
14. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset while mastery, treasures, achievements, town systems, companions, knowledge, relationships, and discoveries persist.
15. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
16. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
17. **Knowledge is power.** Bestiary research and System Comprehension reveal enemy behavior, weaknesses, hidden interactions, and eventually the true nature of the world's systems.
18. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without erasing developed characters.
19. **Multiplayer should feel like visiting another adventurer's world.** World persistence and timeline belong to the host; persistent characters belong to individual players.
20. **The power curve escalates dramatically.** The intended arc moves from vulnerable adventurer to specialized veteran to legendary system-breaking build.
21. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
22. **Isekai progression fantasy is the tone.** The player should feel as though they are gradually learning, mastering, and eventually exploiting the hidden rules of a new fantasy world.

## Repository map

### Core Rules

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core loop, character construction, combat, deck construction, party structure, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — resources, damage, defense, statuses, keywords, triggers, and timing language.
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md) — Foundation Actions, Weapon Arts, Codex Manifestations, weapon sets, five-slot hand, targeting families, and combat-tempo rules.

### Character & Progression Systems

- [`docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md`](docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md) — multiple Origin paths, the Threshold, Skills, System Comprehension, perception lenses, starting vulnerability, and gradual Codex discovery.
- [`docs/STARTING_ORIGINS_AND_OPENINGS.md`](docs/STARTING_ORIGINS_AND_OPENINGS.md) — playable Origin set, previous-world Backgrounds, Threshold variants, opening scenarios, adaptive first manifestations, and convergence into the first shared region.
- [`docs/PROGRESSION.md`](docs/PROGRESSION.md) — master progression model and long-term power arc.
- [`docs/SKILL_MASTERY.md`](docs/SKILL_MASTERY.md) — persistent skill use, mastery tiers, branching upgrades, and hidden evolutions.
- [`docs/EQUIPMENT_PROGRESSION.md`](docs/EQUIPMENT_PROGRESSION.md) — equipment mastery, learned techniques, affixes, crafting, and item evolution.
- [`docs/GUILD_AND_RANK.md`](docs/GUILD_AND_RANK.md) — Adventurer Guild contracts, reputation, certifications, and institutional rank.
- [`docs/COMPANIONS.md`](docs/COMPANIONS.md) — companion Support Decks, party roles, recruitment, progression, injuries, and solo alternatives.
- [`docs/KNOWLEDGE_AND_DEFEAT.md`](docs/KNOWLEDGE_AND_DEFEAT.md) — Bestiary progression, world knowledge, wounds, secured loot, extraction, and recovery runs.

### Lore, Narrative & World Systems

- [`docs/DIVINE_CODEX_LORE.md`](docs/DIVINE_CODEX_LORE.md) — Divine Codex, Transference, soul manifestations, gods, Authorities, native/otherworlder perception, and the central metaphysical mystery.
- [`docs/LIVING_WORLD.md`](docs/LIVING_WORLD.md) — world time, faction reputation, behavioral tendencies, consequence records, faction projects, evolving settlements, world eras, and hero/villain paths.
- [`docs/NARRATIVE_STRUCTURE.md`](docs/NARRATIVE_STRUCTURE.md) — Core Mystery, regional storylines, companion arcs, emergent stories, player campaign history, Story Revelations, and era-based narrative escalation.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.

### Visual & Technical Systems

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md) — stylized anime-fantasy rendering, character direction, equipment evolution, VFX hierarchy, Divine Codex UI, faction/settlement visual language, monsters, and camera.
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine direction, 1–6 player listen-server co-op, world/character ownership, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/) — versioned design changes.

## Current design version

**v0.2.12 — Playable Origins & Opening Scenarios**

The first concrete Origin package now contains five standard paths and one later-unlocked anomaly path:

1. **Accidental Transfer — The Stranded** — survival-heavy, low-information, high-freedom start.
2. **Ritual Summon — The Invited** — institution-supported, politically constrained, moderately system-aware start.
3. **Reincarnated — The Second Life** — culturally integrated start with a slower distinction between native Skills and the deeper Codex.
4. **Failed Hero Summoning — The Rejected** — unstable system information, poor circumstances, and strong mystery hooks.
5. **Divine Bargain — The Contracted** — explicit supernatural advantage tied to obligations, restrictions, or divine attention.
6. **System Anomaly — The Unregistered** — later-unlocked Origin intended to expose or distort major system mysteries.

Origin and previous-world **Background** are separate layers: Origin answers *how you entered this world*; Background answers *who you were before it happened*.

The first manifestation is selected from an adaptive candidate pool based on Origin, Background, starting Skills, and player behavior. The player's earliest card should therefore communicate that **the system noticed what they actually did**.

## First Playable Origin Prototype

The first implementation should fully build only two prologues:

- **Accidental Transfer — The Stranded**
- **Ritual Summon — The Invited**

They test opposite onboarding assumptions while sharing the same underlying game data:

- low-information vs system-aware presentation
- survival vs structured training
- no support vs institutional support
- reactive Codex discovery vs expected/observed Codex discovery

Both converge into the same frontier settlement and first dungeon without erasing Origin-specific consequences.

Open multiplayer begins after the personal prologue reaches this shared regional structure.

## Combat Architecture

Combat uses three formal layers:

1. **Foundation Actions** — movement, dodge, interaction, traversal, camera/aim, and other reliable non-random actions.
2. **Weapon Arts** — reliable combat actions defined by weapon family, class discipline, Skills, equipment mastery, and item evolution.
3. **Codex Manifestations** — the rotating five-slot hand of Techniques, Spells, Reactions, Stances, Summons, transformations, Miracles, Authorities, and other exceptional capabilities.

Prototype formula:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

## Opening Experience

The first roughly 30–60 minutes teach a shared mechanical spine through Origin-specific scenarios:

1. movement and camera
2. interaction
3. physical danger and vulnerability
4. one weapon family and basic Weapon Arts
5. first Skill recognition/acquisition
6. one meaningful threat
7. reaching civilization, shelter, or another stable objective
8. realizing that the player's understanding of the world is incomplete

## Visual Direction

**Ground the world before breaking it.**

The visual target remains **stylized anime fantasy with softly stylized PBR environments and increasingly supernatural visual escalation**.

## Narrative Structure

The game uses a **sandbox-first living world with a discoverable core mystery**. The Core Mystery advances mainly through Story Revelations rather than a rigid quest chain, and there is no permanent global apocalypse timer forcing continuous main-story engagement.

## Narrative Escalation

**Arrival → Adventurer → Heroic → Sovereign → Mythic**

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

## Central Lore Mystery

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

Visitors retain their Origin, Background, Skills, perception lens, character progression, and secured rewards while participating in the host's timeline.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

## Next prototype target — Two-Origin Opening + Combat Proof of Concept

Before the full content vertical slice, validate:

- Accidental Transfer prologue
- Ritual Summon prologue
- shared frontier-settlement convergence
- third-person movement
- keyboard and controller input
- deliberately different starting HUD/perception profiles
- previous-world Background modifier
- one starting Skill per profile
- behavior-driven first Skill recognition
- one weapon family with a small Weapon Art package
- initially hidden five-slot Codex hand
- adaptive first-manifestation reveal
- System Comprehension/HUD expansion
- listen-server multiplayer unlocking after prologue convergence
- one shared first dungeon
- save/reload and join-in-progress

The goal is to prove that **different isekai beginnings can produce distinct first impressions while still converging cleanly into one multiplayer action-RPG system**.

## Following gameplay target — v0.3.0 Combat Prototype

Once the proof of concept is sound, expand into the first real content slice with base classes, multiclassing, class card pools, equipment families, companions, enemy families, elites, a boss, a dungeon run, treasures, hidden qualifications, Guild advancement, wounds, extraction, and the minimal town.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
