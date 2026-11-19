# Phase 1 · Read & Ingest (steps 1–5)

Goal: capture the consultant's own thinking, then pull everything the deck could need out of the paper **once**, with sources, so no later step has to reread it.

## Step 1 · Setup (consultant)
The consultant creates the Project (see the README), opens a new chat and uploads the paper PDF. Nothing for you to do until the PDF arrives.

## Step 2 · Consultant's notes first (consultant) ▶ checkpoint
- Send the opening message from the Project instructions.
- Do not summarize or hint at the content until the consultant replies.
- When their notes arrive, thank them in one line and say what happens next ("I'll pull every finding and number with page references, then summarize. About a minute."). Keep their notes word for word: they go into the master doc as their own section.

## Step 3 · Extract table (you)
Read the whole PDF, including tables, figures and footnotes. Build the extract table (format in `templates/master-doc.md`). One row per item:
- **finding**: each result the authors report (direction + size)
- **number**: every N, percentage, mean, effect size, test statistic or p-value you might use
- **definition**: how the authors define the core concept(s)
- **citation**: the paper's own reference (authors, year, title, journal) and any cited work you might mention

Each row has a **verbatim quote** (short) and a **location** (page, table or figure). Values you read off a figure get the tag "from Fig. N". If a figure is unreadable, add a row saying so. Group rows by study.

## Step 4 · Summary (you)
Write the summary using only the extract table:
- **Main claim**: one paragraph in plain language. What the paper shows, why it matters, and how it connects to the consultant's goal: client-facing, actionable implications for product design. Start from the authors' own main claim; note where the consultant's notes agree or differ.
- **Per-study blocks**: for each study: one-line design · N · conditions · key result with the number and page · its role in the main claim.
- **Which study carries the claim** (the main-claim rule): name the study whose result shows the main claim most directly. Other studies become one supporting line ("this held across 3 studies") unless one shows a *different* effect that matters for product decisions.
- Do **not** propose product implications yet. That happens in Phase 2.

## Step 5 · Number check #1 (you, then consultant) ▶ checkpoint
Check every factual claim in the summary **and in the consultant's notes** against the extract table:
- **Pass** = the number matches a row *and* the row's quote supports the claim.
- **Fail** = no row, a mismatch, or the quote doesn't support it. Cut the claim from the summary (or flag it in the consultant's notes) and list it.

Show a short check log:

| Claim | Extract row | Result |
|---|---|---|

Then ask: **"These are the numbers I'll build on. Do they look right to you? Anything to add or correct?"** The consultant owns the evidence that goes to clients, so wait for their answer before Phase 2.

Then move to `02-iteration.md`.
