# Cohesive Progression Architecture

**Design Version: v0.2.21**

## Purpose

The game has many progression ideas, but the player should not feel as though they are managing a dozen unrelated systems.

The design therefore organizes progression into six player-facing domains:

1. **Character** — Origin, Background, Attributes, Skills
2. **Combat Build** — Weapon, Discipline, Development Grid, Divine Codex
3. **Role** — Jobs
4. **Gear** — Equipment, equipment mastery and evolution
5. **Discovery** — Knowledge, hidden qualifications, System Comprehension
6. **World** — relationships, reputation, factions, economy, citizenship, property, settlements, narrative consequences

Every future progression mechanic should belong clearly to one of these domains unless it has a compelling reason to become a new major system.

**Civilian life is not a seventh progression domain.** It is how the character participates in the World using Skills, Jobs, money, relationships, and choices.

See [`SOCIETY_ECONOMY_AND_REPUTATION.md`](SOCIETY_ECONOMY_AND_REPUTATION.md).

---

## 1. Character

### Origin

How the character entered the world.

Origin establishes narrative context, starting perception, unusual system interactions, and possible hidden progression routes. Origin is not a combat class.

### Background

Who the character was before Transference.

Background may influence starting Skills, knowledge, dialogue, social assumptions, or believable starting competencies.

### Attributes

Prototype attributes remain:

- Might
- Finesse
- Mind
- Spirit
- Vitality

Attributes should support build direction without overpowering equipment, Discipline choices, Codex synergy, player execution, or discovery.

### Skills

Skills represent persistent capabilities such as:

- Swordsmanship
- Tracking
- Appraisal
- Cooking
- Smithing
- Medicine
- Mana Perception
- Deception
- Fieldcraft
- System Comprehension

Skills primarily improve through meaningful use, training, study, accomplishments, teachers, equipment interactions, professional work, and hidden conditions.

**Skills do not use a universal giant skill tree.**

The player-facing rule is:

> Do meaningful things, train them, and become better at them.

Skills may still have mastery tiers, branches, special techniques, or evolutions, but they should share a common mastery language rather than each becoming an independent progression minigame.

---

## 2. Combat Build

Combat consists of four linked parts.

### Foundation Actions

Reliable universal actions such as movement, aim, sprint, dodge, interaction, traversal, and basic target handling.

These never depend on card draw.

### Weapon Arts

Reliable combat actions produced by:

**Weapon Family + Discipline + Equipment Mastery = Weapon Moveset**

Weapon Arts form the dependable action-combat vocabulary.

### Discipline

A Discipline is a combat framework such as Guardian, Arcanist, or Duelist.

Disciplines define:

- combat mechanic/resource
- combat priorities
- manifestation access
- modifications to Weapon Arts
- specialization branches
- multiclass bridges
- hidden combat qualifications

### Divine Codex

The Active Codex is a rotating five-slot hand of extraordinary manifestations.

The Codex provides tactical spikes, reactions, spells, transformations, summons, counters, utility, and other exceptional options without replacing basic action combat.

Deck construction is the Codex's primary customization system.

The Codex should **not** also receive a giant passive skill tree.

---

## 3. Development Points and Discipline Grids

The principal conventional point-spending progression system is the **Discipline Development Grid**.

### Development Points

Character Levels and selected major accomplishments grant **Development Points**.

Prototype direction:

- most normal levels grant Development Points at a predictable cadence
- major Discipline mastery milestones may grant additional Discipline-bound insight or unlock access to special nodes
- rare discoveries may reveal nodes rather than simply grant more currency
- endgame Treasures or Authorities may eventually bend normal limits

Avoid creating many interchangeable point currencies.

Development Points are not used for Jobs, professions, citizenship, reputation, property, or economy progression.

### Why Development Points Exist

Development Points provide the satisfying RPG moment of:

> I leveled up. What part of my combat identity do I want to deepen?

They are not intended to replace activity-driven Skills, Jobs, equipment mastery, professional history, or hidden progression.

---

## 4. Discipline Development Grid

Each mature Discipline should have a compact Sphere-Grid-like specialization layout rather than a giant universal passive web.

Prototype mature target:

**roughly 20–35 meaningful nodes per Discipline**

The exact number is secondary to clarity and distinct playstyles.

### Node Types

#### Connector Nodes

Small improvements that make routes legible and provide modest progression.

