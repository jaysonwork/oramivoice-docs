# Translate Audio

The Audio Translation tool (`/translate.php?mode=audio`) translates spoken audio recordings into another language and synthesizes a localized spoken voice track.

![Translation Studio](assets/images/ui_translate_studio.png)

---

## Supported Formats

- **Audio Inputs**: MP3, WAV, M4A, AAC, FLAC, OGG.
- **Audio Outputs**: Master WAV or MP3.

---

## Processing Pipeline

1. **Speech Transcription**: Transcribes spoken dialogue from the source audio file into timestamped text.
2. **Neural Translation**: Translates the manuscript into the chosen target language.
3. **Voice Synthesis**: Synthesizes the translated transcript using an actor voice from the Voice Catalog.
4. **Mastering**: Renders a balanced audio track matching the duration and pacing of the original recording.

---

## Operating Steps

1. Open **Translate Audio** (`/translate.php?mode=audio`).
2. Upload your source audio recording.
3. Choose the source language, target language, and desired voice model.
4. Click **Start Audio Translation**.
5. Listen to the localized audio preview and click **Download Audio**.
