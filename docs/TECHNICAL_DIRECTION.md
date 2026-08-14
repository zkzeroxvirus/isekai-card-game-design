# Technical Direction & Multiplayer Architecture

Version: **v0.2.5**

## 1. Product Direction

The project is intended to become a **3D PC action-RPG/deckbuilder** with narrative exploration, travel events, persistent character progression, instanced dungeon expeditions, and online cooperative multiplayer.

The card system remains central, but cards represent **capabilities and abilities** rather than board-game movement.

### Core Technical Design Principle

**The deck defines capability; the player controls execution.**

Movement, positioning, aiming, traversal, spacing, dodging, and environmental interaction occur directly in 3D space. Cards determine which techniques, spells, reactions, summons, stances, items, and special actions are available.

## 2. Engine Direction

### Provisional Engine Choice

**Unreal Engine 5** is the preferred engine for the current design direction.

Reasons:

- strong third-person 3D workflow
- mature client/server networking model
- listen-server support for player-hosted co-op
- dedicated-server path remains available later
- strong animation, VFX, cinematics, world building, and character tooling
- Gameplay Ability System is potentially well suited to cards, status effects, costs, attributes, tags, and replicated abilities
- C++ can hold authoritative systems while Blueprint remains useful for content iteration

This remains a provisional technical decision until a small multiplayer combat prototype validates the workflow.

### Architecture Intent

Use a hybrid development model:

**C++ / authoritative systems**

- card and deck state
- combat resolution
- resource validation
- attributes
- status effects
- inventory
- equipment
- mastery
- save data
- networking
- dungeon generation rules
- narrative/world-state flags

**Blueprint / data-driven content**

- ability presentation
- animation hooks
- VFX/SFX
- encounter scripting
- NPC interactions
- narrative events
- quest/event assembly
- environmental interactions

Gameplay-critical logic should remain authoritative and data-driven enough that content does not require bespoke networking code for every card.

## 3. Player Count

### Core Rule

The game supports **1–6 players per world session**.

- 1 host
- up to 5 joining players
- solo play is a first-class mode
- cooperative balance must consider the full 1–6 range

The game should not require a fixed role composition.

## 4. World Ownership Model

### Core Rule

**World persistence belongs to the host. Character persistence belongs to each player.**

The host owns the persistent state of their world, including:

- narrative decisions
- faction outcomes
- town upgrades
- unlocked regions
- NPC states
- completed host-world quests
- world-specific discoveries
- world-specific dungeon milestones
- world-state consequences

Joining players bring their own persistent characters, including:

- character level/progression
- classes
- skill mastery
- known cards
- equipment
- equipment mastery
- treasures
- titles
- achievements
- personal currencies/resources where appropriate
- companion progression where portable

Joining another world should not overwrite a player's own world progression.

## 5. Session Model

### Initial Networking Model

Use **player-hosted listen-server sessions**.

The host runs the authoritative world simulation while also controlling a player character.

### Session Lifecycle

1. Host loads or creates their world.
2. Host opens the world to friends/invited players/public matchmaking according to session settings.
3. Joining player authenticates and loads an eligible persistent character.
4. Server validates imported character state.
5. Player joins the host's current safe region, travel state, or expedition staging point according to join rules.
6. Players may leave and retain secured personal progression.
7. Host world state saves according to authoritative checkpoints.

## 6. Join-in-Progress / Drop-In Drop-Out

### Core Direction

Players should be able to join and leave the host's world with minimal friction.

### Safe Join Points

Prototype join locations should include:

- Town
- Guild Hall
- Camp
- Dungeon staging area
- completed encounter boundary

Joining directly into an active boss phase or sensitive narrative cinematic should be restricted until synchronization rules are proven reliable.

### Leaving

A player may leave voluntarily from a safe state.

Secured character rewards should persist immediately or at frequent authoritative checkpoints.

Unsecured dungeon rewards remain subject to extraction rules.

