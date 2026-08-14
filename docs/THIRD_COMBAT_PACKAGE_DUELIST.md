# Third Combat Package — Duelist & Twin Blades

**Design Version: v0.2.16**

## Purpose

This document defines the third complete playable combat package for the opening prototype.

It is designed to sit between Guardian and Arcanist in combat range and responsibility:

- Guardian proves active defense and frontline control.
- Arcanist proves ranged magical control and setup.
- Duelist proves high-mobility melee pressure, positional chaining, and combo exploitation.

The package must also serve as the first serious multiclass bridge between the two existing disciplines.

## Prototype Discipline — Duelist

**Fantasy:** Read openings, move through danger rather than away from it, maintain pressure through precise footwork, and convert brief vulnerabilities into explosive melee chains.

Duelist is not a button-mashing rogue. It should reward timing, target selection, flank creation, recovery discipline, and knowing when to disengage.

### Core Identity

Duelist rewards:

- staying inside effective melee range without becoming stationary
- attacking around enemy windups and recovery windows
- crossing through or around targets to change angle
- exploiting Exposed, Staggered, Marked, Burning, Shocked, or otherwise prepared enemies
- chaining Weapon Arts together without losing camera control
- using movement offensively
- disengaging before greed turns into punishment

## Discipline Mechanic — Flow

Duelist builds **Flow** by maintaining clean offensive rhythm.

Prototype Flow gains:

- striking shortly after a successful dodge, deflect, or positional evade
- hitting from a new angle after a movement Weapon Art
- attacking an Exposed, Staggered, or Marked target
- completing varied attack sequences without repeating the same action excessively
- crossing through an enemy with a compatible Weapon Art and landing the follow-up

Flow decays if the player disengages for too long, whiffs repeatedly, or takes heavy interruption.

Flow is spent to extend combos, enhance mobility, reduce recovery on selected actions, or empower finishers.

### Design Rule

Flow should reward **clean tempo**, not raw attack speed.

The ideal Duelist player looks deliberate even when moving quickly.

## Starting Skills

A character entering Duelist training should normally have or begin developing:

- **Blade Handling I**
- **Footwork I**
- **Combat Awareness I**

Duelist qualification later develops through Skills such as:

- Dual Weapon Mastery
- Precision
- Evasion
- Battle Rhythm
- Weak-Point Reading
- Counter Fighting

Origin and Background can change which are already known.

## Prototype Weapon Package — Twin Blades

The prototype package uses two short swords or long knives with a matched combat grip.

The weapon family emphasizes speed, directional movement, short recoveries, and angle changes without becoming weightless.

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

#### Light Attack — Alternating Cuts

Fast alternating strikes with modest forward drift.

A short chain should feel responsive but still have readable recovery windows.

#### Heavy Attack — Cross Sever

A committed crossing strike using both blades.

Higher stagger/weak-point pressure than the light chain, but punishable if used carelessly.

#### Weapon Action — Deflect

Perform a brief blade deflection window against compatible melee attacks.

Deflect is narrower and less forgiving than Guardian's Guard.

Successful timing reduces impact and can create a tiny counter opening, but heavy attacks, large creature strikes, area attacks, and many magical effects should simply overpower it.

This keeps Duelist defensive play timing-based and mobile without overlapping Guardian's identity.

## Reliable Weapon Arts

### 1. Passing Cut

Dash a short distance past or alongside the target and strike during the movement.

**Purpose:** offensive angle change.

Landing the attack from a meaningfully different angle than the previous hit grants Flow.

Passing Cut should never phase through arbitrary world geometry or bypass large collision volumes without explicit rules.

### 2. Rising Fang

A quick upward paired-blade strike with increased interruption against light enemies and good weak-point pressure.

**Purpose:** punish recovery windows and set up follow-ups.

Striking an Exposed or Staggered target grants bonus Flow.

### 3. Slipstep

A very short directional evade with low travel distance and fast recovery.

**Purpose:** combat footwork rather than full disengagement.

Successfully avoiding an attack with Slipstep primes the next light or Passing Cut for increased precision.

Slipstep should coexist with the universal dodge: normal dodge creates safety; Slipstep preserves offensive proximity.

### 4. Reversal Cut

A backward or lateral blade turn that attacks while changing facing.

**Purpose:** maintain pressure when an enemy rotates, retreats, or tries to track the Duelist.

If used shortly after Deflect or Slipstep, recovery is reduced and Flow gain is increased.

## Flow Model

Prototype Flow can use a small segmented meter rather than a large mana-like bar.

Possible structure:

- 0–4 Flow segments
- gains from clean timing and varied offensive actions
- selected actions spend 1–3 segments
- short grace period before decay begins

Exact values remain Prototype Defaults.

### Anti-Spam Rule

Repeating the same low-risk action should produce sharply reduced Flow gain.

Duelist should be strongest when alternating between attacks, movement, timing, and opportunity exploitation.

