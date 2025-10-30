# datasiz/badwords

A free, open-source **multilingual dataset of offensive or profane words** — designed for text filtering, moderation, and AI content-safety systems.

This repository contains **only plain-text datasets** (`.txt` files), each representing a list of bad words for a specific language.  
It is meant to be used as a **data source** by other libraries, APIs, or machine learning models — not a standalone code library.

---

## Supported Languages

| Language | Code | File Path     |
|-----------|------|---------------|
| English   | en   | `data/en.txt` |
| Hindi     | hi   | `data/hi.txt` |
| Spanish   | es   | `data/es.txt` |
| French    | fr   | `data/fr.txt` |
| Tamil     | ta   | `data/ta.txt` |
| Arabic    | ar   | `data/ar.txt` |
| Chinese   | zh   | `data/zh.txt` |

> Each file is encoded in **UTF-8** and contains **one word per line**, all lowercase.

---

## Example Format

Example: `data/en.txt`
```text
shit
bitch
bastard
```

Example: `data/hi.txt`
```text
कमीना
हरामी
गधा
साला
```

## Data Rules
✅ One word per line
✅ Lowercase only
✅ UTF-8 encoded
✅ No punctuation, no numbering
✅ No duplicates
❌ No comments or explanations inside files

## Contributing
We welcome contributions from the community!
If you know new words or want to add a new language, please see our CONTRIBUTING.md guide

## Related Projects
coming soon