# Troubleshooting & Frequently Asked Questions (FAQ)

Find answers to common questions, operational tips, and troubleshooting steps across all OramiVoice workspace tools.

---

## Voice Synthesis & Speech Studio

### Why does the synthesized audio sound rushed or too slow?
- Check the **Speed Slider** setting in the voice configuration panel. The standard baseline is `1.0x`.
- Insert natural punctuation (commas, periods) to guide the neural model on breathing pauses.

### How do I correct mispronounced names or technical terms?
- For specialized acronyms, write them phonetically or space them out (e.g., write `A. I.` instead of `AI`).
- For foreign proper nouns, write the approximate phonetic spelling matching the selected voice's primary language.

---

## AI Image Studio

### How do I keep consistent characters across multiple images?
- Use the **Reference Images** upload zone in the Image Studio. Upload a clear character portrait and select `Apply reference to all prompts`.
- Include consistent subject keywords in your prompt (e.g., `same young man with short brown hair, wearing a green trench coat`).

### Why do images disappear after 24 hours in History?
- In accordance with our server retention policy, generated assets are temporarily cached on high-speed servers for 24 hours. Always click **Download** or **Download ZIP** to save important images to your local device.

---

## AI Video Dubbing

### Why is the dubbed audio slightly out of sync with the original video?
- Ensure you click **Translate & Align** before rendering. The timing optimizer adjusts translated sentence length to match the video's original speaking duration.
- You can manually fine-tune subtitle cue start and end timecodes in the Subtitle Editor table.

---

## API & Billing

### Where do I find my API Secret Key?
- Go to your **Profile** (`/profile.php`) and click **API Keys** (`/api-keys.php`). You can generate new keys and configure permissions at any time.

### How are credits billed if an image generation fails?
- Credits are deducted only upon successful asset generation. If a server timeout or invalid parameter error occurs, no credits are deducted from your balance.
