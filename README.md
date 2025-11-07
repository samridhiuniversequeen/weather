# Weather Forecast Dashboard

![Weather Dashboard Preview](https://samridhiuniversequeen.github.io/weather/)  

## 📖 Description

This is a fully responsive, one-page **Weather Forecast Dashboard** built with **HTML**, **CSS (Tailwind CSS)**, and **JavaScript**. It fetches real-time weather data for any city entered by the user and displays current conditions, a 5-day forecast, and smart environment-friendly tips based on air quality, temperature, humidity, and wind.

- **No backend required**: Runs entirely in the browser.
- **API Integration**: Uses the free [Open-Meteo API](https://open-meteo.com/) for weather data (no API key needed!).
- **User Experience**: Features an engaging intro animation, loading spinner, error handling, and dynamic UI changes (e.g., background gradients based on weather).

Perfect for personal use, portfolios, or as a starting point for weather apps.

## 🚀 Features

- **City Search**: Enter any city name (e.g., "London", "New York") to get instant weather.
- **Current Weather**: Temperature (°C), feels-like, humidity (%), wind speed (km/h) & direction (°), pressure (hPa), weather condition with emoji icons.
- **5-Day Forecast**: Daily high/low temps, conditions, and icons for the next 5 days.
- **Air Quality Index (AQI)**: US EPA-based index with status badges (Good to Hazardous).
- **Smart Tips**: Personalized, eco-focused advice (e.g., "High humidity? Air-dry clothes to save energy!").
- **Dynamic UI**:
  - Glassmorphism cards with backdrop blur.
  - Weather-themed background gradients (clear, cloudy, rain, snow).
  - Smooth animations: Intro letter-drop, cloud float, fade-ins, hover scales, bouncing icons.
- **Responsive Design**: Mobile-first, works on phones, tablets, and desktops.
- **Default Load**: Starts with London weather after a fun intro animation.
- **Error Handling**: Graceful messages for invalid cities.

## 🛠 Tech Stack

- **Frontend**: HTML5, Tailwind CSS (via CDN), Vanilla JavaScript.
- **API**: 
  - [Open-Meteo Geocoding](https://geocoding-api.open-meteo.com/) for city-to-lat/lon conversion.
  - [Open-Meteo Forecast](https://api.open-meteo.com/) for current/hourly/daily data.
  - [Open-Meteo Air Quality](https://air-quality-api.open-meteo.com/) for AQI.
- **Animations**: Custom CSS keyframes (no external libraries).
- **Icons**: Emoji-based (lightweight, no assets needed).

## 📱 How to Run

1. **Clone or Download**:
   - Save the code as `index.html` (single file—no separate CSS/JS needed).

2. **Open in Browser**:
   - Double-click `index.html` or open in any modern browser (Chrome, Firefox, Safari, Edge).
   - No server required—runs locally!

3. **Test It**:
   - Page loads with an animated intro ("W E A T H E R" drops in with a floating cloud).
   - Defaults to London weather.
   - Search for "Tokyo" or any city and hit Enter/Search.

4. **Customization**:
   - Edit `weatherMap` in JS for more weather codes/icons.
   - Tweak gradients in CSS for themes.
   - Add dark mode by extending Tailwind config.

## 🔍 API Details

- **No Key Needed**: Open-Meteo is completely free and open-source.
- **Endpoints Used**:
  - Geocoding: `https://geocoding-api.open-meteo.com/v1/search?name={city}&count=1`
  - Forecast: `https://api.open-meteo.com/v1/forecast?latitude={lat}&longitude={lon}&current=temperature_2m,...&daily=temperature_2m_max,...&forecast_days=5&timezone=auto`
  - AQI: `https://air-quality-api.open-meteo.com/v1/air-quality?latitude={lat}&longitude={lon}&hourly=us_aqi`
- **Rate Limits**: Unlimited for non-commercial use; respectful usage recommended.
- **Data Sources**: Aggregated from national weather services (high accuracy).

## 🎨 UI/UX Highlights

- **Intro Animation**: Letters "drop" in with rotation/scale effects, followed by a floating cloud.
- **Glassmorphism**: Semi-transparent cards with blur for a modern, frosted-glass look.
- **Dynamic Backgrounds**: Changes color based on conditions (e.g., pinkish for clear skies).
- **Hover Effects**: Cards scale up; tips "bounce" with icon animations.
- **Accessibility**: High contrast, semantic HTML, keyboard-navigable search.

## 📸 Screenshots

| Desktop View | Mobile View |
|--------------|-------------|
| ![Desktop](https://via.placeholder.com/800x400/667eea/ffffff?text=Desktop+Weather+Dashboard) | ![Mobile](https://via.placeholder.com/400x800/667eea/ffffff?text=Mobile+Weather+Dashboard) |

*(Add real screenshots from browser dev tools.)*

## 🤝 Contributing

1. Fork the repo.
2. Create a feature branch (`git checkout -b feature/amazing-feature`).
3. Commit changes (`git commit -m 'Add amazing feature'`).
4. Push to branch (`git push origin feature/amazing-feature`).
5. Open a Pull Request.

Suggestions welcome—issues for bugs/features!

## ⚠️ Limitations

- **No Historical Data**: Focuses on current/forecast only.
- **AQI Coverage**: US-focused; may vary globally.
- **Offline**: Requires internet for API calls.
- **Icons**: Simple emojis—enhance with SVG libraries if needed.

## 📄 License

This project is licensed under the MIT License - see the MIT file for details.

---

**Built with ❤️ by Samridhi | Last Updated: November 07, 2025**  
