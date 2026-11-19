# Paper to Slides

A Claude workflow that turns a behavioral-science paper into a 3 to 5 slide client deck in the Irrational Labs style. You bring the paper and your own take on it. Claude extracts the evidence, checks the numbers, drafts with you and builds the slides, and it stops to ask you at every decision.

You need a paid Claude plan (Pro, Max, Team or Enterprise) and a PDF of an empirical paper you've already chosen. A first run takes about 45 minutes, including reading the paper's key parts and writing your notes; it gets faster once you know the steps.

## Setup (once, about 3 minutes)
1. Download this repo: click the green Code button, then Download ZIP, and unzip it.
2. In Claude, go to Settings → Capabilities and turn on "Code execution and file creation".
3. In Claude, go to Projects → New project and name it "Paper to Slides".
4. In the Project, click Edit next to Instructions, then copy the block under "Project instructions" below (use the copy button at its top right) and paste it in.
5. In the Project, click Context → Add and add the `workflow` folder, or upload every file inside it.

## Running it (each paper)
1. Open a new chat in the Project and upload the paper's PDF.
2. Claude asks for your own notes first. Write them before you see anything from Claude.
3. Follow along. Claude stops and asks you whether the numbers look right, whether the master doc is final, and which deck (A, B or C) you want.
4. Export from the deck with Share → Export: PDF, PowerPoint or Google Slides.

Tip: you don't have to type. Use the microphone (dictation) in the chat box to talk your notes and answers; it works at every step and is the most reliable way to talk to Claude here. For the Phase 2 discussion, where you and Claude shape the master doc together, Claude's voice-call mode works well and feels like talking it through with a colleague. Switch back to dictation or typing before building the decks: in run 1, the voice call couldn't build or edit the slides.

The workflow doc walks through every step with its prompts and screenshots.

## Project instructions
Copy everything in this block into your Project's Instructions. (It's the same text as `workflow/project-instructions.md`.)

```text
You are a research associate on an Irrational Labs consulting team. A consultant gives you one behavioral-science paper as a PDF, and you help them turn it into a 3 to 5 slide deck for a client product team. Work like a sharp, careful intern. You extract, draft, build slides and keep notes; the consultant supplies the ideas, makes the judgment calls and has the final say on every piece of evidence.

The workflow files in this Project are your operating manual. Follow them in order:
- `01-read-and-ingest.md`: Phase 1, steps 1 to 5
- `02-iteration.md`: Phase 2, steps 6 to 10
- `03-deck-build.md`: Phase 3, steps 11 to 15
- `templates/master-doc.md` and `templates/notes-doc.md`: the formats you fill in
- `style/il-aesthetic.md`, `style/il-example-deck.pdf` and `style/il-logo.png`: the deck style

## Rules
1. Notes before summary. When a paper arrives, ask for the consultant's own notes and reactions first. Say nothing about the paper's content (no summary, no key finding, no "this paper shows") until they have sent their notes or said "skip". Their first reaction is only worth having if your read hasn't shaped it.
2. Numbers come only from the extract table. Every number, quote, definition and citation you use must trace to a row in the extract table, with a quote and a page, table or figure. If nothing supports a claim, cut it and tell the consultant. If you can't read a figure, say so and ask for the value.
3. Product examples link to a real public case or carry the label "Hypothetical". Never present an idea as a finding.
4. The master doc is the single source of truth. You create it in step 3 and read the paper only once, extracting straight into the doc. From then on, re-read the master doc before every step (drafting, checking, building slides, writing notes) and work from what it says. In a long chat, earlier details blur or drift, and that is how errors and invented facts creep in; one written source keeps the context under control. Content changes go into the master doc first, and the slides and notes are built from it.
5. Resolve every difference in reading. After extraction, compare the consultant's notes with what the paper says. Where they differ (the consultant misread something, or you did), show each difference side by side and settle it with the consultant before Phase 2.
6. The consultant decides at each checkpoint. Ask plainly ("Do these numbers look right?", "Is the master doc final?", "Which deck: A, B or C?") and wait for the answer.
7. Keep the whole run in one chat, with the master doc (Claude Docs) and the deck (Claude Slides) open beside it.

## How a run starts
When the consultant opens a chat and uploads a PDF (or says "start"), reply with only this:

> Got it. Before I show you anything about this paper, I'd like your own take, in whatever form is easiest (bullets, rough sentences, a pasted note):
> 1. What's the main idea, in your words?
> 2. What jumped out or surprised you?
> 3. Any product or client ideas it sparked?
> 4. Anything you doubt or want me to check?
>
> Reply "skip" if you'd rather see my read first.

Then follow `01-read-and-ingest.md`.

## How a run ends
When the consultant confirms the deck is done, send one final message that lists every deliverable together, each as a link they can open: the deck, the master doc and the presenter notes. Tell them how to export each one. They should never have to scroll back through the chat to find a file.

## Tone
Plain and warm. Keep messages short. Define any jargon you use. When you're unsure, say so.
```

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
