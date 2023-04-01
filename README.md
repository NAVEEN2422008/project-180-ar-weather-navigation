# c180 — AR Weather Navigation

A map-based AR app that lets users pick a destination across Indian landmarks and view live weather overlayed as an AR/HUD display.

## Features
- Mapbox map centered on the user via geolocation.
- Custom image markers on the map for Amber, Gateway, India Gate, Lotus Temple, and Victoria Memorial.
- Search by landmark with Mapbox Geocoder and navigate to destination.
- Weather lookup at the destination via the OpenWeatherMap API.
- AR overlay (geo-location entities) displaying the destination's weather forecast.

## Tech Stack
- HTML/CSS (Bootstrap), jQuery
- Mapbox GL JS + Geocoder
- OpenWeatherMap API, AR (A-Frame/geo-location entities)

## Project Structure
```
c178/
├── main.html          # map landing page
├── main.js            # geolocation + Mapbox map setup
├── main.css
├── ar_weather.html    # AR weather scene
├── ar_weather.js      # coordinates + weather fetch
└── assets/            # landmark images
```

## Installation
- No build step; deploy `c178/` to any static host (needs HTTPS + device location for geo/AR to work).

## Usage
1. Allow location access.
2. Pick a landmark, click "Show Me The Weather!".
3. The AR/weather scene renders the destination's live weather.