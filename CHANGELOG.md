# EMBER Changelog

All notable rule changes to the EMBER Core Engine and Genre Packs, by version.

---

## Unreleased (on `develop`)

**New content type: Scenario Packs**
- Added `Scenario Player Template.md` and `Scenario GM Template.md` (repo root) — reusable blank templates for prebuilt adventures: history, a main villain, 1+ sub-bosses, resolution conditions, and optional key scenes, built entirely on existing Core mechanics (enemy blocks, Clocks, Threat tiers).
- Added a `Scenarios/` folder, organized by genre, with each pack split into a spoiler-safe Player doc and a GM-only doc.
- Added a **difficulty scaling** convention (Fresh / Seasoned tiers) so a pack's villain can scale to a new character or a veteran one, and a **series-numbering** convention (`SB1`, `SB2`, ...) for scenarios with sequels, documented in `Scenarios/README.md`.
- Added the first example pack: `Scenarios/Fantasy/The Sunken Bell/` (standalone, not yet part of a series).
- Added a "Ready-made adventures" pointer to `EMBER — Player's Guide.md`, alongside the matching README pointer added in this same round, so players discover Scenario Packs from either doc.

## v1.0 — 2026-07-04

First version-stamped release. Consolidates a round of design review (see `Reference/Research/2026-07-03-EMBER-RPG-System-Improvement-Recommendations.md`) into the rules.

**Core Engine:**
- Defined player-dealt harm explicitly: a successful Strike fills 1 segment baseline, 2 with an amplifying tag/weapon/position, 3 for an exploited weakness.
- Added an enumerated GM move list (hard moves) and a universal 7–9 cost menu, plus a "golden opportunity" rule for telegraphed-danger moves made independent of a roll.
- Reworked Push: now triggers *after* seeing a roll, turning a 6− into a 7–9, limited to once per scene (previously a flat +1 for a Condition, taken before rolling).
- Capped total Condition + Scar penalty at −2, mirroring the existing +2 situational cap.
- Stated the full resolution formula explicitly: `2d6 + stat (−1..+3) + situational (−2..+2)`, with tags/Conditions/Scars/push/help all sharing one combined situational bucket.
- Added a GM note that a maxed stat (+3) with a fully stacked situational bonus (+2) cannot miss by design — a narrow, earned edge case, not a gap.
- Added "Used this scene/session" and "Consumables remaining" lines to the STATUS block and Save File Template, to stop long sessions from losing track of limited-use moves and consumables.
- Added an explicit end-of-session XP checkpoint: two yes/no questions (pursued your Drive? deepened a Bond?) replace ad hoc "meaningful this session" judgment calls, capping Drive/Bond XP at 1 each per session. Miss XP is unchanged (marked immediately, uncapped).
- Renamed **Advantage/Disadvantage** to **Edge/Hindrance** throughout Core and the Science Fiction pack, to avoid an AI GM conflating it with D&D 5e's roll-2d20-keep-best mechanic.
- Added a version stamp to all rules files and a "Created under" field to the Character Sheet Template.
- Added a one-page GM Quick-Reference at the very end of Core (resolution, harm severity, XP, Conditions, GM move menus, threat tiers) — a compact end-of-document summary for both the AI GM and human readers.

**Horror pack:**
- Gave Resolve-as-sanity a concrete mechanic: a personal 6-segment "Unraveling" Clock ticks on missed Resolve rolls against the uncanny; filling it produces a psychological Scar and resets the Clock. Replaces the previous vague "coming apart" guidance.

**Minor consistency fixes:**
- Removed a doubled `---` divider near the end of Core.
- Clarified Harden as a permanent ability usable once per scene (was ambiguously worded).
- Fixed the Fantasy spark table header (said "roll d66," tables are single-d6).
- Quantified Recover's 10+ result ("clear up to 2 Harm segments," was unquantified).
- Player's Guide no longer overclaims autosave — now distinguishes desktop (automatic) from voice play (manual copy-back).

**Docs (outside the Fable review):**
- Renamed `PLAYING-BY-VOICE.md` → `PLAYING-ON-MOBILE.md` and reframed it: mobile (typed or spoken) is the actual scope, voice is one advantage of it (the AI can speak back), not the defining trait. Updated cross-references in the Player's Guide, `PLAYING-ON-DESKTOP.md`, and `README.md`.

- Added an annotated Example of Play at the end of "HOW TO RUN THIS GAME" (Sera Vane vs. skeleton warriors), demonstrating the core loop, a 7–9 cost, a miss + hard move, a Push, and a STATUS restatement — a few-shot exemplar for the AI GM and onboarding for human readers.

**Playtest infrastructure:**
- Added `BENCHMARK-SCENARIO.md` — formalizes "The Hollow Keep" (Sera Vane, fixed Session Zero answers, fixed opening framing) as a standard scenario, so different testers and AI models can be compared on the same setup.
- Added `PLAYTEST-LOG-TEMPLATE.md` — a structured log (rules-exercised checklist, drift incidents table, rules the AI got wrong, save-file fidelity check) aimed squarely at "which rules do LLMs break most," rather than freeform impressions.
- Fixed stale `PLAYING-BY-VOICE.md`/`advantage-disadvantage` references in the GitHub Playtest Feedback issue template.
- Wired both new docs into `CONTRIBUTING.md` (a new "Structured playtesting" section) and `README.md`'s file table.

All twelve items from the 2026-07-03 Fable review are now addressed.
