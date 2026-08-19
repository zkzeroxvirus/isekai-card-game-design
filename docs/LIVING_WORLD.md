# Living World, Factions & Consequences

Version: **v0.2.21**

## Canon Design Principle

**The world remembers what the player did, who benefited, who suffered, what people believe happened, and how much time has passed.**

The game should not reduce morality or reputation to a single visible Good/Evil bar. Player behavior is recorded through consequences, faction relationships, NPC memories, professional history, legal status, public stories, hidden behavioral tendencies, settlement changes, and world-state evolution.

See [`SOCIETY_ECONOMY_AND_REPUTATION.md`](SOCIETY_ECONOMY_AND_REPUTATION.md) for the civilian-life, economy, reputation, law, property, and citizenship model.

## 1. World Time

World time advances through meaningful actions rather than requiring a fully simulated real-time world while the player is offline.

Actions that may advance time include:

- travel
- resting
- dungeon expeditions
- crafting projects
- paid work
- recovery from wounds
- major quests
- training
- construction
- faction operations
- political/narrative chapters

Time should create consequences and opportunities, not simply punish the player for exploring.

Examples:

- delayed rescue changes who survives
- ignored monster threats worsen
- caravans reach or fail to reach destinations
- work deadlines pass
- factions complete projects
- seasons change available resources and events
- construction completes
- companions recover from injuries
- shortages improve or worsen

Important deadlines must be communicated clearly enough that failure feels like consequence rather than a trap.

## 2. Host-Owned Timeline

The host world owns canonical world chronology and major narrative state.

Visitors enter the host's timeline and experience its current reality.

Host-world state can include:

- living/dead/relocated NPCs
- NPC memories and local relationships
- settlement ownership
- town development
- economy and shortages
- local legal status and investigations
- property and businesses
- active wars
- faction power
- available routes
- destroyed or rebuilt locations
- diplomatic treaties
- regional monster populations
- divine events

A visitor's portable character progression remains their own, but they do not overwrite the host's timeline.

## 3. Reputation Architecture

Reputation exists at multiple scales rather than as one global score.

### Personal Reputation

What a specific NPC knows, remembers, believes, fears, respects, trusts, or dislikes about the player.

### Group Reputation

How a faction, guild, settlement, profession, church, clan, criminal network, or institution generally regards the player.

### Public Reputation

What people who have never met the character may have heard through witnesses, official records, rumors, propaganda, trade networks, religion, or other communication channels.

These layers may disagree.

A character may simultaneously be:

- personally trusted by a blacksmith
- respected by the Adventurer Guild
- feared by local merchants
- wanted by one jurisdiction
- honored by a monster clan
- publicly misunderstood

## 4. Reputation Evidence and Traits

Reputation should emerge from accumulated evidence rather than arbitrary reputation buttons.

Evidence can include:

- contracts completed or abandoned
- deadlines met or missed
- quality of work
- collateral damage
- promises kept or broken
- debts repaid or ignored
- crimes
- generosity
- rudeness
- professional competence
- discretion
- mercy
- brutality
- reliability
- betrayal
- public heroism

Possible interpreted traits include:

- Reliable / Unreliable
- Efficient
- Thorough
- Careless
- Professional
- Discreet / Loose-Lipped
- Generous
- Expensive
- Merciful
- Brutal
- Honorable
- Opportunistic
- Competent
- Reckless
- Loyal
- Treacherous
- Polite
- Arrogant
- Dangerous

Different groups can interpret the same evidence differently.

A criminal network may value ruthlessness and discretion. A clinic may value compassion and reliability. A military organization may value discipline and competence.

## 5. NPC Memory and Social Networks

Named and mechanically important NPCs remember meaningful interactions.

Possible memories include:

- favors
- insults
- promises
- betrayals
- gifts
- debts
- saved relatives
- killed relatives
- work history
- witnessed crimes
- professional respect
- repeated social behavior

NPC opinions can influence related NPCs through simplified social networks such as family, employer relationships, guild ties, friendship, rivalry, patronage, faction contacts, and informant networks.

Do not simulate a detailed social graph for every ambient NPC. Named NPCs receive richer memory; background populations use settlement-level abstractions.

## 6. Information Propagation

The world distinguishes:

**What happened**

from

**What people know or believe happened.**

Information can spread through:

- witnesses
- guild records
- guards
- merchants
- family networks
- tavern rumors
- faction messengers
- clergy
- criminal informants
- magical communication or public media where appropriate

