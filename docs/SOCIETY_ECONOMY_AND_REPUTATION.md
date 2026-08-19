# Society, Economy & Reputation

**Design Version: v0.2.21**

## Purpose

The game is not only about adventuring through a fantasy world. It is about **living inside one**.

Civilian life, trade, professions, law, property, construction, reputation, and social belonging should make settlements feel like functioning societies rather than quest hubs.

These systems must not become a disconnected life-sim layer. They reuse the existing architecture:

- **Skills** determine what the character can do.
- **Jobs** represent roles the world recognizes.
- **World State** tracks settlement and regional conditions.
- **Relationships and Reputation** determine how people and institutions respond.
- **Hidden Progression** recognizes long-term behavior.
- **Locations** determine which opportunities, institutions, laws, professions, and markets exist.

### Core Principle

> **Every profession participates in the same world rather than existing in its own minigame bubble.**

---

## 1. Civilian Life as World Participation

The player may spend meaningful time participating in ordinary society without abandoning the larger adventure.

Possible activities include:

- buying and selling goods
- working temporary labor
- practicing a profession
- crafting goods for customers
- treating patients
- hunting and selling materials
- running caravans
- operating a shop or workshop
- renting or buying property
- gaining residency or citizenship
- constructing or restoring buildings
- funding settlement projects
- hiring workers
- supplying expeditions
- joining guilds and institutions
- paying taxes, fees, licenses, or dues where appropriate
- navigating local law and social customs

The game should support the fantasy that a character could attempt to **make a life** in the world, even if exploration and the larger mystery eventually pull them into extraordinary events.

---

## 2. Economy Model

The economy should create understandable cause and effect without attempting to simulate every loaf of bread or NPC paycheck.

Settlements and regions track a compact set of economic state categories.

Prototype categories:

- **Food**
- **Raw Materials**
- **Crafted Goods**
- **Medicine**
- **Labor**
- **Housing**
- **Trade Access**
- **Security**
- **Prosperity / Local Wealth**

Specific regions may rename, merge, omit, or add categories when necessary.

### Economic Chain

The general model is:

**Production → Transport → Processing → Commerce → Consumption**

Examples:

- logging camp produces timber
- caravan transports timber
- sawyer converts timber to boards
- carpenter consumes boards
- settlement construction consumes finished work

Or:

- hunters supply monster parts
- apothecary processes glands and herbs
- clinic purchases medicines
- outbreaks increase demand

The player can participate at several points in a chain rather than interacting only with final vendors.

---

## 3. Economic Consequences

World events should propagate through the economy where the connection is understandable.

Example:

**Mirehounds attack livestock**

Possible consequences:

1. Food supply declines.
2. Meat prices increase.
3. Inn costs may rise slightly.
4. Hunter contracts become more common.
5. Hide supply falls later.
6. Tanners and leatherworkers may reduce stock.
7. Nearby communities may request protection.

If the player solves the problem, supply should normalize over time rather than instantly reset.

Economic consequences can also reveal narrative information.

An unexplained metal shortage may indicate war preparations.

A sudden demand for grave salt may foreshadow undead activity.

A merchant quietly buying all available lamp oil may be preparing for a siege or ritual.

### Design Rule

> **The economy should generate stories and consequences, not merely price fluctuations.**

---

## 4. Stores and Markets

Stores are persistent participants in the local economy rather than magical inventories.

A substantial business may conceptually track:

- stock
- specialization
- supply relationships
- purchasing power
- local demand
- proprietor relationship
- faction or legal restrictions
- known recipes / production capability
- world-state dependencies

### Stock

Inventory may depend on:

- local production
- trade-route status
- settlement prosperity
- season
- faction control
- player-supplied materials
- discovered recipes
- merchant contacts
- regional crises

Stock does not need to be perfectly simulated item-by-item. The system may generate inventory from these conditions.

### Merchant Wealth

Merchants should not always possess infinite purchasing power.

