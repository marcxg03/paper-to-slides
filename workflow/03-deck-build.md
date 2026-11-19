# Phase 3 · Deck build (steps 11–15)

Goal: one polished 3–5 slide deck in the Irrational Labs style, built only from the master doc, plus a notes doc, ready to export.

## Step 11 · Build three decks (you)
**First re-read the final master doc in full.** Build from it, not from the chat history. Use **Claude Slides in this chat**. Build **three alternative decks, named A, B and C**, from the final master doc and its outline. Same content, different layouts. Follow `style/il-aesthetic.md` and match `style/il-example-deck.pdf`. Name them "Deck A · [layout idea]" etc. Tell the consultant in two or three lines what differs between them.

### Slide rules
- **3–5 slides**, following the master outline (default arc: concept → evidence → product application).
- **One message per slide.** The title states the takeaway as a full sentence ("Counting changes what counts"), not a topic label, unless the slide's job is different (e.g. a scenario slide asks a question: "Which hotel do you choose?").
- **Visual over text:** about 40 words or fewer of body text per slide. The headline + one visual should carry the slide.
- **Numbers the way IL shows them:** the result as before/after rates or percentages with big data labels; keep the paper's precision. Significance only as a plain-words footnote ("* statistically significant, p < .001"). No p-values in body text. No limitations slide.
- **Source line** bottom-right on every content slide: authors (year), in small gray text.
- **IL logo** (`style/il-logo.png`) bottom-left on every slide, recolored to the slide's palette.
- **Contrast:** no orange body text on a peach background; body text on any color fill must stay readable when projected.
- Every number on a slide must come from the master doc's extract table.

### Charts (adapted from anthropics `data-visualization`)
- Pick the chart by the question: **comparison between groups** → bar chart (start the axis at zero); **change over time** → line chart; **part of a whole** → stacked bar or a single highlighted %, not a pie with many slices.
- One chart per slide, two to four bars where possible. Label values directly on the bars; drop the gridlines and legend if direct labels suffice.
- Label the axis in plain words ("% who chose the luxury hotel").
- Studies on **different measures get separate charts**, never one shared axis.
- Use color to mean something (the highlighted condition in IL orange, the comparison in IL blue). Don't rely on color alone: label too.

### Storytelling (adapted from anthropics `pptx` deck-flow and assertion-evidence)
- Headline = the claim; body = the evidence for that claim.
- Lead with what the audience should conclude, then show why.
- The last slide answers "so what do we do?" for a product team.

## Step 12 · Pick and refine (consultant + you) ▶ checkpoint
Ask: **"Which deck do you want to go with: A, B or C?"** Then refine that one with the consultant: images, colors, wording, chart tweaks. They can also use the **Ask Claude** button under the slides.
- If they want to switch decks midway, confirm the letter and carry their content edits over to the new one.

## Step 13 · Content changes go through the master doc (you)
If a change touches content (a claim, number, example or headline), update the **master doc first**, then patch only the affected slides of the chosen deck. Leave every other slide unchanged. Purely visual changes (color, layout, image) go straight to the slides.

## Step 14 · Notes doc + speaker notes (you)
When the deck is settled, create a Claude Doc **"Presenter notes · [short paper title]"** from `templates/notes-doc.md`, built from the master doc (re-read it first) and the final slides. Then put each slide's notes into that slide's speaker notes.

## Step 15 · Export (consultant) ▶ checkpoint
Tell the consultant:

> Your deck is ready. To export, open the deck, click **Share → Export** and pick:
> - **PDF**: to send as is
> - **PowerPoint**: to edit offline (speaker notes included)
> - **Google Slides**: to edit and share in Drive (speaker notes included; it will ask you to connect Google Drive the first time)
>
> Export the master doc and presenter notes the same way (**PDF**), so the evidence trail travels with the deck.

The workflow ends here; sharing the files is up to the consultant.

---
*Chart and storytelling rules adapted from anthropics/knowledge-work-plugins `data-visualization` and anthropics/skills `pptx` (Apache-2.0, modified). See CREDITS.md.*
