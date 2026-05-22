# Community Content

Markdown articles for the **Literacy** tab in Buhurt Companion — three sections:

| Folder | In-app section | What belongs here |
|--------|---------------|-------------------|
| `workouts/` | Workouts | Training programmes, conditioning circuits, drills with sets/reps |
| `manuals/` | Training Manuals | Technique guides, coaching frameworks, skill breakdowns |
| `historical/` | Historical Sources | Manuscript summaries, period equipment notes, primary source references |

Each section has language subfolders (`en/`, `fi/`, `de/`, …). Always create the English version first; translations go in sibling folders with identical filenames.

---

## File format

Each file is a **Markdown** document with a YAML front-matter block at the top.

```markdown
---
title: Your Article Title
author: Your Name / GitHub handle
tags: [tag1, tag2]
---

# Your Article Title

Content here…
```

### Required front-matter fields

| Field | Description |
|-------|-------------|
| `title` | Display title shown in the app |
| `author` | Your name or GitHub handle |
| `tags` | Array of lowercase tags for search |

### Optional front-matter fields (workouts)

| Field | Example |
|-------|---------|
| `difficulty` | `beginner` / `intermediate` / `advanced` |
| `duration` | `30 min` |
| `equipment` | `none` / `barbell, bench` |

### Optional front-matter fields (historical sources)

| Field | Example |
|-------|---------|
| `period` | `c. 1300–1340` |
| `source` | `Codex Manesse` |
| `repository` | `Heidelberg University Library` |

---

## Writing guidelines

### Workouts
- Use `###` headings for each exercise or station
- Put the target reps/time in bold: `**Target: 12 reps**`
- Use blockquotes (`>`) for coaching cues
- Include warm-up, main work, and cool-down sections
- Add a scaling table for beginner/advanced variants

### Manuals
- Break technique into numbered steps where order matters
- Use `**bold**` for key terms on first use
- Include at least one drill per concept
- Common errors section is highly valued

### Historical Sources
- State the source clearly: title, date, repository, digital access URL
- Note limitations and potential inaccuracies
- Cross-reference with other sources when possible
- Use a citation block at the end

---

## File naming

Use lowercase kebab-case: `footwork-fundamentals.md`, `codex-manesse-combat-postures.md`

Avoid spaces and special characters. Keep names short but descriptive.

---

## Submitting content

See [CONTRIBUTING.md](../CONTRIBUTING.md) for the full pull request workflow.
