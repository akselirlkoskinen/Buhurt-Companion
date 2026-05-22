# Contributing to Buhurt Companion Community Content

Thank you for helping improve Buhurt Companion for the global buhurt community! This repository welcomes:

- **Translations** — new languages or improvements to existing ones
- **Workouts** — conditioning programmes and drills
- **Training Manuals** — technique and coaching guides
- **Historical Sources** — manuscript summaries and primary source references

---

## Quick start

1. **Fork** this repository on GitHub
2. **Clone** your fork: `git clone https://github.com/YOUR-USERNAME/buhurt-companion-content.git`
3. Create a branch: `git checkout -b add-swedish-translation`
4. Make your changes
5. Commit: `git commit -m "Add Swedish translation"`
6. Push: `git push origin add-swedish-translation`
7. Open a **Pull Request** on GitHub

---

## Translations

### Adding a new language

1. Copy `translations/template.json`
2. Rename it to your BCP-47 language code (e.g. `sv.json`, `pl.json`, `nl.json`)
3. Fill in translations — empty strings fall back to English automatically
4. Read `translations/README.md` for rules about placeholders and formatting

**Minimum for a viable PR:** Navigation keys (`nav.*`), common actions (`common.*`), and at least one screen section translated.

### Improving an existing translation

Open the relevant `.json` file, fix the string(s), and submit a PR. Even single-key fixes are welcome — please describe what was wrong in the PR description.

---

## Content (Workouts, Manuals, Historical Sources)

### Where to put your file

```
content/
  workouts/en/your-workout-name.md
  manuals/en/your-manual-name.md
  historical/en/your-source-name.md
```

Always write the English version first. Translations of your own content go in sibling language folders with the **same filename**.

### Format requirements

- Markdown with YAML front-matter (see `content/README.md` for required fields)
- File name: lowercase kebab-case, no spaces or special characters
- Images: not yet supported — text only for now

### Content standards

- **Workouts:** Include a warm-up, main work, and cool-down. State equipment requirements clearly. Provide beginner/advanced scaling.
- **Manuals:** Cite your sources or note when something is your own experience. Flag anything that may be organisation-specific.
- **Historical Sources:** Be accurate about dates, repositories, and digital access links. Note limitations clearly.

---

## PR review process

1. A maintainer will review your PR, usually within a few days
2. Feedback may be requested — please respond to review comments
3. Once approved, your contribution will be merged and included in the next app sync

---

## Code of conduct

- Be respectful in reviews and discussions
- Content must be relevant to buhurt, armoured combat, or historical martial arts
- No political or ideological content unrelated to the sport
- Give credit when adapting someone else's work

---

## Questions?

Open a GitHub Issue with the `question` label, or reach out via the Buhurt Companion community channels.
