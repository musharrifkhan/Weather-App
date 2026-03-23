#🌤️ WeatherBoard — Real-Time Weather App
Project Overview
WeatherBoard is a browser-based weather application that lets users instantly look up current weather conditions for any city in the world. The app fetches live data from a public weather API and displays it in a clean, responsive interface with support for multiple visual themes and temperature unit toggling.

Purpose
The goal of this project is to build a functional, user-friendly weather lookup tool that demonstrates real-world API integration, dynamic DOM manipulation, and responsive UI design — all using vanilla HTML, CSS, and JavaScript with no frameworks or dependencies.

API Used
OpenWeatherMap — Current Weather Data API

Base URL: https://api.openweathermap.org/data/2.5/weather
Authentication: API Key (query parameter appid)
Units: Metric (°C) by default, converted to Fahrenheit client-side
Docs: https://openweathermap.org/current


Features
Implemented

City search by name with Enter key and button support
Live display of temperature, humidity, wind speed, and feels-like temperature
Dynamic weather emoji icons mapped from OpenWeatherMap condition codes
°C / °F toggle (converts client-side, no extra API call)
Three visual themes: Dark, Light, Sunset
Loading spinner during API fetch
Error handling for invalid or not-found cities

Planned for Future Milestones

Search history dropdown with recent cities (search feature)
Filter results by country code to disambiguate cities with the same name
Sort/compare multiple saved city cards by temperature or humidity
5-day forecast view using the OpenWeatherMap Forecast API
Geolocation support to auto-detect the user's city on page load
Persistent theme preference saved to localStorage


Technologies Used
TechnologyPurposeHTML5Page structure and markupCSS3Styling, theming, animations, responsive layoutVanilla JavaScript (ES6+)API calls, DOM updates, event handlingOpenWeatherMap APILive weather dataGoogle Fonts (DM Sans, Syne)TypographyFetch APIAsync HTTP requests

Project Structure
weather-app/
│
├── index.html        # Main application file (HTML + CSS + JS in one file)
└── README.md         # Project documentation

Setup & Running the Project
Prerequisites

A modern web browser (Chrome, Firefox, Edge, Safari)
An active internet connection (required for API calls and Google Fonts)
A free API key from OpenWeatherMap

Steps

Clone or download the repository

bash   git clone [https://github.com/your-username/weather-app.git](https://github.com/musharrifkhan/Weather-App)
   cd weather-app

Add your API key — open index.html and replace the value of apiKey on this line:

javascript   const apiKey = "c8132bbc311fd45a8369d2fccd14a3e1";

Open the app — simply open index.html in your browser. No build step or server required.

bash   # Option 1: double-click index.html
   # Option 2: use VS Code Live Server extension
   # Option 3: serve locally with Python
   python -m http.server 8000

Search for a city — type any city name in the search box and press Enter or click the arrow button.


Notes

This project intentionally uses no external frameworks (no React, Vue, Bootstrap, or Tailwind) to keep the codebase minimal and focused on core web fundamentals.
API key is currently hardcoded for development. In a production environment, API calls should be proxied through a backend to protect the key.
All temperature conversion between °C and °F is handled client-side to avoid unnecessary API calls.


Author
Your Name — musharrif.k25286@nst.rishihood.edu.in

License
This project is open source and available under the MIT License.

