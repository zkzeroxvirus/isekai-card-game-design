# First Combat Package — Guardian & Sword/Shield

**Design Version: v0.2.14**

## Purpose

This document defines the first complete playable combat package for the opening prototype.

It is intentionally designed against the Greyfen March, Hearthcross onboarding, and The Buried Gate rather than as an abstract class document.

The package must prove the full chain:

**Origin → Background → Skill → Weapon Arts → Discipline Mechanic → Codex Manifestations → Mastery → Equipment Evolution → Multiplayer Synergy**

## Prototype Discipline — Guardian

**Fantasy:** Stand where the danger is worst, control space, protect allies, and turn successful defense into offensive momentum.

Guardian is not a passive MMO tank. It should remain active and mobile, with strong solo viability and meaningful offensive options.

### Core Identity

Guardian rewards:

- reading enemy telegraphs
- physically positioning between threats and allies
- blocking or deflecting at the right time
- controlling enemy movement
- converting defense into counter-pressure
- creating safe windows for teammates

### Discipline Mechanic — Resolve

Guardian builds **Resolve** by successfully answering danger.

Prototype Resolve gains:

- well-timed blocks
- intercepting attacks aimed at allies
- staggering an enemy during an attack windup
- surviving heavy impacts while Guarding
- certain Guardian manifestations

Resolve is spent by stronger Guardian manifestations or used to enhance Weapon Arts.

### Design Rule

Resolve should reward successful defensive play, not standing still while holding a block button.

Passive damage absorption should generate little or no Resolve compared with active timing and positioning.

## Starting Skills

A character entering Guardian training should normally have or begin developing:

- **Swordsmanship I**
- **Shield Handling I**
- **Combat Awareness I**

Guardian qualification later develops through Skills such as:

- Shield Mastery
- Interception
- Resolve
- Battle Sense
- Formation Fighting

Origin and Background can change which of these are already known.

## Prototype Weapon Package — Arming Sword & Shield

This package represents a one-handed sword paired with a shield.

It should feel reliable, readable, and versatile without being mechanically bland.

### Foundation Actions

The player retains:

- movement
- sprint
- dodge
- jump/traversal
- interact
- camera/aim
- lock-on where appropriate

### Baseline Weapon Actions

#### Light Attack — Sword Cut

Fast, low-commitment sword strike.

A short chain can vary direction and timing but should remain predictable.

#### Heavy Attack — Driving Cut

Slower committed attack with stronger stagger and Guard-pressure value.

Can be charged modestly if prototype feel supports it.

#### Weapon Action — Guard

Raise the shield and defend a forward arc.

Guard consumes a defensive resource or stamina under pressure rather than functioning as unlimited invulnerability.

Perfectly timed Guard windows provide stronger effects than passive guarding.

## Reliable Weapon Arts

Weapon Arts are always available while the set is equipped and are not drawn from the Codex.

### 1. Advancing Slash

A short forward step into a controlled sword cut.

**Purpose:** close small gaps without replacing normal movement.

**Guardian modification:** striking an enemy currently targeting an ally grants a small amount of Resolve.

### 2. Shield Bash

A compact shield strike with strong interrupt/stagger value and modest damage.

**Purpose:** punish telegraphed attacks and disrupt lighter enemies.

**Guardian modification:** interrupting an active attack grants bonus Resolve.

### 3. Intercept

Quickly step toward a nearby ally or designated point and raise the shield during the movement.

**Purpose:** establish the Guardian fantasy through physical positioning rather than aggro rules.

**Guardian modification:** blocking an attack intended for another character during Intercept grants significant Resolve.

### 4. Counterstep

A short defensive footwork action that shifts position and creates a narrow counter window.

If an enemy attack misses or is deflected during the window, the next Sword Cut gains improved stagger.

**Purpose:** prevent the weapon package from becoming stationary shield play.

## Prototype Guard Model

Guard should have three qualitative outcomes:

### Weak Guard

The player blocks but mistimes or poorly angles the defense.

