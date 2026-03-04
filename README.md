  Scotland Weather Control Center — 3D Live Weather Dashboard
https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white
https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white
https://img.shields.io/badge/JavaScript-323330?logo=javascript&logoColor=F7DF1E
https://img.shields.io/badge/Leaflet.js-199900?logo=leaflet&logoColor=white
https://img.shields.io/badge/OpenWeather_API-FF8C00?logo=cloud&logoColor=white
https://img.shields.io/badge/AWS_S3-569A31?logo=amazonaws&logoColor=white
https://img.shields.io/badge/AWS_CloudFront-FF9900?logo=amazonaws&logoColor=white

This project is a fully interactive, 3D‑styled weather intelligence dashboard I built for key Scottish cities. It brings together real‑time weather data, radar layers, atmospheric calculations, and a custom UI into a single cloud‑hosted application. Everything is powered by the OpenWeather API and deployed globally using AWS S3 and CloudFront for fast, reliable delivery.

🌍 Live Demo
https://dfatncdayllfx.cloudfront.net

🚀 Overview
The Scotland Weather Control Center is designed to provide a clean, high‑contrast interface that makes live weather conditions easy to understand at a glance. It includes a 3D visual representation of Scotland, animated UI elements, and a layout focused on clarity and operational awareness. Users can switch between major Scottish cities and instantly view localized conditions, updated in real time through the OpenWeather API.

✨ Features
I designed the dashboard to feel modern, responsive, and operationally useful. Every component is built to give a clear, real‑time picture of weather conditions across Scotland.

3D Weather Core

• Custom 3D‑styled Scotland visual

• Animated orbit ring with glow effects

• Real‑time temperature, conditions, and descriptions

• Feels‑like temperature, wind speed, humidity, and visibility

Live Radar Map (Leaflet + OpenWeather Tiles)

 • Rain radar

• Cloud coverage

• Wind patterns

• Temperature layers

• Layer toggles for quick switching

• Smooth zoom and pan interactions

City Selector

• Dropdown with major Scottish cities

• Instant refresh via Sync Now

• Automatic map repositioning

5‑Day Forecast

• Condensed forecast layout

• Midday selection for consistent readings

• Temperature and condition summaries

Atmospheric Profile

• Dew point (calculated)

• Cloud base height (calculated)

• Sea level pressure

• Ground level pressure

• Cloud cover percentage

• Human‑readable condition tags

• Last update timestamp

Branding
“Built by Samuel • 2026” signature badge

🧠 Technical Stack

• Frontend

• HTML5

• CSS3 (gradients, animations, glassmorphism)

• JavaScript (ES6+)

• Leaflet.js

APIs
• OpenWeather Current Weather

• OpenWeather 5‑Day Forecast

• OpenWeather Radar Tile Layers

Cloud Deployment

• AWS S3 for static hosting

• AWS CloudFront for global CDN, HTTPS, and caching

📁 Project Structure
/
├── index.html        # Main application file containing UI, JS logic, and styling
└── README.md         # Project documentation


All logic is contained in index.html for simplicity and portability.

⚙️ How It Works
Weather Data Fetching
The dashboard retrieves:
- Current weather
- 5‑day forecast
- Radar tile layers

based on the selected city’s coordinates.

Atmospheric Calculations
The application computes:
- Dew point
- Cloud base height
- Human‑readable condition tags
These values are derived from temperature, humidity, and other API data.

Radar Layers
Leaflet loads OpenWeather tile layers with adjustable opacity to create a smooth meteorological map experience.

Cloud Deployment
The project is hosted on AWS S3 and distributed globally through CloudFront. Cache invalidation ensures that updates to the dashboard appear instantly.

🛠️ Setup Instructions
1. Clone the repository
git clone https://github.com/adeyeyesamuel409-svg/scotland-weather-control-center.git
cd scotland-weather-control-center


2. Add your OpenWeather API key
Inside index.html, replace:
const API_KEY = "33ced6a4eb0fdc5612a9964507e843d8";
const TILE_API_KEY = "33ced6a4eb0fdc5612a9964507e843d8";


3. Deploy to AWS S3
Upload index.html to your S3 bucket.

4. Invalidate CloudFront Cache
In CloudFront → Invalidations:
/*

5. Open your CloudFront URL
Your dashboard is now live.

📸 Screenshots

![Scotland Weather Dashboard Screenshot](https://github.com/adeyeyesamuel409-svg/Scotland-Weather-Control-Centre/blob/main/Scotland%203D%20Weather%20Control%20Center%20and%205%20more%20pages%20-%20Personal%20-%20Microsoft%E2%80%8B%20Edge%203_1_2026%2012_06_14%20PM.png?raw=true)

- Built by Samuel badge


👤 Author
Samuel
Cloud Engineering 
Edinburgh, Scotland

