# Anki - Chinese

Anki deck for learning Chinese, in English (for English learners).

## Live Quiz (Website)

Try the cards in the browser, no Anki needed:

**https://waldmann-dev.github.io/Anki-Chinesisch/**

The quiz loads all `cards.tsv` live from this repo. Cards with audio show a 🔊 button (audio loads from the repo).

## Anki Package (.apkg) – One File, Everything Included

Download **[Anki-Chinesisch.apkg](Anki-Chinesisch.apkg)** (223 cards + 127 card audios + 10 tongue diagrams), double-click / import in Anki – cards + audio + images come in together, no separate file copying needed.

(Alternative: import the individual `cards.tsv` + copy MP3s flat into `collection.media`, see Audio below.)

## Structure

Structure mirrors Anki: each subdeck is a numbered folder, like in the Anki deck overview.

- `Chinese Vocabulary` (top-level)
  - `01. Lesson 1 - Hello` – 54 cards in two directions (no own cards, only subdecks)
    - `01. Chinese to English` (27) – Front: Character + Pinyin, Back: English
    - `02. English to Chinese` (27) – Front: English, Back: Character + Pinyin (same audio)
- `Chinese Grammar`
  - `00. Pinyin` – no own cards, only subdecks (71 cards total)
    - `00. Pinyin Basics` (20), `01. Bilabial and Labiodental` (6), `02. Alveolar` (5), `03. Velar` (4), `04. Retroflex` (5), `05. Palatal` (5), `06. Dental` (4), `07. Simple Finals` (7), `08. Diphthongs` (6), `09. Nasal Finals` (5), `10. Glide Finals` (4)
  - `01. Phonetic Foundations` – no own cards, only subdecks (98 cards total)
    - `01. Syllables, Initials, Finals, Tones, Neutral Tone` (53), `02. Initials, Diphthongs, Nasals, 3rd-Tone Sandhi` (14), `03. Initials, -i, u-Finals` (4), `04. yī-Sandhi, Spelling, Characters` (27)

Total: 223 cards (169 Grammar + 54 Vocabulary). Flat rule: a subdeck is the deepest level, no sub-subdecks, cards directly in the subdeck – EXCEPTION: Vocabulary has two direction subdecks (Chinese → English, English → Chinese).

Pronunciation cards ask *how* to pronounce a group of sounds (e.g. "How do you pronounce the bilabials?", "How do you pronounce the fricatives?"), not *which* sounds belong to a group – place-classification cards ("Which initials are bilabial?" etc.) were removed on purpose. "How do you pronounce X?" cards use the letter's own audio (e.g. `[sound:initial_p.mp3]` = pō), not a whole-word example.

## Card formats

- `Chinese Grammar` (Pinyin + Phonetic Foundations): Q&A knowledge recall (no exercises).
  Columns: `Question | Answer | Example`
- `Chinese Vocabulary`: vocabulary, two directions.
  Columns: `Question | Answer | Example` (`01. Chinese to English`: Question = Character + Pinyin, Answer = English; `02. English to Chinese`: Question = English, Answer = Character + Pinyin)

Example column: Chinese character + Pinyin + English in parentheses, e.g. `你好 nǐ hǎo (hello)`. One example per card if sensible, else `–`.

Import in Anki: File > Import, choose the .tsv, set separator to Tab, map fields.

## Audio

- `audio/Elevenlabs/Lektion1/` – 127 card audios (ElevenLabs, Voice Alice, model eleven_v4): single words (e.g. `ni_hao.mp3`), 21 initial names (`initial_b.mp3` = bō, …), 25 finals in first tone (`final_a.mp3` = ā, …). Linked in cards via `[sound:…]` in the Example column.
- `audio/Lektion1/` – 17 BLCUP lesson tracks (full dialogues / phonetics exercises / classroom phrases), named `NN_dialogue_….mp3`. Lesson audio, NOT linked in cards.

In Anki: copy all MP3s **flat** into `collection.media` (subfolders don't matter for `[sound:]`, only filenames).

## Tongue diagrams (images)

- `images/` – 10 mouth cross-section diagrams in textbook style (red tongue, green contact point, labels with Pinyin + IPA): `tongue_bilabial.png`, `tongue_labiodental.png`, `tongue_dental.png`, `tongue_alveolar.png`, `tongue_retroflex.png`, `tongue_palatal.png`, `tongue_velar.png`, `tongue_nasal.png`, `tongue_lateral.png`, `tongue_fricative.png`.
- Linked in cards via `<img src="tongue_XXX.png">` in the Example column (pronunciation-group cards, individual "How do you pronounce X?" cards, fricative/lateral/nasal definition cards, nasal-final cards, and the 3 difference cards b/p, d/t, g/k).
- In Anki: copy the 10 PNGs **flat** into `collection.media` too (same as the MP3s – `<img>` needs only the filename). On the website they load from `images/` automatically.

## How to add a lesson

1. Create folder `<Parent>/NN. Title/` (NN = 00, 01, 02, ...)
2. Add `cards.tsv` in the same format
3. Keep numbering lesson-wise, always `NN. Title`
