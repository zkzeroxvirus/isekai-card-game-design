# Second Combat Package — Arcanist & Staff/Focus

**Design Version: v0.2.15**

## Purpose

This document defines the second complete playable combat package for the opening prototype.

It is intentionally designed as a strong contrast to Guardian while using the same combat architecture:

**Origin → Background → Skill → Weapon Arts → Discipline Mechanic → Codex Manifestations → Mastery → Equipment Evolution → Multiplayer Synergy**

Guardian proves active defense and frontline control. Arcanist should prove that the same system also supports a ranged magical playstyle built around aiming, setup, spacing, elemental interaction, and battlefield control.

## Prototype Discipline — Arcanist

**Fantasy:** Read the battlefield, shape mana into repeatable magical forms, create favorable geometry, and turn preparation into precise bursts of power.

Arcanist is not a stationary turret and should not be built around endlessly casting from maximum range. It should reward movement, line-of-sight management, aim, setup, and intelligent use of magical zones.

### Core Identity

Arcanist rewards:

- maintaining useful range without abandoning the group
- aiming projectiles and placing effects deliberately
- creating Sigils that alter space
- exploiting elemental/status interactions
- repositioning before enemies collapse onto the caster
- sequencing Weapon Arts and Codex manifestations
- observing enemies and choosing the correct magical response

## Discipline Mechanic — Attunement

Arcanist builds **Attunement** by interacting successfully with magical patterns and prepared effects.

Prototype Attunement gains:

- striking an enemy through or near an active Sigil
- detonating or consuming a prepared magical effect
- exploiting an enemy elemental/status weakness
- successfully interrupting a magical or empowered enemy action
- certain Arcanist manifestations

Attunement is spent to strengthen selected manifestations, accelerate Sigil behavior, or empower Staff/Focus Weapon Arts.

### Design Rule

Attunement should reward successful magical sequencing, not passive waiting for mana to regenerate.

The player should feel that good setup creates more magical freedom.

## Starting Skills

A character entering Arcanist training should normally have or begin developing:

- **Mana Sensitivity I**
- **Arcane Handling I**
- **Focus Control I**

Arcanist qualification later develops through Skills such as:

- Mana Perception
- Elemental Channeling
- Sigilcraft
- Spell Shaping
- Arcane Theory
- Concentration

Origin and Background can change which of these are already known.

## Prototype Weapon Package — Channeling Staff & Arcane Focus

The prototype package uses a one-handed or compact channeling staff paired with an off-hand arcane focus.

The staff establishes reliable ranged magical actions. The focus governs shaping, placement, and controlled magical release.

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

#### Light Attack — Arc Bolt

Fire a fast, low-power magical projectile.

Arc Bolt should be aimable, readable, and useful for maintaining pressure without consuming Codex cards.

#### Heavy Attack — Focused Lance

Charge briefly and release a slower, more committed projectile with increased impact and weak-point pressure.

The player may release early for reduced effect.

#### Weapon Action — Focus Guard

Project a brief directional magical ward.

Focus Guard is weaker than a physical shield against sustained melee pressure but can efficiently answer certain projectiles, magical attacks, or telegraphed bursts.

Perfect timing can refract or destabilize compatible magic.

This action exists to keep the package from depending entirely on dodge while remaining clearly less defensively stable than Guardian.

## Reliable Weapon Arts

### 1. Sigil Cast

Place a small short-lived magical Sigil at the targeted ground location.

**Purpose:** establish the Arcanist's spatial-control language.

Base Sigils modestly empower allied Arcanist projectiles passing through them and can be modified by manifestations.

Only a limited number may exist simultaneously.

### 2. Arc Step

Perform a quick magical lateral or backward reposition.

**Purpose:** preserve spacing without replacing normal movement and dodge.

Arc Step gains additional distance if initiated near an active Sigil, consuming part of the Sigil's duration.

### 3. Disrupting Pulse

Emit a short cone or focused pulse from the arcane focus.

Deals low damage but strong interruption against lighter enemies and certain magical casts.

**Arcanist modification:** interrupting an empowered or magical action grants Attunement.

### 4. Threaded Shot

Fire a precise projectile that gains improved speed and effect when it passes through an active Sigil.

**Purpose:** make geometry and setup matter during reliable baseline combat.

A properly threaded shot can apply a brief **Marked by Mana** state used by later manifestations.

## Prototype Sigil Model

Sigils are small readable magical anchors rather than large permanent hazard fields.

Prototype properties:

- ground placed
- short duration
- limited simultaneous count
- visible to allies
- interact with selected projectiles/manifestations
- may be consumed, transformed, or detonated

### Design Rule

