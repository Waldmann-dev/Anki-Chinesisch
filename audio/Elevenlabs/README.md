# audio/Elevenlabs – ElevenLabs Fallback (Single-Word Card Audio)

ElevenLabs-generated single-word audio for Anki cards. Voice: Alice. Model: eleven_v4.

Files are named by spoken content (ASCII Pinyin, syllables joined by `_`, e.g. `ni_hao.mp3` for 你好, `ba_ba.mp3` for 爸爸). Tone digit only on collisions for single-syllable words with the same base (e.g. `ma1.mp3` 妈, `ma2.mp3` 麻, `ma3.mp3` 马, `ma4.mp3` 骂, `ma0.mp3` 吗, `ba1.mp3` 八, `ba4.mp3` 爸, `shi2.mp3` 十, `shi4.mp3` 是). No track number in names.

Sorted by lesson: `Lektion1/` contains the Lesson 1 card audio (81 words).

In `cards.tsv`, link with `[sound:<filename>.mp3]` in the Example column. Anki needs the MP3s copied FLAT into `collection.media` (subfolders don't matter for `[sound:]`, only filenames).
