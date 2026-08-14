# Mechanics and Keyword Framework

Version: **v0.1.0**

## 1. Design Goals

Mechanics should be:

- readable on cards,
- composable across classes,
- expressive enough to support multiclass engines,
- scalable into high dungeon depths,
- and consistent enough to avoid bespoke exceptions.

Keywords are reserved terms with stable rules meanings. Tags are descriptive labels used for synergy and filtering.

## 2. Core Combat Values

### Health
When Health reaches 0, that unit is defeated unless a rule prevents it.

### Action
Primary per-turn card resource.

**Prototype Default:** Restore to 3 Action at the start of each player turn.

### Guard
Temporary defense that absorbs incoming damage before Health.

**Prototype Default:** Guard is removed at the start of the owner's next turn unless an effect says it is retained.

### Barrier
Persistent or specialized protection distinct from Guard. Barrier rules may vary by source, but should always be stated explicitly.

## 3. Core Damage Rules

Damage follows this default sequence:

1. Determine base damage.
2. Apply attacker modifiers.
3. Apply target modifiers.
4. Apply prevention/reduction.
5. Remove Guard or other applicable shields.
6. Apply remaining damage to Health.
7. Resolve `On Damage`, `On Hit`, and defeat triggers as applicable.

### Hit vs Damage

- **Hit** means an attack successfully resolves against a target, even if all damage is prevented.
- **Take Damage** means Health or a qualifying defensive layer actually loses value due to damage.

This distinction should remain stable for trigger design.

## 4. Prototype Core Keywords

### Exhaust
After this card resolves, place it in the Exhaust zone instead of the Discard pile. It normally cannot be drawn again this combat.

### Retain
This card remains in hand at end of turn instead of being discarded.

### Prepared
Move this card to the Prepared zone. Prepared cards remain available under their stated play conditions without occupying normal hand cycling.

### Fleeting
If this card remains in hand at end of turn, Exhaust it.

### Ethereal
If this card remains in hand at end of turn, Exhaust it. Used primarily for temporary or magical cards; distinction from Fleeting may be revisited during prototyping.

### Innate
Begin combat with this card in the opening hand, subject to hand limits and setup rules.

### Generate
Create the specified card or resource from outside the current deck.

### Discover
Choose one option from a generated subset of eligible cards/effects.

### Scry X
Look at the top X cards of your deck and choose any of them to discard. Return the rest to the top in any order unless an effect says otherwise.

### Draw X
Move X cards from the top of the Deck to the Hand, reshuffling the Discard pile if necessary and legal.

### Discard
Move a card from Hand to Discard without playing it.

### Recycle
Move a card from Discard to Deck or Hand as specified by the effect.

### Seal
Move or mark a card as inaccessible until its seal condition ends.

### Copy
Create a temporary copy of a specified card. Unless otherwise stated, copies inherit the current printed/modified state of the copied card.

### Transform
Replace a card with another card or form according to the effect.

## 5. Combat Status Families

Statuses should be built from a small number of reusable behavior families.

### Damage-over-Time
Examples: Burn, Bleed, Poison.

### Control
Examples: Stun, Root, Silence, Disarm.

### Vulnerability
Effects that increase damage or reduce defenses.

### Stat Modification
Temporary increases or reductions to attack, defense, speed, resource gain, etc.

### Mark
A status that serves primarily as a target for another mechanic.

### Charge/Counter
A stack used as a resource or threshold rather than a direct buff/debuff.

## 6. Prototype Named Statuses

### Burn
At a defined timing point, take Fire damage based on Burn stacks, then reduce Burn by a defined amount.

**Prototype Default:** At end of affected unit's action cycle, take damage equal to Burn, then reduce Burn by 1.

### Bleed
Triggers bonus damage when the affected unit performs certain strenuous actions or when struck by compatible effects.

**Prototype Default:** Precise trigger model is open; avoid printing final Bleed cards until selected.

### Poison
Persistent damage that is harder to remove than Burn but may tick more slowly.

**Prototype Default:** Exact timing open.

### Stagger
Represents destabilization. At a threshold, the unit becomes vulnerable, loses an action, or suffers a break effect.

**Prototype Default:** Threshold model to be playtested.

### Weak
Reduces outgoing damage.

### Vulnerable
Increases incoming damage.

### Taunt
Restricts or strongly biases eligible targets according to the encounter's targeting rules.

### Silence
Prevents specified Spell actions while active.

### Root
Prevents movement/repositioning effects while active.

## 7. Trigger Vocabulary

Use these standardized trigger forms:

- **When Played** — immediately after card declaration/cost payment as defined by resolution rules.
- **After Playing** — after the card's main effect resolves.
- **When Hit** — when a hit resolves against this unit.
- **When Damaged** — when damage is actually dealt through applicable prevention.
- **On Defeat** — when this unit is defeated.
- **Start of Turn**
- **End of Turn**
- **Start of Combat**
- **End of Combat**
- **On Draw**
- **On Discard**
- **On Exhaust**
- **On Gain Guard**
- **On Apply [Status]**
- **On Consume [Resource]**

Avoid casual synonyms in rules text when a standardized trigger exists.

## 8. Resource Mechanics

Classes may have secondary resources beyond Action.

Examples:

- Rage
- Mana
- Focus
- Combo
- Faith
- Heat
- Momentum
- Souls
- Marks
- Charges

### Content Guideline
Secondary resources should answer at least one of these questions:

- What does this class build toward?
- What does this class spend tactically?
- What risk does this class manage?
- What makes its turn sequencing distinct?

Avoid adding a resource solely for flavor.

## 9. Engine Mechanics

### Generator
Creates a resource, card, stack, status, summon, or board state.

### Converter
Turns one resource/state into another.

### Multiplier
Makes an existing resource or trigger produce more value.

### Payoff
Consumes or rewards accumulated setup.

### Finisher
Ends or dramatically swings a combat when an engine succeeds.

Healthy classes should usually contain several of these roles rather than only direct value cards.

## 10. Reaction Timing

Reactions require a printed trigger.

Prototype priority:

1. Trigger occurs.
2. Mandatory reactions enter the queue.
3. Player may use eligible optional Reactions.
4. Resolve queued reactions in chosen order unless an effect defines priority.
5. Resume the interrupted effect.

Nested reaction depth should be limited during prototyping if excessive chains slow play.

## 11. Stacking Rules

Unless otherwise stated:

- Numerical statuses with the same name stack by value.
- Duration-based statuses refresh or add duration only if their individual rule says so.
- Identically named persistent Stances do not stack unless explicitly allowed.
- Unique effects cannot have more than one active copy.

## 12. Mechanical Design Rule

Every recurring mechanic added to the game should document:

1. How it is generated.
2. How it is consumed or removed.
3. What counterplay exists.
4. What classes/tags can interact with it.
5. How it behaves at extreme stack values.
6. Whether dungeon scaling can modify it safely.
