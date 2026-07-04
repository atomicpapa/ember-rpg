# Playing EMBER on Desktop (with True Autosave)

On a computer, you can give EMBER the experience it was actually designed for: **the AI reads and writes your character and save files directly**, so autosave, resume, and carryover just *happen* — no copy-pasting text blocks. The trick is connecting a **filesystem MCP server** so the AI can touch the files in your EMBER folder.

> ⚠️ **This setup hasn't been playtested with EMBER yet.** The mechanism is standard, but the play experience is unproven. If you try it, [feedback is welcome](https://github.com/atomicpapa/ember-rpg/issues/new/choose).

## What you get

With a filesystem MCP pointed at your EMBER folder, the AI can:

- **Autosave for real** — write updates straight to `Saves/<Character> — <Scenario>.md` at every checkpoint, exactly as the rules describe. Power dies? Your progress is already on disk.
- **Resume by just asking** — "let's continue Sera's adventure" and it reads the character + save files itself; no pasting.
- **Handle carryover automatically** — at a scenario's end it updates the character file and appends the Legacy log.
- **Enforce genre-lock** — it reads the character's genre stamp from the file before starting a scenario.

## Who can do this

- **Claude Desktop app (Mac/Windows)** — yes, via a local filesystem MCP server (below).
- **Claude Code (CLI / IDE)** — yes, natively; it reads/writes your project files with no extra setup.
- **Claude.ai web / mobile app** — no local file access. Use [`PLAYING-BY-VOICE.md`](PLAYING-BY-VOICE.md) or the plain paste-and-play flow instead.
- **Other AIs** — if your app supports a local filesystem MCP/tool, the same idea applies.

## Setup: filesystem MCP on Claude Desktop

1. In Claude Desktop, open **Settings → Developer → Edit Config** (this opens `claude_desktop_config.json`).
2. Add a filesystem server scoped to **only your EMBER folder** (so the AI can't roam your whole disk):

```json
{
  "mcpServers": {
    "ember-files": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-filesystem",
        "/full/path/to/your/EMBER"
      ]
    }
  }
}
```

Replace `/full/path/to/your/EMBER` with the real path to the folder holding `EMBER — Core Engine.md`, `Characters/`, and `Saves/`.

3. **Restart Claude Desktop.** You should see the `ember-files` tools available.
4. Keep the rules handy: either paste the Core Engine + a Genre Pack into the chat, or (better) add them to a **Project** so every chat already knows them.

## Tell the AI how to use it

Give it a standing instruction at the start (or in your Project instructions):

> *You are my EMBER Game Master. The rules are in this folder via the filesystem tools. Read `EMBER — Core Engine.md` and the genre pack for rules. My characters live in `Characters/` and saves in `Saves/`. Follow EMBER's autosave rule literally: write my save file to `Saves/` at every checkpoint without me asking, and update my character file on XP spends and at scenario end. To resume, read the relevant character and save files yourself.*

Then just play. Roll your **2d6**, report the numbers, and let the AI keep the files current in the background.

## Notes & cautions

- **Scope the folder tightly.** Point the MCP only at your EMBER directory, not your home folder.
- **Back it up.** These are plain text files — a folder in a synced/backed-up location (or a git repo) means a bad write is never fatal.
- **It's still an AI.** Skim your save file now and then to confirm it's tracking state faithfully; the file being on disk doesn't guarantee the AI recorded everything perfectly. Early reports on how well this holds up are exactly the feedback we're after.

---

*Tried desktop autosave? Tell us how it went — [Playtest Feedback](https://github.com/atomicpapa/ember-rpg/issues/new/choose).*
