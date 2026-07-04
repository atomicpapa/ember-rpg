# Contributing to EMBER

Thanks for helping test and shape EMBER! Right now the project is in its **playtest phase**, so the most valuable contribution is simply **playing the game and telling us how it went**. You don't need to know Git or code — reading, playing, and reporting back is exactly what we need.

## How to playtest

1. **Grab the rules.** Open `EMBER — Core Engine.md`. If you want a genre other than fantasy, also grab one pack: `EMBER — Horror.md`, `EMBER — Science Fiction.md`, or `EMBER — Apocalypse.md`.
2. **Bring 2d6.** Two six-sided dice, physical or an app. You roll; the AI runs everything else.
3. **Paste Core (+ a pack) into your AI** of choice and say: *"Run Session Zero and be my Game Master."*
4. **Play.** Build a character or grab a pre-gen, and go. Try to reach an actual ending, or at least a natural stopping point.
5. **Report back** (see below).

## What makes feedback most useful

- **Be specific.** "The AI kept inventing difficulty numbers on Sway rolls" beats "combat felt off." Real rolls and real moments are gold.
- **Tell us the numbers' feel.** The **7–9 "success at a cost"** band, how deadly **Harm/Scars** felt, and the **XP costs** (5 tag / 5 move / 8 stat / 8 harden) are the things most likely to need tuning.
- **Note what the AI did**, not just the rules. If the GM forgot a Condition, skipped autosaving, or misread a move, that's a finding — the rules are written *for the AI to run*, so AI behavior is part of the test.
- **Try variety.** Different genres, different lenses, and a **multi-session save/resume** all stress different parts of the system.

## Structured playtesting (for comparable results)

Freeform play is great, but if you want your results to be directly comparable to someone else's — especially across different AI models — use:

- **`BENCHMARK-SCENARIO.md`** — a fixed setup ("The Hollow Keep," Sera Vane, same Session Zero answers every time) so everyone's starting from the same place.
- **`PLAYTEST-LOG-TEMPLATE.md`** — a structured log (rules exercised, drift incidents, specific rules the AI got wrong, save-file fidelity) instead of freeform impressions.

The goal of structured runs specifically is answering **"which rules do LLMs break most?"** — since EMBER's whole design bet is that an AI can run it consistently, that's the single most useful signal we can collect. Post the filled-in log as a Playtest Feedback issue, or link it if it's long.

## How to report

- **Playtest report:** Open a [new issue](https://github.com/atomicpapa/ember-rpg/issues/new/choose) and pick **Playtest Feedback**. The form walks you through it.
- **Just a rules question?** Start a [Discussion](https://github.com/atomicpapa/ember-rpg/discussions) instead.
- **Found a specific broken/unclear rule?** A regular issue is fine too.

Issues get triaged with these labels so nothing gets lost:

- `playtest` — a playtest report (applied automatically by the form)
- `balance` — number/difficulty tuning
- `rules-clarity` — a rule was unclear, ambiguous, or contradictory
- `new-content` — ideas for new genres, lenses, archetypes, or threats

## House rules & hacks welcome

EMBER is meant to be hacked. If you invented a house rule, a new lens, or a whole genre that worked at your table, tell us about it (an issue with `new-content`, or a Discussion). Good ideas may make it into the official rules — with credit.

## Proposing changes directly (optional, for the Git-comfortable)

If you'd like to submit an edit yourself:

1. Fork the repo and create a branch.
2. Make your change (everything is plain, portable Markdown — please keep it that way: no editor-specific syntax).
3. Open a pull request describing what you changed and why. For rules changes, a note on *why* it plays better is more persuasive than the change alone.

Small fixes (typos, clarity) are always welcome. For bigger mechanical changes, please open an issue to discuss first so we can talk it through before you spend the effort.

## License

EMBER is released under **[CC BY-SA 4.0](LICENSE)**. By contributing, you agree that your contributions are licensed under the same terms — anyone can share and adapt them with attribution, and derivatives stay open under the same license.
