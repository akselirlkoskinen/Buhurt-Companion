# Translations

Community-contributed UI translations for [Buhurt Companion](https://github.com/RylaiBlueheart/buhurt-companion).

## Current languages

| File | Language | Coverage |
|------|----------|----------|
| `en.json` | English | 100% — source of truth |
| `fi.json` | Finnish (Suomi) | 100% |
| `de.json` | German (Deutsch) | ~30% — contributions welcome |
| `ru.json` | Russian (Русский) | ~30% — contributions welcome |

## Adding a new language

1. Copy `template.json` and rename it to your [BCP-47 language code](https://en.wikipedia.org/wiki/IETF_language_tag) (e.g. `sv.json`, `pl.json`, `cs.json`).
2. Fill in as many keys as you can. Any key you leave as `""` will automatically fall back to English in the app.
3. Delete the `_instructions`, `_placeholders`, `_language`, `_nativeName`, `_code`, and `_contributors` meta-keys before submitting (or keep them — they are ignored by the app loader).
4. Open a pull request. See [CONTRIBUTING.md](../CONTRIBUTING.md) for the full workflow.

## Rules for translators

### Keep placeholders intact
Strings containing `{{variable}}` must keep those placeholders — only translate the surrounding text.

```json
// English source
"sparring.round": "ROUND {{round}} / {{total}}"

// ✅ Correct Finnish
"sparring.round": "ERÄ {{round}} / {{total}}"

// ❌ Wrong — placeholder renamed
"sparring.round": "ERÄ {{erä}} / {{yhteensä}}"
```

### Keep special symbols
Timer symbols like `▶`, `⏸`, `■`, `↺`, `⚡` are part of the UI — keep them as-is.

### Partial translations are welcome
You don't have to translate everything. Start with the keys you use most (navigation, training timers) and skip the rest. Any missing key falls back to English.

### Capitalization
The app uses ALL-CAPS for section headings and button labels in many places. Follow the same convention in your language where it makes sense — in some languages (e.g. German with noun capitalization) use your judgement.

### Plurals
Where the English has separate singular/plural keys (e.g. `common.doc` / `common.docs`), provide appropriate forms for your language. For languages with more complex plural rules, use the most common form and note it in your PR description.

## Improving an existing translation

Open the relevant `.json` file, fix the strings, and submit a pull request. Even small fixes (typos, awkward phrasing) are very welcome.
