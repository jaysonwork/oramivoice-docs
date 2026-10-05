# Translate Subtitles

The Subtitle Translation tool (`/translate.php?mode=subtitles`) translates subtitle files into over 30 languages while preserving precise timecodes and subtitle formatting.

![Translation Studio](assets/images/ui_translate_studio.png)

---

## Supported Formats

- **Import**: `.srt` (SubRip), `.vtt` (WebVTT), `.txt` (Plain Transcript).
- **Export**: `.srt`, `.vtt`, `.txt`.

---

## Features

- **Side-by-Side Bilingual Editor**: Displays source subtitle lines alongside translated text for quick proofreading and manual adjustments.
- **Context-Aware Translation**: Processes complete conversational blocks to preserve natural sentence structure and tone.
- **Timestamp Integrity**: Retains original start and end timestamps down to the millisecond.
- **Batch Translation**: Translates hundreds of subtitle cues in a single operation.

---

## How to Translate Subtitles

1. Open **Translate Subtitles** (`/translate.php?mode=subtitles`).
2. Upload your `.srt` or `.vtt` file.
3. Select the source language (or Auto-Detect) and your desired target language.
4. Click **Translate Subtitles**.
5. Review the translated lines in the editor and edit any individual entries.
6. Click **Export Subtitles** to download your translated `.srt` or `.vtt` file.
