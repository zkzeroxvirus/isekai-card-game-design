# Core Rules Framework

Version: **v0.1.0**

## 1. Game Structure

### Core Rule
The game alternates between two major states:

1. **Town Phase** — persistent preparation, upgrades, character management, crafting, class training, treasure configuration, and progression.
2. **Dungeon Run** — a self-contained expedition where the player fights, explores, gains temporary upgrades, and attempts to reach an exit or defeat a boss.

The macro loop is:

**Town → Build Character → Enter Dungeon → Gain Temporary Run Power → Defeat/Retreat/Die → Resolve Rewards → Town**

## 2. Character Structure

A character contains:

- Origin
- Attributes
- Health
- Class loadout
- Class mastery
- Deck
- Equipment
- Treasures
- Titles
- Achievements
- Persistent unlocks

### Prototype Default Attributes

- **Might** — physical power and heavy techniques
- **Finesse** — precision, speed, ranged and agile techniques
- **Mind** — arcane knowledge, calculation, spell shaping
- **Spirit** — faith, willpower, summoning, supernatural resilience
- **Vitality** — health, endurance, recovery

Attributes should create build identity but should not overpower card synergy.

## 3. Class System

### Core Rule
Classes are modular disciplines rather than permanent character identities.

A class provides some combination of:

- cards
- passive traits
- keyword access
- equipment permissions
- class-specific upgrade choices
- mastery rewards
- hybrid/multiclass interactions

### Prototype Default Class Loadout

A character begins with:

- 1 **Primary Class**
- 1 **Secondary Class**

Later progression may unlock additional Secondary or Specialization slots.

### Multiclassing

A character may build a legal deck using cards available through all equipped classes plus any neutral/universal cards.

Multiclassing should reward interaction rather than simple accumulation. Certain class combinations can unlock:

- Hybrid Cards
- Cross-Class Passives
- Hidden Classes
- Combo Keywords
- Alternate card upgrades

## 4. Deck Construction

### Prototype Default

- Minimum deck size: **15 cards**
- Recommended range: **15–25 cards**
- Maximum copies of one non-signature card: **2**
- Signature/Legendary cards may use stricter limits.

### Core Rule
The character's **Known Card Pool** may be much larger than the equipped deck.

Progression should primarily expand options rather than forcing deck size inflation.

## 5. Combat Loop

Combat is turn-based.

### Prototype Default Player Turn

1. Start of Turn triggers resolve.
2. Restore turn resources.
3. Draw to hand size.
4. Player may play cards while able to pay costs.
5. End Turn effects resolve.
6. Enemy intent resolves.
7. Enemy End effects resolve.
8. Begin next player turn.

### Prototype Default Values

- Starting hand: **5 cards**
- Draw per turn: **5 cards** or refill to hand size, pending testing
- Primary turn resource: **3 Action**
- Maximum hand size: **10 cards**

When the draw pile is empty, shuffle the discard pile to create a new draw pile unless a rule prevents it.

## 6. Card Zones

The standard card zones are:

- **Deck** — cards waiting to be drawn
- **Hand** — currently playable cards
- **Discard** — used cards awaiting reshuffle
- **Exhaust** — cards removed for the current combat
- **Prepared** — cards intentionally held outside normal hand cycling
- **In Play** — persistent cards such as Stances, Summons, or ongoing effects
- **Sealed** — temporarily inaccessible cards

Not every class must interact with every zone.

## 7. Card Resolution

Unless a card states otherwise:

1. Declare card.
2. Choose legal targets.
3. Pay costs.
4. Trigger `On Play` effects.
5. Resolve card text from top to bottom.
6. Resolve reactions created by that effect.
7. Move the card to its destination zone.

If part of a card cannot resolve, resolve as much as legally possible unless the card states that all conditions are required.

## 8. Enemy Intent

### Core Rule
Enemies should generally communicate intended actions before they occur.

Intent may reveal:

- target
- expected damage
- status application
- defense
- charging/channeling
- summon
- special mechanic

Higher-depth enemies may obscure, distort, or alter intent through explicit dungeon rules rather than arbitrary hidden information.

## 9. Encounter Outcomes

A combat ends when:

- all hostile enemies are defeated,
- an alternate encounter objective is completed,
- the player successfully escapes,
- or the player character is defeated.

Combat rewards may include:

- currency
- temporary cards
- card upgrades
- consumables
- equipment
- class mastery
- materials
- treasure chances
- dungeon-specific resources

## 10. Run Structure

A dungeon run is made of connected rooms or nodes.

Common room categories:

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

A player should frequently choose between safer routes and higher-value danger.

## 11. Temporary vs Persistent Progression

### Temporary Run Progression
Usually resets when the run ends:

- temporary cards
- temporary card upgrades
- temporary blessings
- run currencies
- temporary consumables
- temporary stat bonuses
- dungeon-specific effects

### Persistent Progression
Usually survives runs:

- known cards
- class mastery
- unlocked classes
- equipment
- treasures
- achievements
- titles
- town upgrades
- recipes
- account/world unlocks
- maximum dungeon depth

## 12. Defeat and Retreat

### Core Rule
A failed run should still produce some meaningful progress, but successful risk-taking should be more rewarding.

Potential retained rewards after defeat may depend on:

- extraction rules
- secured treasure
- insurance systems
- town upgrades
- achievements
- dungeon milestones

Exact loss rules remain a prototype question.

## 13. Rules Priority

When rules conflict, use this hierarchy:

1. Explicit card or encounter text
2. Dungeon Law
3. Character/Class passive
4. Keyword rule
5. Core rules

Specific rules override general rules.

If two simultaneous effects conflict at the same priority, the active player chooses the order unless a card or encounter explicitly defines priority.

## 14. Golden Design Rule

**Levels and progression expand options. Synergies create power.**

Raw numerical progression should support the player's growth fantasy without replacing deck construction, timing, and build interactions as the main source of strength.
