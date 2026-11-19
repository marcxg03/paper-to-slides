# Phase 3: Deck build (steps 11 to 15)

Goal: one polished 3 to 5 slide deck in the Irrational Labs style, built only from the master doc, plus presenter notes, ready to export.

## Step 11: Build three decks (you)
Re-read the final master doc in full and build from it, not from the chat history. Using Claude Slides in this chat, build three alternative decks named A, B and C from the master doc and its outline. They share the content and differ in layout. Follow `style/il-aesthetic.md` and match `style/il-example-deck.pdf`. Name them "Deck A · [layout idea]" and so on, and tell the consultant in two or three lines how they differ.

Slide rules:
- 3 to 5 slides, following the master outline (by default: concept, evidence, product application).
- One message per slide. The title states the takeaway as a full sentence ("Counting changes what counts"), unless the slide does a different job; a scenario slide, for example, can ask a question ("Which hotel do you choose?").
- Visual over text: about 40 words of body text per slide at most. The headline and one visual should carry the slide.
- Show numbers the way Irrational Labs does: results as before-and-after rates or percentages with large data labels, at the paper's precision. Significance appears only as a plain-words footnote ("* statistically significant, p < .001"). No p-values in body text and no limitations slide.
- A source line goes bottom right on every content slide: authors (year), in small gray text.
- The logo (`style/il-logo.png`) goes bottom left on every slide, recolored to match the slide.
- Never put orange body text on a peach background. Body text on a colored fill has to stay readable when projected.
- Every number on a slide comes from the master doc's extract table.

Charts (adapted from Anthropic's `data-visualization` skill):
- Choose the chart by the question. Comparing groups: a bar chart with the axis starting at zero. Change over time: a line chart. Part of a whole: a stacked bar or one highlighted percentage, never a pie with many slices.
- One chart per slide, with two to four bars where possible. Label values on the bars, and drop gridlines and the legend when the labels do the job.
- Label the axis in plain words ("% who chose the luxury hotel").
- Studies measured in different units get separate charts, never one shared axis.
- Color carries meaning: the highlighted condition in orange, the comparison in blue. Label as well, so color isn't the only cue.

Storytelling (adapted from Anthropic's `pptx` skill and the assertion-evidence method):
- The headline makes the claim and the body shows the evidence for it.
- Lead with what the audience should conclude, then show why.
- The last slide answers what a product team should do next.

## Step 12: Pick and refine (consultant and you; checkpoint)
Ask: "Which deck do you want to go with: A, B or C?" Then refine that deck with the consultant: images, colors, wording and charts. They can also use the Ask Claude button under the slides. If they switch decks partway through, confirm the letter and carry their content edits over.

## Step 13: Content changes go through the master doc (you)
When a change touches content (a claim, number, example or headline), update the master doc first, then change only the affected slides of the chosen deck and leave the rest alone. Visual changes such as color, layout or images go straight to the slides.

## Step 14: Presenter notes (you)
When the deck is settled, re-read the master doc and the final slides, then create a Claude Doc called "Presenter notes · [short paper title]" from `templates/notes-doc.md`. Copy each slide's key message and talking points into that slide's speaker notes.

## Step 15: Hand over everything in one place (you, then consultant; checkpoint)
When the consultant says the deck is done, send one message that gathers every deliverable, each as a link they can open, so nothing has to be found by scrolling:

> Everything is ready:
> 1. Deck: [deck name, linked]. Open it, click Share → Export and choose PDF (to send as is), PowerPoint (to edit offline; speaker notes included) or Google Slides (to edit and share in Drive; speaker notes included, and the first time it asks you to connect Google Drive).
> 2. Master doc: [linked]. Export it as a PDF the same way. It's the evidence trail: every number with its page.
> 3. Presenter notes: [linked]. Export as a PDF.

The workflow ends here. Sharing the files is up to the consultant.

---
Chart and storytelling rules are adapted from anthropics/knowledge-work-plugins `data-visualization` and anthropics/skills `pptx` (Apache-2.0, modified). See CREDITS.md.
