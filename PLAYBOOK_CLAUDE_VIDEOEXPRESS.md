# Claude + VideoExpress Short-Form Video Studio

Master production playbooks for planning, generating, and assembling high-converting short-form lifestyle and brand promotional videos using **Claude** as the director/browser operator and **VideoExpress.ai** as the generation and editing engine.

---

## 1. Core Production Architecture

1. **Outcome-First Strategy**: Define viewer motivation, the core problem/curiosity hook, and the exact destination URL before writing prompts or selecting tools.
2. **Decoupled Roles**:
   - **Claude Planning**: Handles creative strategy, scriptwriting, scene breakdown, continuity tracking, and phonetic audio formatting.
   - **VideoExpress Execution**: Handles image creation, video motion generation, text-to-speech rendering, and timeline assembly via browser automation.
   - **GitHub Storage**: Houses all permanent master playbooks, prompt templates, and case studies.
3. **Phonetic Script Formatting**: TTS engines mispronounce condensed domains (e.g., `ZenGenUSA.com` -> `zengen u s a .com`). Always format brand URLs with spaced capital letters or phonetic spellings.
4. **Audio Continuity**: Never leave visual pauses completely silent. Layer a continuous ambient instrumental track at 12%–15% volume under spoken lines to eliminate dead air.

---

## 2. Voiceover & CloneVoice Selection Standards

### A. Default Built-In VideoExpress Voices (TTS Panel)
- **Male Master**: `Andrew Multilingual` (Tone: Calm, grounded, warm conversational pacing).
- **Female Master**: Standard warm conversational female voice (e.g., `Jenny` or `Aria` in US English).

### B. CloneVoice.ai Direct Integration (Preferred for Custom Brand Voices)
- VideoExpress integrates directly with CloneVoice.ai via **Import Media -> Import from CloneVoice.ai**.
- **Workflow**:
  1. Generate custom voiceovers or cloned brand voices in CloneVoice.ai.
  2. In VideoExpress, open **Import Media -> CloneVoice.ai (Text to Speech Integration)**.
  3. Pull approved audio directly into the Media Library under `My AI Audio`.
  4. Drag audio blocks to **Audio Track 2** on the timeline.

---

## 3. Planning & Intake Template (For Claude)

When starting any new brand short, provide Claude with this brief:

```text
PROJECT: [Brand Name] Short-Form Promo
PLATFORM: Vertical 9:16 (TikTok / Reels / Shorts)
TARGET RUNTIME: 25–30 Seconds

BRAND CONTEXT:
- Name & Destination URL: [e.g., ZenGen USA / zengen u s a .com]
- Core Identity: [e.g., Intentional living, artisan candles, home sanctuary]
- Forbidden Claims: No medical, health cure, or unrealistic outcome claims.

VOICE SELECTION:
- Mode: [Built-In TTS | CloneVoice.ai Integration]
- Voice Type: [Consistent Male Master (Andrew) | Consistent Female Master | Cloned Brand Voice]
- Phonetic Pronunciation: [Explicit phonetic spelling for brand name/URL]

CREATIVE DIRECTION:
- Concept/Hook: [e.g., "Your phone is quiet. Why isn't your mind?"]
- Arc: Everyday Overload -> Silence Device -> Deliberate Pause -> Warm Sanctuary -> Discovery CTA.
- Style: Cinematic, intimate, premium editorial lifestyle.
- Character: One consistent relatable adult (mid-30s, natural appearance).
- Narration Mode: Off-screen warm voiceover with continuous low ambient background music.
```

---

## 4. Verified VideoExpress Generation Settings

| Setting / Toggle | Production State | Why |
|---|---|---|
| **Orientation** | `Vertical 9:16` | Native mobile reel format |
| **Image Type** | `Human` | Natural skin tones and realistic anatomy |
| **Automatically enhance prompt** | `OFF` | Prevents the engine from rewriting negative constraints |
| **Creative Mode** | `OFF` | Retains photorealistic adherence |
| **Consistent Character** | `OFF` (for multi-prompt) | Use self-contained visual prompts or reference image slots |
| **Lipsync HD** | `OFF` | Prevents artificial mouth flapping during narration |
| **Narration Video** | `OFF` | Narration is layered cleanly on Timeline Track 2 |
| **Advanced Mode** | `ON` | Unlocks manual duration and silent video rendering |
| **Video Only (No Sound)** | `ON` | Generates clean B-roll without synthetic background noise |
| **Manual Video Length** | `ON` (Set 4s–8s) | Aligns each shot with exact scene script targets |

---

## 5. Timeline Assembly & Audio Routing

1. **Video Sequence (Track 1)**: Place all generated scene clips contiguously on Track 1. Use clean hard cuts.
2. **Audio Generation & Import**:
   - For Built-In TTS: Generate lines under *Import Media -> Text to Speech* using phonetic brand spellings.
   - For CloneVoice: Pull generated audio via *Import Media -> CloneVoice.ai*.
3. **Audio Track Routing (Track 2 & Track 3)**:
   - *Note*: VideoExpress drops newly imported TTS clips onto Video Track 1 by default.
   - **Action**: Manually drag all voiceover blocks down to **Audio Track 2**.
   - Align Line 1 at `0:00`.
   - Align Closing CTA with Scene 5 (e.g., `0:22.9`), leaving a 2–3 second visual tail.
   - Place low ambient instrumental music across Track 3 at ~12%–15% volume.
4. **Project Save**: Save project before exporting.

---

## 6. Case Study: ZenGen USA "Quiet Mind" (28.2s Master)

### Scene Breakdown
- **Scene 1 (0:00–0:05 / 5s)**: Standing at wood table, distracted glance at phone.
  - *Audio 1 (0:00–0:02.8)*: *"Your phone is quiet. Why isn't your mind?"*
- **Scene 2 (0:05–0:09.1 / 4.1s)**: Close-up of hand placing phone face down on wood table.
- **Scene 3 (0:09.1–0:14.1 / 5s)**: Quiet corner table; hand switches lamp from OFF to warm ON. Candle lit.
- **Scene 4 (0:14.1–0:20.2 / 6.1s)**: Medium shot seated in warm linen armchair; subtle breath and settling into calm.
- **Scene 5 (0:20.2–0:28.2 / 8s)**: Master seated portrait; slow cinematic push-in toward peaceful expression.
  - *Audio 2 (0:22.9–0:25.4)*: *"Discover your calm at zengen u s a .com."* (Phonetic fix)
  - *Outro (0:25.4–0:28.2)*: Clean visual hold for overlaid text CTA.

---

## Related Video-Creation Workflow

[Our VideoExpress Consistent-Character Talking-Video Workflow](https://github.com/jkcassoc/our-videoexpress-consistent-character-talking-video)

Use this related repository for our consistent-character talking-video workflow. This playbook covers our short-form brand-video planning and production process. 10/19/2028
