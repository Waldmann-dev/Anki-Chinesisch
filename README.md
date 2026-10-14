# Anki - Chinese

Anki deck for learning Chinese, in English (for English learners).

Structure mirrors Anki: each subdeck is a numbered folder, like in the Anki deck overview.

```
Chinese/
  00. Phonetic Foundation Course/
    cards.tsv
  01. Greetings/
    cards.tsv
  ...
```

In Anki the decks are named:
- `Chinese::00. Phonetic Foundation Course`
- `Chinese::01. Greetings`
- ...

## Card formats

- `00. Phonetic Foundation Course`: Q&A knowledge recall (no exercises).
  Columns: `Question | Answer | Example`
- Other lessons (e.g. `01. Greetings`): vocabulary.
  Columns: `Chinese | Pinyin | English | Example (Chinese) | Example (Pinyin) | Example (English)`

Import in Anki: File > Import, choose the .tsv, set separator to Tab, map fields.

## How to add a lesson

1. Create folder `Chinese/NN. Title/` (NN = 00, 01, 02, ...)
2. Add `cards.tsv` in the same format
3. Keep numbering lesson-wise, always `NN. Title`
