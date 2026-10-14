# Anki - Chinese

Anki deck for learning Chinese, in English (for English learners).

Structure mirrors Anki: each subdeck is a numbered folder, like in the Anki deck overview.

```
Chinese/
  01. Greetings/
    cards.tsv
  02. Numbers/
    cards.tsv
  ...
```

In Anki the decks are named:
- `Chinese::01. Greetings`
- `Chinese::02. Numbers`
- ...

## Card format

Each `cards.tsv` is tab-separated, with header:

`Chinese | Pinyin | English | Example (Chinese) | Example (Pinyin) | Example (English)`

Import in Anki: File > Import, choose the .tsv, set separator to Tab, map fields.

## How to add a lesson

1. Create folder `Chinese/NN. Title/` (NN = 01, 02, 03, ...)
2. Add `cards.tsv` in the same format
3. Keep numbering lesson-wise, always `NN. Title`
