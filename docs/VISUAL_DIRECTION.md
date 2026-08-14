# Visual Direction

**Design Version:** v0.2.9 — Visual Direction

## Core Visual Identity

The game uses **stylized anime fantasy with grounded environments and increasingly supernatural visual escalation**.

The visual target combines:

- anime-influenced character proportions and facial design
- believable fantasy materials and environments
- strong silhouettes and readable equipment
- restrained early-game supernatural effects
- increasingly extravagant late-game magic
- diegetic Divine Codex interface elements
- visible world-state and faction divergence

The intended look is **softly stylized PBR**, not full photorealism and not full cel shading.

The world should initially feel credible enough that divine, dungeon, Codex, and Authority phenomena can visibly break its normal rules.

---

## Visual Design Principles

### 1. Ground the world before breaking it

Early environments, equipment, settlements, monsters, and abilities should feel tangible and understandable.

As player power and knowledge increase, visual language may become increasingly impossible:

- floating geometry
- world-space glyphs
- spatial fractures
- altered lighting rules
- impossible materials
- environmental color suppression or inversion
- divine architecture
- Authority-driven reality distortion

Visual escalation should mirror progression escalation.

### 2. Readability outranks spectacle

Six-player combat, summons, enemies, projectiles, areas, cards, status effects, and telegraphs can create extreme visual density.

Effects must preserve:

- player silhouette readability
- enemy attack readability
- hazard visibility
- targeting clarity
- ally/enemy distinction
- important status recognition

Spectacle should intensify hierarchy rather than obscure gameplay.

### 3. Equipment progression must be visible

Equipment is a major progression system and should evolve visually as well as numerically.

Mastery, rarity, evolution, monster materials, divine influence, corruption, and Authority fragments may alter:

- silhouette
- materials
- rune patterns
- animation
- particle treatment
- geometry
- idle effects

The player should be able to recognize important equipment progression without opening a stat panel.

### 4. World state should be visually persistent

Settlements, faction territory, war damage, prosperity, corruption, religious influence, monster integration, and player rule should be represented in the physical world.

Visiting another player's world should produce immediate visual evidence that their timeline differs.

### 5. The Codex is supernatural, not a physical card deck

Cards shown to the player are interface manifestations of the soul-bound Active Codex.

Card presentation should avoid looking primarily like parchment collectible cards floating in the world.

The UI should instead feel like an elegant supernatural system combining:

- translucent layers
- geometric sigils
- subtle divine script
- class and source iconography
- animated borders
- manifestation effects
- rarity/source-specific treatment
- corruption or instability artifacts when appropriate

---

# Character Direction

## Proportions

Characters should use anime-influenced heroic proportions while remaining believable in full 3D.

Preferred traits:

- slightly idealized anatomy
- slightly enlarged or emphasized eyes
- simplified facial planes compared with photoreal humans
- readable hairstyles
- strong silhouettes
- expressive posing
- clear equipment shapes

Avoid:

- heavily exaggerated chibi proportions as the default
- photoreal scanned-human facial treatment
- extreme skin pore/detail emphasis
- proportions that make armor and weapon interaction physically implausible

## Faces

Faces should prioritize expression and identity over realism.

Target qualities:

- clean skin shading
- readable eyes and brows
- clear mouth shapes
- restrained subsurface/detail noise
- stylized hair clumping rather than individual realistic strands everywhere

The goal is anime influence without requiring strict 2D-anime imitation.

## Customization

Player customization should remain compatible with the art style.

Long-term character creation may support:

- body type
- face archetype
- skin tone
- eyes
- hair
- scars/marks
- tattoos or magical markings
- voice
- selected supernatural traits where lore allows

Customization should not compromise silhouette readability or animation quality.

---

# Environment Direction

## Overall Rendering

Environments use grounded fantasy materials with controlled stylization.

Preferred characteristics:

- readable material families
- slightly simplified texture noise
- deliberate color grouping
- strong atmospheric lighting
- stylized shape language where useful
- believable weather and time-of-day treatment

Avoid making every surface equally detailed or visually noisy.

## Early-Game World

Early spaces should emphasize vulnerability and scale:

- worn roads
- modest villages
- dangerous forests
- practical fortifications
- cold stone dungeons
- imperfect tools and construction
- patched equipment

The player should look small relative to the world.

## Late-Game World

Later spaces can increasingly expose deeper system architecture:

- impossible dungeon geometry
- floating structures
- divine monuments
- broken causality cues
- spaces that fold or repeat
- ancient system glyphs
- world-law anomalies
- visible boundaries between normal reality and Authority effects

---

