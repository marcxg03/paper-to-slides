# Paper → Slides

A workflow that turns a behavioral-science paper into a 3–5 slide, client-ready deck in the Irrational Labs style, inside Claude. You bring the paper and your own take; Claude does the extracting, checking, drafting and slide-building; you make every call that matters.

**You need:** a paid Claude plan (Pro, Max, Team or Enterprise) and a PDF of an empirical paper you've already chosen.
**Takes:** about 20–30 minutes, including writing your notes.

## Setup (once, about 3 minutes)
1. **Download this repo.** Click the green **Code** button → **Download ZIP**, then unzip it.
2. **Turn on file creation.** In Claude: **Settings → Capabilities →** turn on **Code execution and file creation**.
3. **Create a Project.** In Claude: **Projects → New project**. Name it "Paper to Slides".
4. **Add the instructions.** Open `workflow/project-instructions.md`, copy everything below the first line, and paste it into the Project's **Instructions** (click **Edit**).
5. **Add the workflow folder.** In the Project, click **Context → Add** and add the `workflow` folder (or upload every file inside it).

## Run it (each paper)
1. Open a **new chat** in the Project and upload the paper PDF.
2. Claude asks for **your own notes first**. Write them before you see anything from Claude.
3. Follow along. Claude will stop and ask you at each decision:
   - do the numbers look right?
   - is the master doc final?
   - which deck, A, B or C?
4. Export from the deck: **Share → Export** → PDF, PowerPoint or Google Slides.

The full walkthrough, with every step, prompt and screenshot, is in the **workflow doc**.

## What's in here
| File | What it is |
|---|---|
| `workflow/project-instructions.md` | The rules Claude follows in every chat (paste into Instructions) |
| `workflow/01-read-and-ingest.md` | Phase 1: your notes, extraction, summary, number check |
| `workflow/02-iteration.md` | Phase 2: building the master doc together |
| `workflow/03-deck-build.md` | Phase 3: three decks, refine one, presenter notes, export |
| `workflow/templates/` | Master doc and presenter-notes formats |
| `workflow/style/` | Irrational Labs style guide, example deck, logo |
| `CREDITS.md` | Open-source sources adapted in the workflow |

Version 1.0 · Built by Marcus Gao for the Irrational Labs work test, November 2026.
