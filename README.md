# SkyPulse 🌤️

> **Weather, beautifully simplified.**

SkyPulse is a lightweight weather dashboard built with **HTML, CSS, and vanilla JavaScript**. It turns Open-Meteo forecast data into a clean, responsive weather experience with city search, geolocation, saved places, forecasts, and practical weather insights.

## ✨ What you can do

| Experience | Included |
|---|---|
| 🌡️ Live conditions | Temperature, feels-like, humidity, wind, clouds, precipitation |
| 🌧️ Rain outlook | Current precipitation + daily rain probability |
| 📅 Forecast | 7-day weather forecast |
| 📈 Hourly view | Next 12 hours temperature visualization |
| 🔎 City search | Open-Meteo geocoding with city lookup |
| 📍 My location | Browser geolocation support |
| ⭐ Saved places | Up to 6 locations stored locally |
| 💡 Smart insights | Simple weather-aware recommendations |
| 🔄 Fresh data | Automatic refresh every 10 minutes |
| 📱 Responsive UI | Desktop, tablet, and mobile layouts |

## 🧭 How it works

```text
             ┌──────────────────┐
             │     SkyPulse     │
             │ HTML/CSS/JS UI   │
             └────────┬─────────┘
                      │
          ┌───────────┴───────────┐
          ▼                       ▼
┌──────────────────┐    ┌────────────────────┐
│ Open-Meteo       │    │ Browser Geolocation│
│ Forecast API     │    │ + localStorage     │
└──────────────────┘    └────────────────────┘
```

The app uses Open-Meteo's **Forecast API** for weather data and **Geocoding API** for city searches. Saved locations and preferences stay in the browser through `localStorage`.

## 🛠️ Stack

- **HTML5** — application structure
- **CSS3** — responsive glass-style dashboard UI
- **Vanilla JavaScript** — state, API requests, rendering, persistence
- **Open-Meteo** — forecast and geocoding data
- **Browser APIs** — Geolocation and localStorage

No frontend framework or build step is required.

## 🚀 Run locally

The simplest option is to open `index.html` in a modern browser.

For reliable browser geolocation and local development, serve the folder with any static HTTP server, for example:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## 🔐 API & privacy

SkyPulse does not require an API key for normal non-commercial Open-Meteo usage. Weather requests are made from the browser to the Open-Meteo endpoints.

The app stores saved locations in browser `localStorage`. It does not include a custom backend or user account system.

## 📁 Project structure

```text
SkyPulse/
└── index.html    # Complete application: UI, styles, and JavaScript
```

The intentionally small structure makes SkyPulse easy to understand, fork, host, and extend.

## 🎯 Project highlights

SkyPulse demonstrates practical frontend development without relying on a framework:

- asynchronous REST API consumption with `fetch`
- geocoding and coordinate-based weather queries
- dynamic DOM rendering
- responsive CSS layouts
- browser geolocation
- client-side persistence
- automatic data refresh
- graceful loading and error states
- weather-code interpretation and derived insights

## ☁️ Hosting

Because SkyPulse is a static frontend, it can be hosted on services such as GitHub Pages, Netlify, Vercel, or any static web server.

## 📄 License

MIT License.

---

Built by **Harsh** · [@Harsh0675](https://github.com/Harsh0675)
