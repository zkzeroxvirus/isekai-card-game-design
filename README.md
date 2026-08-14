# Isekai Card Game Design

Design repository for a progression-fantasy **3D PC action-RPG/deckbuilder** built around customizable characters, weapon-driven combat, a soul-bound Divine Codex, Skills, modular disciplines, Jobs, hidden progression, equipment mastery, living-world consequences, narrative discovery, infinitely scaling dungeons, town progression, and 1–6 player online co-op.

## Design pillars

1. **Build a character, not just a deck.** Cards are exceptional manifestations inside a larger build made from Origin, Background, Skills, Jobs, weapons, disciplines, equipment, mastery, titles, knowledge, relationships, and world history.
2. **The deck defines capability; the player controls execution.** Movement, positioning, aiming, traversal, dodging, and interaction happen directly in 3D space.
3. **Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**
4. **Cards are manifestations of the soul.** The Active Codex represents permitted interactions with the laws of the world.
5. **Origins change both history and perception.** Arrival method, Background, Skills, divine involvement, combat experience, and System Comprehension can alter onboarding and narrative access.
6. **Skills are broader than cards.** Skills affect combat, crafting, survival, exploration, social interaction, class qualification, and perception.
7. **Jobs describe recognized roles; Disciplines describe combat frameworks.** Jobs provide effects, Skills, permissions, social recognition, and qualification routes without becoming alternate combat bars.
8. **Visible progression tells the player what they can pursue. Hidden progression rewards the person they accidentally became.**
9. **New places expand the character-build space.** Jobs are embedded in institutions, cultures, environments, activities, and secrets rather than a universal catalogue.
10. **Settlement growth increases depth before breadth.** A settlement becomes better at what it already is rather than eventually teaching every profession in the world.
11. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later.
12. **Morality emerges from behavior.** Heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths are supported without a single Good/Evil meter.
13. **The story is discovered, not merely followed.** The Core Mystery advances through Story Revelations, exploration, factions, companions, and world state.
14. **Visual progression mirrors character progression.** The world begins grounded and becomes increasingly supernatural as power rises.
15. **Classes are modular disciplines.** Characters qualify for and combine disciplines rather than being permanently locked into one identity.
16. **Mastery changes abilities.** Skills and equipment branch and evolve through meaningful use, training, accomplishments, and discoveries.
17. **Magic should shape the battlefield, not merely replace arrows with colored projectiles.** Ranged magic should use positioning, geometry, preparation, statuses, and spatial control.
18. **Depth changes rules, not only numbers.** Infinite dungeon scaling uses enemy affixes, hazards, mutations, and Dungeon Laws alongside controlled stat growth.
19. **Discovery is progression.** Hidden Jobs, hidden Disciplines, titles, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
20. **Knowledge is power.** Bestiary research and System Comprehension eventually expose deeper world rules and hidden qualification information.
21. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without deleting developed characters.
22. **Multiplayer should feel like visiting another adventurer's world.** World persistence belongs to the host; character persistence belongs to each player.
23. **The power curve escalates dramatically.** Vulnerable outsider becomes a specialized veteran and eventually a system-breaking legendary build.
24. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
25. **Isekai progression fantasy is the tone.** The player gradually learns, masters, and eventually exploits the hidden rules of a new fantasy world.

## Repository map

### Core Rules & Combat

- [`docs/RULES_FRAMEWORK.md`](docs/RULES_FRAMEWORK.md) — core loop, character construction, combat, deck construction, party structure, run flow, and rules hierarchy.
- [`docs/CARD_CATEGORIES.md`](docs/CARD_CATEGORIES.md) — card taxonomy, anatomy, rarity, sources, tags, and upgrade structure.
- [`docs/MECHANICS.md`](docs/MECHANICS.md) — resources, damage, defense, statuses, keywords, triggers, and timing language.
- [`docs/WEAPON_ARTS_COMBAT_LAYERS.md`](docs/WEAPON_ARTS_COMBAT_LAYERS.md) — Foundation Actions, Weapon Arts, Codex Manifestations, weapon sets, five-slot hand, targeting families, and combat-tempo rules.
- [`docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md`](docs/FIRST_COMBAT_PACKAGE_GUARDIAN.md) — Guardian, Arming Sword & Shield, Resolve, Guard timing, Weapon Arts, starter manifestations, mastery, and equipment evolution.
- [`docs/SECOND_COMBAT_PACKAGE_ARCANIST.md`](docs/SECOND_COMBAT_PACKAGE_ARCANIST.md) — Arcanist, Channeling Staff & Arcane Focus, Attunement, Sigils, ranged Weapon Arts, starter spells, mastery, and magical readability rules.
- [`docs/THIRD_COMBAT_PACKAGE_DUELIST.md`](docs/THIRD_COMBAT_PACKAGE_DUELIST.md) — Duelist, Twin Blades, Flow, mobile Weapon Arts, starter manifestations, team-opening creation, mastery, and multiclass bridges.

