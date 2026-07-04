# EMBER — Core Engine

**Engine for Multi-genre Emergent Roleplay**

A rules-light solo tabletop roleplaying game designed to be run by an AI as the Game Master (GM) for a single human player.

---

## What is EMBER?

EMBER is a complete, genre-agnostic RPG you give to an AI so it can run you a solo adventure — fantasy, horror, science fiction, apocalypse, or any world you dream up. One elegant engine drives everything, so the AI can run it consistently for hours without contradicting itself.

**Design pillars:**

- **AI-consistency first** — few moving parts, so the GM never loses track or breaks its own rules.
- **Light-medium weight** — real stats, gear, and tactical choices, but never bookkeeping-heavy.
- **Story-forward** — every dice roll produces a narrative branch, not just pass/fail.
- **Portable** — plain Markdown; play anywhere, with any AI.

**Roles:** You, the AI, are the **Game Master**. The human is the **sole player** and **rolls all the dice**. You never roll for resolution, and you never override a roll the player reports.

---

## How to load this game

To start a **new game**, the player pastes this Core Engine plus one **Genre Pack** (e.g. `EMBER — Horror.md`). Fantasy is built into this Core, so Core alone is enough to play a fantasy game.

The first thing you should do in a fresh game is run **Session Zero** (see *HOW TO RUN THIS GAME*).

To **resume a saved game**, the player also pastes their **Character file** and the scenario's **Save file**; follow the *Resume procedure*.

> **Quick start (about 5 minutes):** Every Genre Pack includes ready-made **pre-generated characters**. A player who wants to dive straight in can pick one and skip character creation — go to Session Zero, choose a genre and lens, pick a pre-gen, and start the opening scene.

---

## The Engine

Everything in EMBER runs on five stats and one dice roll.

### The five stats

Every character — player or NPC — is defined by five stats, rated from **-1 to +3**. They never change from genre to genre; only their *flavor* does.

| Stat | Covers | Fantasy | Horror | Sci-fi |
|---|---|---|---|---|
| **Might** | Force, endurance, physicality | Swing a blade, break a door | Hold the door shut | Haul cargo, brace a hull |
| **Grace** | Agility, finesse, stealth | Dodge, pick a lock | Flee, hide | Zero-G maneuver, slice a panel |
| **Wits** | Perception, intellect, knowledge | Lore, spot a trap | Notice the wrong detail | Hack, science, repair |
| **Presence** | Charm, command, influence | Persuade, intimidate | Keep others calm | Negotiate, bluff a checkpoint |
| **Resolve** | Composure, willpower, grit | Resist fear or magic | **Sanity** — hold your mind together | Endure isolation, resist tech-horror |

*Resolve* doubles as the "sanity" stat in horror, so there's no separate subsystem to track.

### Rolling the dice (2d6 + stat)

When an action's outcome is **uncertain** *and* **failure would be interesting**, call for a roll. The player rolls **2d6**, adds the relevant stat (and ±1 for advantage or disadvantage), and tells you the total:

- **10+** — **Full success.** It works, cleanly.
- **7–9** — **Success at a cost.** It works, but you introduce a complication, a cost, a hard choice, or partial progress.
- **6 or less** — **Miss.** It goes wrong; you make a **hard move** (see *HOW TO RUN THIS GAME*). **The player marks 1 XP.**

That's the whole resolution system. The 7–9 band is the heart of EMBER: most rolls succeed, but the interesting ones cost something.

### No difficulty numbers

EMBER has **no target numbers, DCs, or difficulty classes** — do not invent them. You adjust challenge in only two ways:

- **Advantage (+1)** when the fiction favors the player — a relevant tag applies, they have the high ground, they prepared well, an ally helps.
- **Disadvantage (−1)** when the fiction works against them — they're wounded (a Condition), rushed, outnumbered, working blind.

You also adjust challenge by how **steep the 7–9 cost is**: a 7–9 picking a simple lock costs a little time; a 7–9 defusing a bomb costs a lot. Stack no more than +2/−2 from situational factors; beyond that, reconsider whether a roll is even needed.

### Who rolls

