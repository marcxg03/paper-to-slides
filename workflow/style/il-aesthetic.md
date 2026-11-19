# Irrational Labs deck style

Reference: `il-example-deck.pdf` and `il-example-slide-1.png` to `il-example-slide-5.png`, Irrational Labs' example deck on Chang, Kirgios, Mullainathan and Milkman (2024). Match this look.

## Format
16:9, 3 to 5 slides, plenty of white space, one idea per slide.

## Type
| Role | Font | Size | Notes |
|---|---|---|---|
| Headline | Oswald SemiBold | about 30 pt | condensed, bold, sentence case; a takeaway or a question |
| Body | Proxima Nova (Figtree or Montserrat if it's unavailable) | 15 to 25 pt | short sentences; bold the key phrase |
| Source line | body font | about 8 pt, gray `#888888` | bottom right on every content slide |
| Footnote | body font | about 8 pt | statistics in plain words, e.g. "* p < 0.001 (statistically significant)" |

## Color
| Name | Hex | Use |
|---|---|---|
| IL blue | `#016DB6` | full-bleed title panel; setup slides |
| Chart blue | `#266DB0` | comparison bar and its label |
| Navy text | `#0B4A7E` (approximate) | headlines and body text on light slides |
| Light blue panel | `#DBEAF4` | half-slide background on setup slides |
| IL orange-red | `#EC5431` | result headline, highlighted bar, emphasis |
| Peach panel | `#FBE3DD` | half-slide background on result slides |
| Muted gray-blue | `#9FB2BF` | de-emphasized elements |
| White | `#FFFFFF` | base |

Each slide sticks to one color family: blue for the concept and setup, orange-red for the result and everything after it. The switch in color marks the move from setup to finding.

## Layout
- Half-panel split: one half is a solid pastel or brand-color block, with text on one side and the visual on the other.
- Hand-drawn line illustrations and simple line icons, with at most one hero illustration (on slide 1).
- Charts: plain bars, light gridlines, very large colored data labels (in Oswald) above the bars, a dot legend, and the axis labelled in plain words.
- Logo: `il-logo.png` bottom left on every slide, tinted to the slide's color (white on IL blue).

## Voice
Speak to the audience as "you" ("You're planning a vacation…"). When the study allows it, let them experience the effect before you name it, as Irrational Labs' slides 2 and 3 do. Titles state takeaways rather than topics.

## Irrational Labs' example arc (a reference, not a template)
1. Concept: the name, a one-sentence plain definition and an illustration.
2. Scenario: the audience makes the study's choice themselves.
3. Twist: the same choice, shown again with the manipulation.
4. Result: one takeaway headline, one sentence and one two-bar chart.
5. Robustness: "What if…", answered with "The results still hold!"

Our decks must also cover product implications, which the example doesn't. Give them their own slide in the same style.