Sigils must remain readable in six-player combat. Their footprint should be compact and their visual language should communicate ownership and function without creating floor-effect clutter.

## Five-Card Starter Manifestation Package

### 1. Ember Rune

**Category:** Spell / Preparation

**Targeting:** Ground Target

Transform an active Sigil into an Ember Rune.

Projectiles passing through it gain Fire and build **Burning**. The Rune can later be consumed by compatible effects.

If no Sigil exists, Ember Rune creates a weaker temporary one at the target location.

**Prototype purpose:** test a manifestation modifying a reliable Weapon Art and establish elemental setup.

### 2. Detonate Sigil

**Category:** Spell / Technique

**Targeting:** Current Sigil / Ground Target

Consume a targeted Sigil or Rune and release an area burst.

The burst changes based on the Sigil's current property.

Ember Rune → fire burst and stronger Burning.

Future Sigils may produce control, frost, shock, healing, or utility outcomes.

Gain Attunement for striking at least one valid target with a deliberate detonation.

**Prototype purpose:** test setup-to-payoff gameplay.

### 3. Mana Thread

**Category:** Spell / Stance

**Targeting:** Instant

For a short duration, Threaded Shot and Focused Lance automatically inherit the property of the next compatible Sigil they pass through without consuming it.

Repeated successful threaded hits increase projectile stability and precision during the stance.

**Prototype purpose:** test a ranged stance that modifies reliable Weapon Arts rather than replacing them.

### 4. Gravitic Snare

**Category:** Spell / Control

**Targeting:** Ground Target

Create a compact distortion field that slows and subtly pulls light enemies toward its center.

Heavy enemies resist displacement but suffer reduced movement while inside.

Enemies already **Marked by Mana** are affected more strongly.

**Prototype purpose:** test battlefield control and team setup without hard crowd-control spam.

### 5. Arc Lance

**Category:** Spell / Finisher

**Targeting:** Aim / Projectile

Spend Attunement to fire a high-speed piercing magical lance.

Arc Lance gains a bonus effect against targets that are:

- Burning
- Marked by Mana
- Shocked
- Frosted
- Exposed
- otherwise affected by a compatible ally or Arcanist setup

If Arc Lance passes through an active Sigil, it inherits that Sigil's property before impact.

**Prototype purpose:** test precision burst, resource spend, and cross-player synergy.

## Starter Deck Expansion Candidates

After the first five manifestations are proven, Arcanist can expand toward approximately fifteen class manifestations.

Candidate families:

- elemental Sigils
- projectile shaping
- beam/channel effects
- short-range emergency magic
- mana barriers
- teleport anchors
- enemy debuffing
- area denial
- status conversion
- spell reflection/refraction
- prepared traps
- utility detection
- anti-magic
- ritual-style high-commitment effects
- advanced spatial manipulation

## Mana and Attunement

Arcanist should not become a traditional mana-bar class where the correct play is simply to wait for mana regeneration.

Prototype direction:

- basic Staff/Focus Weapon Arts remain broadly available
- manifestations may use normal Codex costs and selected Attunement spends
- expensive magical effects can require Attunement, preparation, or both
- mana-like resources may still exist, but should not replace the more interactive Attunement loop

Exact resource layering remains a Prototype Default.

## Greyfen Encounter Fit

### Greyfen Goblin Skirmishers

Arcanist tests:

- aim and projectile pressure
- controlling retreat lanes with Sigils
- using Gravitic Snare to disrupt skirmishing
- exploiting exposed ranged enemies

### Goblin Bruisers

Arcanist tests:

- maintaining range against pressure
- Arc Step timing
- detonating prepared Sigils as bruisers commit
- Focus Guard as a limited emergency response rather than a full solution

### Mirehounds

Arcanist tests:

- rapid spacing decisions
- avoiding tunnel vision while aiming
- compact control placement
- short-range Disrupting Pulse usage

### Dungeon-Altered Vermin

Arcanist tests:

- area control
- Sigil placement under swarm pressure
- controlled Detonate Sigil usage

### Gatebound Hob

The first boss should deliberately include:

- a ranged or magical attack that can be answered with Focus Guard timing
- a charge that forces Arc Step or normal dodge
- a vulnerability window where prepared Sigils and Arc Lance are valuable
- adds or hazards that reward Gravitic Snare
- movement patterns that punish static casting
- a dungeon anomaly that reacts visibly to Mana Sensitivity/System Comprehension

## First Cross-Player Synergy Tests

### Guardian + Arcanist

1. Guardian interrupts Gatebound Hob with Shield Bash.
2. Arcanist places Ember Rune and threads a projectile through it.
3. Burning is applied while the boss becomes Exposed.
4. Guardian can capitalize with Severing Riposte.
5. Arcanist can instead spend Attunement on Arc Lance.

