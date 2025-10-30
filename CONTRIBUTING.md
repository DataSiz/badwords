## **CONTRIBUTING.md**

# Contributing to badwords

Thank you for your interest in contributing!  
This project relies on the community to build and maintain a reliable multilingual dataset of offensive words.  
Please follow the guidelines below to keep the data consistent and clean.

---

## Repository Structure

datasiz/badwords/
│
├── data/
│ ├── en.txt # English
│ ├── hi.txt # Hindi
│ ├── es.txt # Spanish
│ └── ... # Other languages
│
├── CONTRIBUTING.md
├── README.md
└── LICENSE


## Adding a New Language

1. Create a new file inside `/data/` named using the **ISO language code**.  
   Example: `data/fr.txt` for French, `data/de.txt` for German.
2. Add your list of bad words — **one per line**, all **lowercase**, **UTF-8 encoded**.
3. Avoid duplicates and blank lines.
4. Submit a **Pull Request** with a short description:
   - Language added  
   - Approximate number of words  
   - Source or method (if available)

---

## Updating Existing Lists

- Add missing words relevant to the language.
- Remove false positives (e.g., normal words that aren’t offensive).
- Ensure new words follow format rules.
- Avoid slang that may not be universally offensive unless contextually consistent.

---

## Data Format Rules

| Rule | Description |
|------|--------------|
| Encoding | UTF-8 only |
| Case | Lowercase only |
| Format | One word per line |
| Comments | Not allowed inside data files |
| Duplicates | Should be removed |
| File Name | Must match ISO 639-1 language code (e.g., `en`, `hi`, `es`) |

---

## Example

✅ **Correct:**
fuck
shit
bitch

❌ **Incorrect:**
fuck,
shit!
"Bitch"

## Optional Quality Check

Before submitting your PR, you can check for duplicates using any simple script or tool.  
For example (in Linux/Mac):

```bash
sort data/en.txt | uniq -d
```

If this returns nothing, you’re good!


## License and Attribution
By contributing, you agree that your additions will be released under the MIT License,
and may be used by downstream projects freely.

## Thank You
Your contribution helps developers worldwide build safer and more responsible platforms.
Together, we can make open datasets useful for global moderation systems.