A poor frontier trader may be unable to buy a legendary relic at full theoretical value.

Options may include:

- partial payment
- barter
- consignment
- referral to a wealthier buyer
- delayed payment
- trade credit
- refusal because the item is outside the merchant's market

### Player Influence on Stock

Selling rare materials, teaching recipes, improving trade routes, recruiting specialists, or investing in a settlement can expand what local shops produce and carry.

Example:

> The player supplies Greyfen alloy and helps the Split Anvil understand it.
>
> Later, Greyfen Alloy equipment becomes part of the smith's normal production pool.

---

## 5. Money and Economic Freedom

Currency should represent freedom and leverage, not only combat power.

Potential expenditures include:

- food and lodging
- travel
- equipment
- repairs
- crafting materials
- training
- licenses
- guild dues
- taxes
- fines
- property
- rent
- construction
- hired labor
- employees
- businesses
- caravans
- information
- bribes
- faction contributions
- expedition funding
- luxury goods
- political projects

Basic maintenance costs must remain restrained enough that they create texture rather than constant financial punishment.

### Progression Fantasy

Early:

> Can I afford somewhere safe to sleep?

Midgame:

> Can I afford the equipment, training, or workshop I want?

Later:

> Can I finance an expedition or caravan?

High influence:

> Can I fund a district, army supply contract, guild hall, hospital, or regional project?

Wealth becomes another form of agency without replacing character power.

---

## 6. Work and Menial Jobs

Settlements should offer ordinary work that helps establish the feeling of entering an unfamiliar society.

Examples:

- unload caravans
- carry goods
- split firewood
- repair palisades
- stable work
- kitchen work
- gather herbs
- clean Guild facilities
- inventory counting
- messenger work
- road maintenance
- field labor
- workshop assistance
- corpse / monster cleanup
- warehouse labor

These are not intended as repetitive grind loops.

A small work opportunity can provide:

- money
- Skill progress
- Job qualification progress
- NPC relationships
- local knowledge
- rumors
- reputation evidence
- hidden discoveries
- adventure hooks

### Mundane-to-Extraordinary Rule

> **Ordinary life should be capable of colliding with extraordinary events.**

Example:

While unloading a merchant caravan, Appraisal reveals that one sealed crate does not match its declaration.

The player can ignore it, report it, investigate it, steal it, blackmail the merchant, or later discover it relates to a larger plot.

---

## 7. Professions as Playable Roles

A profession should be something the player can meaningfully **perform**, not merely equip as a passive bonus.

### Blacksmith

Possible activity:

- repair customer gear
- assess damaged items
- fulfill commissions
- forge stock
- experiment with materials
- apprentice under specialists
- operate a rented forge
- own a workshop
- train assistants

### Cook

Possible activity:

- work kitchens
- prepare expedition meals
- develop recipes
- source ingredients
- operate an inn or food stall
- cater faction events

### Field Medic / Physician

Possible activity:

- treat injuries
- diagnose conditions
- work clinics
- serve expeditions
- respond to disasters
- develop medicine-related Skills

### Merchant

Possible activity:

- negotiate
- buy and resell goods
- establish suppliers
- organize caravans
- manage storage
- fulfill procurement contracts
- invest in trade routes

### Surveyor / Cartographer

Possible activity:

- map routes
- inspect terrain
- record dungeons
- sell information
- verify claims
- assist construction and expeditions

### Hunter / Trapper

Possible activity:

- track creatures
- fulfill meat/hide contracts
- remove dangerous wildlife
- identify migration changes
- harvest monster materials

### Design Rule

> **If a Job claims to represent a profession, the player should eventually be able to perform recognizable work from that profession.**

Not every profession requires equal mechanical complexity, but each should connect to the shared world.

---

## 8. Profession Progression

Profession progression continues to use the Job + Skill model rather than a new profession-tree currency.

Example:

**Smith Job**

