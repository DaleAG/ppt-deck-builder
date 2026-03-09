# PPT Deck Builder

[中文版本](./README.md)

A reusable OpenClaw skill for planning, writing, restructuring, prototyping, and polishing Chinese presentation decks / PPTs.

This skill was abstracted from a real end-to-end project: building an internal OpenClaw presentation deck for boss-facing and internal-team communication. The project-specific experience was distilled into a general deck-building workflow that can be reused for AI/product/strategy/solution decks.

## What this skill helps with

- Turn a vague topic into a clear deck storyline
- Build boss-facing / internal-share presentation structures
- Use cases and proof points instead of abstract preaching
- Refactor drifting decks by rebuilding v2 / v3 cleanly
- Produce editable HTML/CSS slide prototypes
- Export printable decks with cleaner PDF behavior
- Reuse intake briefs and output templates for future projects

## Included files

- `ppt-deck-builder.skill` — packaged skill file
- `SKILL.md` — core skill entry
- `references/` — workflow, templates, examples, and export rules

## Quick use on your own OpenClaw

### Option A: Use the packaged .skill file
If your OpenClaw setup supports skill import / distribution, use:

- `ppt-deck-builder.skill`

### Option B: Use the skill folder directly
Place the skill folder into your local skills directory and make it available to your OpenClaw runtime.

Recommended structure:

```
ppt-deck-builder/
├── SKILL.md
├── references/
│   ├── ppt-workflow.md
│   ├── story-architecture.md
│   ├── cases-and-evidence.md
│   ├── html-prototyping-and-export.md
│   ├── input-brief-template.md
│   ├── output-templates.md
│   └── openclaw_example.md
```

## Suggested workflow

1. Start from `references/input-brief-template.md`
2. Build the storyline with `references/story-architecture.md`
3. Build the evidence pool with `references/cases-and-evidence.md`
4. Draft the deck using `references/output-templates.md`
5. If needed, build HTML/CSS slides using `references/html-prototyping-and-export.md`
6. Use `references/openclaw_example.md` as a concrete worked example

## Best fit scenarios

- Internal AI / Agent sharing decks
- Boss-facing product or strategy decks
- Solution presentations
- Case-study presentations
- Emerging-technology education decks

## Notes

- This is a **general PPT/deck skill**, not an OpenClaw-topic-only skill.
- The OpenClaw presentation project is preserved only as a worked example.
- If you want fast iteration, editable HTML/CSS is often better than image-generation-first workflows.

## 中文文档

See [README.md](./README.md).