## 7. Host Loss

### Prototype Rule

Full seamless host migration is **not required for the first implementation**.

If the host ends or loses the session:

- the active host world session ends
- each player keeps progression already confirmed as secured
- unresolved/unsecured expedition state may be lost or restored from the last authoritative checkpoint
- host world state restores from its last valid save/checkpoint

### Future Option

Possible later upgrades:

- resumable session snapshots
- elected-host migration
- cloud-hosted continuation
- optional dedicated persistent worlds

The initial architecture should avoid assumptions that make a dedicated-server version impossible later.

## 8. Authority Model

### Core Rule

The game is **server authoritative** for gameplay state.

Clients request actions; the authority validates and executes them.

Examples of authoritative state:

- card hand/deck/discard state
- Action/resource values
- damage and healing
- status effects
- inventory changes
- loot ownership
- mastery gains
- enemy AI state
- dungeon objectives
- narrative/world flags

Example ability flow:

1. Client selects `Flame Lance`.
2. Client submits target/input request.
3. Authority validates card availability, resource cost, state, range, target legality, and activation restrictions.
4. Authority activates the gameplay ability.
5. Animation/VFX/projectile presentation replicates.
6. Authority resolves damage/status results.
7. Updated game state replicates to all relevant clients.

Single-player should use the same authoritative rules path wherever practical.

## 9. Card-to-3D Ability Model

Cards are not merely UI buttons. They are access objects for executable gameplay abilities.

### Proposed Data Separation

**Card Definition**

- Card ID
- name
- class/source
- card type
- tags
- Action/resource cost
- targeting rules
- range
- timing restrictions
- hand/deck behavior
- mastery/evolution links
- granted/activated ability reference

**Gameplay Ability**

- animation
- movement commitment
- targeting execution
- projectile/trace/area logic
- gameplay effects
- replication
- interruption rules
- combo windows
- world interaction

This permits multiple cards, upgrades, equipment forms, or mastery variants to share underlying ability components where useful.

## 10. Real-Time 3D Combat

### Design Direction

Combat should support direct 3D movement while card availability creates tactical constraints.

Potential player actions include:

- move
- sprint
- dodge
- block/parry where build allows
- aim
- interact
- play ability card
- use prepared/reaction card
- manage targeting
- coordinate with allies

The deck should constrain **available actions**, not basic locomotion.

### Multiplayer Combat Principle

Cross-player synergy should be powerful but not mandatory.

Examples:

- one player applies `Soaked`; another uses Lightning
- a Defender creates a safe zone for a channeling caster
- a Rogue exposes a weak point for another player
- a Summoner creates bodies that enable another class's corpse or sacrifice mechanics

The game should avoid forcing MMO-style Tank/Healer/DPS composition for normal content.

## 11. Scaling from 1 to 6 Players

Encounter scaling should consider more than enemy HP.

Possible scaling dimensions:

- enemy count
- enemy composition
- elite modifiers
- simultaneous mechanics
- target pressure
- arena hazards
- reinforcement timing
- boss pattern complexity

Raw health multiplication should be limited so larger parties do not merely produce longer fights.

Solo players may receive compensating systems such as:

- companion slots
- adaptive enemy count
- solo blessings
- increased preparation options
- alternate encounter objectives

## 12. Narrative World Integration

The host world maintains persistent narrative state.

Narrative systems may react to:

- Origin
- classes
- known skills
- equipment
- treasures
- titles
- Guild Rank
- Bestiary knowledge
- companions
- factions
- previous decisions
- world discoveries

### Build as Narrative Keyring

Character progression should unlock narrative options as well as combat power.

Examples:

- a Ranger notices tracks during travel
- a Necromancer recognizes disturbed burial magic
- a high-Guild-Rank character gains authority in negotiations
- a rare Treasure changes an NPC response
- Bestiary research reveals a noncombat solution