## Five-Card Starter Manifestation Package

### 1. Pursuit

**Category:** Technique / Enhancement

**Targeting:** Current Target

Empower the next Passing Cut or Reversal Cut.

The movement gains improved target tracking and the follow-up strike deals increased effect against Marked, Exposed, or retreating enemies.

If the empowered movement passes through an allied Sigil, elemental or magical properties may be inherited where compatible.

**Prototype purpose:** connect Duelist movement to Arcanist geometry.

### 2. Perfect Tempo

**Category:** Stance

**Targeting:** Instant

For a short duration, varied successful Weapon Arts build Flow faster, while repeating the same action does not.

At maximum Flow, Perfect Tempo transforms in the same hand slot into **Tempo Break**.

#### Tempo Break

Spend all Flow to perform a rapid multi-angle strike sequence around the current target.

The sequence should preserve player readability and avoid excessive cinematic camera takeover.

**Prototype purpose:** test same-slot transformation on an offensive class and reward varied action sequencing.

### 3. Open Vein

**Category:** Technique / Debuff

**Targeting:** Current Target

A precise committed strike that applies **Opened** to a vulnerable target.

Opened increases the effectiveness of the next compatible precision, stagger, or elemental follow-up rather than functioning as a generic damage multiplier.

If the target is already Exposed or Staggered, Open Vein applies a stronger version.

**Prototype purpose:** let Duelist create team opportunities rather than only consume them.

### 4. Echoing Steel

**Category:** Technique / Reaction

**Targeting:** Instant / Contextual

For a short window after a successful Deflect, Slipstep evade, or Perfect Guard performed by a nearby ally, activating this card performs an accelerated Reversal Cut or Passing Cut depending on movement input.

If triggered by an ally's Perfect Guard or magical interruption, gain a small amount of Flow.

**Prototype purpose:** create direct Guardian and Arcanist bridge opportunities.

### 5. Sever the Moment

**Category:** Technique / Finisher

**Targeting:** Current Target

Spend Flow to perform a high-commitment precision strike.

It gains additional effects based on the target's current state:

- **Exposed/Staggered:** increased weak-point pressure
- **Marked by Mana:** improved tracking/precision
- **Burning:** follow-through gains a brief fire edge
- **Shocked:** reduced target reaction/turn speed during the hit window
- **Opened:** consumes Opened for a stronger finisher effect

**Prototype purpose:** prove that shared status vocabulary creates flexible multiclass/team interactions.

## Starter Deck Expansion Candidates

After the first five manifestations are proven, Duelist can expand toward roughly fifteen discipline manifestations.

Candidate families:

- angle-changing attacks
- short-range pursuit
- precision debuffs
- stance chains
- counterattacks
- weapon throws with retrieval or reposition hooks
- Flow-preserving movement
- anti-ranged gap pressure
- ally-assisted finishers
- status exploitation
- brief decoy/afterimage effects
- wound/bleed-style pressure where appropriate
- dual-element blade imbuement through multiclassing
- high-risk execution chains

## Greyfen Encounter Fit

### Greyfen Goblin Skirmishers

Duelist tests:

- chasing mobile targets without overextending
- angle changes around cover
- Slipstep vs projectile/melee follow-ups
- Passing Cut through small openings

### Goblin Bruisers

Duelist tests:

- respecting heavy attacks that cannot be safely Deflected
- exploiting recovery after Guardian or self-created stagger
- using Rising Fang and Sever the Moment during openings

### Mirehounds

Duelist tests:

- target switching
- avoiding being surrounded
- short-range evasive footwork
- maintaining Flow under chaotic pressure

### Dungeon-Altered Vermin

Duelist tests:

- movement through clustered enemies
- avoiding overcommitted finishers
- using Reversal Cut to maintain awareness

### Gatebound Hob

The boss should support:

- Passing Cut angle opportunities during large windups
- a heavy attack that punishes Deflect and demands full dodge
- a recovery window after Guardian interruption
- Marked/Burning setup from Arcanist for Duelist finishers
- a positional hazard that punishes mindless circling
- a phase where Flow maintenance becomes difficult and disciplined disengagement matters

## First Three-Discipline Synergy Tests

### Guardian → Duelist

1. Guardian Perfect Guards a heavy attack.
2. Gatebound Hob becomes briefly Exposed.
3. Duelist triggers Echoing Steel from the ally defensive event.
4. Passing Cut changes angle and builds Flow.
5. Sever the Moment converts the opening into precision pressure.

### Arcanist → Duelist

1. Arcanist applies Marked by Mana through Threaded Shot.
2. Duelist uses Pursuit-enhanced Passing Cut.
3. Mark improves movement tracking and precision.
4. Duelist applies Opened.
5. Arcanist or Duelist can capitalize depending on hand state.

### Guardian → Arcanist → Duelist