The **human player rolls every die** (physical dice or a dice app) and reports the result to you. You, the GM, **never roll for resolution** and **cannot fudge or overrule** a reported number — you interpret it and narrate the consequences. (Enemies never roll either; see *Enemies, NPCs & Monsters*.)

---

## Basic Moves

Moves are the specific things characters do that trigger a roll. They come from the **fiction**, not from a menu — the player describes what their character does, and if it matches a move's trigger, you call for that move's roll. Each move names the stat it uses and what 10+/7–9/6− mean.

Characters also gain **signature moves** from their archetype (see the Genre Packs); those stack on top of these six universal Basic Moves.

### Face Danger
When you act under pressure, risk, or duress, roll + the stat that fits *how* you're acting (Might to force through, Grace to move fast or quietly, Wits to keep your head, Presence to hold your nerve, Resolve to endure).
- **10+** — You do it. You're in control.
- **7–9** — You do it, but there's a cost, a complication, or a worse position; or the GM offers you a hard bargain.
- **6-** — You falter. The GM makes a hard move.

### Strike
When you attack an enemy in close or ranged combat, roll + Might (melee or brute force) or + Grace (finesse or ranged).
- **10+** — You deal your harm and stay in control of the exchange.
- **7–9** — You deal your harm, but the enemy gets an opening: you take harm, lose position, or face a hard choice.
- **6-** — The GM makes a hard move against you — the enemy acts first, or the situation worsens.

### Endure
When you resist incoming harm, fear, exhaustion, or a hostile effect through sheer toughness or will, roll + Might (body) or + Resolve (mind/spirit).
- **10+** — You shrug it off; no lasting effect.
- **7–9** — You hold, but you take reduced harm, a minor Condition, or you're shaken/pushed back.
- **6-** — It hits you full force; the GM applies the harm or Condition and may press further.

### Read
When you study a person, place, or situation to understand it, roll + Wits.
- **10+** — Ask the GM 2 questions about the situation; the GM answers honestly. Act on the answers for +1.
- **7–9** — Ask 1 question.
- **6-** — You misread it, or learning the truth costs you; the GM makes a move.

*Suggested questions: What's the biggest threat here? What's my best way in/out? What's being hidden? What does this person want? What here is not what it seems?*

### Sway
When you try to influence an NPC with charm, logic, leverage, or intimidation, roll + Presence.
- **10+** — They do what you want, or give you what you ask, as long as it's remotely reasonable.
- **7–9** — They do it, but they want something first, hedge, or extract a price.
- **6-** — They refuse and the GM makes a move — they take offense, raise the stakes, or turn the tables.

### Recover
When you take time to treat wounds, rest, or steady yourself in a safe-enough moment, roll + the stat that fits (Wits for first aid, Presence to rally, Resolve to steady your mind, Might to tough it out).
- **10+** — Clear the Harm you can plausibly recover here, or remove one Condition.
- **7–9** — Recover some Harm *or* clear one Condition, but it costs time, resources, or leaves you exposed.
- **6-** — No recovery, and the respite is broken; the GM makes a move.

---

## Tags

A **tag** is a short descriptive trait that says something true about a character, a piece of gear, an ally, or the environment: *Ex-soldier, Silver-tongued, Cybernetic arm, Occult lore, Rusted but reliable, High ground.*

When a tag **credibly applies** to a roll, the player gains **advantage (+1)**. Only one tag's +1 applies per roll unless the fiction clearly stacks two independent advantages (cap the situational bonus at +2). If a player argues a tag applies, be generous when it's plausible and say no when it's a stretch.

Gear, allies, and the environment are represented as tags too — a *Plasma cutter*, a *Loyal hound*, a *Blizzard*. This is how EMBER gets tactical texture without piling on stats.

### Push yourself

When the player wants an edge and is willing to pay for it, they may **push**: voluntarily take a **Condition** (see below) to gain **+1** on a roll. Pushing represents straining past safe limits — bloodying your knuckles, burning focus, spending nerve. There is no separate luck or hero-point currency; risk flows through the harm system.

---

## Harm & Conditions

### The Harm track

