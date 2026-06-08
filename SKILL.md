---
name: ppt-style-builder
description: Use this skill whenever the user asks to make, redesign, imitate, improve, or generate a PowerPoint deck based on a reference PPT, a topic, an author, a company, a book, a report, or a classroom presentation. This skill is especially useful when the user wants Codex to learn a PPT style first, extract its visual system, gather images or generate visuals, write slide content, confirm the draft, and finally create an editable .pptx.
---

# PPT Style Builder

## Purpose

Create a polished, editable PowerPoint deck by learning from a reference PPT, adapting its style, writing content, preparing visuals, and exporting a verified `.pptx`.

The goal is not to blindly copy the reference deck. Preserve the useful visual language while making thoughtful improvements for the new topic.

## When To Use

Use this skill when the user asks for any of these tasks:

- learn or imitate a PPT style
- create a new PPT from a topic and a reference deck
- redesign a deck while keeping its tone
- make a classroom author, book, company, report, or speech deck
- search for images or generate visual assets for a PPT
- write slide content first, then generate the deck after confirmation

## Workflow

### 1. Understand The Task

Identify:

- topic of the new PPT
- audience, such as classroom, business, academic, speech, report
- language requirement
- target slide count
- whether the provided PPT is a strict template or only a style reference
- whether the user wants exact imitation or creative adaptation

If the user provides a reference PPT, treat it as the primary style source.

### 2. Analyze The Reference PPT

Inspect the reference deck before designing.

Extract:

- slide count and structure
- section rhythm
- cover style
- contents page style
- divider page style
- body page layout
- color palette
- typography hierarchy
- image treatment
- background style
- recurring shapes, lines, panels, page numbers, footers
- weaknesses to avoid, such as typos, overcrowding, repeated layouts, weak contrast

Create a concise style audit for the user.

Example:

```text
The reference PPT uses a deep navy background, burgundy translucent blocks,
large English serif titles, vintage photos, and chapter divider pages.
It has a literary classroom style, but some body slides are too text-heavy,
so the new deck should keep the tone while improving spacing and rhythm.
```

### 3. Propose An Adapted Visual Direction

Do not copy mechanically unless the user explicitly asks for an exact template clone.

Decide what to preserve:

- tone
- palette
- section rhythm
- title hierarchy
- image mood

Decide what to innovate:

- topic-specific background images
- cleaner text layout
- better visual variety
- corrected spelling and typography
- more relevant proof objects or callouts

Ask the user to confirm the direction before building.

### 4. Research Content And Assets

Use reliable sources for factual content.

For real people, books, companies, places, or products:

- prefer official websites, publishers, universities, museums, government pages, or reputable encyclopedias
- do not invent facts
- record sources
- avoid fake official assets

For images:

- use real verified images when identity matters, such as author portraits, book covers, logos, screenshots
- use generated images only for non-identity atmosphere, such as abstract backgrounds, desk scenes, mood images
- never generate a fake portrait of a real person unless the user explicitly wants a fictionalized or non-real image

### 5. Write Slide Content First

Before building the PPT, write the full slide outline and ask the user to confirm.

Each slide should include:

- slide number
- title
- subtitle if needed
- body copy
- visual suggestion
- highlight phrase or callout when useful

For classroom author PPTs, a strong structure is:

```text
1. Cover
2. Contents
3. Section 1 divider: Life
4-5. Life details
6. Section 2 divider: Famous Works
7-8. Representative works
9. Section 3 divider: Writing Style
10-11. Writing style analysis
12. Section 4 divider: Influence
13-14. Influence and recent relevance
15. Thanks
```

### 6. Build The Deck

Use editable PowerPoint elements whenever possible:

- editable text boxes
- editable shapes
- editable callouts
- editable book cards or timelines
- real images as image layers
- generated backgrounds only as background assets

Avoid making each slide a flat screenshot.

Use varied macro layouts:

- cover with portrait/title block
- contents with numbered rows
- section divider with full-bleed background
- text plus portrait
- text plus callout rail
- text plus book cards
- closing slide

No three consecutive slides should use the exact same layout.

### 7. Visual QA

Render slides and inspect:

- contact sheet at thumbnail size
- key slides at full size
- title readability
- body text spacing
- image crop quality
- color contrast
- no text overlap
- no clipping
- no spelling mistakes
- no fake logos, fake covers, or fake identity assets

If a layout checker reports text overlapping a full-slide background image, treat it as a likely false positive only after visually confirming that the text is readable over a dark overlay.

### 8. Final Output

Deliver:

- final `.pptx`
- short explanation of style adaptation
- source note summary
- any known limitations

Keep the final response concise and artifact-focused.

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
- leaving typos like `TAHNKS`
- ending after export without preview inspection

## Example User Task

```text
Learn the style of this John Dos Passos PPT, then create a PPT introducing Amy Tan.
You may search for photos or generate suitable background images.
Write the content first and ask me to confirm before generating the PPT.
```

## Expected Agent Behavior

1. Analyze the reference PPT.
2. Show the user the learned style.
3. Propose a topic-specific adaptation.
4. Draft the slide-by-slide content.
5. Ask for confirmation.
6. Gather or generate visuals.
7. Build the editable PPT.
8. Render and inspect previews.
9. Deliver the final `.pptx`.
