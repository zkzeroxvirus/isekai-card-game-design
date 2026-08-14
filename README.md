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
9. **The world remembers.** Time passes, factions act, settlements change, and consequences can return much later.
10. **Morality emerges from behavior.** Heroic, villainous, pragmatic, revolutionary, tyrannical, and mixed paths are supported without a single Good/Evil meter.
11. **The story is discovered, not merely followed.** The Core Mystery advances through Story Revelations, exploration, factions, companions, and world state.
12. **Visual progression mirrors character progression.** The world begins grounded and becomes increasingly supernatural as power rises.
13. **Classes are modular disciplines.** Characters qualify for and combine disciplines rather than being permanently locked into one identity.
14. **Mastery changes abilities.** Skills and equipment branch and evolve through meaningful use, training, accomplishments, and discoveries.
15. **Magic should shape the battlefield, not merely replace arrows with colored projectiles.** Ranged magic should use positioning, geometry, preparation, statuses, and spatial control.
16. **Depth changes rules, not only numbers.** Infinite dungeon scaling uses enemy affixes, hazards, mutations, and Dungeon Laws alongside controlled stat growth.
17. **Discovery is progression.** Hidden Jobs, hidden Disciplines, titles, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
18. **Knowledge is power.** Bestiary research and System Comprehension eventually expose deeper world rules and hidden qualification information.
19. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without deleting developed characters.
20. **Multiplayer should feel like visiting another adventurer's world.** World persistence belongs to the host; character persistence belongs to each player.
21. **The power curve escalates dramatically.** Vulnerable outsider becomes a specialized veteran and eventually a system-breaking legendary build.
22. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
23. **Isekai progression fantasy is the tone.** The player gradually learns, masters, and eventually exploits the hidden rules of a new fantasy world.

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

**v0.2.17 — Jobs, Multiclassing & Hidden Progression**

The character-build architecture now formally separates **Jobs** from combat **Disciplines**.

A Discipline primarily answers **how you fight**. A Job answers **what role or identity the world/system has recognized you as fulfilling**.

Jobs can provide:

- contextual passive effects
- Job-specific Skills
- crafting/exploration/social permissions
- faction and NPC recognition
- advanced and hidden Job evolution routes

Characters may know many Jobs but only attune a limited number as **Active Jobs** at full strength. The prototype begins with **one Active Job slot**, with additional slots becoming possible later through progression and eventually through unusual Codex manipulation.

## Hidden Progression

Hidden progression is now a foundational reward structure.

The core rule is:

**The world tracks what you repeatedly prove about yourself. The Codex eventually gives that pattern a name.**

Hidden qualifications can depend on:

- behavior
- mastery
- narrative choices
- world state
- equipment history
- failure/survival
- unusual combinations
- negative conditions: things the player deliberately refused or never did

Some paths are mutually exclusive so character history creates real commitments rather than every character becoming the same completion checklist.

System Comprehension controls how much of these qualifications can be seen, ranging from vague `Unknown Qualification Progressed` feedback to exact hidden requirements at exceptional comprehension.

## Multiclassing

Prototype multiclassing remains **Primary + Secondary Discipline**, but both Disciplines should materially shape the build.

Multiclassing can change:

- manifestation access
- Weapon Art modifications
- resource interactions
- Skill qualification routes
- hidden Job/Discipline access
- narrative identity
- Hybrid Manifestations

It should create integrated identities rather than simply adding more unrelated cards.

### First hybrid bridges

**Guardian + Duelist** — Blade Warden / Vanguard direction

- defensive counters preserve Flow
- Intercept can transition into movement attacks
- protection through aggressive disruption

**Arcanist + Duelist** — Spellblade direction

- Sigils imbue movement attacks
- elemental blade states
- Arc Step connects into melee chains

**Guardian + Arcanist** — Runic Bastion / Arcane Warden direction

- physical Guard interacts with magical wards
- Intercept can create defensive Sigils
- magical attacks can be converted into stored protective charge

These names remain provisional. The important system is the hybrid-recognition framework.

## Jobs as Build Modifiers

Jobs can reshape multiclass identity without becoming universal mandatory recipes.

Examples:

