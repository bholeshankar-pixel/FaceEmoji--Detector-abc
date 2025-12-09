# 🪬 FaceEmoji Detector

**Real-time facial emotion detection using your webcam** – Turn faces into live emojis directly in your browser. Built for hackathon demos, workshops, and quick prototypes.

## ✨ Features

- **Live Webcam Detection**: 30fps emotion analysis with smooth emoji overlay (😊😢😲😠😐)
- **Confidence Scores**: Real-time bars showing happy, sad, angry, surprised, neutral percentages
- **Session Stats**: Track total detections, average emotion duration, and peak emotion
- **Export Data**: Download session results as JSON for analysis or presentation
- **Zero Backend**: Runs entirely client-side using face-api.js
- **PWA-Ready**: Single-file deployment, works offline after first load
- **Mobile-Responsive**: Touch-friendly controls, full-screen video support

## 🚀 Tech Stack

- **HTML5 + CSS3** (dark theme: `#0f172a` + `#38bdf8` accents)
- **Vanilla JavaScript** (no frameworks, no build tools)
- **face-api.js** (tinyFaceDetector + faceExpressionNet via CDN)
- **Canvas API** for drawing detections + emoji animations
- **requestAnimationFrame** for smooth 30fps processing

## 🎯 Quick Start

1. **Clone or download** this repo
2. Open `index.html` in Chrome/Edge/Firefox (HTTPS required for camera)
3. Click **Start Camera** and allow webcam permissions
4. Watch your emotions turn into live emojis!

**Live Demo**: [GitHub Pages URL here]

## 📦 Deployment (GitHub Pages)

1. Push `index.html` to your repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/root` folder
4. Access at `https://your-username.github.io/repo-name/`

Zero configuration needed – it's a single file!

## 🎨 Customization

### Change Emojis
Edit the `EMOJI_MAP` object in the `<script>` section:
```js
const EMOJI_MAP = {
    happy: "😊",  // Change to any emoji you want
    sad: "😢",
    angry: "😠",
    surprised: "😲",
    neutral: "😐"
};
