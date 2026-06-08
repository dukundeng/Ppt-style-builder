---
name: ppt-style-builder
description: Use this skill whenever the user asks to make, redesign, imitate, improve, or generate a PowerPoint deck based on a reference PPT, a topic, an author, a company, a book, a report, or a classroom presentation. This skill is especially useful when the user wants Codex to learn a PPT style first, extract its visual system, gather images or generate visuals, write slide content, confirm the draft, and finally create an editable .pptx.
---

# PPT Style Builder

Use this skill to create a polished, editable PowerPoint deck by learning from a reference PPT, adapting its style, writing content, preparing visuals, and exporting a verified `.pptx`.

The repository-level workflow is platform-neutral. In Codex, follow the same sequence and use the local presentation, document, image, browser, and research tools that fit the task.

## Core Workflow

1. Understand the task:
   - topic
   - audience
   - language
   - target slide count
   - whether the reference is a strict template or a style source
   - whether the user wants close imitation or creative adaptation

2. Analyze the reference deck:
   - slide count and structure
   - section rhythm
   - cover, contents, divider, body, and closing slide patterns
   - color palette
   - typography hierarchy
   - image treatment
   - background style
   - recurring shapes, lines, panels, page numbers, and footers
   - weaknesses to avoid

3. Propose an adapted visual direction:
   - preserve useful tone, palette, hierarchy, image mood, and rhythm
   - improve spacing, readability, visual variety, factual visuals, and typography
   - ask the user to confirm before building

4. Research content and assets:
   - use reliable sources for facts
   - use verified real images for real people, books, companies, places, products, logos, screenshots, and covers
   - use generated images only for non-identity atmosphere
   - record sources

5. Write slide content first:
   - slide number
   - title
   - subtitle if useful
   - body copy
   - visual suggestion
   - highlight phrase or callout
   - ask the user to confirm the outline before generating the deck

6. Build editable slides:
   - use editable text boxes, shapes, callouts, timelines, cards, and image layers
   - avoid making every slide a flat screenshot
   - vary macro layouts
   - avoid three consecutive slides with the exact same layout

7. Render and inspect:
   - check thumbnails and full-size slides
   - verify readability, spacing, crops, contrast, overlap, clipping, spelling, and source integrity
   - treat automated background-overlap warnings as possible false positives only after visual inspection

8. Deliver:
   - final editable `.pptx`
   - short style adaptation note
   - source summary
   - known limitations

## Useful Repository Files

- `workflow.md` contains the complete platform-neutral workflow.
- `prompts/style-analysis.md` helps analyze the reference deck.
- `prompts/slide-outline.md` helps draft content before building.
- `prompts/slide-design.md` helps build the deck.
- `prompts/visual-qa.md` helps inspect the rendered result.
- `examples/classroom-author-presentation.md` provides a 15-slide classroom structure.

## Quality Rules

A good PPT should:

- feel related to the reference deck but not mechanically copied
- match the subject matter emotionally
- have a clear structure
- use fewer, stronger visual ideas
- keep body text readable
- use real sources for facts
- use verified identity images
- preserve editability

Avoid:

- copying every reference slide exactly
- using random decorative images
- overcrowding body slides
- making fake book covers, logos, portraits, or screenshots
- using generated images as factual evidence
- leaving typos such as `TAHNKS`
- ending after export without preview inspection
