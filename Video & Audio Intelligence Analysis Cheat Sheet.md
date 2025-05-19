# 🎧🎥 OSINT Cheat Sheet – Video & Audio Intelligence Analysis

**Purpose:** Extract truth from video, audio, and voice content on platforms like Telegram, TikTok, YouTube, Podcasts, and Live Streams using OSINT-grade workflows and AI-enhanced tools.

---

## 1. 🗂️ Metadata Extraction

**Objective:** Identify original source info, GPS coordinates, device types, creation/modification times.

**How-To:**
- Use tools to extract embedded EXIF/XMP/MP4 metadata from original files.
- Look for GPS tags, camera info, software footprints, and creation times.
- Always compare against visible content and claimed upload date.

**Tools:** ExifTool, MediaInfo, FOCA

---

## 2. 📝 Audio Transcription & Translation

**Objective:** Convert speech to searchable text. Enable language pivoting and keyword indexing.

**How-To:**
- Transcribe with Whisper (local) or Otter.ai (cloud).
- Translate using DeepL or GPT-based LLMs for nuanced language.
- Use LLMs (like ChatGPT) to summarize or highlight key phrases.

**Tools:** Whisper, Otter.ai, Google STT, DeepL, GPT-4

---

## 3. 🌍 Video Geolocation via Scene & Environment

**Objective:** Determine where the footage was recorded using visual and environmental cues.

**How-To:**
- Extract keyframes with InVID.
- Match visual details using Google Earth, Maps, Mapillary, and SunCalc.
- Analyze natural lighting for time-of-day estimation.

**Tools:** InVID, Google Earth, SunCalc, Mapillary

---

## 4. 🗣️ Voice Recognition & Speaker Verification

**Objective:** Confirm identity or link voices across media.

**How-To:**
- Create voice embeddings with Resemblyzer.
- Compare voice samples or run voiceprint analysis.
- Use AI to flag synthetic/deepfake speech anomalies.

**Tools:** Resemblyzer, Batvox, i2 Voice Biometrics

---

## 5. 🔉 Ambient Sound & Environmental Audio

**Objective:** Extract context from background audio (location, time, local culture).

**How-To:**
- Use spectrograms to identify birds, prayer calls, traffic, accents.
- Cross-reference ambient cues with known locations or regional audio libraries.

**Tools:** Audacity, iZotope RX, OpenSMILE, Shazam API

---

## 6. 🧠 Pattern, Symbol & Object Detection

**Objective:** Identify recurring visual elements (logos, faces, gear, flags).

**How-To:**
- Run object detection models on video frames (YOLO, OpenCV).
- Use facial recognition tools to track individuals.
- Detect edited/reused footage via visual anomalies.

**Tools:** YOLOv8, OpenCV, DeepFace, TensorFlow

---

## 7. 💬 Sentiment & Intent Analysis

**Objective:** Assess tone, stress, and emotional charge in speech.

**How-To:**
- Run transcripts through LLMs to summarize, classify tone, or detect threat rhetoric.
- Use acoustic tools to detect stress, aggression, deception.

**Tools:** VADER, TextBlob, OpenSMILE, GPT-4

---

## 8. 🧑‍💻 Feature Extraction (Face, Voice, Symbols)

**Objective:** Isolate faces, insignia, gestures, voice markers for entity mapping.

**How-To:**
- Segment and tag faces or emblems.
- Build pattern-of-life from recurring features across videos.

**Tools:** Face++, DeepFace, YOLOv8, Maltego CE

---

## 9. ⏱️ Timestamp & Temporal Verification

**Objective:** Detect fakes by validating claimed time vs. visual/audio evidence.

**How-To:**
- Extract internal timestamps using FFmpeg.
- Compare lighting, weather, broadcast overlays, or live event markers.

**Tools:** FFmpeg, InVID, SunCalc

---

## 10. 📈 Cross-Platform Correlation

**Objective:** Link identities, voices, and visuals across platforms.

**How-To:**
- Pivot from voice to face, face to username, username to location.
- Use graphing tools to visualize relationships and timelines.

**Tools:** Maltego, SpiderFoot, CaseFile, Neo4j

---

## ⚖️ Legal & Ethical Guidelines

- ✅ Use only publicly available or user-consented media.
- ❌ Do not access private, encrypted, or protected data without legal authority.
- ⚖️ Follow GDPR, CCPA, and local data laws.
- 🧭 Maintain investigative integrity and clear OSINT purpose.

---

## 📚 Tools & Resources Reference

| Tool                | Purpose                                   | Link |
|---------------------|-------------------------------------------|------|
| ExifTool            | Metadata extraction                       | https://exiftool.org |
| MediaInfo           | Media stream analysis                     | https://mediaarea.net/en/MediaInfo |
| FOCA                | Office/PDF metadata extraction            | https://github.com/ElevenPaths/FOCA |
| Whisper             | Offline speech-to-text                    | https://github.com/openai/whisper |
| Otter.ai            | Cloud transcription w/ speaker ID         | https://otter.ai |
| Google STT          | Cloud-based speech-to-text                | https://cloud.google.com/speech-to-text |
| DeepL API           | High-accuracy translation                 | https://www.deepl.com/docs-api |
| InVID Plugin        | Keyframe extraction, reverse search       | https://www.invid-project.eu |
| Google Earth        | Satellite image geolocation               | https://www.google.com/earth |
| SunCalc             | Sun position and lighting calculator      | https://www.suncalc.org |
| Resemblyzer         | Speaker embedding & comparison            | https://github.com/resemble-ai/Resemblyzer |
| Batvox              | Voice biometrics analysis                 | https://falcon-analytical.com |
| Audacity            | Audio editing & spectrum view             | https://www.audacityteam.org |
| iZotope RX          | Professional audio forensics              | https://www.izotope.com/en/products/repair-and-edit/rx.html |
| YOLOv8              | Object detection (real-time)              | https://github.com/ultralytics/ultralytics |
| OpenCV              | Vision pattern recognition                | https://opencv.org |
| DeepFace            | Facial recognition                        | https://github.com/serengil/deepface |
| TensorFlow          | AI/ML model building                      | https://www.tensorflow.org |
| Face++              | Face attribute API                        | https://www.faceplusplus.com |
| VADER               | Sentiment analysis                        | https://github.com/cjhutto/vaderSentiment |
| OpenSMILE           | Acoustic feature extraction               | https://audeering.com/technology/opensmile |
| FFmpeg              | Frame & metadata extraction               | https://ffmpeg.org |
| Maltego             | Relationship mapping                      | https://www.paterva.com |
| CaseFile            | Offline link analysis                     | https://www.maltego.com/casefile |
| SpiderFoot          | Passive recon and automation              | https://www.spiderfoot.net |
| GPT-4 (ChatGPT Pro) | Summarization, sentiment, pivot reasoning | https://chat.openai.com |