## 13. Travel & Narrative Events

Travel should function as active game content rather than a loading-screen abstraction.

Potential travel events:

- ambush
- weather
- wounded traveler
- monster tracks
- faction patrol
- ruined shrine
- caravan encounter
- companion conversation
- rare merchant
- world anomaly
- temporary dungeon entrance
- resource discovery
- moral or political choice

Events can be triggered by:

- route
- biome
- time/world state
- party composition
- host decisions
- character builds
- achievements
- random event tables

Some travel scenes may occur in explorable 3D spaces; others may use compact narrative-event presentation where appropriate.

## 14. Instancing Strategy

The game does not need to be a seamless MMO.

Preferred structure:

- persistent host-owned world state
- explorable towns/hubs
- overworld/travel regions
- instanced dungeons
- instanced major narrative encounters
- party session capped at 6 players

This keeps the fantasy of a shared online world while containing networking and content scope.

## 15. Persistent Server Compatibility

Dedicated persistent servers are a future option, not a launch dependency.

The architecture should therefore separate:

- world owner identity
- world-state save data
- authoritative simulation
- player character persistence
- session transport

A future dedicated server should be able to assume the authority role currently held by a listen-server host without redesigning combat rules.

## 16. Save Data Boundaries

### Player-Owned Data

- character identity
- level/progression
- class unlocks
- skill mastery
- known cards
- equipment
- treasures
- titles/achievements
- portable companion state

### World-Owned Data

- world seed/state
- narrative flags
- factions
- town state
- NPC state
- world quests
- region unlocks
- host-world discoveries
- persistent environmental changes

### Session-Owned Data

- active dungeon state
- current hand/deck combat zones
- temporary run cards
- temporary buffs/debuffs
- encounter state
- unsecured loot

Session-owned data normally expires when the expedition/session ends unless promoted into secured persistent data.

## 17. Technical Risks to Prototype Early

Before full production, validate:

1. six-player replicated combat with card-driven abilities
2. hand/deck synchronization under latency
3. join/rejoin state transfer
4. host save reliability
5. ability prediction/latency feel
6. projectile and AoE replication
7. large enemy-count performance
8. companion AI in multiplayer
9. instanced dungeon transitions
10. narrative/world-state synchronization
11. secured/unsecured reward boundaries
12. Steam/EOS or other online-session integration choice

## 18. Recommended First Technical Vertical Slice

Build a deliberately small Unreal prototype containing:

- third-person movement
- listen-server hosting
- 1–6 player connection support
- one replicated enemy type
- one simple arena
- a five-card test deck
- draw/discard/hand replication
- one melee Technique
- one projectile Spell
- one defensive Reaction
- one status effect
- one cross-player combo
- one loot pickup
- one secure/extract checkpoint
- one save/reload test
- one join-in-progress test

The purpose is not to prove content quantity. It is to prove that **3D action, cards, replication, persistence, and co-op feel coherent together**.

## 19. Current Locked Direction

- PC game
- third-person 3D presentation
- card-driven abilities
- direct 3D movement
- narrative exploration and travel events
- 1–6 player cooperative sessions
- player-hosted worlds
- host-owned world progression
- player-owned persistent characters
- server-authoritative gameplay
- listen servers first
- dedicated-server-compatible architecture
- Unreal Engine 5 as the provisional engine choice

## 20. Open Technical Questions

- exact combat pacing and whether any systems slow/pause time in solo play
- exact dodge/block baseline available independent of cards
- targeting scheme for mouse/keyboard and controller
- whether world travel is contiguous, region-based, or node-assisted
- Steam networking versus EOS versus another service layer
- character-save anti-cheat model for peer-hosted sessions
- reconnect grace period
- whether companions consume player-party slots
- how host-world quest rewards transfer to visiting players
- whether PvP will ever exist; assume no until deliberately designed
- whether cross-platform support is a goal
- whether mod support is a future requirement