A reputation event may track source, witnesses, credibility, evidence strength, social reach, and whether the player's identity is known.

Rumors may distort events.

A character can therefore maintain a good public image despite secret wrongdoing, or suffer a bad reputation for something they did not actually do.

## 7. Crime, Law and Jurisdiction

Crime interacts with witnesses, evidence, local law, faction control, legal status, and investigation capability.

Killing someone unseen does not automatically reduce reputation everywhere.

Evidence can later surface through survivor testimony, stolen property, divination, forensic clues, accomplices, public boasting, or other setting-appropriate means.

Possible legal consequences include:

- fines
- restitution
- confiscation
- arrest
- imprisonment
- exile
- license loss
- citizenship loss
- guild sanctions
- bounties
- trial
- faction retaliation
- blackmail

Different societies define crimes differently.

## 8. Reputation Is Not Morality

Reputation measures perception and social track record.

Hidden behavioral history records what the player actually tends to do.

They are related but not identical.

A secretly cruel character may be publicly beloved.

A compassionate outlaw may be officially condemned.

A tyrant may be feared, respected, and administratively effective.

The world may judge the player incorrectly; the simulation must still remember what actually happened.

## 9. Hidden Behavioral Tendencies

The game may track broad tendencies as hidden or partially revealed history rather than morality scores.

Prototype axes:

- **Mercy ↔ Ruthlessness**
- **Order ↔ Freedom**
- **Selflessness ↔ Ambition**
- **Sacred ↔ Profane**

These axes describe patterns, not objective morality.

They may influence:

- Titles
- hidden Jobs
- hidden Disciplines
- divine reactions
- companion approval
- narrative options
- Skill evolutions
- Authority access

**No choice exists only to fill an alignment meter.**

Choices should change tangible people, places, resources, factions, relationships, or world conditions. Behavioral tracking observes those choices afterward.

## 10. Consequence Records

Important decisions create persistent world-state records.

A consequence record may contain:

- event/decision ID
- timestamp
- affected region
- affected factions
- affected NPCs
- actual outcome
- public/known interpretation
- delayed outcome hooks
- reputation evidence
- legal consequences
- economic consequences
- narrative tags
- future event prerequisites

This allows consequences to return much later.

## 11. Economy and Civilian Life

Settlements function as societies with abstract but consequential economies.

Possible tracked categories include:

- food
- raw materials
- crafted goods
- medicine
- labor
- housing
- trade access
- security
- prosperity

Economic state can influence:

- prices
- shop stock
- work opportunities
- construction
- migration
- faction projects
- crime
- shortages
- Job availability
- political pressure

The world economy should generate understandable stories and opportunities rather than exist only as a market-price simulation.

## 12. Citizenship and Belonging

The player may begin without recognized legal identity depending on Origin.

Societies may distinguish between statuses such as:

- unregistered foreigner
- registered traveler
- temporary resident
- permanent resident
- citizen or subject
- licensed professional
- landholder
- business owner
- officeholder

Requirements and rights vary by location.

Citizenship can affect property ownership, training, guild access, legal protection, taxes, weapon rights, civic participation, institutional Jobs, and social belonging.

The progression from outsider to recognized member of society should be a meaningful isekai arc.

## 13. Faction Projects

Major factions pursue goals even when the player is not directly participating.

A **Faction Project** is a time-based world objective that can progress, stall, succeed, mutate, or fail.

Examples:

- invasion preparations
- rebellion recruitment
- trade-route expansion
- religious conversion
- monster-clan unification
- fortress construction
- housing development
- hospital construction
- magical research
- artifact recovery

Players can assist, sabotage, ignore, redirect, negotiate, or profit.

Projects should create visible political, social, or economic consequences.

## 14. Dynamic Settlements

Settlements are persistent world entities rather than static quest hubs.

Tracked settlement state may include:

- population
- security
- prosperity
- food/resources
- trade
- labor
- housing
- faction control
- magical stability
- corruption
- infrastructure
- active threats
- refugee pressure
- local reputation
- legal climate

Player actions and faction projects may visibly transform locations.

Examples:

- walls constructed or destroyed
- districts added
- refugee camps appear
- shops close or expand
- black markets form
- monster residents integrate
- undead labor becomes normalized
- guards become hostile
- caravan traffic increases
- workshops gain new production capability

## 15. Property, Construction and Business

Players may eventually rent or own rooms, workshops, homes, shops, warehouses, farms, frontier claims, and other properties where local law allows.

Construction uses plots, renovations, civic projects, or claims rather than unrestricted survival-game building by default.