- determines recognized role, access, customers, and contextual effects
- teaches or accelerates Smithing, Repair, Metallurgy, Tempering Skills
- unlocks forge permissions
- creates social recognition among artisans
- can evolve through actual practice and location-specific instruction

The quality, difficulty, novelty, context, and consequences of work should matter more than raw repetition.

A player should not become a legendary smith by producing 10,000 identical nails.

---

## 9. Work Commitments and Reliability

Accepting work creates a social commitment.

A work contract can contain:

- employer
- task
- agreed compensation
- deadline or time window
- quality expectations
- supplied materials or equipment
- legal conditions
- cancellation terms

Failure is contextual.

Missing one low-stakes shift should not permanently ruin the character, but patterns matter.

Behavior that may affect reputation includes:

- failing to appear
- abandoning work
- completing late
- damaging supplied equipment
- stealing materials
- overdelivering
- working efficiently
- keeping clients alive
- discovering additional problems
- behaving professionally
- renegotiating honestly before failure

### Scheduling Guardrail

Time commitments should create consequence without turning the game into calendar micromanagement.

Important deadlines must be clearly communicated.

Where appropriate, players can cancel, reschedule, subcontract, or warn an employer rather than being punished simply for exploring.

---

## 10. Reputation Architecture

Reputation is not one universal meter.

The world forms opinions at three primary scales.

### Personal Reputation

What an individual NPC knows, believes, remembers, fears, respects, likes, or dislikes about the player.

### Group Reputation

How an institution, faction, profession, settlement, guild, criminal network, church, clan, or other community generally regards the player.

### Public Reputation

What people who may never have met the character have heard through stories, records, rumors, witnesses, propaganda, or reputation networks.

These layers can disagree.

Example:

- personally trusted by a blacksmith
- institutionally respected by the Guild
- publicly feared as a dangerous foreign adventurer

---

## 11. Reputation Traits

Reputation should describe patterns rather than reduce personality to a single positive/negative number.

Possible traits include:

- Reliable
- Unreliable
- Efficient
- Thorough
- Careless
- Professional
- Generous
- Expensive
- Discreet
- Loose-Lipped
- Merciful
- Brutal
- Honorable
- Opportunistic
- Lawful
- Defiant
- Dangerous
- Competent
- Reckless
- Loyal
- Treacherous
- Polite
- Arrogant
- Intimidating

These are examples, not a requirement that every character expose dozens of numerical meters.

### Trait Evidence

The simulation should store **evidence events** and derive reputational interpretation from them.

Example:

- completed five contracts before deadline
- abandoned two jobs without warning
- spared surrendered enemies
- repeatedly damaged employer property
- returned a lost purse
- extorted a merchant
- successfully treated plague victims

Different communities may interpret the same evidence differently.

A criminal network may value ruthlessness and discretion.

A hospital may value compassion and reliability.

A military organization may value discipline, competence, and obedience.

---

## 12. NPC Memory and Relationships

NPCs remember meaningful interactions.

Memory should prioritize events relevant to that NPC rather than recording every trivial action forever.

Possible memory categories:

- favors
- insults
- promises
- betrayals
- gifts
- debts
- saved relatives
- killed relatives
- completed work
- failed work
- witnessed crimes
- ideological conflicts
- professional respect
- repeated social behavior

Personal relationships can modify or resist broader reputation.

An NPC may defend someone with a poor public reputation because of personal experience.

Another may distrust a celebrated hero because they witnessed a hidden atrocity.

---

## 13. Information Propagation

The world should distinguish between:

**What happened**

and

**What people know or believe happened.**

Reputation information can spread through:

- witnesses
- official reports
- guild records
- guards
- merchants
- tavern rumor
- family and social networks
- faction messengers
- religion
- criminal informants
- newspapers, broadsheets, magical communication, or equivalent institutions where setting-appropriate

### Information Properties

A reputation event may track:

- source
- witnesses
- credibility
- evidence strength
- affected social network
- propagation range
- distortion / rumor risk
- whether the player is publicly identified

This prevents omniscient reputation updates.

---

