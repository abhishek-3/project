# 🌤 Weather App

A fully client-side weather app — no server, no API key, no dependencies. Just open `index.html` in any browser.

**Features:**
- 🔍 Search any city or country worldwide with live autocomplete
- 🌡 Current temperature, feels-like, humidity & wind speed
- 🕐 Live clock with date
- 📈 24-hour temperature chart with smooth SVG curve
- 📅 5-day forecast cards with weather icons
- 💨 Air Quality Index (US AQI + EU AQI) with PM2.5, PM10, NO₂, O₃
- 📍 "Use my location" via browser Geolocation
- 🌙 Auto dark / light mode (`prefers-color-scheme`)
- 🌍 Country flag + region shown for every city
- 📶 Offline fallback — shows cached data if the network is unavailable

**Data sources (all free, no key needed):**
- Weather & forecast: [Open-Meteo](https://open-meteo.com)
- Air quality: [Open-Meteo Air Quality API](https://open-meteo.com/en/docs/air-quality-api)
- City search: [Open-Meteo Geocoding API](https://open-meteo.com/en/docs/geocoding-api)
- Reverse geocoding: [Nominatim / OpenStreetMap](https://nominatim.org)

---

## 🚀 Getting Started

### Option 1 — Download the ZIP (easiest)

1. Click the green **`<> Code`** button at the top of this page
2. Click **Download ZIP**
3. Extract the ZIP on your computer
4. Open the `index.html` file in any browser — that's it!

---

### Option 2 — Clone with Git

You'll need [Git](https://git-scm.com/downloads) installed.

```bash
# Clone the repository
git clone https://github.com/abhishek-3/project.git

# Go into the folder
cd project

# Open the app
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

---

### Option 3 — GitHub CLI

You'll need the [GitHub CLI](https://cli.github.com) installed.

```bash
gh repo clone abhishek-3/project
cd project
start index.html
```

---

## 🌐 Live Demo (GitHub Pages)

Enable GitHub Pages to get a shareable link — no installation needed:

1. Go to **Settings → Pages** in this repo
2. Set **Branch** to `main` → Save
3. Your app will be live at:

```
https://abhishek-3.github.io/project
```

---

## 📁 Project Structure

```
project/
├── index.html   ← The entire app (HTML + CSS + JS, single file)
└── README.md    ← This file
```

---

## 🛠 How It Works

The app is a single `index.html` file. When you open it:

1. It geocodes "Tokyo" via the Open-Meteo API and loads live weather
2. As you type in the search box, it fetches city suggestions live
3. Selecting a city fetches weather + air quality data **in parallel**
4. Everything renders client-side — no server, no build step

---

## 📋 Requirements

| Requirement | Details |
|---|---|
| Browser | Any modern browser (Chrome, Edge, Firefox, Safari) |
| Internet | Required for live data; falls back to cached data offline |
| Server | ❌ Not needed |
| API Key | ❌ Not needed |
| Node / npm | ❌ Not needed |

---

## 📄 License

MIT — free to use, modify, and distribute.