Projects may require:

- permission
- land
- plans
- materials
- labor
- specialist professions
- money
- time
- security

Businesses may later support player-owned forges, shops, clinics, taverns, caravan companies, warehouses, and similar ventures.

Ownership should create meaningful decisions and world participation rather than only passive income.

## 16. Player Town as Campaign Record

The persistent home settlement should visually reflect campaign history.

Town evolution may depend on:

- chosen alliances
- major quests
- recruited populations
- faction influence
- crimes
- divine patronage
- monster diplomacy
- economic policy
- property development
- business investment
- war outcomes

Two host worlds that began identically should be capable of becoming dramatically different.

## 17. Heroic, Villainous & Mixed Play

The game supports heroic, villainous, pragmatic, opportunistic, revolutionary, tyrannical, criminal, mercantile, civic, and mixed trajectories.

Villainous play should unlock distinct content rather than merely destroy existing content.

Possible villainous progression includes:

- extortion
- forbidden magic
- assassinations
- criminal alliances
- black-market economies
- monopolistic trade
- political coups
- coercive rule
- hostile divine patronage

Heroic progression may include:

- rescue networks
- rebuilding
- fair trade
- medical work
- peace treaties
- institutional reform
- monster-human reconciliation
- civic investment

Mixed routes are expected and encouraged.

## 18. Companion Reactions

Companions maintain their own values, loyalties, fears, ambitions, and opinions of the player's behavior.

They may react to:

- violence
- kindness
- rudeness
- professional conduct
- missed commitments
- criminal behavior
- wealth and status
- political choices
- treatment of workers
- loyalty and betrayal

Companion reaction is based on the companion's values, not a universal morality table.

## 19. Narrative Events from World State

Narrative events may unlock from combinations of:

- reputation traits
- faction standing
- NPC memories
- public notoriety
- legal status
- profession/Job
- economic conditions
- faction projects
- world time
- settlement condition
- known Skills
- equipment
- Titles
- Knowledge
- companions
- Origin
- prior decisions
- hidden behavioral tendencies

This allows character builds and social history to function as narrative keys.

## 20. World Eras

Long campaigns may progress through broad eras reflecting escalating influence.

1. **Arrival Era** — survival, local work, legal identity, low recognition.
2. **Adventurer Era** — Guild advancement, professions, regional factions, contracts, property.
3. **Heroic Era** — cities, wars, major trade and political consequences.
4. **Sovereign Era** — nations, large businesses, rulership, major institutions.
5. **Mythic Era** — gods, Authorities, Dungeon Laws, world-level threats.

Era progression should be based on narrative/world milestones, not simply character level.

## 21. Escalation Principle

The scope of consequences grows with player influence.

Early game:

- individual lives
- employment
- local shops
- small settlements
- minor crime
- monster nests

Midgame:

- cities
- factions
- businesses
- trade routes
- construction
- political disputes
- wars

Late game:

- nations
- economies
- institutions
- divine orders
- world rules
- ancient systems

## 22. Multiplayer Narrative Rule

**When visiting another player's world, the visitor experiences the host's consequences.**

Visitors may bring portable character progression, but local NPC memories, property, business ownership, citizenship, economic state, and local legal consequences belong to the host timeline unless explicitly shared by the fiction.

## 23. Design Guardrails

- Do not label every choice Good or Evil.
- Do not make reputation a single universal positive/negative score.
- Do not make villain routes merely reduced-content routes.
- Avoid omniscient crime reporting.
- Avoid irreversible consequences from trivial or unclear choices.
- Telegraph meaningful deadlines.
- Allow consequences to be surprising without being arbitrary.
- Preserve disagreement between factions and NPCs.
- Avoid forcing every player into politics, business management, or property ownership.
- Simulate only enough economic/social detail to create player-facing choice and consequence.
- Ensure civilian play feeds the same Skills, Jobs, relationships, world state, and hidden progression as adventuring.

## 24. Canon Principles Added / Refined in v0.2.21

- **The world remembers behavior and social history.**
- **What happened and what people believe happened are different state.**
- **Reputation exists at Personal, Group, and Public scales.**
- **Reputation is not morality.**
- **Crime requires information flow, evidence, or witnesses.**
- **Work reliability and professional quality matter.**
- **Citizenship and property represent belonging and legal access.**
- **Settlements have abstract but meaningful economies.**
- **Civilian life uses the same systems as adventuring rather than becoming a disconnected minigame layer.**
- **The world functions without the player, but the player can materially change how it functions.**
