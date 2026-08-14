# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven action combat, a soul-bound Divine Codex, multiclass progression, Skills, equipment mastery, narrative exploration, a persistent living world, infinitely scaling dungeons, town development, companions, achievements, legendary treasures, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards represent exceptional manifestations of a larger character build made from Skills, weapons, classes, equipment, mastery, titles, knowledge, and relationships.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and environmental interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.** Reliable Weapon Arts form the combat backbone while the Active Codex creates tactical variation and supernatural escalation.
4. **Cards are manifestations of the soul.** The card interface represents the character's permitted interactions with the laws of the world through a soul-bound Active Codex.
5. **Origins change both history and perception.** Arrival method, previous-world experience, Skills, divine involvement, combat experience, and System Comprehension can change how the game initially presents itself.
6. **Skills are broader than cards.** Persistent Skills can affect combat, crafting, survival, exploration, social interaction, perception, class qualification, and narrative access.
7. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later in the campaign.
8. **Morality emerges from behavior.** Heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths are supported without a single Good/Evil meter.
9. **The story is discovered, not merely followed.** A central mystery exists, but players uncover it through revelations, exploration, factions, companions, and world state rather than a rigid main-quest chain.
10. **Visual progression mirrors character progression.** The world begins grounded and readable while equipment, magic, dungeons, divine phenomena, and Authorities become increasingly supernatural.
11. **Classes are modular disciplines.** Characters combine disciplines and qualifications rather than being permanently locked into one class identity.
12. **Mastery changes abilities.** Skills and equipment can improve, branch, and evolve through meaningful use, training, accomplishments, and discoveries.
13. **Runs create temporary power; the world creates permanent possibility.** Dungeon upgrades reset while mastery, treasures, achievements, town systems, companions, knowledge, relationships, and discoveries persist.
14. **Depth changes rules, not only numbers.** Infinite dungeon scaling adds affixes, hazards, mutations, and Dungeon Laws alongside controlled numerical scaling.
15. **Discovery is progression.** Hidden classes, hybrid cards, titles, achievements, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
16. **Knowledge is power.** Bestiary research and System Comprehension reveal enemy behavior, weaknesses, hidden interactions, and eventually the true nature of the world's systems.
17. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without erasing developed characters.
18. **Multiplayer should feel like visiting another adventurer's world.** World persistence and timeline belong to the host; persistent characters belong to individual players.
19. **The power curve escalates dramatically.** The intended arc moves from vulnerable adventurer to specialized veteran to legendary system-breaking build.
20. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
21. **Isekai progression fantasy is the tone.** The player should feel as though they are gradually learning, mastering, and eventually exploiting the hidden rules of a new fantasy world.

## Repository map

### Core Rules

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core loop, character construction, combat, deck construction, party structure, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — resources, damage, defense, statuses, keywords, triggers, and timing language.
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md) — Foundation Actions, Weapon Arts, Codex Manifestations, weapon sets, five-slot hand, targeting families, and combat-tempo rules.

### Character & Progression Systems

- [`docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md`](docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md) — multiple Origin paths, the Threshold, Skills, System Comprehension, perception lenses, starting vulnerability, and gradual Codex discovery.
- [`docs/STARTING_ORIGINS_AND_OPENINGS.md`](docs/STARTING_ORIGINS_AND_OPENINGS.md) — playable Origin set, Background layer, Threshold scenes, adaptive first manifestations, and opening-scenario convergence.
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
- [`docs/FIRST_REGION_AND_DUNGEON.md`](docs/FIRST_REGION_AND_DUNGEON.md) — Greyfen March, Hearthcross, first regional factions, early living-world seeds, the Buried Gate dungeon, Gatebound Hob, and the first shared Story Revelation.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — dungeon generation and infinite depth framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town and building progression framework.

### Visual & Technical Systems

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md) — stylized anime-fantasy rendering, character direction, equipment evolution, VFX hierarchy, Divine Codex UI, faction/settlement visual language, monsters, and camera.
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine direction, 1–6 player listen-server co-op, world/character ownership, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled game terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved design decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/) — versioned design changes.

## Current design version

**v0.2.13 — First Region & Dungeon**

The first shared region is now **the Greyfen March**, centered on the frontier settlement of **Hearthcross**. Hearthcross is the convergence point for Origin-specific prologues and the first place where open co-op becomes available.

The region is intentionally compact and reactive rather than open-world-scale. Its early factions include the Adventurer Guild, March Wardens, Returning Flame clergy, Fenroad Consortium, and Underbridge Network. Their interests overlap and conflict without collapsing into simple hero/villain alignment.

The first dungeon is **The Buried Gate**, a quarry/fortification ruin that transitions from believable frontier archaeology into architecture that does not fit known history or normal magical explanations.

Its first boss, the **Gatebound Hob**, introduces a restrained dungeon/system anomaly. After the fight, the party reaches the true Buried Gate and receives the first shared Core Mystery Story Revelation:

**The Gate recognizes the party in some way, but does not fully open.**

Origin and System Comprehension alter how individual characters interpret the same event.

## First Region

