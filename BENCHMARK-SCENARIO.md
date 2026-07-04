# EMBER — Benchmark Scenario: The Hollow Keep

*A standard, ready-to-run scenario for structured playtesting. Same setup every time, so results are comparable across different testers and different AI models — the point is to answer "which rules do LLMs break most?" with actual data, not vibes. For casual play, ignore this and build your own character; use `PLAYTEST-LOG-TEMPLATE.md` to record results here.*

## Setup (use exactly — don't customize, so runs stay comparable)

- **Rules:** `EMBER — Core Engine.md` only (Fantasy is baked in). No Genre Pack.
- **Lens:** Low & Hidden Magic (dials: Magic/Tech 1, Weirdness 1).
- **Character:** the pre-gen **Sera Vane — Disgraced Knight (Warrior)**. Might +2, Resolve +1, Grace +1, Presence 0, Wits −1. Tags: *Veteran, Enchanted blade, Reads people's tells.* Move: Hold the Line. Drive: *Clear her name.* Bond: *The squire who still believes in her (Pell).*
- **Session Zero answers to give the AI:** "Grim, tense folk-horror-ish fantasy. No lines or veils."
- **Opening framing** (paste this to the AI verbatim as the scenario prompt, after Session Zero and character selection):

  > *Sera Vane and her squire Pell have tracked the real killer of her old unit to the abandoned Hollow Keep. They've learned the deaths she was blamed for were the work of a wight-lord binding the dead to its will. Open the scene with Sera fighting through skeleton guardians into the flooded lower crypt — water rising, something ancient stirring behind a sealed door.*

## Target beats

*Things this scenario should naturally produce. Don't force them — but note in your playtest log if the AI never reaches one, or botches it.*

1. A **Read** or **Face Danger** roll landing 7–9 (a cost or Condition).
2. A **Strike** landing both 10+ and 7–9 at some point — confirms the harm-severity rule (1 / 2 / 3 segments) is applied correctly.
3. A **miss (6−)** and the resulting hard move.
4. Sera **pushing** at least once (taking a Condition to turn a 6− into a 7–9).
5. The **"crypt floods" Clock** advancing.
6. At least one **STATUS block** restatement.
7. A **save/resume cycle** — stop mid-scene, reload with the character and save files, confirm state restores exactly.
8. A scenario **ending** (through the sealed door, Taken Out, or retreat) that triggers carryover and a Legacy log entry.

## Why this scenario specifically

- The combat-heavy opening exercises Strike and hard moves immediately, without a slow warm-up.
- The rising-water Clock stress-tests Clock-ticking under time pressure.
- The Bond (Pell) and Drive (clear her name) are positioned to pay off if the run reaches the end-of-session XP checkpoint.
- Reforming skeleton guardians in a tight, flooding space are a good testbed for stacked Conditions (Wounded, Shaken, Compromised) against the −2 cap.
- It already has a known-good reference save state — see `Saves/Example — Sera Vane — The Hollow Keep.md` — so testers can compare their own resume against it rather than guessing whether their result looks right.

Use `PLAYTEST-LOG-TEMPLATE.md` to record a structured run, or the GitHub **Playtest Feedback** issue form for lighter, freeform notes.