- Guardian + Priest → sacred/oath protection paths
- Duelist + Assassin → execution/stealth paths
- Arcanist + Scholar → deeper magical analysis
- Arcanist + Blacksmith → runic equipment and Runesmith-style progression
- Guardian + Arcanist + Blacksmith → possible Runic Bastion hidden qualification
- Duelist + Arcanist + Hunter → possible Arcane Stalker hidden qualification

## Endgame Classification Drift

Job identity becomes increasingly conceptual as the character grows.

**Hunter / Blacksmith / Soldier → Monster Tamer / Runeforger / Relic Seeker → Dragonslayer / Saint / Heretic / Tyrant → Gatekeeper / Worldwalker / Godslayer / Lawbreaker**

At extreme progression the Codex may no longer be describing a profession. It may be classifying what the character has become, creating a natural bridge into Titles and Authorities.

## Initial Three-Discipline Combat Triangle

### Guardian — Arming Sword & Shield

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

### Arcanist — Channeling Staff & Arcane Focus

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

### Duelist — Twin Blades

**Read opening → Slipstep/angle change → build Flow → create or exploit vulnerability → commit finisher → disengage before greed is punished.**

## First Region

The first shared region remains **the Greyfen March**, centered on **Hearthcross**. The first dungeon is **The Buried Gate**, whose first boss is the **Gatebound Hob**.

Hearthcross is now also the first place to test Jobs socially and institutionally. A Hunter, Blacksmith, Scholar, Priest, Smuggler, or other active Job should be able to produce different interactions even when the characters share the same combat Discipline.

## Origins & Opening Experience

Origin and Background remain separate:

- **Origin:** how did you enter this world?
- **Background:** who were you before that happened?

The first two complete opening paths are **The Stranded** and **The Invited**. Both converge on Hearthcross while retaining different Skills, social circumstances, perception lenses, and narrative flags.

Otherworlders may eventually prove unusually flexible at perceiving, retaining, swapping, and combining Job Imprints through the Divine Codex, but native characters remain capable of deep mastery and rare culturally specific progression.

## Combat Architecture

Combat uses three formal layers:

1. **Foundation Actions** — movement, dodge, interaction, traversal, camera/aim, and other reliable non-random actions.
2. **Weapon Arts** — reliable actions defined by weapon family, discipline, Skills, equipment mastery, and item evolution.
3. **Codex Manifestations** — rotating exceptional options such as Techniques, Spells, Reactions, Stances, Summons, Miracles, and Authorities.

Prototype formula:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

## Visual Direction

**Ground the world before breaking it.**

Visual target: **stylized anime fantasy with softly stylized PBR environments and increasingly supernatural escalation**.

**Practical fantasy → refined supernatural craft → legendary manifestations → divine intervention → Authority-driven reality distortion.**

## Narrative Structure

The game uses a **sandbox-first living world with a discoverable core mystery**. The Core Mystery advances mainly through Story Revelations rather than a rigid quest chain.

## Living World Principle

**The world remembers what the player did, who benefited, who suffered, and how much time has passed.**

Faction reputation is organization-specific, and morality emerges through persistent behavior and consequences rather than a universal meter.

## Central Lore Mystery

**The gods gave me this system → the gods only control parts of it → the system predates the known gods → the Endless Dungeon and soul transfer are part of the same ancient architecture → why are souls crossing worlds at all?**

## Multiplayer Direction

**World persistence belongs to the host. Character persistence belongs to each player.**

A host loads their timeline and up to five visitors join with their own characters. Visitors retain Origin, Skills, Jobs, perception lens, progression, and secured rewards.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

## Next prototype target — Jobs + Multiclass Discovery in Hearthcross

Validate:

- Primary + Secondary Discipline
- one Active Job slot
- at least four ordinary Jobs
- at least one hidden Job
- one hidden Skill or manifestation
- Guardian + Duelist hybrid manifestation
- Arcanist + Duelist hybrid manifestation
- Guardian + Arcanist hybrid manifestation
- System Comprehension hiding/revealing qualification progress
- one mutually exclusive hidden path
- one qualification driven partly by negative conditions
- one Hearthcross interaction changed by active Job
- one Job-modified equipment evolution route
- solo and co-op builds using different combinations without one obvious best recipe

The goal is to prove that **multiclassing, Jobs, hidden progression, narrative identity, and hybrid manifestations create genuinely different characters from the same underlying combat systems**.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