# Equipment Visual Progression

A broad equipment escalation should follow this pattern.

## Early

- rough wood
- basic iron
- worn leather
- cloth wraps
- repaired gear
- practical adventuring equipment

## Mid

- refined metals
- class-specific silhouettes
- monster-material inserts
- etched runes
- crafted composite materials
- visible mastery modifications

## Late

- legendary silhouettes
- animated runes
- unusual materials
- floating components
- soul-reactive elements
- transformation states
- persistent aura treatment

## Mythic / Authority-Touched

- geometry that disobeys normal construction
- effects that alter surrounding space
- unusual shadow/light behavior
- material responses unavailable to normal equipment
- temporary world-rule visualization

Authority visuals should not be reducible to "more glow."

---

# Combat & VFX Hierarchy

VFX intensity communicates supernatural hierarchy.

## Mortal Technique

- strong physical motion
- controlled trails
- impact sparks/debris
- readable hit reaction
- minimal screen takeover

## Art / Advanced Skill

- stronger stylized trails
- brief glyphs or energy forms
- distinct class language
- more dramatic hit punctuation

## Spell

- clear magical construction
- elemental or conceptual identity
- readable projectile/area boundaries
- stronger environmental lighting response

## Evolved Ability

- recognizable transformation of the base technique
- signature animation or VFX motif
- greater spatial presence

## Blessing / Miracle

- sacred or higher-order visual grammar
- world-space symbols
- environmental response
- deliberate sense of intervention

## Authority

Authorities visually interact with **rules rather than only energy**.

Examples:

- Distance Authority fractures or removes perceived space between locations.
- Death Authority suppresses color, sound, or ambient motion around a target.
- Time Authority creates temporal echoes or duplicated motion states.
- Contract Authority manifests bindings, seals, names, or visible terms in space.

Authority use should feel qualitatively different from casting a larger spell.

---

# Combat Readability Rules

In multiplayer combat:

- enemy telegraphs must remain readable through allied VFX
- hostile ground effects require consistent boundary language
- allied persistent areas require a distinct but less dominant presentation
- boss mechanics take visual priority over player spectacle
- critical interrupt/counter windows require a consistent language
- summons should not obscure major targets
- camera-space effects should be brief and configurable

Accessibility settings should eventually support reduced flashes, reduced screen shake, reduced bloom, VFX density reduction, and alternative telegraph treatments.

---

# Divine Codex UI Direction

## General Identity

The Codex should feel like a supernatural translation layer between the soul and world law.

The interface may combine:

- translucent cards/panels
- geometric borders
- sigils
- elegant iconography
- luminous text accents
- layered depth
- brief manifestation animations

The interface should remain highly readable at combat speed.

## Card Presentation

A combat card should prioritize:

1. ability name
2. recognizable icon/silhouette
3. input binding
4. cost/resource state
5. targeting/timing state
6. critical tags or status information

Long descriptive text belongs primarily in menus, inspection, deckbuilding, and learning contexts rather than the live combat HUD.

## Lore-Driven UI Evolution

The Codex interface may reveal deeper metadata as the player gains knowledge.

Early presentation might expose only:

- name
- cost
- category
- basic effect

Later knowledge could reveal:

- manifestation classification
- origin/source signatures
- permission layer
- Authority dependencies
- corruption markers
- system conflicts
- sealed metadata

UI progression can therefore become narrative progression.

## Corrupted / Forbidden Presentation

Forbidden or unstable manifestations may use controlled interface abnormalities such as:

- broken borders
- displaced glyphs
- unreadable fragments
- desynchronized animation
- partially hidden metadata

These effects must remain readable and should not rely on aggressive glitching that becomes irritating during normal play.

---

# Faction Visual Language

Every major faction should have a defined visual grammar covering:

- architecture
- heraldry
- silhouettes
- equipment
- materials
- magical motifs
- iconography
- environmental dressing
- NPC presentation

Faction territory should be recognizable before the player reads a nameplate.

Faction changes can spread physically through settlements and regions as their influence rises or falls.

---

# Settlement & Timeline Divergence

Town progression should create visible transformations rather than only menu upgrades.

Possible visual states include:

## Prosperous / Heroic

- repaired structures
- markets
- gardens
- public monuments
- open trade
- guild expansion
- civilian density

## Militarized / Authoritarian

- checkpoints
- towers
- banners
- barracks
- walls
- patrol density
- restricted districts

## Occult / Forbidden

- ritual structures
- sealed buildings
- unusual lighting
- black-market spaces
- undead or supernatural labor where appropriate
- corrupted or repurposed dungeon material

## Mercantile