- higher stamina/Guard strain
- no Resolve bonus
- possible chip damage depending on attack type

### Solid Guard

The attack is properly faced and absorbed.

- normal defensive cost
- small Resolve gain for meaningful attacks

### Perfect Guard

A narrow timing window around impact.

- reduced defensive cost
- increased Resolve
- stronger stagger resistance or enemy recoil
- may qualify Codex reactions or transformations

The exact frame window remains a Prototype Default.

## Five-Card Starter Manifestation Package

This is a test hand package, not the final Guardian deck list.

The cards are deliberately chosen to touch different parts of the combat architecture.

### 1. Brace

**Category:** Reaction / Technique

**Targeting:** Instant

For a short window, greatly improve Guard stability. A successful block during the window transforms Brace into **Perfect Guard** in the same hand slot.

#### Perfect Guard

For a short follow-up window, activating the slot performs an empowered defensive response that reduces impact and generates Resolve.

If the triggering attack was heavy, Perfect Guard can briefly expose the attacker.

**Prototype purpose:** test same-slot card transformation and defensive timing.

### 2. Shield Counter

**Category:** Technique

**Targeting:** Current Target / Directional

Spend Resolve to deliver a powerful shield-and-sword counter.

Deals increased stagger to an enemy recently interrupted, blocked, or Perfect Guarded.

**Prototype purpose:** prove defense-to-offense conversion.

### 3. Guardian's Advance

**Category:** Technique

**Targeting:** Directional

Empower the next Advancing Slash.

The movement gains greater interruption resistance and grants temporary Guard to allies passed through or standing close to the endpoint.

**Prototype purpose:** test a manifestation modifying a reliable Weapon Art rather than replacing it.

### 4. Hold Fast

**Category:** Stance

**Targeting:** Area Around Self

Enter a short stance that improves resistance to stagger and causes successful Shield Bashes and Perfect Guards to create a small defensive pulse for nearby allies.

Movement remains possible but sprinting and weapon swapping may break the stance.

**Prototype purpose:** test co-op support that emerges from active frontline play rather than healing spam.

### 5. Severing Riposte

**Category:** Technique / Finisher

**Targeting:** Current Target

A committed sword strike that gains bonus effect against **Exposed**, **Staggered**, or otherwise vulnerable enemies.

If the target is Burning, Shocked, Frosted, Marked, or afflicted by another compatible ally-applied status, Severing Riposte gains an additional synergy effect rather than simply raw damage.

**Prototype purpose:** test cross-player combo recognition and encourage Guardian participation in team offense.

## Starter Deck Expansion Candidates

After the first five manifestations are proven, Guardian can expand toward approximately fifteen class manifestations.

Candidate families:

- interception
- counters
- ally Guard
- formation control
- stagger
- enemy displacement
- defensive Stances
- shield throws or supernatural shield techniques
- taunt-like challenge effects that do not depend on artificial threat tables
- vow-based abilities
- counterattacks
- protective Miracles at advanced progression

## No Mandatory Aggro Table

Guardian should not depend on MMO-style threat generation as its identity.

Enemy attention can be influenced through:

- proximity
- body blocking
- attacks
- control effects
- challenge-type abilities
- AI priorities
- protecting vulnerable allies

But standard encounters should remain physically understandable without invisible threat arithmetic being the primary mechanic.

## Greyfen Encounter Fit

### Greyfen Goblin Skirmishers

Guardian tests:

- projectile facing
- protecting weaker allies
- closing distance through Advancing Slash
- interrupting retreating or attacking goblins

### Goblin Bruisers

Guardian tests:

- heavy telegraph recognition
- Perfect Guard
- Shield Bash interruption
- Resolve generation

### Mirehounds

Guardian tests:

- rapid target switching
- positional protection
- avoiding being surrounded
- Counterstep

### Dungeon-Altered Vermin

Guardian tests:

- crowd pressure
- area control
- maintaining mobility while guarding

### Gatebound Hob

The first boss should deliberately include:

