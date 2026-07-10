# 🌹 Red Flower Bloom — Hand Gesture Controlled Animation

An interactive web experience where you grow and bloom a red flower using **your own hands** — no mouse, no keyboard, just gestures in front of your webcam.

## 🔗 Repository
[github.com/SGMahaswi/FLOWER-BLOOM](https://github.com/SGMahaswi/FLOWER-BLOOM)

## 🎥 Live Demo
🔴 **[Try it live](https://flower-bloom-3lghkfvrr-mahaswi.vercel.app)** — allow camera access, then use your left hand to grow the stem and your right hand to bloom the flower.

## ✨ Concept

This project turns hand tracking into a creative canvas. Instead of clicking buttons, you control a growing flower using two independent gestures:

| Hand | Role | Effect |
|------|------|--------|
| ✋ **Left Hand** | Growth | Controls the stem/plant growing upward |
| ✋ **Right Hand** | Bloom | Controls the flower opening into full bloom |

The idea is simple: nature grows and blooms in stages, and this project lets your own movement mirror that process in real time.

## 🛠️ Tech Stack

- **HTML5** — structure and canvas/SVG rendering
- **CSS3** — styling, animations, and transitions for the flower's visual growth
- **JavaScript** — core logic, animation control, and gesture-to-animation mapping
- **MediaPipe Hands** — real-time hand landmark detection via webcam

## 🚀 How It Works

1. The webcam feed is captured using the browser's `getUserMedia` API.
2. MediaPipe Hands processes the video stream and detects hand landmarks in real time.
3. The app distinguishes between the **left** and **right** hand based on landmark data.
4. Movement/position of the **left hand** is mapped to the flower's **growth stage** (stem height, leaf size).
5. Movement/position of the **right hand** is mapped to the **bloom stage** (petal opening angle, size, color intensity).
6. CSS transitions and JS-driven animations render the flower growing and blooming smoothly based on this input.

## 📦 Getting Started

### Prerequisites
- A modern browser (Chrome/Edge recommended for best webcam + MediaPipe support)
- A working webcam
- Local server (for camera permissions to work correctly)

### Installation

```bash
git clone https://github.com/SGMahaswi/FLOWER-BLOOM.git
cd FLOWER-BLOOM
```

### Run Locally

You can use any simple local server, for example:

```bash
# Using Python
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser and allow camera access.

## 📁 Project Structure

```
FLOWER-BLOOM/
├── index.html      # Main structure & canvas/SVG setup
├── style.css       # Flower styling & growth/bloom animations
├── app.js          # Hand tracking logic & gesture-to-animation mapping
├── LICENSE
└── README.md
```

## 💡 Future Improvements

- Support for multiple flower colors based on gesture speed
- Add sound/ambient effects during bloom
- Mobile camera support
- Save/share a snapshot of the fully bloomed flower

## 🙋 Author

Built by **Maha** ([@s_g_maha](https://github.com/s_g_maha))

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
