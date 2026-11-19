# Paper to Slides

A Claude workflow that turns a behavioral-science paper into a 3 to 5 slide client deck in the Irrational Labs style. You bring the paper and your own take on it. Claude extracts the evidence, checks the numbers, drafts with you and builds the slides, and it stops to ask you at every decision.

You need a paid Claude plan (Pro, Max, Team or Enterprise) and a PDF of an empirical paper you've already chosen. Plan on 20 to 30 minutes, including the time to write your notes.

## Setup (once, about 3 minutes)
1. Download this repo: click the green Code button, then Download ZIP, and unzip it.
2. In Claude, go to Settings → Capabilities and turn on "Code execution and file creation".
3. In Claude, go to Projects → New project and name it "Paper to Slides".
4. Open `workflow/project-instructions.md`, copy everything below its first line, and paste it into the Project's Instructions (click Edit).
5. In the Project, click Context → Add and add the `workflow` folder, or upload every file inside it.

## Running it (each paper)
1. Open a new chat in the Project and upload the paper's PDF.
2. Claude asks for your own notes first. Write them before you see anything from Claude.
3. Follow along. Claude stops and asks you whether the numbers look right, whether the master doc is final, and which deck (A, B or C) you want.
4. Export from the deck with Share → Export: PDF, PowerPoint or Google Slides.

The workflow doc walks through every step with its prompts and screenshots.

## Files
| File | What it is |
|---|---|
| `workflow/project-instructions.md` | The rules Claude follows in every chat (paste into Instructions) |
| `workflow/01-read-and-ingest.md` | Phase 1: your notes, the master doc, extraction, summary, number check |
| `workflow/02-iteration.md` | Phase 2: finishing the master doc together |
| `workflow/03-deck-build.md` | Phase 3: three decks, refining one, presenter notes, export |
| `workflow/templates/` | The master doc and presenter-notes formats |
| `workflow/style/` | The Irrational Labs style guide, example deck and logo |
| `CREDITS.md` | Open-source sources adapted in the workflow |

Version 1.0. Built by Marcus Gao for the Irrational Labs work test, November 2026.
