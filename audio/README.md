# audio

Audio files for Anki cards (`[sound:...]` in `cards.tsv`).

- `audio/Lektion1/` – BLCUP native lesson tracks (dialogues, phonetics exercises, classroom phrases). NOT single-word card audio – do NOT link with `[sound:]`.
- `audio/Elevenlabs/Lektion1/` – ElevenLabs single-word card audio (Voice Alice, model eleven_v4), named by spoken content (e.g. `ni_hao.mp3`). Link with `[sound:<filename>.mp3]` in the Example column.

Anki: copy ALL MP3s from both folders FLAT into `collection.media` (subfolders don't matter for `[sound:]`, only filenames).