- warehouses
- caravans
- foreign architecture
- dense signage
- expanded roads
- merchant compounds

These are examples, not fixed morality templates. Settlement visuals should emerge from faction influence, upgrades, consequences, resources, and player choices.

---

# Monster Direction

Monsters should prioritize silhouette, behavior readability, and progression identity over generic realism.

A base creature family should support visually meaningful variants rather than simple recolors.

A goblin family, for example, might visually diverge into:

- scavenger
- vanguard
- beastmaster
- rune-user
- corrupted variant
- Authority-touched variant

Variants should communicate role through:

- body language
- equipment
- silhouette
- animation
- materials
- visible supernatural traits

Early creatures should remain dangerous without needing enormous size or exaggerated spectacle.

---

# Color & Lighting Direction

The default world should use controlled, grounded color rather than constant maximum saturation.

Supernatural systems introduce stronger color and contrast as needed.

This supports progression:

- mundane gear feels mundane
- rare materials stand out
- legendary equipment feels exceptional
- divine effects feel intrusive
- Authorities can intentionally violate normal color logic

Lighting should carry substantial atmospheric weight in forests, dungeons, settlements, weather, and divine spaces.

---

# Camera Direction

The default camera is **third-person action RPG**, moderately close but adjustable.

Goals:

- character and equipment remain visually important
- players retain enough awareness for six-player combat
- AoEs and telegraphs remain readable
- targeting can tighten framing without becoming a permanent shooter-style over-the-shoulder camera

Expected features:

- exploration camera
- combat camera behavior
- optional lock-on
- aim/targeting adjustments
- ability-specific framing where safe
- configurable camera shake

Avoid frequent forced cinematic camera takeover during active multiplayer combat.

---

# Narrative Presentation

The game should not depend on expensive full cinematics for every story interaction.

Preferred hierarchy:

- systemic in-world conversations for routine content
- strong camera composition and character staging for important scenes
- portrait/dialogue support where efficient
- expressive poses and facial animation
- full cinematic treatment reserved for major story, boss, divine, and era-transition moments

Narrative presentation must account for multiplayer presence and host-owned world state.

---

# Production Guardrails

The visual direction should remain achievable for a system-heavy game.

Prioritize reusable systems for:

- modular character equipment
- faction material sets
- settlement state changes
- VFX families
- card/Codex templates
- dungeon kits
- monster family variants

Avoid making every asset bespoke when a modular visual language can produce equivalent identity.

Stylization should reduce unnecessary asset-detail burden rather than simply adding another rendering layer on top of photoreal assets.

---

# Visual Prototype Target

The technical proof of concept should also validate a miniature art target containing:

- one stylized player character
- one grounded fantasy arena/environment
- one basic equipment set
- one evolved equipment visual
- one normal enemy
- one visually distinct enemy variant
- one Technique VFX
- one Spell VFX
- one Reaction VFX
- one prototype Authority-style rule-breaking effect
- one five-card Divine Codex combat HUD
- keyboard and controller glyph presentation
- one faction/environment visual motif

The goal is not final art quality. The goal is to verify that **anime-influenced characters, softly stylized PBR environments, supernatural Codex UI, and readable multiplayer VFX belong in the same visual world**.

---

# Locked Visual Direction

1. The game uses stylized anime fantasy rather than full photorealism.
2. Rendering uses a softly stylized PBR approach rather than committing to full cel shading.
3. Characters use anime-influenced proportions, faces, silhouettes, and expression.
4. Environments remain comparatively grounded so supernatural escalation has contrast.
5. Equipment progression is visibly represented.
6. VFX intensity escalates with supernatural hierarchy.
7. Authorities visually alter rules/reality rather than merely increasing particle count.
8. The Divine Codex UI is supernatural and diegetic rather than a literal physical-card presentation.
9. Factions and world-state changes require recognizable visual identities.
10. Town and settlement progression must be physically visible.
11. Monster variants require meaningful silhouette/equipment/behavior changes rather than relying on recolors.
12. Combat readability takes priority over spectacle in multiplayer.
13. The default camera is third-person action-RPG with enough spatial awareness for cooperative combat.
14. Full cinematics are reserved for high-value moments; routine narrative presentation should use scalable in-engine systems.

---

# Deliberately Unresolved

- final character concept-art style
- exact shader implementation
- degree of outline/rim-light treatment
- final color-script and palette library
- exact post-processing profile
- final Codex typography and glyph language
- final faction visual identities
- final pantheon visual language
- final character creator scope
- exact camera distances and FOV values
- final animation style and exaggeration level
- exact VFX density targets by platform