Hearthcross provides the first dense systemic hub:

- Adventurer Guild Hall
- The Split Anvil blacksmith
- Lantern House inn/social hub
- Shrine of the Returning Flame
- Survey Office / Archive Annex
- Underbridge Market

Early regional state can track refugee population, road safety, goblin organization, merchant confidence, Warden control, Guild influence, dungeon activity, shrine influence, and Underbridge strength.

The production rule for this region is:

**Prioritize density and consequence over acreage.**

## Combat Architecture

Combat uses three formal layers:

1. **Foundation Actions** — movement, dodge, interaction, traversal, camera/aim, and other reliable non-random actions.
2. **Weapon Arts** — reliable combat actions defined by weapon family, class discipline, Skills, equipment mastery, and item evolution.
3. **Codex Manifestations** — the rotating five-slot hand of Techniques, Spells, Reactions, Stances, Summons, transformations, Miracles, Authorities, and other exceptional capabilities.

Prototype formula:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

## Origins & Opening Experience

The initial playable Origin framework separates **Origin** from **Background**.

Origin answers: **How did you enter this world?**

Background answers: **Who were you before that happened?**

The prototype fully implements two contrasting openings first:

1. **Accidental Transfer — The Stranded**
2. **Ritual Summon — The Invited**

Both eventually converge on Hearthcross while retaining Origin-specific narrative flags, Skills, social circumstances, and System Comprehension.

The first Codex manifestation is selected from an adaptive pool based on Origin, Background, starting Skills, and actual player behavior. The system should communicate early that **it noticed what the player did**.

## Visual Direction

**Ground the world before breaking it.**

The visual target remains **stylized anime fantasy with softly stylized PBR environments and increasingly supernatural visual escalation**.

Broad progression:

**Practical fantasy → refined supernatural craft → legendary manifestations → divine intervention → Authority-driven reality distortion.**

## Narrative Structure

The game uses a **sandbox-first living world with a discoverable core mystery**.

Narrative layers:

1. Core Mystery
2. Regional Storylines
3. Character & Companion Arcs
4. Emergent World Stories
5. Player Campaign History

The Core Mystery advances mainly through Story Revelations rather than a rigid quest chain, and there is no permanent global apocalypse timer forcing continuous main-story engagement.

## Narrative Escalation

**Arrival → Adventurer → Heroic → Sovereign → Mythic**

Scale rises from:

**Personal survival → regional conflicts → major faction/divine attention → nations and system control → gods, Authorities, Transference, and world laws.**

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

Faction reputation remains independent by organization, and morality emerges from persistent behavior and concrete consequences rather than a universal Good/Evil meter.

## Central Lore Mystery

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

Mechanics should increasingly become lore as the player gains knowledge and System Comprehension.

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their persistent timeline and up to five other players may join with their own characters. Visitors participate in the host's narrative reality while retaining their own character progression, Origin, Skills, perception lens, and secured rewards.

Initial multiplayer uses player-hosted listen servers, with architecture intended to remain compatible with dedicated servers later.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

Early enemies should be dangerous and resources meaningful. Midgame opens multiclassing, equipment evolution, crafting, companions, faction influence, deeper Skills, and increasingly elaborate engines. Endgame rewards extreme specialization, rare classes, legendary equipment, political influence, unusual interactions, Authorities, and mastery of hidden systems.

## Design status labels

- **Core Rule** — foundational unless deliberately changed.
- **Canon Lore** — current setting truth unless deliberately retconned.
- **Narrative Rule** — foundational structure for authored and emergent story content.
- **Visual Direction** — production-facing visual target subject to prototype validation where noted.
- **Prototype Default** — chosen for testing; expected to change.
- **Content Guideline** — direction for future content design.
- **Technical Direction** — intended implementation architecture subject to prototype validation.
- **Open Question** — intentionally unresolved.

## Next prototype target — Hearthcross + Buried Gate Slice

Before scaling content production, validate:

- one complete Origin prologue path
- Hearthcross town gate and compact hub loop
- Guild Hall, blacksmith, inn, shrine, and Underbridge access
- one surrounding travel route
- two enemy families
- one adaptive Skill recognition
- one first-manifestation reveal
- one weapon family and Weapon Art package
- five-slot Active Codex hand after revelation
- one regional choice with a persistent consequence
- one goblin encounter with combat and noncombat outcomes
- the Buried Gate dungeon
- one route split
- one secure/extract checkpoint
- Gatebound Hob boss
- one shared Story Revelation with two different System Comprehension presentations
- 1–6 player co-op from Hearthcross onward
- host-owned regional state and visitor-owned character state

The goal is to prove that **Origin onboarding, Hearthcross, weapon combat, Skills, Codex revelation, living-world consequences, dungeon play, narrative mystery, and multiplayer all function as one coherent early-game slice**.

## Following gameplay target — v0.3.0 Combat Prototype

Once the proof of concept is sound, expand into the first real content slice with base classes, multiclassing, class card pools, equipment families, companions, enemy families, elites, a boss, deeper dungeon variation, treasures, hidden qualifications, Guild advancement, wounds, extraction, and expanded town progression.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
