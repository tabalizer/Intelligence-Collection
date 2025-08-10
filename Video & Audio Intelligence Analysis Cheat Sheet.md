# Video & Audio Intelligence Analysis OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). For lawful OSINT and investigative use only._

---

## 🎯 1) Purpose
To extract, analyze, and interpret intelligence from video and audio sources using lawful, open-source techniques — revealing location, time, context, and authenticity indicators while preserving evidentiary integrity.

---

## 🎬 2) Core Video Analysis Workflow (The 5E Method)
1. **Extract** — Obtain highest-quality, original source files whenever possible.  
2. **Examine** — Conduct frame-by-frame review for visible and audible clues.  
3. **Enhance** — Apply tools to clarify obscured or distorted details (lawfully).  
4. **Enrich** — Cross-reference findings with external datasets and OSINT platforms.  
5. **Evaluate** — Assign confidence level and assess relevance before reporting.

---

## 🛠 3) Tool Arsenal

### Metadata & File Intelligence
- **ExifTool** — Extract embedded metadata from video/audio files.  
- **MediaInfo** — Detailed codec, bitrate, resolution, and timestamp data.  
- **FFmpeg** — Extract frames, convert formats, analyze streams, isolate tracks.  
- **Ghiro** — Automated image metadata & hash analysis (for stills from video).  
- **DROID (UK National Archives)** — File format identification.

### Video Analysis & Enhancement
- **InVID & WeVerify** — Keyframe extraction, reverse image search integration, video forensics toolkit.  
- **VLC Media Player** — Frame-by-frame review and basic snapshot export.  
- **Kinovea** — Motion analysis and object tracking.  
- **Amped FIVE** (commercial) — Professional forensic video enhancement.  
- **DaVinci Resolve** (free/pro) — Color grading, sharpening, and frame stabilization.  
- **Matroska tools** — Inspect MKV container metadata.

### Audio Analysis
- **Audacity** — Waveform and spectral analysis, noise isolation.  
- **Sonic Visualiser** — Frequency domain visualization for background noise identification.  
- **Praat** — Phonetic analysis and voice pattern profiling.  
- **Ocenaudio** — Quick-edit audio inspection.  
- **Spek** — Spectrogram viewer for format and compression artifacts.

### Integrated OSINT & Verification
- **SunCalc.org** — Sun position & shadow analysis for time-of-day estimation.  
- **Timeanddate.com / Meteostat.net** — Historical weather matching to visual/audio clues.  
- **Google Lens / Yandex Images / Bing Visual Search** — Reverse search extracted stills.  
- **YouTube DataViewer** — Extract upload timestamps and thumbnails from YouTube videos.  
- **Amnesty International YouTube Dataviewer** — Cross-check YouTube content metadata.  
- **WatchFrameByFrame.com** — Online frame-by-frame YouTube analysis.

---

## 🔍 4) Visual Clue Categories
- **Environmental** — Weather, lighting, shadows, vegetation.  
- **Architecture** — Building styles, signage, street layouts.  
- **Objects** — Vehicles, uniforms, tools, weapons.  
- **Screens & Displays** — Digital readouts, clocks, in-scene devices.  
- **People** — Clothing, tattoos, gait, speech.  
- **Text** — Banners, posters, shopfronts, graffiti.

---

## 🎧 5) Audio Clue Categories
- **Voices & Accents** — Language, dialect, speech patterns.  
- **Background Noise** — Traffic, nature, machinery, music.  
- **Echo & Acoustics** — Indoor vs. outdoor, spatial characteristics.  
- **Electronic Signals** — Device notifications, alarms, system prompts.

---

## 🗺 6) Cross-Platform Pivoting
- Reverse search video stills via **Google Lens**, **Yandex**, **Bing**.  
- Search transcribed dialogue keywords in local news archives.  
- Compare environmental sound cues to field recordings in open audio archives.

---

## 📍 7) Timeline & Sequence Analysis
- Use metadata + sun/shadow data to estimate filming time.  
- Match weather patterns to historical meteorological records.  
- Sequence multiple videos by cross-referencing scene elements and timestamps.

---

## ⚠️ 8) 2025 Threat Landscape & Cautions
- AI-generated video/audio (“deepfakes”) now highly realistic — verify with multiple forensic tools.  
- Social platforms strip most metadata — request or seek original files when possible.  
- Short-form platforms (TikTok, Instagram Reels) heavily compress content — may mask details.

---

## 🛡 9) Investigator Tips
- Always keep an untouched copy of the original media file.  
- Perform **multiple tool cross-checks** — no single tool is infallible.  
- Archive both original and annotated findings for reproducibility.

---

## 🗂 10) Documentation Hygiene
- Store: original file, extracted stills, audio samples, transcripts, coordinates, tool outputs, and confidence ratings.  
- Maintain **chain of custody** for any evidentiary use.

---

### 📜 Changelog (2025-08-10)
- Added full **OSINT tool arsenal** with metadata, visual, and audio analysis utilities.  
- Included **deepfake detection** consideration in 2025 context.  
- Expanded integrated verification methods across time, weather, and geolocation.
