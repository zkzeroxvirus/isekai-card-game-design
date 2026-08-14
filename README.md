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

**v0.2.15 — Arcanist Ranged/Magic Combat Package**

The second fully specified prototype discipline is **Arcanist**, paired with **Channeling Staff & Arcane Focus**.

Arcanist is a mobile ranged magical-control discipline built around aim, spatial setup, projectile shaping, compact Sigils, elemental/status interaction, and converting successful preparation into **Attunement**.

### Reliable Arcanist weapon package

Baseline actions:

- **Arc Bolt** — quick aimable magical projectile.
- **Focused Lance** — chargeable precision projectile with higher commitment and weak-point pressure.
- **Focus Guard** — brief directional magical ward; useful against selected projectiles and magical bursts but intentionally less stable than Guardian's shield.

Reliable Weapon Arts:

- **Sigil Cast** — place a compact magical anchor that can modify projectiles and be transformed by manifestations.
- **Arc Step** — magical repositioning that interacts with nearby Sigils.
- **Disrupting Pulse** — close-range interruption tool, especially useful against empowered or magical actions.
- **Threaded Shot** — precision projectile that gains additional properties when fired through a Sigil.

### Discipline mechanic — Attunement

Attunement is earned through successful magical sequencing rather than passive regeneration. Sources include threading attacks through Sigils, consuming prepared effects, exploiting weaknesses, and interrupting empowered magical actions.

Attunement can then strengthen higher-impact manifestations and magical Weapon Art interactions.

### First five Arcanist manifestations

1. **Ember Rune** — transforms a Sigil into a Fire property source that builds Burning.
2. **Detonate Sigil** — consumes a prepared Sigil for a property-dependent area effect.
3. **Mana Thread** — temporary stance that improves projectile/Sigil interaction.
4. **Gravitic Snare** — compact control field that slows and draws lighter enemies inward.
5. **Arc Lance** — Attunement-powered precision finisher that rewards Burning, Marked, Shocked, Frosted, Exposed, and other compatible setup states.

The key magic principle is:

**Magic should shape the battlefield, not merely replace arrows with colored projectiles.**

## Prototype Disciplines

### Guardian

**Arming Sword & Shield**

**Read threat → Guard/Intercept/Interrupt → build Resolve → convert defense into counter-pressure.**

Guardian tests active defense, physical protection, stagger, melee timing, same-slot card transformations, and frontline co-op support.

### Arcanist

**Channeling Staff & Arcane Focus**

**Position → place/shape Sigils → thread or control → build Attunement → convert setup into magical payoff.**

Arcanist tests ranged aiming, ground targeting, magical spatial control, elemental/status interactions, controller placement ergonomics, and VFX readability.

Neither discipline should require the other. Their shared status vocabulary should create optional co-op synergies.

## First Region

The first shared region is **the Greyfen March**, centered on **Hearthcross**. The first dungeon is **The Buried Gate** and its first boss is the **Gatebound Hob**.

Gatebound Hob now serves as a shared combat benchmark:

- Guardian must distinguish blockable, interruptible, and dodge-required attacks.
- Arcanist must maintain useful range, place Sigils under pressure, control adds/hazards, and avoid static casting.
- Both disciplines can contribute to shared status and Exposed windows.

After the boss, the party reaches the true Buried Gate and receives the first shared Story Revelation:

**The Gate recognizes the party in some way, but does not fully open.**

## Origins & Opening Experience

Origin and Background are separate concepts:

- **Origin:** how did you enter this world?
- **Background:** who were you before that happened?

The first two complete opening paths are **The Stranded** and **The Invited**. Both converge on Hearthcross while retaining different Skills, social circumstances, perception lenses, and narrative flags.

Both Guardian and Arcanist can be discovered organically or through formal instruction depending on Origin and Background.

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

## Next prototype target — Guardian + Arcanist in the Buried Gate

Validate both combat extremes against the same content:

- Sword/Shield active defense and Staff/Focus ranged magic before Codex access
- Guardian Resolve and Arcanist Attunement
- Weak/Solid/Perfect Guard timing
- aimable Arc Bolt and Focused Lance
- Sigil placement and Threaded Shot geometry
- five-slot Active Codex hands
- Brace → Perfect Guard transformation
- Ember Rune → Detonate Sigil setup/payoff
- Gravitic Snare crowd-control readability
- Guardian/Arcanist cross-status synergy
- Gatebound Hob under solo and co-op pressure
- **Gatewarden Shield** and **Gate-Echo Staff** equipment evolution hooks
- keyboard/mouse and controller targeting
- magical VFX readability at 1–6 players

The next combat-content decision should add a **third discipline with a different movement/resource profile**, giving the prototype a three-point comparison rather than two variations on the same pattern.

## License

TBD. All game names, terminology, mechanics documentation, setting text, and assets should be treated as project material until a license is selected.
