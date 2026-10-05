# Auto Edit Video Studio

The **Auto Edit Studio** (`/auto-edit.php`) is a next-generation AI video montage and slide synchronization studio built directly into OramiVoice. It enables creators to transform batches of still images, concept art, and voiceovers into dynamic, motion-rich slideshows and explainer videos in minutes.

---

## Key Highlights

- **CapCut Multi-Track Timeline**: Full non-linear editing workspace with time ruler, thumbnail filmstrips, synchronized voiceover tracks, and subtitle cue ribbons.
- **1:1 Smart Auto-Sync**: Automatically calculates audio segment durations and stretches each scene to match its corresponding voice clip (001.mp3 -> 001.png).
- **Pro Ken Burns Motion Engine**: Smooth, camera-grade motion algorithms including adaptive smart zooms, cinematic drifts, dynamic pans, and handheld camera shakes.
- **Client-Side GPU Video Rendering**: Powered by modern browser WebCodecs and MediaRecorder APIs, rendering 1080p Full HD MP4 files directly on your computer with zero server queue times.
- **Multi-Format Aspect Ratios**: Switch instantly between **16:9** (YouTube / Widescreen), **9:16** (TikTok, Reels & Shorts), and **1:1** (Square Social Feeds).

---

## Studio Interface & Controls

### 1. Batch Media (Images & Video Clips)
- Drag and drop dozens of images or video snippets (PNG, JPG, WebP, MP4).
- Built-in **Compact Toggle (<kbd>↕</kbd>)** allows you to collapse the drop area into a sleek mini bar so your motion controls are never clipped on laptop screens.
- Drag the bottom edge to resize the card height as needed.

### 2. Audio & Subtitle Tracks
- **Voiceover Audio**: Upload batch audio tracks (e.g. `001.mp3`, `002.mp3`) or a continuous voiceover file.
- **Subtitles (.SRT / .VTT)**: Attach subtitle files. Subtitles automatically render dynamically on top of the video with configurable styling.
- **Background Music (BGM)**: Add an optional ambient music track to elevate engagement.

### 3. Studio Motion & Aesthetics
- **Canvas Theme**: Choose canvas stages including *Dark Cinema Stage*, *Modern Slate*, *Studio Light*, *Cyber Grid Matrix*, or *Deep Purple Gradient*.
- **Ken Burns Motion**:
  - `🎲 Smart Random (Adaptive)`: Intelligently varies pan and zoom directions between consecutive scenes to prevent visual fatigue.
  - `🔍 Smooth Zoom In`: Slowly pushes into the subject to build tension or focus.
  - `🔎 Slow Zoom Out`: Reveals wider environmental details.
  - `↔️ Dynamic Horizontal Pan`: Sweeps horizontally across panoramic artworks.
  - `🌊 Cinematic Drift`: Subtly floats across the frame with harmonic oscillation.
  - `🎬 Handheld Camera Shake`: Adds authentic documentary-style camera jitter.
  - `⏸️ Static Frame`: Disables motion for infographics or still title slides.
- **Transitions**: Seamless crossfade, dip to black, dip to white, or instant cut.
- **Subtitles**: Toggle real-time canvas subtitles and choose between *Dark Pill Box*, *Frosted Glass*, or *Bold Outline*.

---

## Timeline Editing & Filmstrips

### Filmstrip Image Previews
Each scene on the timeline renders a continuous repeating thumbnail filmstrip (`repeat-x`), giving you an immediate visual cue of the artwork across its entire duration.

### Interactive Duration Resizing (CapCut Right Handle)
- Hover over the right edge of any scene block to reveal the **Resize Handle**.
- Drag left or right to increase or decrease that scene's duration.
- A live floating tooltip displays the exact duration in seconds (e.g., `8.5s`) while you drag.

### Drag & Drop Scene Reordering
- Click and drag any scene clip along the timeline.
- Blue placement indicator lines appear to show the drop position (before or after adjacent scenes).
- Release to reorder. Timeline start times and audio synchronization update instantly.

### One-Click Auto-Fit & Auto-Sync
- Click **Auto Sync 1:1** on the top toolbar or timeline header.
- The engine measures each audio track in the voice queue and automatically sets each image slide duration to match its corresponding audio file perfectly.

---

## Video Export & Download

1. Click **Render & Export MP4**.
2. The modal displays real-time frame-by-frame GPU rendering progress.
3. Once completed (100%), click **Download Video (.MP4)** to save your high-retention video directly to your storage.
