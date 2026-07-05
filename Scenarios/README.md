# Scenarios

A Scenario Pack is a prebuilt adventure — history, a villain, sub-bosses, resolution conditions, and optional key scenes — built entirely on existing Core mechanics. Packs are organized by genre subfolder (`Fantasy/`, `Horror/`, etc.).

Each pack splits into two files: a **Player doc** (safe to read — paste it to the AI or read it yourself) and a **GM doc** (spoilers — the true backstory, the villain, the resolution; don't read it yourself). Each pack's own folder README explains this split for that specific pack. Start here: `Scenarios/Fantasy/SB1 - The Sunken Bell/`.

## Module numbering

Every scenario pack gets a module code from the moment it's written — standalone or not. The code is a 2-3 letter abbreviation derived from the scenario's own name, dropping articles like "The" (e.g. "The Sunken Bell" → `SB`, "The Ashworth Acquisition" → `AA`). Every pack starts at `1`: `SB1`, `AA1`, and so on.

The folder **and** both filenames (Player + GM docs) always carry the `<Code>N - ` prefix, e.g. `Scenarios/Fantasy/SB1 - The Sunken Bell/`, `SB1 - The Sunken Bell - Player.md`. In-document H1 titles stay plain (no code in the title itself) — the code is a filename/folder cataloging convention, not part of the story's presentation.

Because every pack is born with its code already in place, a first installment never needs to be renamed later. If "The Sunken Bell" (`SB1`) ever earns a sequel, that sequel becomes `SB2` — `SB1`'s own folder and filenames don't change at all. Every entry after the first states plainly near the top, "Part 2 of the Sunken Bell series — play SB1 first" (and `SB1`'s own docs get a matching "Part 1 of..." note added at that point). A true standalone with no sequel simply stays at `<Code>1` forever, with no "Part 1 of..." note needed.

This is a labeling and discoverability convention, not a mechanical gate — carry the same character forward via Core's normal carryover, no new mechanism needed. If a code would collide with an existing one, just pick a different 2-3 letter abbreviation.

## Ruleset compatibility

Every pack's Player and GM docs carry a **"Built for Core Engine"** line (e.g. `v1.0`) stating which ruleset version they were written against. This is a compatibility marker, not an independent version number for the pack itself — packs don't need bumping every time Core changes, only if a future Core rules change (say, to the enemy-block format) actually affects how the pack plays.

## Starting a new pack

Copy `../Scenario Player Template.md` and `../Scenario GM Template.md` (repo root) and fill them in. Give the new pack its module code from the start (see "Module numbering" above) — don't ship it without one.
