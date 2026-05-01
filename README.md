# 🌸 Cozy Study Studio

A cozy, aesthetic study productivity web app featuring a Pomodoro-style timer, task list, ambient sounds, live weather, and embedded Spotify playlists — all wrapped in a dreamy glassmorphism UI.

---

## ✨ Features

- **⏱️ Pomodoro Timer** — Countdown timer defaulting to 30 minutes with start/pause, custom time input, stepper arrows, and keyboard spacebar support
- **✅ Task List** — Add, check off, and delete tasks with smooth animations; tracks study session completions (Goal: 4 sessions)
- **🌧️ Ambient Audio** — Toggle local rain or lofi MP3s; ambient rain drops animated in the background
- **🎧 Spotify Playlists** — Collapsible embedded playlists: Rain Mode, Lofi Mode, and Academic Comeback
- **🌦️ Live Weather** — Fetches real-time temperature via Open-Meteo API with a dynamic icon (☀️ / 🌦️ / ❄️)
- **🕐 Live Clock & Date** — Real-time clock with AM/PM and formatted date display
- **🎉 Session Completion** — Confetti animation, browser notification, and alarm sound on timer end with auto-stop after 30 seconds
- **📱 Responsive Design** — Fully responsive layout that collapses to a single column on mobile and tablet

---

## 🗂 Project Structure

```
CozyStudy/
├── index.html          # All HTML, CSS, and JavaScript in one file
├── vibe.jpg            # Background image
├── favicon.png         # Browser tab icon
├── alarm.mp3           # Timer completion alarm sound
├── rain.mp3            # Looping ambient rain audio
└── lofi.mp3            # Looping ambient lofi audio
```

---

## 🛠 Tech Stack

| Technology | Use |
|------------|-----|
| HTML/CSS/JavaScript | Core structure, styling, and logic |
| [Bootstrap 5.3](https://getbootstrap.com/) | Layout utilities and collapsible Spotify panels |
| [Canvas Confetti](https://github.com/catdad/canvas-confetti) | Session completion celebration |
| [Open-Meteo API](https://open-meteo.com/) | Free real-time weather data (no API key required) |
| Spotify Embed | Embedded playlist iframes |
| Google Fonts | Poiret One, Lobster Two, Quicksand, Borel |

---

## 🚀 Getting Started

1. Clone or download this repository
2. Add the required local assets to the project root:
   - `vibe.jpg` — background photo
   - `favicon.png` — tab icon
   - `alarm.mp3`, `rain.mp3`, `lofi.mp3` — audio files
3. Open `index.html` in any modern browser

> No build tools, frameworks, or installations required — it's a single HTML file.

---

## ⌨️ Keyboard Shortcut

| Key | Action |
|-----|--------|
| `Space` | Start / Pause the timer (when not focused on an input) |

---

## 🎨 Design System

The UI uses a soft pastel glassmorphism aesthetic with these CSS variables:

| Variable | Color | Use |
|----------|-------|-----|
| `--peach` | `#ffb38a` | Input borders, accents |
| `--soft-pink` | `#fce4ec` | Button hover states |
| `--accent-pink` | `#ff80ab` | Headers, active states |
| `--text` | `#5d4a4a` | Body text |
| `--glass` | `rgba(255,255,255,0.85)` | Card backgrounds |

Fonts used: **Poiret One** (headers), **Lobster Two** (timer display), **Quicksand** (body/buttons), **Borel** (accent tagline)

---

## 📍 Weather API

Weather is fetched from the [Open-Meteo](https://open-meteo.com/) free API — no API key needed. Coordinates are currently set to **Austin, TX** (latitude: 30, longitude: -97). Update these values in the fetch call inside `index.html` to match your location.

```javascript
fetch('https://api.open-meteo.com/v1/forecast?latitude=30&longitude=-97&current_weather=true&temperature_unit=fahrenheit')
```

---

## 👩‍💻 Author

Natalie M. Leal — created 2026 for fun