This allows both disciplines to contribute to the same setup without requiring a fixed combo order.

### Arcanist + Any Future Status Build

Arcanist should naturally interact with statuses applied by other disciplines.

The goal is a shared combat vocabulary where **Burning, Marked, Exposed, Shocked, Frosted, Staggered**, and similar states create opportunities across class boundaries.

## Mastery Examples

### Sigil Cast Mastery

**Learned:** place a basic Sigil.

**Practiced:** improved placement speed or duration after successful threaded attacks.

**Refined:** choose a branch.

- **Stable Sigil** — longer duration and improved projectile threading.
- **Reactive Sigil** — creates a small effect when an enemy crosses its center.
- **Linked Sigil** — allows limited interaction between two placed Sigils.

### Arc Step Mastery

Possible evolution conditions:

- evade attacks with Arc Step
- reposition through/near Sigils
- avoid elite or boss abilities
- protect uninterrupted casting windows through movement

Possible evolved form:

**Phase Thread** — Arc Step briefly leaves a magical thread between start and endpoint that can modify the next projectile crossing it.

## Equipment Evolution Example

### Hearthcross Survey Staff

Early properties:

- reliable Arc Bolt
- stable Focused Lance
- one basic Sigil channel
- modest Focus Guard

Mastery and Buried Gate attunement can eventually produce:

### Gate-Echo Staff

Visual changes:

- repaired darkwood shaft
- Greyfen metal fittings
- geometric Buried Gate inlays
- faint shifting glyphs visible during Attunement gain

Gameplay changes:

- Threaded Shot through a Sigil stores a temporary **Echo Charge**
- next Detonate Sigil can spend Echo Charge for improved control or radius
- Focus Guard against anomalous/dungeon magic can reveal a brief directional trace toward the source

This establishes equipment evolution as both combat progression and world-lore discovery.

## Origin Interaction Examples

### The Stranded

Arcanist can emerge organically when a character with Mana Sensitivity or strong curiosity repeatedly interacts with Greyfen anomalies, magical debris, shrines, or dungeon architecture.

The first magical Skill may feel accidental before formal training begins.

### The Invited

The summoning faction may identify magical aptitude immediately and provide controlled Staff/Focus instruction.

The player's first Codex manifestation can then challenge the institution's assumptions about what their magic should look like.

## Control Intent

The player should be able to:

- move freely while using Arc Bolt
- aim Focused Lance
- place Sigils without opening a menu
- Arc Step while maintaining camera control
- activate five manifested cards
- identify active Sigils quickly

Ground-targeting must be fast enough for controller use and should support sensible aim assist or placement prediction without removing player intent.

## Multiplayer Readability Rules

Arcanist is the first major test of magical visual clutter.

Prototype limits:

- Sigils remain compact
- control fields use restrained opacity
- projectile trails prioritize direction clarity
- detonations communicate impact without obscuring enemy telegraphs
- allied Sigils remain distinguishable but do not require reading text during combat

## Prototype Success Criteria

The package succeeds if:

1. Staff/Focus feels functional before any Codex cards are available.
2. Arcanist feels meaningfully different from Guardian.
3. Aim and placement matter without becoming cumbersome on controller.
4. Sigils are useful without turning combat into stationary trap setup.
5. Attunement rewards active sequencing rather than passive regeneration.
6. The five manifestations alter baseline combat instead of replacing it.
7. Arcanist remains viable solo under pressure.
8. Guardian + Arcanist creates obvious but nonmandatory synergy.
9. Gatebound Hob meaningfully tests ranged movement, control, and magical timing.
10. Spell VFX remain readable in 1–6 player combat.

## Locked Prototype Principles

1. Arcanist is the second fully specified discipline for the playable prototype.
2. Channeling Staff & Arcane Focus is the first fully specified ranged/magic weapon package.
3. Attunement is earned primarily through successful magical sequencing and prepared-effect interaction.
4. Sigils are reliable Weapon Art anchors rather than cards by default.
5. Arc Bolt and Focused Lance provide dependable ranged offense outside the Codex.
6. Focus Guard provides limited magical defense but does not replace positioning or dodge.
7. Starter manifestations are Ember Rune, Detonate Sigil, Mana Thread, Gravitic Snare, and Arc Lance.
8. Arcanist manifestations should frequently transform or exploit Sigils and ranged Weapon Arts.
9. Guardian and Arcanist should share status/synergy vocabulary without becoming mutually required.
10. Arcanist is the prototype benchmark for aim, ground targeting, magical VFX readability, and ranged combat tempo.