# Playing EMBER on Your Phone (Mobile)

EMBER plays great on a phone — type or talk, the AI narrates, you roll. If your app supports voice, it's a real bonus here: you talk, the AI speaks back, and you can play hands-free without looking at the screen. But mobile play in general (typed or spoken) has one wrinkle to plan around, and a simple setup that handles it.

> ⚠️ **This workflow hasn't been playtested yet.** It's our best-guess setup based on how the apps behave. If you try it, **feedback is especially appreciated** — what worked, what was clunky, what you'd change. Please [open a Playtest Feedback issue](https://github.com/atomicpapa/ember-rpg/issues/new/choose) and mention you were playing on mobile.

## The one wrinkle

On a phone, **the AI can't write files on your device.** So EMBER's automatic file-saving becomes: the AI keeps your game state in the conversation and **hands you an updated block of text to store** whenever you ask. You keep that text in a note. That's the whole trick — this applies whether you're typing or talking.

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

**During play:**
- Type or talk naturally — describe what your character does.
- When asked to roll, use a **dice app** (or just say/type *"I rolled a 9"*). You need **2d6**.
- Every so often, ask the AI to **read back your status** (*"Where do I stand — Harm, Conditions, what's on stage?"*) so you stay oriented without scrolling.
- At any pause, say/type *"Give me the updated save file,"* and paste it over your **save note**. Do this whenever you take a break, so a dropped connection or dead battery costs you nothing.

**When you spend XP or finish the scenario:**
- Say/type *"Give me the updated character file too,"* and store it in your **character note**. That's your permanent record.

## If you're playing by voice

Voice is the biggest advantage of mobile play — the AI can speak back, so you can go fully hands-free. A few tips specific to that mode:

- **Save often.** You can't rely on the app keeping the chat alive forever. A quick "give me the save file" every few scenes is cheap insurance.
- **Ask for status recaps out loud** instead of scrolling — the AI keeping you oriented verbally is what makes hands-free play work.
- **Let the AI drive the bookkeeping.** The rules tell it to track everything; you only reconcile your two notes at pauses.
- **Switching to desktop later?** Your character note is already portable Markdown — paste it into `Characters/` and keep going with the full file setup.

---

*Tried this? Tell us how it went — [Playtest Feedback](https://github.com/atomicpapa/ember-rpg/issues/new/choose). Mobile-play reports (typed or voice) help us make this smoother for everyone.*
