# Phase 1: Read and ingest (steps 1 to 5)

Goal: capture the consultant's own thinking, then read the paper once and put everything the deck could need into the master doc, with sources, so no later step has to reread the paper or lean on the chat.

## Step 1: Setup (consultant)
The consultant sets up the Project (see the README), opens a new chat and uploads the paper. You wait for the PDF.

## Step 2: The consultant's notes come first (consultant, checkpoint)
- Send the opening message from the Project instructions.
- Don't summarize or hint at the content until the consultant replies.
- When their notes arrive, thank them in one line and say what comes next: "I'll set up the master doc and pull every finding and number from the paper with page references. About a minute."

## Step 3: Create the master doc and extract into it (you)
Create a Claude Doc named "Master doc · [short paper title]" from `templates/master-doc.md` and open it beside the chat. Paste the consultant's notes, word for word, into section 1.

Then read the whole PDF, including tables, figures and footnotes, and fill the extract table (section 5) directly in the doc. One row per item:
- finding: each result the authors report, with direction and size
- number: every N, percentage, mean, effect size, test statistic or p-value you might use
- definition: how the authors define the core concept
- citation: the paper's own reference, and any cited work you might mention

Each row gets a short verbatim quote and a location (page, table or figure). Tag any value read off a figure "from Fig. N". If a figure is unreadable, add a row that says so. Group rows by study. Don't put extracted content in the chat; it lives in the doc.

## Step 4: Summary (you)
Re-read the extract table, then write sections 2 and 3 of the master doc from it:
- Main claim: one plain-language paragraph on what the paper shows, why it matters, and how it connects to the consultant's goal of client-facing, actionable implications for product design. Start from the authors' own main claim, and note where the consultant's notes agree or differ.
- Studies: for each one, a one-line design, N, conditions, the key result with its number and page, and its role in the main claim.
- Featured study (the main-claim rule): name the study whose result shows the main claim most directly. The other studies become one supporting line ("this held across 3 studies"), unless one shows a different effect that matters for product decisions.

Leave product implications for Phase 2. In the chat, give a three or four line overview and point the consultant to the doc.

## Step 5: Number check 1 (you, then consultant; checkpoint)
Check every factual claim in sections 2 and 3, and in the consultant's notes, against the extract table.
- A claim passes when its number matches a row and the row's quote supports it.
- A claim fails when there's no row, the number doesn't match, or the quote doesn't support it. Cut it from the summary (or flag it in the consultant's notes) and list it.

Write the results into the number-check log (section 6) and show the short list of cuts and flags in the chat. Then ask: "These are the numbers I'll build on. Do they look right to you? Anything to add or correct?" The consultant answers for the evidence that reaches clients, so wait for their reply before Phase 2.

Then move to `02-iteration.md`.
