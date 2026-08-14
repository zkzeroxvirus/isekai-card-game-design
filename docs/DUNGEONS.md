# Dungeon Framework

Version: **v0.1.0**

## Core Principle

Infinite dungeon scaling should create increasingly complex combinations of rules, not merely larger enemy health totals.

A generated dungeon can be described as:

**Biome + Depth Tier + Enemy Families + Room Set + Affixes + Dungeon Modifiers + Boss + Dungeon Laws**

## Dungeon Run Structure

A run is a sequence or map of connected rooms. The player should regularly make route choices involving risk, information, recovery, and reward.

### Room Categories

- Combat
- Elite
- Boss
- Event
- Treasure
- Merchant
- Rest Site
- Shrine
- Puzzle
- Hazard
- Class Event
- Anomaly
- Secret Room

## Biomes

Biomes define encounter identity, presentation, likely enemy families, hazards, loot themes, and event pools.

Prototype examples:

- Verdant Ruins
- Ashen Citadel
- Crystal Caverns
- Drowned Archive
- Hollow Kingdom
- Celestial Stair
- Abyssal Wilds

## Depth

Dungeon Depth is a persistent measure of proven progression.

Depth can influence:

- enemy baseline stats
- enemy ability complexity
- elite frequency
- number of enemy affixes
- room hazards
- encounter compositions
- boss mutations
- treasure rarity
- reward multipliers
- number or severity of Dungeon Laws

## Depth Milestones

Prototype milestone philosophy:

- **Depth 1–9:** base rules
- **Depth 10+:** elites become standard dungeon features
- **Depth 25+:** enemy affixes expand
- **Depth 50+:** boss mutations
- **Depth 100+:** corrupted/anomalous rooms
- **Depth 200+:** multiple enemy affixes become common
- **Depth 500+:** Dungeon Laws become major run-defining rules

These are conceptual milestones, not locked values.

## Enemy Affixes

Affixes modify enemies with reusable behaviors.

Examples:

- Armored
- Burning
- Vampiric
- Swift
- Reflective
- Regenerating
- Explosive
- Summoner
- Phasing
- Enraged

Affixes must be legible and previewable where practical.

## Boss Mutations

Boss mutations alter encounter behavior rather than merely increasing values.

Examples:

- additional phase
- altered summon pattern
- environmental hazard
- extra reaction window
- transformed damage type
- modified victory condition

## Dungeon Modifiers

Dungeon Modifiers apply to a specific floor, region, run, or contract.

Examples:

- healing reduced
- merchants more expensive
- elites more frequent
- fire damage enhanced
- fewer rest sites
- greater treasure chance
- cards Exhaust on first use

Risk-enhancing modifiers should usually provide a corresponding reward incentive.

## Dungeon Laws

Dungeon Laws are high-impact rules that alter fundamental assumptions of the run.

Examples:

### Law of Blood
Healing also interacts with Bleed or sacrifice mechanics.

### Law of Silence
The first Spell played each turn is Sealed or weakened.

### Law of Giants
Enemies gain substantially more Health but become easier to Stagger.

### Law of Mirrors
The first card played each turn is copied or echoed by an enemy effect.

### Law of Greed
Treasure rewards increase, but retreat is disabled.

### Design Rule
A Dungeon Law must:

1. be clearly communicated before it can punish the player,
2. meaningfully change deck/route decisions,
3. have at least some build archetypes that can exploit or mitigate it,
4. not create unavoidable losses for otherwise legal characters.

## Scaling Model

Numerical scaling should use controlled curves and caps where needed. At higher depths, a larger percentage of difficulty should come from:

- more complex enemy combinations
- affix interactions
- resource pressure
- altered encounter rules
- dungeon laws
- smarter sequencing requirements

rather than raw HP/damage inflation alone.

## Dungeon Completion

A dungeon can end through:

- boss defeat
- extraction
- objective completion
- voluntary retreat where legal
- player defeat

Completion can unlock:

- next depth
- treasure rolls
- achievements
- hidden classes
- town resources
- new biomes
- boss records
- titles

## Endless Mode

A future Endless mode may continue until defeat or extraction. Endless scaling should use rotating law/affix packages and milestone rewards so the experience does not become a pure endurance check.