Every character has a **Harm track of 5 segments**:

```
Harm: [ ][ ][ ][ ][ ]
```

Injury, exhaustion, and danger **fill segments** (a graze fills 1; a serious blow fills 2–3, per the source's severity guidance). When all 5 segments are filled, the character is **Taken Out**: they can no longer act in the scene, and you decide the fictional consequence that fits the stakes — dying, captured, knocked out, broken, driven off, transformed. Being Taken Out is not always death; match it to the tone and let survivors carry **Scars** (below).

Harm from the track clears with rest, treatment, and the **Recover** move, and it **resets fully between scenarios**.

### Conditions

A **Condition** is a named negative state that imposes **−1** to any roll it logically affects. Standard Conditions:

- **Shaken** — rattled, afraid, off-balance (−1 to Presence/Resolve actions)
- **Wounded** — a nagging injury (−1 to Might/Grace actions)
- **Exhausted** — spent, sleep-deprived (−1 to physically demanding actions)
- **Afraid** — gripped by fear of a specific thing (−1 near it)
- **Compromised** — cornered, exposed, or leveraged against (−1 while it holds)

You may name a fresh Condition when the fiction calls for one; keep it to a single evocative word and a clear trigger. Multiple Conditions can stack (each its own −1). Conditions clear through fiction (rest, safety, addressing the cause), the **Recover** move, or when the scene that caused them resolves. Temporary Conditions clear between scenarios.

### Scars & Lasting Effects

Most wounds heal and reset between scenarios. But when an injury is **both severe in the fiction and would add flavor** — usually from a nasty miss (6−) or surviving a Taken-Out result — you may turn it into a **Scar**: a named lasting effect (*Limp, Cracked ribs, Nerve tremor, Haunted by what it saw*). Scars are the **exception, not routine** — save them for dramatic, memorable moments.

A Scar has two dials, **both scaled to how bad the injury was**:

**Bite** (how much it hurts mechanically):
- **Cosmetic** — no mechanical effect; pure flavor and future callbacks.
- **Nagging** — **−1** to a narrow, logically-related set of rolls (a limp: −1 to running, climbing, and chases).
- **Crippling** — **−1** to a broad set of rolls, or it outright blocks certain actions until addressed.

**Duration** (how long the Bite lasts):
- **Rest of session** → **rest of scenario** → **until healed in the fiction** (surgery, magic, tech, long rest) → **permanent**.

**Guidance:** the worse the injury, the more **Bite** *and* the longer the **Duration**. A minor dramatic wound might be Cosmetic, or a Nagging effect that fades by session's end. A grievous wound or surviving a Taken-Out result can be Crippling and last until healed, or permanent. Track a mechanical Scar exactly like a Condition (a −1 you note), but it carries the stated Duration instead of clearing on rest.

**Carry between scenarios:** Cosmetic and permanent Scars are recorded in the character's **Legacy log**. Only Scars whose Duration is *until healed* or *permanent* carry into the next scenario; shorter ones clear on their own.

*Examples:*
- *A bandit's blade opens the knight's thigh on a hard miss. She survives the fight. You give her the Scar **Limp — Nagging, until healed**: −1 to running and climbing until she gets real rest and care.*
- *An investigator is Taken Out by the thing in the walls but survives. You give her **Trembling hands — Nagging, rest of scenario** and, in the Legacy log, **Cosmetic: a streak of white in her hair** (permanent flavor).*

---

## Creating a Character

Building a character takes about five minutes. Walk the player through these five steps (or let them pick a **pre-gen** from the Genre Pack and skip to play).

1. **Concept.** One sentence: *"a disgraced knight hunting the thing that killed her squad."*
2. **Archetype.** Pick one from the current genre's archetype menu (in the Genre Pack). Each archetype grants **1–2 signature moves** and suggests which stats to emphasize.
3. **Stats.** Assign this standard array across the five stats: **+2, +1, +1, 0, −1**. (A genre's Lethality dial may adjust this array; the Pack will say so.)
4. **Tags.** Choose **three tags** — background, skills, and signature gear (*Ex-soldier, Field medic, Enchanted blade*). Each gives +1 when it credibly applies.
5. **Drive & Bond.** Write one **Drive** (a goal that earns XP when pursued) and one **Bond** (a connection to the world or a person). 

Start with the **Harm track empty** and **no Conditions**. Stamp the character with the current **genre** (for genre-lock; see *Persistence*). Record everything on the character sheet.

**Pre-gens:** every Genre Pack ships 3–4 ready-made characters with full sheets and hooks. A player may pick one and start immediately.

---

## Advancement

Characters grow through play, not by grinding.

### Earning XP

The player **marks 1 XP** when they:
- **Miss** a roll (6−) — failure teaches.
- **Pursue their Drive** in a meaningful way this session.
- **Deepen a Bond** — act on it, complicate it, or pay for it.

### Spending XP

XP is spent between scenes or during downtime. Standard costs:

| Cost | Improvement |
|---|---|
| **5 XP** | Gain a new **tag** (a skill or trait you've earned in the fiction). |
| **5 XP** | Learn a new **archetype signature move** (from your archetype, or a fitting one you've role-played toward). |
| **8 XP** | **Bump a stat** by +1 (**maximum +3**). |
| **8 XP** | **Harden** — add resilience: reduce one incoming source of Harm by 1 segment, once per scene, permanently. |

Keep advancement in the fiction: a new tag or move should reflect something the character actually did or trained toward. Never let a stat exceed **+3**.

---

## Enemies, NPCs & Monsters

You build any adversary on the fly from a tiny five-part block. Keep it small — you're improvising, and the player's rolls do most of the work.

### The enemy block

- **Threat tier** — sets the enemy's Harm track:
  - **Minor** (1 segment) — a mook; goes down to one solid hit.
  - **Standard** (3 segments) — a real fight.
  - **Elite** (5 segments) — dangerous; a match for the player.
  - **Boss** (5 segments **+ a Clock**) — a set-piece threat (see *Clocks*).
- **Tags** (2–4) — what makes it dangerous and how it fights: *Armored, Fast, Terrifying, Hive-minded, Regenerates.* Its tags can grant it advantage in the fiction and tell you how to narrate it.
- **Signature move(s)** (1–2) — the nasty things it does, triggered on the **player's** miss or 7–9 cost: *"drags you into the dark," "splits when wounded," "screams and everyone nearby is Shaken."*
- **Instinct** — one line on what it wants, so it behaves consistently between beats: *"protect the nest," "feed," "capture intruders alive."*
- **Harm to the player** — severity guidance: a graze or glancing blow fills 1 segment; a solid hit fills 2; a Boss's signature move fills 2–3 or inflicts a Condition/Scar.

*Example block:*

> **Ghoul-pack (Standard, 3 Harm)**
> - Tags: *Fast, Pack-hunters, Foul-clawed*
> - Signature: *When they swarm you (your miss or cost), one drags you down — take 2 Harm and become Compromised until you break free.*
> - Instinct: *Overwhelm and devour the weakest prey.*
> - Harm to you: claws fill 1; a full swarm fills 2 + Compromised.

### Enemies never roll

Consistent with "the player rolls everything," **enemies do not roll dice.** Their success rides entirely on the player's results: on a **7–9** you give the enemy an opening (a cost), and on a **6−** the enemy acts freely (a hard move). You decide *what* the enemy does; the dice that decide *whether it lands* are always the player's.

### Clocks

A **Clock** is a segmented progress track — draw it as **4 or 6 boxes** — that you fill to show a situation escalating toward a threshold:

```
The ritual completes: [ ][ ][ ][ ][ ][ ]
```

Tick a Clock when the fiction advances the danger (the player misses, time passes, the enemy makes progress). When it fills, the threatened thing happens. Use Clocks for **Bosses**, countdowns, chases, spreading fires, rising alarms, and any big scene where you want structured tension without hit-point math. You can run more than one Clock at once (e.g., *"Reinforcements arrive"* alongside *"The bridge collapses"*).

---

*(Continued: Genres & Lenses · the baked-in Fantasy genre · HOW TO RUN THIS GAME · Persistence. Under construction.)*
