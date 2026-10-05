# Prompt Engineering & Style Guide

Writing high-impact prompts is key to getting photorealistic, consistent, and aesthetically pleasing results from the OramiVoice Image Studio models.

---

## Anatomy of an Effective Prompt

A high-performing visual synthesis prompt typically follows this 5-part structure:

```text
[Subject & Core Action] + [Art Style & Medium] + [Environment & Lighting] + [Camera Perspective & Composition] + [Quality Modifiers]
```

### Example Breakdown:
- **Subject**: `An elderly artisan clockmaker inspecting the golden gears of a vintage mechanical timepiece`
- **Art Style**: `Cinematic realism, oil-rubbed bronze textures, fine artisan craftsmanship`
- **Environment & Lighting**: `Warm amber lamplight in a cozy Victorian workshop, soft volumetric dust motes`
- **Camera Perspective**: `Macro close-up shot, shallow depth of field, 85mm lens, f/1.8 bokeh background`
- **Quality Modifiers**: `Hyper-detailed, 8k resolution, award-winning photography`

---

## Recommended Style Presets

### 1. Cinematic Photorealism
```text
Cinematic 35mm film still of [Subject], natural dramatic lighting, shallow depth of field, subtle film grain, color graded by Kodak Portra 400, highly detailed 8k.
```

### 2. Digital Concept Art & Fantasy
```text
Epic fantasy concept art of [Subject], intricate architectural details, atmospheric haze, rim lighting, vibrant color palette, matte painting by ArtStation master.
```

### 3. Anime & Stylized Illustration
```text
Studio anime key visual of [Subject], clean cel shading, dynamic line art, soft pastel color grading, beautiful background detailing, Makoto Shinkai aesthetic.
```

### 4. 3D Isometric & Product Rendering
```text
Isometric 3D render of [Subject], soft studio lighting, clean glossy materials, pastel backdrop, ray-traced reflections, minimalist Octane render.
```

---

## Camera Angles & Framing Reference

| Camera Framing | Visual Impact | Prompt Keyword Examples |
| :--- | :--- | :--- |
| **Extreme Close-Up** | Intense emotion, microscopic texture | `macro shot`, `extreme close-up`, `intricate eye reflection` |
| **Medium Portrait** | Character focus with environment context | `medium portrait shot`, `waist-up framing`, `85mm lens portrait` |
| **Wide Angle** | Majestic landscapes, environmental scale | `wide angle landscape shot`, `panoramic view`, `vast establishing shot` |
| **Low Angle** | Power, dominance, heroic stature | `low angle perspective`, `heroic upward view`, `dramatic worm's-eye view` |
| **Bird's Eye** | Strategic layout, geometric symmetry | `overhead top-down view`, `drone photography`, `satellite perspective` |

---

## Common Prompting Pitfalls & Fixes

1. **Avoid Vague Modifiers**: Words like "nice", "good", or "beautiful" provide minimal guidance to neural models. Replace them with specific visual cues like `volumetric sunlight`, `intricate gold filigree`, or `subtle subsurface scattering`.
2. **Avoid Conflicting Keywords**: Do not mix contradictory lighting (e.g., `bright noon sunlight` with `dark neon night`).
3. **Pacing Keywords**: Put your most important subject keywords at the beginning of the prompt.