### Character & Progression Systems

- [`docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md`](docs/ORIGINS_SKILLS_SYSTEM_PERCEPTION.md) — multiple Origin paths, the Threshold, Skills, System Comprehension, perception lenses, starting vulnerability, and gradual Codex discovery.
- [`docs/STARTING_ORIGINS_AND_OPENINGS.md`](docs/STARTING_ORIGINS_AND_OPENINGS.md) — playable Origin set, Background layer, Threshold scenes, adaptive first manifestations, and opening convergence.
- [`docs/JOBS_MULTICLASS_AND_HIDDEN_PROGRESSION.md`](docs/JOBS_MULTICLASS_AND_HIDDEN_PROGRESSION.md) — Jobs, Active Job slots, hidden qualifications, System Comprehension visibility tiers, Discipline multiclassing, Hybrid Manifestations, mutual exclusivity, and endgame classification drift.
- [`docs/HEARTHCROSS_JOB_ECOSYSTEM.md`](docs/HEARTHCROSS_JOB_ECOSYSTEM.md) — first location-based Job roster, Greyfen/Buried Gate discovery, hidden Jobs, settlement expansion branches, Job-access tradeoffs, and the future-region Job template.
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
- [`docs/FIRST_REGION_AND_DUNGEON.md`](docs/FIRST_REGION_AND_DUNGEON.md) — Greyfen March, Hearthcross, first factions, regional state, The Buried Gate, Gatebound Hob, and first shared Story Revelation.
- [`docs/DUNGEONS.md`](docs/DUNGEONS.md) — infinite dungeon framework.
- [`docs/TOWN.md`](docs/TOWN.md) — persistent town progression framework.

### Visual & Technical Systems

- [`docs/VISUAL_DIRECTION.md`](docs/VISUAL_DIRECTION.md) — stylized anime-fantasy rendering, character direction, equipment evolution, VFX hierarchy, Divine Codex UI, factions, monsters, and camera.
- [`docs/TECHNICAL_DIRECTION.md`](docs/TECHNICAL_DIRECTION.md) — Unreal Engine 5 direction, listen-server co-op, ownership, persistence, instancing, and multiplayer risks.
- [`docs/GLOSSARY.md`](docs/GLOSSARY.md) — controlled terminology.
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — unresolved decisions and prototype questions.
- [`PATCHLOG.md`](PATCHLOG.md) and [`patches/`](patches/) — versioned design changes.

## Current design version

**v0.2.18 — Hearthcross Job Ecosystem**

Hearthcross is now the first complete implementation of **location-based Job discovery**.

The governing rules are:

**Locations create opportunities. Actions create qualifications. The Codex recognizes the result.**

and:

**Settlement growth increases depth before breadth.**

Hearthcross is a frontier settlement, so its available Jobs are intentionally practical, local, and incomplete. It teaches roots that can later branch into specialized professions elsewhere rather than becoming a universal profession capital.

### Initial Hearthcross Job roots

Openly discoverable:

- **Adventurer** — Guild contracts, expedition capability, and professional frontier work.
- **Scout** — Warden patrols, route knowledge, tracking, and threat detection.
- **Smith** — practical repair, Greyfen materials, and frontier metalwork.
- **Field Medic** — triage, wound treatment, and crisis medicine.
- **Trader** — regional scarcity, logistics, negotiation, and caravan opportunity.
- **Survey Assistant** — field records, mapping, research, and ruin documentation.

Relationship/semi-hidden:

- **Acolyte of the Returning Flame** — shrine rites, spiritual work, and religious relationships.
- **Smuggler** — Underbridge trust, covert routes, restricted goods, and illicit logistics.

Environment/activity driven:

- **Forager**
- **Trapper**

Buried Gate discovery:

- **Dungeon Surveyor**
- **Relic Seeker**

### First hidden Job seeds

- **Greyfen Guide** — repeatedly proving that others can safely follow you through the March.
- **Gate Listener** — sustained, non-destructive investigation of the Buried Gate's anomalous structures.
- **Fen Scavenger** — salvage, improvisation, and possible learning from goblin scavenger traditions.
- **Oathbearer** — a behavioral identity recognized through repeatedly honoring responsibility even when doing so costs reward or convenience.

These are precursor identities rather than endgame destinations.

## Hearthcross Expansion

Town progression can deepen existing Job roots without eliminating the need to travel.

Possible development projects include:

- **Guild Expedition Desk** — deeper Adventurer, Scout, and Dungeon Surveyor progression.
- **Split Anvil Frontier Forge** — deeper Smith/equipment mastery and Greyfen-specific techniques.
- **Survey Office Field Archive** — deeper Survey Assistant, Dungeon Surveyor, Relic Seeker, and Gate Listener progression.
- **Shrine Hospice & Spirit House** — deeper Field Medic, Acolyte, funerary, and spirit-related opportunities.
- **Underbridge Hidden Routes** — deeper Smuggler, Trader, Fen Scavenger, and illicit Relic Seeker progression.

A fully developed Hearthcross becomes exceptionally capable at frontier survival, logistics, Greyfen knowledge, practical craft, expedition support, and Buried Gate research. It still does not replace major academies, master forges, royal institutions, exotic cultures, specialist temples, or hidden regions elsewhere.

## Job Availability as World State

Job access can change with the host timeline.

Examples:

- stronger Wardens improve Scout opportunities while making Smuggling harder
- stronger Underbridge expands illicit progression while affecting merchant confidence
- shrine growth deepens spiritual/medical paths while potentially opposing forbidden research
- preserving Buried Gate artifacts strengthens research routes; selling everything produces faster immediate wealth
- integrating Greyfen goblin scavengers can reveal nonhuman Job traditions such as Scrapwright-like branches
- losing mentors, factions, or communities can remove Job opportunities from that timeline

New locations should therefore expand the character-build space by offering new ways to become someone.

## Hidden Progression

Hidden progression remains foundational.

**The world tracks what you repeatedly prove about yourself. The Codex eventually gives that pattern a name.**

Hidden qualifications can depend on behavior, mastery, narrative choices, world state, equipment history, failure/survival, unusual combinations, and negative conditions.

System Comprehension controls how much of those qualifications can be seen.

## Multiclassing

Prototype multiclassing remains **Primary + Secondary Discipline**, with both Disciplines materially shaping the build.

First hybrid bridges remain:

- **Guardian + Duelist** — Blade Warden / Vanguard direction
- **Arcanist + Duelist** — Spellblade direction
- **Guardian + Arcanist** — Runic Bastion / Arcane Warden direction

Jobs can alter these routes without becoming universal mandatory recipes.

## Initial Three-Discipline Combat Triangle

### Guardian — Arming Sword & Shield

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

### Arcanist — Channeling Staff & Arcane Focus

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

### Duelist — Twin Blades

**Read opening → Slipstep/angle change → build Flow → create or exploit vulnerability → commit finisher → disengage before greed is punished.**

## First Region

The first shared region remains **the Greyfen March**, centered on **Hearthcross**. The first dungeon is **The Buried Gate**, whose first boss is the **Gatebound Hob**.

Hearthcross now serves simultaneously as the first shared multiplayer hub, first living-world settlement, first multiclass/Job testbed, and the first demonstration that location and world state directly shape character-building opportunities.

## Origins & Opening Experience

Origin and Background remain separate:

- **Origin:** how did you enter this world?
- **Background:** who were you before that happened?

The first two complete opening paths are **The Stranded** and **The Invited**. Both converge on Hearthcross while retaining different Skills, social circumstances, perception lenses, and narrative flags.

Otherworlders may eventually prove unusually flexible at perceiving, retaining, swapping, and combining Job Imprints through the Divine Codex, but native characters remain capable of deep mastery and culturally specific progression unavailable through generic systems alone.

## Combat Architecture

Combat uses three formal layers:

1. **Foundation Actions** — movement, dodge, interaction, traversal, camera/aim, and other reliable non-random actions.
2. **Weapon Arts** — reliable actions defined by weapon family, discipline, Skills, equipment mastery, and item evolution.
3. **Codex Manifestations** — rotating exceptional options such as Techniques, Spells, Reactions, Stances, Summons, Miracles, and Authorities.

Prototype formula:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

Faction reputation is organization-specific, and morality emerges through persistent behavior and consequences rather than a universal meter.

## Central Lore Mystery

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their timeline and up to five visitors join with their own characters. Visitors retain Origin, Skills, Jobs, perception lens, progression, and secured rewards, while available local opportunities are determined by the host world's Hearthcross state.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

## Next prototype target — Hearthcross Job Discovery in Play

Validate:

- one Active Job slot
- six openly discoverable frontier Job roots
- at least two relationship/semi-hidden Jobs
- one environment-driven Job discovery
- Dungeon Surveyor qualification inside The Buried Gate
- one hidden Job signaled only through System Comprehension
- one Job opportunity affected by Warden/Underbridge world state
- one mentor or institution whose loss changes Job availability
- one nonhuman Job tradition seed through Greyfen goblin interaction
- one town expansion that deepens an existing Job without adding an unrelated profession
- one advanced specialization that explicitly requires leaving Hearthcross
- Primary + Secondary Discipline integration with active Jobs
- visitor characters interacting with the host's local Job opportunities without overwriting their own persistent character state

The goal is to prove that **exploration, settlement development, faction choices, world state, and character progression all feed the same discovery loop**.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