- a heavy strike that strongly rewards Perfect Guard
- a charge or displacement attack that can be Intercepted or redirected
- an exposed window created by stagger or successful counterplay
- an add or ally-pressure moment where Hold Fast matters
- at least one attack that should be dodged rather than blocked, proving Guard is not the answer to everything

## First Cross-Player Synergy Test

Prototype example:

1. Guardian interrupts the Gatebound Hob with Shield Bash.
2. Another player applies Burning with a Spell.
3. The boss becomes Exposed.
4. Guardian uses Severing Riposte.
5. The game recognizes both the defensive setup and ally status contribution.

The combat HUD should communicate the synergy clearly without flooding the screen with text.

## Mastery Examples

### Shield Bash Mastery

**Learned:** basic interrupt tool.

**Practiced:** reduced recovery after a successful interrupt.

**Refined:** choose a branch.

- **Crushing Bash** — increased stagger and armor pressure.
- **Guardian Bash** — successful interrupts briefly grant nearby ally Guard.
- **Runic Bash** — can inherit a compatible elemental or magical property from equipment.

### Intercept Mastery

Possible evolution conditions include:

- block attacks aimed at allies
- prevent ally knockdowns
- protect low-health allies
- intercept elite or boss attacks

Possible evolved form:

**Hold the Line** — Intercept creates a short protective zone at the endpoint after a successful rescue.

## Equipment Evolution Example

### Hearthcross Militia Shield

Early properties:

- reliable Guard
- basic Shield Bash
- modest stability

Mastery path can eventually produce:

### Gatewarden Shield

Visual changes:

- repaired Greyfen iron
- reinforced rim
- subtle Buried Gate geometric motif after dungeon attunement

Gameplay changes:

- Perfect Guard against heavy attacks stores a temporary **Gate Charge**
- next Shield Bash can spend Gate Charge for increased stagger
- Intercept has improved Guard coverage

This establishes equipment evolution as a mechanical and visual transformation.

## Origin Interaction Examples

### The Stranded

Guardian can emerge organically through survival behavior.

A player who repeatedly protects another survivor, blocks for civilians, or uses improvised shields may receive early Shield Handling or Protective Impulse recognition before formal Guardian training.

### The Invited

The summoning faction may deliberately test shield aptitude and identify Guardian potential through structured training.

The player reaches similar mechanics through a completely different narrative lens.

## Control Intent

The weapon package must remain comfortable while the five-card hand is active.

The player should be able to:

- move
- Guard
- dodge
- Light/Heavy attack
- use Weapon Arts
- activate manifestations

without entering menus or stopping camera control.

Exact bindings remain Prototype Defaults and should be validated on keyboard/mouse and controller.

## Prototype Success Criteria

The package succeeds if:

1. Sword/Shield feels functional before any cards are available.
2. Guardian rewards timing and positioning rather than passive blocking.
3. Resolve is understandable without excessive HUD complexity.
4. The five manifestations change combat decisions without replacing Weapon Arts.
5. Same-slot transformation feels intuitive.
6. Guardian remains enjoyable solo.
7. Guardian contributes meaningful co-op support without becoming mandatory.
8. The Gatebound Hob meaningfully tests the package.
9. Equipment mastery visibly changes the moveset.
10. Players can understand all of the above during active 1–6 player combat.

## Locked Prototype Principles

1. Guardian is the first fully specified discipline for the playable prototype.
2. Arming Sword & Shield is the first fully specified weapon package.
3. Resolve is earned primarily through successful active defense.
4. Guard has Weak, Solid, and Perfect outcomes.
5. Guardian uses physical interception and space control rather than relying on MMO threat tables.
6. Weapon Arts remain reliable and non-random.
7. Starter manifestations include Brace, Shield Counter, Guardian's Advance, Hold Fast, and Severing Riposte.
8. Guardian manifestations should frequently modify or capitalize on Weapon Arts.
9. The first boss must require both blocking and dodging so defense has meaningful limits.
10. This package becomes the template for the next prototype disciplines.