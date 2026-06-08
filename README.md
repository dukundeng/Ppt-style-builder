# PPT Style Builder

PPT Style Builder is a reusable workflow for creating polished, editable presentation decks from a reference PowerPoint style.

It is not limited to one AI tool. You can use the workflow with Codex, ChatGPT, Claude, Gemini, a design team, or your own manual slide-production process.

## What It Helps With

- Learn the visual system of a reference PPT.
- Adapt the style to a new topic without blindly copying it.
- Write slide content before building the final deck.
- Choose or generate visuals responsibly.
- Build editable PowerPoint slides instead of flat screenshots.
- Render and inspect the final deck before delivery.

## Repository Contents

```text
.
├── README.md
├── workflow.md
├── prompts/
│   ├── style-analysis.md
│   ├── slide-outline.md
│   ├── slide-design.md
│   └── visual-qa.md
├── examples/
│   └── classroom-author-presentation.md
└── codex/
    └── SKILL.md
```

## Quick Start

1. Read [workflow.md](workflow.md).
2. Pick the prompt template that matches your current step from [prompts/](prompts).
3. Provide your reference PPT, topic, audience, language, and target slide count.
4. Confirm the slide outline before building the final deck.
5. Render or preview the deck and check it against the QA prompt.

## Codex Installation

To install this as a Codex skill, clone the repository and copy or symlink the `codex` folder into your skills directory:

```bash
mkdir -p ~/.codex/skills/ppt-style-builder
cp codex/SKILL.md ~/.codex/skills/ppt-style-builder/SKILL.md
```

If you want live updates from the repository, use a symlink instead:

```bash
mkdir -p ~/.codex/skills
ln -s "$(pwd)/codex" ~/.codex/skills/ppt-style-builder
```

Restart Codex after installation if the skill does not appear immediately.

## Example Request

```text
Learn the style of this reference PPT, then create a 15-slide classroom presentation about Amy Tan.
Write the slide content first and ask me to confirm before generating the deck.
```

## License

MIT. See [LICENSE](LICENSE).
