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
13. **Magic should shape the battlefield, not merely replace arrows with colored projectiles.** Ranged magic should use positioning, geometry, preparation, statuses, and spatial control.
14. **Depth changes rules, not only numbers.** Infinite dungeon scaling uses enemy affixes, hazards, mutations, and Dungeon Laws alongside controlled stat growth.
15. **Discovery is progression.** Hidden classes, titles, equipment evolutions, recipes, divine permissions, system information, and dungeon phenomena reward experimentation.
16. **Knowledge is power.** Bestiary research and System Comprehension eventually expose deeper world rules.
17. **Failure creates consequences and stories.** Defeat can cause wounds, damaged equipment, injured companions, and lost unsecured loot without deleting developed characters.
18. **Multiplayer should feel like visiting another adventurer's world.** World persistence belongs to the host; character persistence belongs to each player.
19. **The power curve escalates dramatically.** Vulnerable outsider becomes a specialized veteran and eventually a system-breaking legendary build.
20. **The gods do not necessarily own the system.** They can influence, administer, exploit, or misunderstand the deeper infrastructure behind the Divine Codex and Transference.
21. **Isekai progression fantasy is the tone.** The player gradually learns, masters, and eventually exploits the hidden rules of a new fantasy world.

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

**v0.2.16 — Duelist Mobile Melee Combat Package**

The third fully specified prototype discipline is **Duelist**, paired with **Twin Blades**.

Duelist fills the fast offensive melee role between Guardian and Arcanist. Its resource, **Flow**, is built through clean varied offensive rhythm: angle changes, successful close-range evasions, exploiting Exposed/Marked/Staggered states, and chaining different Weapon Arts without falling into repetitive spam.

### Reliable Duelist weapon package

Baseline actions:

- **Alternating Cuts** — fast paired-blade light chain.
- **Cross Sever** — higher-commitment precision/stagger heavy attack.
- **Deflect** — a narrow timing-based melee defense that is deliberately less stable than Guardian Guard.

Reliable Weapon Arts:

- **Passing Cut** — move past or alongside a target while striking, rewarding real angle changes.
- **Rising Fang** — fast upward paired strike that punishes vulnerable enemies.
- **Slipstep** — very short evasive footwork used to stay in offensive range rather than disengage.
- **Reversal Cut** — attack while changing facing, with bonuses after Deflect or Slipstep.

### Discipline mechanic — Flow

Flow rewards varied timing and positioning rather than attack speed. The prototype uses a small segmented meter, likely 0–4 segments, with gains reduced sharply when the player repeats the same low-risk action.

Flow can be spent to extend pressure, reduce recovery on selected actions, or empower finishers.

### First five Duelist manifestations

1. **Pursuit** — empowers Passing Cut/Reversal Cut and interacts with Marked, Exposed, retreating enemies, and compatible Sigils.
2. **Perfect Tempo → Tempo Break** — offensive same-slot transformation; varied Weapon Arts build Flow until the card becomes a multi-angle finisher.
3. **Open Vein** — applies **Opened**, creating a team opportunity rather than only consuming one.
4. **Echoing Steel** — reactive mobility attack triggered by Deflect, Slipstep, or nearby ally defensive/magical interruption events.
5. **Sever the Moment** — Flow-powered finisher that changes payoff based on Exposed, Marked, Burning, Shocked, or Opened states.

## Initial Three-Discipline Combat Triangle

### Guardian — Arming Sword & Shield

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

Role emphasis: active defense, physical protection, stagger, space control.

### Arcanist — Channeling Staff & Arcane Focus

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

Role emphasis: ranged setup, battlefield geometry, magical control, status interaction.

### Duelist — Twin Blades

**Read opening → Slipstep/angle change → build Flow → create or exploit vulnerability → commit finisher → disengage before greed is punished.**

Role emphasis: mobility, precision, opening creation/exploitation, offensive tempo.

None of these disciplines should be mandatory. The purpose of the triangle is to prove that one shared Weapon Art + Active Codex architecture can support genuinely different playstyles.

## First Multiclass Bridges

Duelist establishes two obvious future hybrid paths without locking their final class names.

### Guardian + Duelist

Potential direction: **Vanguard / Blade Warden**

- defensive counters that preserve Flow
- aggressive interception
- protection through disruption and positioning
- Guard/Deflect transitions into movement attacks

### Arcanist + Duelist

Potential direction: **Spellblade**

- Sigils imbue movement attacks
- elemental blade states
- Arc Step transitions into melee chains
- Marked by Mana enables precision finishers
- mana-threaded weapon arcs

These remain future hybridization hooks rather than confirmed hidden classes.

## First Region

The first shared region is **the Greyfen March**, centered on **Hearthcross**. The first dungeon is **The Buried Gate** and its first boss is the **Gatebound Hob**.

Gatebound Hob now serves as the shared benchmark for all three prototype disciplines:

- Guardian distinguishes blockable, interruptible, and dodge-required attacks.
- Arcanist maintains range, shapes Sigils, controls pressure, and avoids static casting.
- Duelist changes angles, preserves melee pressure, exploits recovery windows, and learns when Deflect is insufficient.

After the boss, the party reaches the true Buried Gate and receives the first shared Story Revelation:

**The Gate recognizes the party in some way, but does not fully open.**

## Origins & Opening Experience

Origin and Background are separate concepts:

- **Origin:** how did you enter this world?
- **Background:** who were you before that happened?

The first two complete opening paths are **The Stranded** and **The Invited**. Both converge on Hearthcross while retaining different Skills, social circumstances, perception lenses, and narrative flags.

Guardian, Arcanist, and Duelist can each be discovered organically or through formal instruction depending on Origin, Background, and behavior.

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

A host loads their timeline and up to five visitors join with their own characters. Visitors retain Origin, Skills, perception lens, progression, and secured rewards.

## Power Curve

**Vulnerable Adventurer → Competent Specialist → Synergy-Driven Veteran → System-Breaking Legendary Build**

## Next prototype target — Three Disciplines in the Buried Gate

Validate the initial combat triangle against the same content:

- Guardian Resolve, Arcanist Attunement, and Duelist Flow
- Sword/Shield, Staff/Focus, and Twin Blades baseline combat before Codex access
- Guard, Focus Guard, Deflect, Slipstep, and universal dodge having clearly different jobs
- five-slot Active Codex hands for all three disciplines
- same-slot transformations on Guardian and Duelist
- Sigil geometry and ground targeting
- angle-changing melee under keyboard/mouse and controller input
- shared states: Exposed, Staggered, Burning, Marked by Mana, Shocked, Frosted, and Opened
- Guardian → Duelist, Arcanist → Duelist, and three-way synergy sequences
- Gatebound Hob under solo and mixed-party pressure
- **Gatewarden Shield**, **Gate-Echo Staff**, and **Gate-Split Blades** equipment evolution hooks
- 1–6 player combat readability

If these three packages all feel strong alone and create optional synergies together, the next major combat-design step should shift from isolated class kits to **multiclass rules, deck construction, and hybrid manifestations**.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
