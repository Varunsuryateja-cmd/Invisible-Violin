# 🎻 Invisible Violin

An interactive, AI-powered browser "Air Violin" that transforms your webcam into a musical instrument. Play realistic violin tones in mid-air using hand gestures and test your musical ear with an integrated pitch-matching mini-game.

---

## 🚀 How It Works

Invisible Violin combines real-time computer vision with low-latency Web Audio synthesis:

- **Hand & Gesture Tracking (MediaPipe Hands)**: Tracks 21 3D hand landmarks in real time via your webcam directly in the browser with zero server latency.
  - **Left Hand (Fingerboard / Pitch)**: Position your left hand and index fingertip vertically to choose notes along the virtual violin fingerboard.
  - **Right Hand (Bowing / Dynamics)**: Move your right hand back and forth horizontally like drawing a violin bow across strings. Bow velocity dynamically controls volume, filter resonance, and articulation. Stop moving to rest naturally into silence.
- **Audio Engine (Tone.js & Web Audio API)**: Synthesizes rich violin timbres using sawtooth/triangle oscillators, dynamic lowpass filtering, vibrato modulation, and polyphonic celebration chimes.

---

## ✨ Features

- **🎻 Free Play Mode**: Expressive mid-air violin playing with continuous pitch or snapped scales, real-time audio waveform visualizer, and bow velocity meters.
- **🎯 Match the Note Game**: An interactive pitch-training game. Hit the glowing target notes, hold steady intonation, earn points, and build score multiplier streaks with visual particle bursts and reward chimes.
- **🎼 Scale-Snapped Modes**:
  - D Major Scale (default)
  - D Minor Scale
  - Visual fingerboard guides and note labels for easy intonation.
- **🌓 Modern Aesthetics**: Sleek dark/light theme toggle, glassmorphism HUD overlays, particle canvas effects, and responsive layout for desktop and laptop webcams.
- **🔒 100% Client-Side & Private**: All video processing and audio synthesis run locally in your browser. No video or audio feeds are uploaded to any server.

---

## 🛠️ Getting Started

### Prerequisites
- A modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, or Brave) with webcam and audio permissions enabled.

### Running Locally

#### Option 1: Direct File Open
Simply double-click [`invisible-violin.html`](invisible-violin.html) or drag and drop it into your web browser.

#### Option 2: Local HTTP Server (Recommended)
You can start a local development server using Python:

```bash
# Python 3
python -m http.server 8000
```

Or using Node.js:
```bash
npx serve .
```

Then open your browser at:
```
http://localhost:8000/invisible-violin.html
```

---

## 🎮 How to Play

1. Click **🎥 Start Camera** and grant browser webcam permissions.
2. Click **🔊 Enable Sound** to start the Tone.js audio context.
3. **Left Hand**: Raise your left hand in front of the camera to position your finger on the virtual fingerboard.
4. **Right Hand**: Draw your right hand horizontally back and forth to bow notes!
5. Switch between **🎯 Match the Note Game** and **🎻 Free Play** using the top navigation tabs.

---

## 🧰 Tech Stack

- **Computer Vision**: [Google MediaPipe Hands](https://github.com/google-ai-edge/mediapipe)
- **Audio Synthesis**: [Tone.js](https://tonejs.github.io/) (Web Audio API)
- **Frontend**: HTML5, Canvas API, Modern Vanilla CSS3, ES6+ JavaScript

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) (or open source). Feel free to fork and build your own gestures!
