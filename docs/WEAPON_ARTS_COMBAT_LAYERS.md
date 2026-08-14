# Weapon Arts & Combat Layers

**Design Version: v0.2.10**

## Core Principle

**Weapons determine how you fight. Cards determine what extraordinary options you can manifest while fighting.**

Combat is built from three interacting layers so the player always has reliable actions while the Divine Codex remains the source of tactical variation, specialization, and supernatural escalation.

## Layer 1 — Foundation Actions

Foundation Actions are universal or near-universal actions that should not depend on drawing a card.

Typical Foundation Actions include:

- move
- camera / aim
- sprint
- dodge
- jump / traversal where appropriate
- interact
- lock-on / target handling
- basic contextual actions

Blocking is not universally guaranteed. Access may depend on equipment, weapon family, class, shield use, stance, or other character capabilities.

### Design Rule

A player should never become unable to move, evade, interact, or perform basic combat simply because their current Codex hand is unfavorable.

## Layer 2 — Weapon Arts

Weapon Arts are reliable combat actions granted by the equipped weapon family and modified by class discipline, equipment mastery, individual item traits, and evolution.

Weapon Arts are not random draws.

A weapon family defines a recognizable baseline combat vocabulary.

Example — Sword:

- Light Attack
- Heavy Attack
- Guard or Weapon Action where supported
- Advancing Slash
- Rising Cut
- Counterstep

Example — Bow:

- Basic Shot
- Aimed Shot
- Evasive Shot
- Power Draw
- Marking Shot

Example — Shield:

- Guard
- Shield Bash
- Intercept
- Brace / Fortify actions where supported

These names are illustrative, not final content.

## Weapon + Discipline + Mastery

A weapon should not behave identically for every character.

The intended model is:

**Weapon Family + Class Discipline + Equipment Mastery = Weapon Moveset**

Examples:

- Guardian + Longsword emphasizes protection, counters, interception, and Guard generation.
- Swordmaster + Longsword emphasizes timing, chains, mobility, and finishers.
- Spellblade + Longsword emphasizes elemental channeling and magical follow-ups.

This allows weapon identity to remain strong while class identity changes how the weapon is expressed.

## Equipment Evolution Must Change Play

Evolving equipment should alter more than statistics.

Example:

Old Tower Shield

- Shield Block
- Shield Bash
- Intercept

may evolve into Bulwark of the Fallen Gate:

- Fortified Block
- Gatebreaker
- Hold the Line

Evolution can change Weapon Arts, animations, resource interactions, tags, timing windows, defensive geometry, or synergy conditions.

## Layer 3 — Codex Manifestations

The Active Codex supplies rotating manifestations that create exceptional options beyond the reliable weapon vocabulary.

Manifestations can include:

- Techniques
- Spells
- Reactions
- Stances
- Summons
- movement abilities
- transformations
- counters
- team-combo enablers
- buffs/debuffs
- utility
- miracles
- Authorities

The current hand should create tactical opportunities without replacing basic play.

## Weapon–Codex Interaction

Cards should frequently interact with baseline attacks and Weapon Arts.

Example — Flame Edge

> Your next three compatible weapon attacks gain Fire and build Ignite.

Example — Perfect Reversal

> After a successful Counterstep, transform this manifestation into Execution Cut for a short window.

Example — Guardian's Advance

> Your next Advancing Slash grants Guard to allies you pass.

Example — Crescent Form

> Enter a Stance. Heavy attacks become wide arcs until the Stance ends.

The ideal result is that the player does not stop fighting in order to “play cards.” Manifestations alter and expand the action combat already underway.

## Weapon Sets

Prototype direction: support up to **two equipped weapon sets**.

Weapon swapping provides a second reliable combat vocabulary and should be meaningful rather than mandatory constant bar-swapping.

Examples:

- Sword + Shield → defense/control
- Greatsword → pressure/burst
- Bow → ranged precision
- Staff → magical control

Cards may explicitly react to swapping.

Example — Adaptive Warrior

> When you change Weapon Set, Manifest a compatible Technique.

Example — Momentum

> After changing Weapon Set, your next Technique gains a temporary benefit.

Exact swap timing, cooldown, animation commitment, and in-combat restrictions remain Prototype Defaults.

## Five-Slot Active Hand

The current real-time prototype direction remains a five-slot manifested hand.

Keyboard defaults can map slots to `1–5`.

Controller should support a fast five-slot modifier scheme and an optional radial selection scheme for accessibility and preference.

The control action should target a hand slot rather than a permanent skill:

- ActivateCardSlot(0)
- ActivateCardSlot(1)
- ActivateCardSlot(2)
- ActivateCardSlot(3)
- ActivateCardSlot(4)

When a card leaves a slot, a replacement can enter that same slot without changing the player's input mapping.

## Card Draw as Combat Tempo

Prototype preference: test whether deck cycling can replace or reduce traditional cooldown dependence.

Possible model:

1. A manifestation is used.
2. It leaves the active hand according to its deck rules.
3. A replacement manifests in that slot.
4. The used card eventually returns through discard/reshuffle/recovery rules unless Exhausted or otherwise restricted.

Cooldowns may still exist where necessary, but should not automatically be the default solution for every ability.

## Combo and Transformation Design

A card slot can become part of the combo language.

Example:

Sword Combo I → Sword Combo II → Sword Combo III

or:

Brace → Perfect Guard → Counterstrike

or:

Fire Rune → Ignite Rune → Detonate

Transformations should be visually obvious and preserve control-slot consistency.

## Targeting Families

Every combat manifestation should use a standardized targeting family where possible:

- Instant
- Current Target
- Aim / Projectile
- Ground Target
- Directional
- Area Around Self
- Channel
- Contextual Reaction

This standardization supports keyboard/mouse, controller, networking, UI, AI prediction, and content authoring.

## Multiplayer Readability

Weapon Arts and manifestations must remain readable in 1–6 player combat.

Priority order:

1. Threat readability
2. Player control response
3. Ally synergy recognition
4. Ability spectacle

No individual build should require visual effects so large or opaque that other players cannot understand encounter mechanics.

## Prototype Questions

- exact number of Weapon Arts per family
- whether Weapon Arts consume stamina, class resources, or neither
- weapon-swap timing and restrictions
- how much a class may replace a weapon family's baseline moveset
- whether every weapon family has a defensive action
- whether deck cycling alone provides enough ability pacing
- how Stances interact with weapon swapping
- how companions use Weapon Arts
- how dual-wielding is represented
- whether off-hand items independently contribute actions

## Locked Combat Architecture

1. Foundation Actions are reliable and non-random.
2. Weapon Arts are reliable actions defined by equipment and character training.
3. Codex Manifestations are rotating exceptional options.
4. Weapon family, class discipline, and mastery combine to shape movesets.
5. Equipment evolution can change actions, not only statistics.
6. The five-slot hand should be usable without stopping movement.
7. Cards should interact with baseline combat rather than replace it.
8. Two weapon sets are a Prototype Default worth testing.
9. Deck cycling should be tested as a primary ability-tempo mechanism.
10. Combat must remain readable at six-player scale.
