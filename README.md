# Weather App

A simple weather app I made for a school project using Ionic, Angular (standalone components), and Capacitor.

## Features

- **Home:** Shows current weather and a 5-day forecast using Open-Meteo and my device GPS. It can refresh, show loading/error states, and use Gapan as a fallback if location is not available.
- **Map:** Shows my location and saved places on a Leaflet + OpenStreetMap map.
- **Places:** Lets me add, edit, and delete saved places. Places are stored locally on the device.
- **Add/Edit Place:** Uses a form with a note and GPS coordinates filled from my current location.
- **Offline cache:** Saves the last weather data and shows it if the app cannot load new data.
- **Vibration:** Uses haptics for some actions like refresh, save, delete, and errors.

## Tech Used

- Ionic + Angular
- Capacitor
- Open-Meteo API (no API key)
- Leaflet + OpenStreetMap
- Capacitor Geolocation, Preferences, and Haptics

## Screenshots

<!-- Add your screenshots here -->
- Home screen: `screenshots/home.png`
- Map screen: `screenshots/map.png`
- Places screen: `screenshots/places.png`
- Add/Edit Place screen: `screenshots/add-place.png`

## How to Run (Web)

```bash
npm install
ionic serve
```

## How to Build for Android

```bash
npm install
ionic build
npx cap sync android
npx cap open android
```

Then run the app on an Android device or emulator from Android Studio.

## Notes

- This project does not use a backend or REST API for saved places.
- Saved places are stored locally with Capacitor Preferences.
- Weather data comes from Open-Meteo.
- If GPS is denied or unavailable, the app falls back to Gapan, Nueva Ecija.