## 14. Crime, Law and Evidence

Crime should interact with law, witnesses, evidence, relationships, and jurisdiction.

Possible factors:

- crime type
- victim status
- witnesses
- physical evidence
- local laws
- faction control
- player legal status
- known aliases
- corruption
- investigation capability
- public notoriety

Killing someone unseen does not automatically inform every settlement.

However, evidence can surface later.

Examples:

- recognizable stolen property
- survivor testimony
- divination
- tracked blood trail
- distinctive weapon wounds
- player boasting publicly
- an accomplice informing

### Legal Consequences

Depending on society:

- fines
- restitution
- arrest
- confiscation
- imprisonment
- exile
- revocation of license
- citizenship loss
- guild sanctions
- bounty
- trial
- faction retaliation
- blackmail

Law is contextual. Different societies may define crimes differently.

---

## 15. Reputation Is Not Morality

Reputation measures perception and track record.

Hidden behavioral history records patterns in actual choices.

They are related but not identical.

A secretly cruel character may maintain an excellent public reputation.

A misunderstood character may be publicly hated despite compassionate actions.

A tyrant may be feared, respected, and administratively effective.

A criminal may be beloved by an oppressed community.

### Design Rule

> **The world may judge the player incorrectly. The simulation must still remember what actually happened.**

---

## 16. Social Consequences of Reputation

Reputation can affect:

- dialogue tone
- greetings
- rumors
- prices
- credit
- willingness to negotiate
- access to jobs
- contract quality
- advance payment
- trust with valuable materials
- invitations
- sponsorship
- guild membership
- apprenticeships
- residency
- citizenship
- legal scrutiny
- guards
- criminal contacts
- political access
- romance or personal relationships
- hidden Job qualifications
- Titles
- companion reactions

Not every effect should be explicitly announced.

The player should often **feel** their reputation through changed treatment.

---

## 17. Fear, Respect and Affection

Social standing should not collapse into a simple like/dislike scale.

An NPC or faction may simultaneously:

- dislike the player
- respect their competence
- fear their violence
- owe them a debt
- trust them professionally

This supports villainous and morally mixed characters without making all negative relationships equivalent to content loss.

Example:

A frightened merchant may still serve a feared warlord, but:

- conversation becomes guarded
- guards watch closely
- rumors spread
- prices or service terms change
- private opportunities disappear
- coercive opportunities appear

---

## 18. Citizenship, Residency and Legal Identity

Otherworlders begin without an automatically recognized legal identity unless their Origin provides one.

Possible legal-status progression:

- Unregistered Foreigner
- Registered Traveler
- Temporary Resident
- Permanent Resident
- Citizen / Subject
- Guild-Recognized Professional
- Landholder
- Licensed Business Owner
- Officeholder or equivalent special status

Exact categories vary by society.

### Requirements May Include

- identity registration
- sponsor
- local reputation
- residence period
- employment
- taxes
- guild membership
- property
- military or civic service
- faction allegiance
- religious standing
- family / marriage ties
- exceptional grant by ruler or council

### Benefits May Include

- legal protection
- property rights
- business licenses
- better access to courts
- political participation
- certain Jobs
- restricted training
- public services
- reduced tariffs
- legal weapon ownership
- inheritance rights

Citizenship should create belonging and access, not merely a passive bonus.

---

## 19. Property

Property progresses from temporary shelter toward meaningful ownership.

Possible forms:

- inn room
- rented room
- rented workshop
- apartment
- house
- shop
- forge
- warehouse
- farm
- frontier claim
- estate
- guildhall

Property may provide:

- storage
- crafting access
- social status
- business operations
- worker housing
- relationship scenes
- customization
- local legal stake
- construction options

Property availability depends on local law, land supply, reputation, wealth, and world state.

---

## 20. Construction

Construction should use plots, properties, renovation opportunities, civic projects, and frontier claims rather than unrestricted survival-game wall placement by default.

Projects may require:

