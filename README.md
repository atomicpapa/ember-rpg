# EMBER

**Engine for Multi-genre Emergent Roleplay** — a rules-light solo tabletop RPG designed to be run by an AI as your Game Master.

Paste the rules to an AI, tell it to run Session Zero, and play a solo adventure in any genre — fantasy, horror, sci-fi, apocalypse, or a world you invent on the spot. You roll the dice; the AI runs the world.

> **Status:** In development. The rulebook is being written; this repo is private until v1 is ready.

## What makes EMBER work

- **One elegant engine.** Roll **2d6 + a stat**: 10+ full success, 7–9 success at a cost, 6- a miss. Every roll becomes a story beat.
- **You roll all the dice.** The AI never rolls and can't fudge outcomes.
- **Five universal stats** (Might, Grace, Wits, Presence, Resolve) that reskin across any genre.
- **Genre-agnostic.** Swappable Genre Packs, each with tonal *lenses*, plus a procedure for the AI to build a brand-new genre from a one-line pitch.
- **Persistent characters.** Your character is saved to a file, carries XP and gear forward between adventures (within their genre), and the AI autosaves your progress so multi-session play never loses the thread.

## How to play

**You'll need two six-sided dice (2d6)** — physical dice or any dice-roller app. That's the only thing to bring; you roll, the AI runs everything else.

**New to EMBER?** Read **[`EMBER — Player's Guide.md`](EMBER%20%E2%80%94%20Player's%20Guide.md)** first — a plain-language overview of how the game works, without the rules meant for the AI.

1. Paste **`EMBER — Core Engine.md`** plus one **Genre Pack** (e.g. `EMBER — Horror.md`) into your AI of choice.
2. Tell it: *"Run Session Zero and be my Game Master."*
3. Build a character (or pick a pre-gen) and start playing. Roll real dice when asked and report the results.
4. To resume later, also paste your **Character** file and **Save** file.

Want to play hands-free on your phone? See **[`PLAYING-BY-VOICE.md`](PLAYING-BY-VOICE.md)** (untested — feedback wanted).

## Files

| File | What it is |
|---|---|
| `EMBER — Player's Guide.md` | Plain-language overview of how the game works — read this first. (You don't paste this to the AI.) |
| `EMBER — Core Engine.md` | The complete game + a baked-in Fantasy genre. Paste this to the AI. Playable on its own. |
| `EMBER — Horror.md` / `EMBER — Science Fiction.md` / `EMBER — Apocalypse.md` | Lensed Genre Packs. |
| `Character Sheet Template.md` | Blank, portable character sheet. |
| `Save File Template.md` | Blank save/resume snapshot. |
| `Characters/` · `Saves/` | Your persistent characters and in-progress scenarios. |

## Design lineage & credits

EMBER's core is built on the shoulders of the **Powered by the Apocalypse (PbtA)** family of games, and it owes them an open thank-you:

- **[Apocalypse World](https://apocalypse-world.com/)** by D. Vincent Baker & Meguey Baker — the origin of the 2d6 **10+ / 7–9 / 6−** resolution, "moves" that trigger from the fiction, marking XP on a miss, and GM principles like "be a fan of the characters" and "make a hard move."
- **Dungeon World** by Sarah Richardson, Sage LaTorra & Adam Koebel — a big influence on the fantasy framing, Bonds, and the advancement style.
- **[Ironsworn](https://www.ironswornrpg.com/)** by Shawn Tomkin — the model for solo play, oracle/spark tables, and progress tracks.

What EMBER brings of its own is the *assembly and tuning* rather than the primitives: the genre-agnostic five-stat array, the Bite × Duration **Scar** system, the umbrella-genre **lens** structure, persistent character files with genre-lock and carryover, and the whole design around being **run by an AI Game Master** (autosave, state-tracking, and the GM operating manual). Game mechanics aren't copyrightable — only their expression — and all of EMBER's text is original wording, but crediting lineage is simply good manners in the tabletop community.

## License

EMBER is released under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](LICENSE). You're free to share and adapt it, including commercially, as long as you give credit and license your derivatives under the same terms.
