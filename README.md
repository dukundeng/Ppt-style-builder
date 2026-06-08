# PPT Style Builder

`ppt-style-builder` is a Codex skill for creating polished, editable PowerPoint decks from a reference presentation style.

It guides Codex through a full deck-building workflow:

- analyze a reference PPT's visual system
- propose an adapted direction
- research factual content and visual assets
- draft slide-by-slide content before building
- create editable PowerPoint slides
- render and inspect the deck before delivery

## Installation

Clone this repository into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
git clone <your-repo-url> ~/.codex/skills/ppt-style-builder
```

Restart Codex after installation if the skill does not appear immediately.

## Usage

Ask Codex for a presentation task that involves learning, imitating, redesigning, or adapting a PPT style.

Example:

```text
Learn the style of this reference PPT, then create a 15-slide classroom presentation about Amy Tan.
Write the slide content first and ask me to confirm before generating the deck.
```

## Repository Structure

```text
.
├── README.md
└── SKILL.md
```

## Notes

This skill is intentionally workflow-focused. It does not ship templates or bundled assets; instead, it instructs Codex to inspect the user's reference deck and build a new editable PowerPoint based on that style.

## License

No license has been selected yet.
