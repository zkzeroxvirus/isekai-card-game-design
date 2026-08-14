# Card Categories and Anatomy

Version: **v0.1.0**

## 1. Card Anatomy

Every playable card should define the following fields where applicable:

- **Name**
- **Card Type**
- **Source**
- **Class / Discipline**
- **Cost**
- **Target**
- **Rules Text**
- **Keywords**
- **Tags**
- **Rarity**
- **Upgrade Path**
- **Destination Zone**
- **Flavor Text** (optional)

## 2. Primary Card Types

### Technique
Physical or martial action.

Examples: sword attacks, shield maneuvers, archery, grapples, mobility skills.

### Spell
Magical action powered by arcane, elemental, divine, spiritual, or occult systems.

### Reaction
A card that may be played in response to a defined trigger.

Examples: parry, dodge, counterspell, retaliation.

### Stance
A persistent combat mode that changes future actions or rules.

Stances normally enter **In Play** rather than Discard.

### Summon
Creates a creature, spirit, construct, familiar, or temporary allied unit.

### Skill
Utility action that does not cleanly fit Technique or Spell.

Examples: scouting, traps, stealing, analysis, crafting tricks.

### Item
Consumable or equipment-linked action represented as a card.

### Ultimate
High-impact limited-access ability. Usually carries a special requirement, cooldown, charge condition, or strict deck limit.

### Curse
A detrimental card that enters the player's deck, hand, discard, or other zone.

### Blessing
A beneficial supernatural card or persistent effect, usually acquired during runs.

### Event Card
A card used outside normal combat resolution for events, exploration, or dungeon interactions.

## 3. Card Source Categories

Card **Type** describes what the card does. Card **Source** describes where it came from.

Sources include:

- **Class** — learned from a class
- **Hybrid** — unlocked by a specific multiclass interaction
- **Neutral** — usable without a class requirement
- **Origin** — granted by character origin
- **Equipment** — granted by equipped gear
- **Treasure** — created or granted by a persistent treasure
- **Dungeon** — temporary card acquired during a run
- **Achievement** — unlocked through achievement conditions
- **Title** — associated with a title
- **Monster** — learned, stolen, copied, or adapted from enemies
- **Town** — unlocked through a building or NPC
- **Unique** — special one-off card with explicit acquisition rules

## 4. Functional Categories

Cards may carry one or more functional tags for design and search purposes.

### Offense
- Direct Damage
- Multi-Hit
- Execute
- Damage Over Time
- Area Damage
- Scaling Damage
- Retaliation

### Defense
- Guard
- Barrier
- Dodge
- Parry
- Damage Reduction
- Immunity
- Healing
- Recovery

### Control
- Stun
- Root
- Silence
- Disarm
- Taunt
- Slow
- Push/Pull
- Intent Manipulation

### Economy
- Draw
- Resource Generation
- Resource Conversion
- Cost Reduction
- Card Creation
- Retrieval

### Deck Manipulation
- Scry
- Tutor/Search
- Discard
- Exhaust
- Recycle
- Copy
- Transform
- Upgrade
- Seal

### Scaling / Engine
- Combo
- Charge
- Stack Builder
- Trigger Engine
- Persistent Growth
- Finisher

### Summoning
- Summon
- Command
- Sacrifice
- Companion Buff
- Token Creation

### Exploration
- Lockpicking
- Scouting
- Survival
- Diplomacy
- Crafting
- Treasure Detection
- Hazard Interaction

## 5. Damage/Theme Tags

Tags should enable synergy without requiring every tag to be a separate rules subsystem.

Prototype examples:

- Physical
- Fire
- Frost
- Lightning
- Arcane
- Radiant
- Shadow
- Poison
- Bleed
- Spirit
- Earth
- Wind
- Water
- Beast
- Undead
- Dragon
- Construct
- Weapon
- Shield
- Unarmed
- Projectile

## 6. Rarity

### Prototype Default Rarities

- **Common** — fundamental building blocks
- **Uncommon** — stronger specialization and synergy
- **Rare** — build-defining or unusually efficient
- **Epic** — highly specialized, difficult to acquire, or major engine pieces
- **Legendary** — unique or near-unique effects that can reshape a build

Rarity is not intended to mean "strictly stronger." Higher rarity should generally mean greater complexity, specialization, scarcity, or build impact.

## 7. Class Card Categories

Each class should ideally contain cards across several internal roles:

- **Foundation** — basic class identity
- **Generator** — creates class resources or states
- **Payoff** — rewards successful setup
- **Defense** — survival tool
- **Utility** — flexibility and deck manipulation
- **Bridge** — deliberately interacts with other classes/tags
- **Finisher** — strong payoff for a developed engine
- **Signature** — iconic class-defining card

This prevents a class from becoming a one-dimensional pile of attacks.

## 8. Hybrid Cards

### Core Rule
Hybrid cards require two or more defined disciplines, classes, tags, or mastery conditions.

Example:

**Molten Aegis**  
Source: Hybrid — Knight/Pyromancer  
Type: Stance  
Effect concept: Whenever you gain Guard, apply Burn to an enemy.

Hybrid cards should generally do something neither parent class does as efficiently alone.

## 9. Card Upgrades

Cards may have one or more upgrade branches.

Prototype upgrade dimensions:

- lower cost
- increased magnitude
- additional target
- new keyword
- changed destination zone
- altered trigger
- conversion to another damage/status type
- increased synergy with another class
- specialization branch

### Content Guideline
Whenever feasible, upgrades should create **choices**, not only `+2 damage`.

Example:

**Shield Bash**
- Base: Deal damage. Gain Guard.
- Upgrade A — **Crushing Bash**: More damage; applies Stagger.
- Upgrade B — **Fortress Bash**: Less damage; much more Guard.

## 10. Card Ownership and Persistence

Distinguish three concepts:

- **Known Card** — permanently unlocked for deck construction.
- **Equipped Card** — currently included in the character's deck.
- **Run Card** — temporary card added during the current dungeon run.

A card may exist in more than one state depending on acquisition rules.

## 11. Card Template

```text
Name:
Type:
Source:
Class/Discipline:
Rarity:
Cost:
Target:
Tags:
Keywords:

Rules Text:

Upgrade A:
Upgrade B:

Design Role:
Notes:
```
