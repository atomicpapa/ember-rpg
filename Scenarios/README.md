# Scenarios

A Scenario Pack is a prebuilt adventure — history, a villain, sub-bosses, resolution conditions, and optional key scenes — built entirely on existing Core mechanics. Packs are organized by genre subfolder (`Fantasy/`, `Horror/`, etc.).

Each pack splits into two files: a **Player doc** (safe to read — paste it to the AI or read it yourself) and a **GM doc** (spoilers — the true backstory, the villain, the resolution; don't read it yourself). Each pack's own folder README explains this split for that specific pack. Start here: `Scenarios/Fantasy/The Sunken Bell/`.

## Series numbering

Most scenario packs are standalone one-shots and need no code. When a scenario has earned a sequel, give the series a 2-3 letter code derived from the *first* scenario's name — drop articles like "The" (e.g. "The Sunken Bell" → `SB`). Number sequentially: `SB1`, `SB2`, `SB3`, so they sort together in a folder listing and give you reading order for free.

Once a series exists, the folder **and** both filenames (Player + GM docs) get the `<Code>N - ` prefix, e.g. `Scenarios/Fantasy/SB1 - The Sunken Bell/`, `SB1 - The Sunken Bell - Player.md`. A standalone scenario that later gets a sequel is renamed at that point to add the prefix.

Every entry after the first states plainly near the top, "Part 2 of the Sunken Bell series — play SB1 first" (and part 1 gets a matching "Part 1 of..." note added retroactively once a sequel exists).

This is a labeling and discoverability convention, not a mechanical gate — carry the same character forward via Core's normal carryover, no new mechanism needed. If a code collides with an existing series, just pick a different 2-3 letter abbreviation.

## Ruleset compatibility

Every pack's Player and GM docs carry a **"Built for Core Engine"** line (e.g. `v1.0`) stating which ruleset version they were written against. This is a compatibility marker, not an independent version number for the pack itself — packs don't need bumping every time Core changes, only if a future Core rules change (say, to the enemy-block format) actually affects how the pack plays.

## Starting a new pack

Copy `../Scenario Player Template.md` and `../Scenario GM Template.md` (repo root) and fill them in.