1. Guardian creates an Exposed window.
2. Arcanist threads Ember Rune pressure and applies Burning/Marked.
3. Duelist enters with Pursuit.
4. Open Vein creates Opened.
5. Sever the Moment consumes the stacked opportunity.

This should feel like emergent cooperation, not a mandatory scripted rotation.

## First Multiclass Bridge Concepts

Duelist is the first discipline intended to expose obvious future hybridization paths.

### Guardian + Duelist

Possible hybrid identity: **Vanguard / Blade Warden**

Themes:

- defensive counters that preserve Flow
- shieldless interception through aggressive positioning
- protection through threat disruption
- Perfect Guard or Deflect transitions into movement attacks

### Arcanist + Duelist

Possible hybrid identity: **Spellblade**

Themes:

- Sigils imbue Passing Cut
- elemental blade states
- Arc Step transitions into melee chains
- Marked by Mana enables precision finishers
- mana-threaded weapon arcs

These are design hooks, not yet locked hidden classes.

## Mastery Examples

### Passing Cut Mastery

**Learned:** short angle-changing dash attack.

**Practiced:** reduced recovery after successful angle change.

**Refined:** choose a branch.

- **Hunting Cut** — improved pursuit against retreating/Marked targets.
- **Crosswind Cut** — stronger angle-change Flow generation and wider lateral control.
- **Spellthread Cut** — better inheritance from compatible Sigils or magical weapon effects.

### Slipstep Mastery

Possible evolution conditions:

- evade attacks without leaving melee range
- counterattack immediately after Slipstep
- avoid elite/boss attacks at close range
- maintain high Flow through repeated danger windows

Possible evolved form:

**Ghost Step** — a perfectly timed Slipstep briefly suppresses enemy target tracking and empowers the next positional strike.

## Equipment Evolution Example

### Hearthcross Twin Irons

Early properties:

- responsive light chain
- stable Deflect
- basic Passing Cut
- modest precision

Mastery and Buried Gate attunement can produce:

### Gate-Split Blades

Visual changes:

- matching Greyfen steel blades
- dark geometric inlays on opposing blade faces
- brief mirrored glyph flare when Flow reaches maximum

Gameplay changes:

- changing attack angle stores a temporary **Split Mark**
- alternating left/right positional attacks strengthens the next Reversal Cut
- striking through a compatible Sigil can grant one blade its property for a short duration

## Origin Interaction Examples

### The Stranded

Duelist may emerge from survival behavior centered on improvised blades, evasive close-range fighting, protecting mobility, and learning to exploit small openings rather than overpowering enemies.

### The Invited

Structured assessment may identify unusual coordination, footwork, or dual-weapon aptitude and funnel the character into formal Duelist training.

## Control Intent

The package must remain comfortable while moving quickly.

The player should be able to:

- maintain camera control during Passing Cut
- choose Slipstep direction reliably
- keep normal dodge distinct from Slipstep
- understand Deflect timing without visual ambiguity
- activate the five-slot hand without losing movement
- read Flow without staring at the HUD

Auto-facing and target assistance should support, not replace, directional intent.

## Multiplayer Readability Rules

Duelist introduces rapid movement that can become visually noisy.

Prototype rules:

- short travel distances
- restrained afterimages
- strong start/end silhouettes
- no repeated teleport-style disappearance for basic movement
- finishers should not lock the camera for long sequences
- ally effects should clearly signal when Exposed, Marked, Opened, or similar states become usable

## Prototype Success Criteria

The package succeeds if:

1. Twin Blades feel functional before Codex cards appear.
2. Duelist feels clearly different from Guardian and Arcanist.
3. Flow rewards varied timing and positioning rather than attack spam.
4. Slipstep and universal dodge have distinct jobs.
5. Deflect is useful without becoming a smaller Guardian Guard.
6. Passing Cut improves angle play without becoming uncontrollable dash spam.
7. Starter manifestations deepen the Weapon Art loop rather than replace it.
8. Duelist can both create and exploit team openings.
9. Guardian + Duelist and Arcanist + Duelist both suggest natural multiclass identities.
10. Movement remains readable in 1–6 player combat.

## Locked Prototype Principles

1. Duelist is the third fully specified discipline for the playable prototype.
2. Twin Blades are the third prototype weapon package.
3. Flow rewards clean varied offensive rhythm, positional changes, and opening exploitation.
4. Slipstep is offensive footwork and remains distinct from universal dodge.
5. Deflect is narrower and less stable than Guardian Guard.
6. Starter manifestations are Pursuit, Perfect Tempo → Tempo Break, Open Vein, Echoing Steel, and Sever the Moment.
7. Duelist can create team opportunities through Opened rather than only consume ally setup.
8. Duelist deliberately bridges Guardian and Arcanist multiclass concepts.
9. Rapid melee movement must remain readable at six-player scale.
10. Guardian, Arcanist, and Duelist now form the initial three-discipline combat triangle for the v0.3.0 prototype.
