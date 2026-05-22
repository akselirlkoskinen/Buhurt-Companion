# Buhurt Companion — Community Content

Community-maintained translations and content for the [Buhurt Companion](https://apps.apple.com/app/buhurt-companion) mobile app.

---

## What's in this repository

| Folder | Purpose |
|--------|---------|
| [`translations/`](translations/) | App UI strings in JSON — one file per language |
| [`content/workouts/`](content/workouts/) | Conditioning programmes and drills |
| [`content/manuals/`](content/manuals/) | Technique guides and coaching resources |
| [`content/historical/`](content/historical/) | Manuscript summaries and primary source references |

---

## How to contribute

**Short version:** fork → edit → pull request. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full workflow.

### Translations
Copy `translations/template.json`, rename it to your language code (e.g. `sv.json`), fill in as many keys as you can, and open a PR. Partial translations are welcome — missing keys fall back to English in the app.

See [`translations/README.md`](translations/README.md) for rules about placeholders and formatting.

### Content
Write a Markdown file with YAML front-matter, place it in the correct `content/` subfolder, and open a PR.

See [`content/README.md`](content/README.md) for the required format and writing guidelines.

---

## Languages

| Language | File | Status |
|----------|------|--------|
| English | `translations/en.json` | Complete — source of truth |
| Finnish | `translations/fi.json` | Complete |
| German | `translations/de.json` | Partial — help welcome |
| Russian | `translations/ru.json` | Partial — help welcome |

Want to add your language? [Open an issue](../../issues/new) or just submit a PR directly.

---

## Content library

### Workouts
- [Buhurt Conditioning Circuit](content/workouts/en/buhurt-conditioning-circuit.md) — full-body, no equipment, 45 min

### Training Manuals
- [Footwork Fundamentals](content/manuals/en/footwork-fundamentals.md) — beginner guide to movement and stance

### Historical Sources
- [Combat Postures in the Codex Manesse](content/historical/en/codex-manesse-combat-postures.md) — 14th-century German illustrated manuscript

---

## For app maintainers

Content from this repository is pulled into the app via the Arena Web content sync. Merged PRs are included in the next manifest rebuild.

Translation files are loaded directly at app build time. After merging a new language file, add the language code to the app's language picker in `SettingsScreen.tsx`.

---

## License

Translations and content in this repository are contributed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) unless otherwise noted in the individual file. App source code is not included here.