- legal permission
- land
- plans
- raw materials
- processed materials
- labor
- specialist professions
- money
- time
- security
- infrastructure

Relevant Skills and Jobs can reduce costs, unlock options, improve quality, or allow the player to perform parts of the work directly.

### Construction Types

- personal property upgrades
- workshop expansion
- commercial buildings
- fortifications
- roads / bridges
- civic structures
- faction projects
- housing
- hospitals
- shrines
- warehouses
- farms
- district redevelopment

Construction changes the physical world when feasible.

---

## 21. Settlement Development

The settlement system should treat buildings as parts of an economy and society rather than abstract upgrade buttons.

A settlement project can affect:

- labor demand
- material demand
- housing
- prosperity
- security
- trade
- services
- Job availability
- NPC migration
- faction power
- property values
- future construction

### Depth Before Breadth

Hearthcross remains governed by:

> **Settlement growth increases depth before breadth.**

A better Hearthcross becomes better at frontier life, expedition support, repair, medicine, local trade, Greyfen knowledge, and regional logistics.

It does not eventually contain every institution in the world.

---

## 22. Businesses and Ownership

Advanced civilian progression may allow the player to own or operate businesses.

Possible businesses:

- forge
- tavern
- clinic
- shop
- warehouse
- caravan company
- alchemy practice
- construction company
- mercenary office
- farm
- expedition company

Ownership should create decisions rather than passive money generation only.

Possible decisions:

- suppliers
- employees
- product specialization
- contracts
- pricing policy
- faction alignment
- expansion
- security
- illegal side business

Large businesses may eventually function partly through delegation so the player does not become trapped in management UI.

---

## 23. Hiring and Labor

Players may hire NPCs for work appropriate to the world.

Examples:

- guards
- porters
- builders
- craftspeople
- caravan workers
- clerks
- apprentices
- household staff
- specialists

Workers have costs, qualifications, relationships, and availability.

The game should abstract routine payroll and scheduling where detail would not create meaningful decisions.

---

## 24. Social Networks

NPC opinions can propagate through relationships.

NPCs may have simplified links such as:

- family
- employer / employee
- guild colleague
- friend
- rival
- patron
- client
- faction contact
- informant

A respected NPC endorsement can improve initial trust elsewhere.

A disliked NPC may spread negative stories.

Different social networks propagate information at different speeds and credibility.

### Guardrail

Do not attempt a fully simulated social graph for every ambient NPC.

Named and mechanically important NPCs receive richer relationship networks; background populations use settlement-level abstractions.

---

## 25. Integration with Jobs

Jobs are the primary way civilian capability becomes recognized identity.

Examples:

**Smith**

- can access forge work
- earns artisan reputation
- receives commissions
- may qualify for specialist Jobs

**Merchant**

- receives procurement opportunities
- gains access to wholesale markets
- can organize caravans

**Field Medic**

- can work clinics
- gains professional trust
- may receive emergency requests

**Smuggler**

- gains illicit logistics opportunities
- depends heavily on discretion reputation

Job qualification may consider professional reputation.

Example:

Smith Skill + completed commissions + artisan endorsement + low defect history → **Weaponsmith qualification**

---

## 26. Integration with Hidden Progression

Civilian behavior can contribute to hidden progression.

Examples:

- repeatedly working dangerous jobs without abandoning coworkers
- refusing exploitative contracts
- becoming famous for perfect delivery reliability
- quietly treating criminals without reporting them
- manipulating shortages for profit
- funding public works anonymously
- becoming indispensable to a settlement

Possible hidden identities:

- Oathbound Laborer
- Master Provisioner
- Black-Market Broker
- Civic Patron
- Plague Saint
- War Profiteer
- Kingmaker

Names are provisional examples.

---

## 27. Integration with Multiplayer

Player-owned character reputation travels with the character when appropriate, but social consequences occur inside the host's timeline.

Portable character state may include:

- professional history
- broad Titles
- Jobs
- Skills
- personal notoriety with cross-world institutions where fictionally valid