#### Behavior Nodes

Change how an action works.

#### Build Nodes

Reward a particular play pattern.

#### Keystone Nodes

Large identity-defining effects that require meaningful investment.

#### Bridge Nodes

Connect compatible Discipline spaces after multiclass qualification.

#### Hidden Nodes

Appear through behavior, mastery, Jobs, world state, equipment, narrative decisions, or System Comprehension.

Most value should come from behavior, build, Keystone, Bridge, and Hidden nodes rather than percentage accumulation.

---

## 5. Prototype Discipline Shapes

### Guardian

**Bulwark** — Guard, Intercept, protection, Resolve efficiency

**Vanguard** — stagger, advancing pressure, aggressive counters

**Oathkeeper** — sacrifice, ally protection, defensive commitments, hidden oath bridges

Possible hidden branch: **Last Bastion**

### Arcanist

**Sigilcraft** — placement, duration, geometry, chained fields

**Threading** — linking attacks and effects through established magical structures

**Battle Focus** — mobile casting, precision, defensive magical timing

Possible hidden branch: **Law Reader**

### Duelist

**Tempo** — Flow, timing, clean sequences

**Predation** — openings, execution, pursuit

**Reversal** — Deflect, angle changes, punish windows

Possible hidden branch: **Perfect Interval**

---

## 6. Multiclass Bridge Architecture

The Development Grid visually reinforces multiclass integration.

Example bridges:

- Guardian Vanguard ↔ Duelist Reversal
- Arcanist Battle Focus ↔ Duelist Tempo
- Guardian Oathkeeper/Bulwark ↔ Arcanist Sigilcraft

Bridge access may require investment, mastery, Skills, Jobs, equipment familiarity, meaningful cross-system behavior, or hidden conditions.

Bridge Nodes can unlock Hybrid Manifestations, modified Weapon Arts, resource interactions, special targeting behavior, and hidden Discipline qualifications.

Multiclassing must create integrated identities rather than a larger pile of unrelated abilities.

---

## 7. Jobs and Professions

Jobs do not receive giant point trees.

Jobs are discovered identities rooted in places, cultures, institutions, environments, activities, professions, and secrets.

Jobs progress primarily through relevant activity and can provide:

- contextual effects
- Skills
- permissions
- social/institutional recognition
- professional opportunities
- evolution routes
- hidden qualifications

A profession-oriented Job should eventually support recognizable work in the world.

Example:

**Smith** can repair equipment, assist a forge, take commissions, work materials, and eventually operate a workshop where allowed.

The progression model is:

> **Skills determine capability. Jobs recognize role. Reputation records track record. The World provides opportunity.**

There is no separate universal profession skill tree or profession-point currency.

---

## 8. Equipment and Mastery

Equipment is one player-facing system: **Gear**.

Individual items may gain familiarity, mastery, traits, techniques, affixes, and evolution opportunities, but the player-facing language should remain consistent:

> Use meaningful equipment in meaningful situations and deepen your relationship with it.

Avoid separate visible XP bars for every subcomponent unless testing proves they are useful.

---

## 9. Achievements, Titles and Treasures

### Achievements

Primarily records of accomplishment and discovery hooks.

### Titles

In-world recognitions that can affect social reactions, hidden qualifications, rare events, and identity presentation.

Titles must not become another mandatory equipment inventory.

### Treasures

Rare, limited, rule-changing artifacts.

**Equipment primarily modifies the character. Treasures may modify rules.**

---

## 10. Knowledge and System Comprehension

Knowledge and System Comprehension belong to **Discovery**.

### Knowledge

What the character has learned about creatures, locations, materials, factions, professions, laws, markets, dungeon structures, anomalies, and recipes.

### System Comprehension

How clearly the character can perceive deeper Codex/system metadata such as status information, hidden qualification progress, compatibility tags, hidden nodes, Dungeon Laws, and Authority signatures.

No additional general-purpose analysis progression layer should be added without a strong reason.

---

## 11. Hidden Progression

Hidden progression runs mostly in the background and tracks meaningful patterns in:

- behavior
- mastery
- professional history
- reliability
- reputation
- narrative decisions
- world state
- equipment history
- failures and recovery
- combinations
- deliberate refusals

The Codex may eventually give those patterns names through Skills, Jobs, hidden Discipline branches, Grid Nodes, Hybrid Manifestations, equipment evolutions, Titles, Treasures, narrative states, and eventually Authorities.

