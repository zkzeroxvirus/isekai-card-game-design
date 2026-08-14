# Core Rules Framework

Version: **v0.2.0**

## 1. Game Structure

### Core Rule
The game alternates between two major states:

1. **Town Phase** — persistent preparation, upgrades, character management, crafting, class training, equipment mastery, companion management, research, treasure configuration, and progression.
2. **Dungeon Run** — a self-contained expedition where the player fights, explores, gains temporary upgrades, learns about the world, and attempts to reach an exit or defeat a boss.

The macro loop is:

**Town → Build Character/Party → Accept Contract or Choose Expedition → Enter Dungeon → Gain Temporary Power & Knowledge → Defeat/Retreat/Extract → Resolve Consequences & Rewards → Town**

## 2. Character Structure

A character contains:

- Origin
- Attributes
- Health
- Class loadout
- Skill Mastery
- Class Mastery
- Deck
- Equipment and Equipment Mastery
- Treasures
- Titles
- Achievements
- Guild Rank / certifications
- Knowledge / Bestiary records
- Companion relationships
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
Classes are modular learned disciplines rather than permanent character identities.

A class provides some combination of:

- class mechanic
- cards
- passive traits
- keyword access
- equipment permissions
- class-specific upgrade choices
- mastery rewards
- hybrid/multiclass interactions

A class should feel mechanically distinct because of what it teaches the character, not only because its cards share an aesthetic.

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
- Alternate skill evolutions
- Equipment evolution paths

## 4. Skills and Mastery

### Core Rule
Cards representing learned abilities may possess persistent **Skill Mastery**.

Skill Mastery can be earned through meaningful use, training, achievements, class objectives, or hidden conditions.

Mastery may unlock:

- alternate upgrades
- evolution branches
- associated passives
- Skill Family techniques
- hidden progression conditions

See [`SKILL_MASTERY.md`](SKILL_MASTERY.md).

## 5. Equipment

### Core Rule
Equipment is an active progression layer, not merely a stat container.

Equipment may:

- grant cards
- unlock techniques
- gain mastery
- gain or modify affixes
- evolve after conditions are met
- interact with Skill Mastery and classes

See [`EQUIPMENT_PROGRESSION.md`](EQUIPMENT_PROGRESSION.md).

## 6. Deck Construction

### Prototype Default

- Minimum deck size: **15 cards**
- Recommended range: **15–25 cards**
- Maximum copies of one non-signature card: **2**
- Signature/Legendary cards may use stricter limits.

### Core Rule
The character's **Known Card Pool** may be much larger than the equipped deck.

Progression should primarily expand options rather than forcing deck size inflation.

## 7. Party and Companions

### Core Rule
The player character owns the primary deck. Persistent companions contribute smaller Support Decks or visible support actions.

Companions are intended to add party dependence and tactical synergy without requiring the player to operate multiple full decks.

### Prototype Default

- 0–2 active companions
- 4–8 Support Cards per companion

Solo play remains a supported build path.

See [`COMPANIONS.md`](COMPANIONS.md).

## 8. Combat Loop

Combat is turn-based.

### Prototype Default Player Turn

1. Start of Turn triggers resolve.
2. Restore turn resources.
3. Draw to hand size.
4. Companion/support availability updates.
5. Player may play cards while able to pay costs.
6. End Turn effects resolve.
7. Enemy intent resolves.
8. Enemy End effects resolve.
9. Begin next player turn.

### Prototype Default Values

- Starting hand: **5 cards**
- Draw per turn: **5 cards** or refill to hand size, pending testing
- Primary turn resource: **3 Action**
- Maximum hand size: **10 cards**

When the draw pile is empty, shuffle the discard pile to create a new draw pile unless a rule prevents it.

## 9. Card Zones

The standard card zones are:

- **Deck** — cards waiting to be drawn
- **Hand** — currently playable cards
- **Discard** — used cards awaiting reshuffle
- **Exhaust** — cards removed for the current combat
- **Prepared** — cards intentionally held outside normal hand cycling
- **In Play** — persistent cards such as Stances, Summons, or ongoing effects
- **Sealed** — temporarily inaccessible cards

Not every class must interact with every zone.

## 10. Card Resolution

Unless a card states otherwise:

1. Declare card.
2. Choose legal targets.
3. Pay costs.
4. Trigger `On Play` effects.
5. Resolve card text from top to bottom.
6. Resolve reactions created by that effect.
7. Move the card to its destination zone.

If part of a card cannot resolve, resolve as much as legally possible unless the card states that all conditions are required.

## 11. Enemy Intent and Knowledge

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

The **amount and precision of information** may improve through Bestiary Knowledge.

Higher-depth enemies may obscure, distort, or alter intent through explicit dungeon rules rather than arbitrary hidden information.

See [`KNOWLEDGE_AND_DEFEAT.md`](KNOWLEDGE_AND_DEFEAT.md).

## 12. Encounter Outcomes

A combat ends when:

- all hostile enemies are defeated,
- an alternate encounter objective is completed,
- the party successfully escapes,
- or the player character is defeated.

Combat rewards may include:

- currency
- temporary cards
- card upgrades
- consumables
- equipment
- Skill Mastery
- Class Mastery
- materials
- knowledge
- treasure chances
- dungeon-specific resources

## 13. Guild and Contracts

The Adventurer Guild provides structured world progression through contracts, certifications, reputation, and rank.

Guild Rank is separate from Character Level and primarily unlocks opportunities rather than raw stats.

See [`GUILD_AND_RANK.md`](GUILD_AND_RANK.md).

## 14. Run Structure

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

Contracts can layer additional objectives onto a dungeon run.

## 15. Temporary vs Persistent Progression

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
- Skill Mastery
- Class Mastery
- unlocked classes
- equipment and Equipment Mastery
- Treasures
- achievements
- titles
- Guild Rank and certifications
- companion progression
- Bestiary/world knowledge
- town upgrades
- recipes
- account/world unlocks
- maximum dungeon depth

## 16. Defeat, Retreat, and Extraction

### Core Rule
A failed run should matter, but failure should not erase a developed character.

Normal defeat may cause:

- loss of unsecured dungeon rewards
- Wounds
- equipment damage
- companion Injuries
- contract or reputation consequences

Knowledge, major permanent unlocks, and previously secured progression normally survive.

Loot may be **Secured** or **Unsecured**, creating a push-your-luck decision between extraction and deeper exploration.

See [`KNOWLEDGE_AND_DEFEAT.md`](KNOWLEDGE_AND_DEFEAT.md).

## 17. Rules Priority

When rules conflict, use this hierarchy:

1. Explicit card or encounter text
2. Dungeon Law
3. Character/Class/Equipment/Treasure passive
4. Keyword rule
5. Core rules

Specific rules override general rules.

If two simultaneous effects conflict at the same priority, the active player chooses the order unless a card or encounter explicitly defines priority.

## 18. Golden Design Rules

**Build a character, not just a deck.**

**Levels expand capability. Mastery deepens identity. Knowledge reveals possibilities. Synergies create power.**

The player should begin by surviving the world's rules and eventually become powerful because they understand how to combine, exploit, and transcend them.
