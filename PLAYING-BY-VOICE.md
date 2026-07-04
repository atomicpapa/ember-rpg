# Playing EMBER on Your Phone (by Voice)

EMBER plays beautifully as a hands-free, voice-driven solo game on your phone — you talk, the AI narrates, you roll. But phone/voice play has one wrinkle to plan around, and a simple setup that handles it.

> ⚠️ **This workflow hasn't been playtested yet.** It's our best-guess setup based on how the apps behave. If you try it, **feedback is especially appreciated** — what worked, what was clunky, what you'd change. Please [open a Playtest Feedback issue](https://github.com/atomicpapa/ember-rpg/issues/new/choose) and mention you were playing by voice.

## The one wrinkle

On a phone, **the AI can't write files on your device.** So EMBER's automatic file-saving becomes: the AI keeps your game state in the conversation and **hands you an updated block of text to store** whenever you ask. You keep that text in a note. That's the whole trick.

## Set it up once

**1. Put the rules in a persistent "project" so you never re-paste them.**
- **Claude app:** create a **Project**, add `EMBER — Core Engine.md` and one Genre Pack (e.g. `EMBER — Horror.md`) as project knowledge. In the project instructions, put: *"You are my EMBER Game Master. Follow these rules. Run Session Zero on our first chat, and keep my SAVE FILE updated as we play so I can ask for it anytime."*
- **ChatGPT:** a **Project** or **Custom GPT** with the same files attached and the same instructions.
- **Gemini:** a **Gem** with the files and instructions.

Now every new chat in that project already knows EMBER — you just start talking.

**2. Make two notes** in something that syncs across your devices (Apple Notes, Google Keep, a Drive/iCloud text file):
- **Character note** — your durable, long-term record. This travels between scenarios *and* devices.
- **Save note** — the AI's working memory for the current scenario. Disposable; the AI regenerates it on request.

## Why two separate files (not one)

The two files change at very different rates, and keeping them separate keeps your character portable:

- **Save file** — changes constantly *during* a scenario (scene, Harm, Conditions, Clocks). You copy this back often.
- **Character file** — barely changes mid-scenario. It only updates when you **spend XP** or reach **the end of a scenario** (carryover). This is the file you carry to a new adventure — or back to your computer, where it drops straight into `Characters/` as plain Markdown.

Keeping them separate means your **character is a clean keepsake** you can reuse anywhere, while the save stays a throwaway scratchpad for one story.

## Playing a session

**Start:**
- Open a new chat in your EMBER project.
- Paste **both** your character note and save note, and say *"Resume from these."*
- *(First time ever:* just say *"Run Session Zero and be my Game Master."* Build a character; the AI will generate both files for you to save into your two notes.)

**During play (hands-free):**
- Talk naturally — describe what your character does.
- When asked to roll, use a **dice app** (or just say *"I rolled a 9"*). You need **2d6**.
- Every so often, ask the AI to **read back your status** (*"Where do I stand — Harm, Conditions, what's on stage?"*) so you stay oriented without looking at a screen.
- At any pause, say *"Give me the updated save file,"* and paste it over your **save note**. Do this whenever you take a break, so a dropped call or dead battery costs you nothing.

**When you spend XP or finish the scenario:**
- Say *"Give me the updated character file too,"* and store it in your **character note**. That's your permanent record.

## Voice tips

- **Save often.** You can't rely on the app keeping the chat alive forever. A quick "give me the save file" every few scenes is cheap insurance.
- **Ask for status recaps** instead of scrolling — voice play is better when the AI keeps you oriented out loud.
- **Let the AI drive the bookkeeping.** The rules tell it to track everything; you only reconcile your two notes at pauses.
- **Switching to desktop later?** Your character note is already portable Markdown — paste it into `Characters/` and keep going with the full file setup.

---

*Tried this? Tell us how it went — [Playtest Feedback](https://github.com/atomicpapa/ember-rpg/issues/new/choose). Voice-play reports help us make this smoother for everyone.*
