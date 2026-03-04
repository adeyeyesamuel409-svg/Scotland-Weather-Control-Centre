Scotland Weather Control Center — 3D Live Weather Dashboard
This project is a fully interactive, 3D‑styled weather intelligence dashboard built for key Scottish cities. It combines real‑time weather data, radar layers, atmospheric calculations, and a custom UI design into a single cloud‑hosted application. The dashboard is powered by the OpenWeather API and deployed globally using AWS S3 and CloudFront.

🌍 Live Demo
https://dfatncdayllfx.cloudfront.net

🚀 Overview
The Scotland Weather Control Center provides a modern, high‑contrast interface that displays live weather conditions, radar layers, and a detailed atmospheric profile. It includes a 3D visual representation of Scotland, animated UI elements, and a clean layout designed for clarity and operational awareness.
The dashboard updates in real time using the OpenWeather API and allows users to switch between major Scottish cities to view localized conditions.

✨ Features
3D Weather Core
- Custom 3D‑styled Scotland visual
- Animated orbit ring and glow effects
- Real‑time temperature, conditions, and weather description
- Feels‑like temperature, wind speed, humidity, and visibility
Live Radar Map (Leaflet + OpenWeather Tiles)
- Rain radar layer
- Clouds layer
- Wind layer
- Temperature layer
- Layer toggle control
- Smooth zoom and pan interactions
City Selector
- Dropdown menu with major Scottish cities
- Instant data refresh using the “Sync Now” button
- Automatic map repositioning based on selected city
5‑Day Forecast
- Condensed forecast for the next five days
- Midday forecast selection for consistency
- Temperature, conditions, and descriptions
Atmospheric Profile
- Dew point (calculated)
- Cloud base height (calculated)
- Sea level pressure
- Ground level pressure
- Cloud cover percentage
- Human‑readable “conditions tag”
- Last update timestamp
Branding
- “Built by Samuel • 2026” signature badge displayed on the interface

🧠 Technical Stack
Frontend
- HTML5
- CSS3 (custom gradients, animations, glassmorphism)
- JavaScript (ES6+)
- Leaflet.js for interactive mapping
APIs
- OpenWeather Current Weather API
- OpenWeather 5‑Day Forecast API
- OpenWeather Tile Layers (Radar)
Cloud Deployment
- AWS S3 for static hosting
- AWS CloudFront for global CDN distribution, HTTPS, and caching

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

