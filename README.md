# Weather Dashboard

Single-file weather app. Search any city or use your current location.

## Setup

1. Get a free API key: https://openweathermap.org/api → sign up → API keys tab.
   (New keys can take up to an hour to activate.)

2. Open `index.html` and replace this line near the top of the `<script>`:
```js
const API_KEY = "YOUR_OPENWEATHERMAP_API_KEY";
```
with your actual key.

3. Just open `index.html` in a browser — no build step, no server needed.

## Deploy on GitHub Pages

```
git init
git add .
git commit -m "Weather dashboard"
git branch -M main
git remote add origin https://github.com/<your-username>/weather-dashboard.git
git push -u origin main
```

Then: repo → **Settings** → **Pages** → Source: `main` branch, `/ (root)` folder → Save.

Your live link will be `https://<your-username>.github.io/weather-dashboard/`.

## Note on the API key

This is a client-side-only project, so the key is visible in the page source — fine for a free-tier student project, not for production. If you want it hidden, you'd need a backend proxy, which adds complexity not needed here.