Host-world state includes:

- local NPC memories
- local legal status
- property
- settlement economy
- local business ownership
- local citizenship
- local crime investigations

Visitors should not automatically own property or citizenship in another player's timeline.

Co-op can support differentiated roles:

- adventurer
- crafter
- merchant
- surveyor
- healer
- logistics specialist

The game should not require every player to perform every profession.

---

## 28. Simulation Scope Guardrails

The goal is a **believable reactive world**, not exhaustive simulation.

Do not simulate detail unless it creates meaningful player-facing consequences.

Prefer:

- category-level settlement economy
- event-driven price changes
- generated shop stock from world state
- meaningful named-NPC memory
- abstract background-population behavior
- construction projects with visible results
- profession activities with decisions

Avoid by default:

- individual daily budgets for every NPC
- fully simulated food consumption for every citizen
- real-time offline economic collapse
- dozens of currencies
- mandatory daily chores
- excessive appointment micromanagement
- business spreadsheets that overwhelm adventuring

### Core Guardrail

> **Simulate causes deeply enough that consequences feel earned; abstract everything the player does not need to meaningfully understand or influence.**

---

## 29. Hearthcross Vertical-Slice Implementation

The first demo should prove only a thin slice of civilian life.

Recommended proof:

1. **Basic commerce** — buy and sell at two businesses with distinct stock and purchasing behavior.
2. **One ordinary work opportunity** — e.g. unloading a caravan, assisting the Split Anvil, or helping the Lantern House.
3. **Reliability consequence** — completing or abandoning an accepted work commitment changes later treatment.
4. **One professional-quality evaluation** — efficient/thorough/careless outcome changes reward or future work.
5. **One personal NPC memory** — a named NPC explicitly remembers a prior behavior.
6. **One small information-propagation event** — an action witnessed in one place affects a related NPC or institution later.
7. **One legal-status step** — player moves from unregistered outsider to registered traveler / recognized Hearthcross resident candidate.
8. **One settlement economic variable** — e.g. Road Safety or Medicine Supply affects stock, price, or available work.
9. **One profession interaction** — active Smith, Field Medic, Scout, or Survey Assistant changes how civilian content can be solved.
10. **No full property ownership, business management, or advanced citizenship simulation required for the first demo.**

This is enough to prove that Hearthcross is a society rather than a menu hub.

---

## Locked Principles

1. Civilian life belongs primarily to the World domain and reuses Skills, Jobs, relationships, and hidden progression.
2. Settlements have abstract but consequential economies.
3. Economic changes should produce stories, opportunities, shortages, and visible consequences.
4. Stores react to supply, prosperity, relationships, legality, and local capability rather than functioning as infinite static inventories.
5. Money supports living, property, professions, projects, travel, and social power in addition to combat progression.
6. Ordinary work exists and can lead naturally into relationships, Skills, Jobs, rumors, and adventures.
7. Professions are performable activities, not passive stat packages.
8. Job and Skill progression remain the primary profession-progression language; no separate universal profession tree is added.
9. Accepted work creates meaningful but fair commitments.
10. Reputation has Personal, Group, and Public layers.
11. Reputation derives from accumulated evidence and may be interpreted differently by different communities.
12. The game distinguishes what actually happened from what people know or believe happened.
13. Crime requires witnesses, evidence, investigation, or information propagation rather than omniscient global reputation loss.
14. Reputation is not morality.
15. Social standing may include fear, respect, trust, affection, debt, and professional confidence simultaneously.
16. Citizenship and residency represent social belonging, legal rights, and access.
17. Property and construction use locations, plots, law, materials, labor, money, and time rather than unrestricted free-building by default.
18. Settlement projects participate in the same economy and visibly alter the world when feasible.
19. Businesses can become meaningful advanced progression without becoming mandatory management games.
20. Simulation detail is added only when it creates player-facing choice or consequence.
21. The world should function without the player, but the player must be capable of changing how it functions.