Hidden unlocks should be surprising but interpretable in hindsight.

---

## 12. Advanced Manifestation Mechanics

Covenants, Compound Manifestations, Domains, and other rule-manipulation concepts are advanced families of Codex Manifestations rather than separate base progression systems.

Authorities remain rare endgame permissions over deeper world laws.

---

## 13. The World Domain

The World domain now explicitly includes:

- NPC relationships
- Personal, Group, and Public Reputation
- faction standing
- public rumor and notoriety
- legal status
- citizenship / residency
- employment history
- economy
- shops and supply
- property
- construction
- businesses
- settlement development
- narrative consequences

These are not separate progression ladders. They are interconnected state describing the player's place in society and the condition of the host timeline.

### Reputation

Reputation is derived from behavior and evidence rather than a single positive/negative score.

The world can know the player as reliable, efficient, brutal, discreet, generous, careless, dangerous, professional, or other context-relevant traits.

Reputation is not morality.

### Economy

Settlements use compact economic categories and event-driven consequences rather than exhaustive simulation.

The economy exists to create shortages, opportunities, work, trade, construction, business, and narrative hooks.

### Citizenship

Citizenship and residency represent belonging, rights, obligations, property access, licenses, and institutional recognition.

### Property and Business

Property, construction, and business ownership are advanced ways to participate in a settlement, not mandatory character progression.

---

## 14. Temporary Expedition Progression

Temporary expedition progression remains restrained.

Dungeon runs may contain temporary tactical choices, consumables, blessings, anomalies, situational modifications, and unsecured loot.

The player should not rebuild an entire temporary character every dungeon.

---

## 15. Player-Facing Progression Summary

### Character

Who am I, and what can I do?

### Combat Build

How do I fight, and how have I specialized?

### Role

What has this world recognized me as being, and what work can I actually perform?

### Gear

What equipment have I learned and evolved?

### Discovery

What have I learned, and what hidden possibilities can I perceive?

### World

Who knows me, what do they think of me, where do I belong, how do I make a living, and how have my choices changed this timeline?

If a future feature cannot fit naturally into one of these questions, it should be treated as a potential bloat warning.

---

## 16. Vertical Slice Rule

For the Hearthcross vertical slice, implement only enough to prove the architecture.

Recommended progression proof:

- Character Level with a small number of Development Points
- one lightweight Attribute allocation moment
- one partial Discipline Grid per Guardian, Arcanist, and Duelist
- approximately 6–10 nodes per prototype Discipline
- one hidden node reveal
- one Job slot
- activity-driven Skills
- one equipment mastery/evolution proof
- five-slot Active Codex
- one hidden qualification
- Knowledge/System Comprehension feedback

Recommended civilian-world proof:

- two distinct shops
- one ordinary work opportunity
- one reliability consequence
- one professional-quality consequence
- one named NPC memory
- one propagated reputation event
- one legal-status step
- one economic variable affecting stock, price, or work
- one Job/Skill changing a civilian interaction

Do not implement full mature Discipline grids, advanced multiclass bridges, extensive business management, full property systems, complex taxes, Covenants, Domains, Authorities, or deep economic simulation before the base loop is fun.

---

## Locked Principles

1. The game uses six player-facing progression domains rather than presenting every subsystem as equal.
2. Civilian life belongs to the World domain and reuses Skills, Jobs, reputation, money, and world state.
3. Skills improve primarily through meaningful activity and training.
4. Development Points are the main conventional point-spending currency and primarily customize Discipline Grids.
5. Discipline Grids are compact, meaningful, and specialization-focused.
6. Jobs progress through activity, discovery, culture, institutions, location, and profession practice rather than giant point trees.
7. Profession gameplay does not create a separate universal profession tree or point currency.
8. Equipment mastery and evolution share one Gear language.
9. Achievements and Titles are supporting systems; Treasures remain rare and rule-changing.
10. Knowledge and System Comprehension form the Discovery domain.
11. Reputation is multidimensional social state, not morality or a single global bar.
12. Economy, citizenship, property, construction, and business are interconnected World state rather than separate progression ladders.
13. Hidden progression can observe civilian as well as adventuring behavior.
14. Temporary dungeon progression remains lighter than persistent development.
15. New major systems require strong justification and must survive the bloat test.
