# Anki - Chinese

Anki deck for learning Chinese, in English (for English learners).

## Live Quiz (Website)

Try the cards in the browser, no Anki needed:

**https://waldmann-dev.github.io/Anki-Chinesisch/**

The quiz loads all `cards.tsv` live from this repo. Cards with audio show a 🔊 button (audio loads from the repo).

## Anki Package (.apkg) – One File, Everything Included

Download **[Anki-Chinesisch.apkg](Anki-Chinesisch.apkg)** (200 cards + 81 card audios), double-click / import in Anki – cards + audio come in together, no separate MP3 copying needed.

(Alternative: import the individual `cards.tsv` + copy MP3s flat into `collection.media`, see Audio below.)

## Structure

Structure mirrors Anki: each subdeck is a numbered folder, like in the Anki deck overview.

- `Chinese Vocabulary` (top-level)
  - `01. Lesson 1 - Hello` – 27 cards (Front: Character + Pinyin, Back: English)
- `Chinese Grammar`
  - `00. Pinyin` – no own cards, only subdecks (71 cards total)
    - `00. Pinyin Basics` (20), `01. Bilabial and Labiodental` (6), `02. Alveolar` (5), `03. Velar` (4), `04. Retroflex` (5), `05. Palatal` (5), `06. Dental` (4), `07. Simple Finals` (7), `08. Diphthongs` (6), `09. Nasal Finals` (5), `10. Glide Finals` (4)
  - `01. Phonetic Foundations` – no own cards, only subdecks (102 cards total)
    - `01. Syllables, Initials, Finals, Tones, Neutral Tone` (55), `02. Initials, Diphthongs, Nasals, 3rd-Tone Sandhi` (15), `03. Initials, -i, u-Finals` (5), `04. yī-Sandhi, Spelling, Characters` (27)

Total: 200 cards. Flat rule: a subdeck is the deepest level, no sub-subdecks, cards directly in the subdeck.

## Card formats

- `Chinese Grammar` (Pinyin + Phonetic Foundations): Q&A knowledge recall (no exercises).
  Columns: `Question | Answer | Example`
- `Chinese Vocabulary`: vocabulary.
  Columns: `Question | Answer | Example` (Question = Character + Pinyin, Answer = English)

Example column: Chinese character + Pinyin + English in parentheses, e.g. `你好 nǐ hǎo (hello)`. One example per card if sensible, else `–`.

Import in Anki: File > Import, choose the .tsv, set separator to Tab, map fields.

## Audio

- `audio/Elevenlabs/Lektion1/` – 81 single-word card audios (ElevenLabs, Voice Alice, model eleven_v4), named by spoken content (e.g. `ni_hao.mp3`). Linked in cards via `[sound:…]` in the Example column.
- `audio/Lektion1/` – 17 BLCUP lesson tracks (full dialogues / phonetics exercises / classroom phrases), named `NN_dialogue_….mp3`. Lesson audio, NOT linked in cards.

In Anki: copy all MP3s **flat** into `collection.media` (subfolders don't matter for `[sound:]`, only filenames).

## How to add a lesson

1. Create folder `<Parent>/NN. Title/` (NN = 00, 01, 02, ...)
2. Add `cards.tsv` in the same format
3. Keep numbering lesson-wise, always `NN. Title`
