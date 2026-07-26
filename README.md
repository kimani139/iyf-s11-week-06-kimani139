# Week 6 — Asynchronous JavaScript

## Files

- **`lesson11-async-exercises.js`** — All of Lesson 11 (sync vs async, callbacks,
  callback hell, Promises, chaining, `Promise.all`/`Promise.race`, async/await,
  try/catch, sequential vs parallel timing). Runnable directly in Node:
  ```
  node lesson11-async-exercises.js
  ```

- **`daily-challenges.js`** — Day 1–5 challenges (`delay()`, chained random-delay
  promises with timing, a fetch-with-fallback-on-404 helper, an async/await
  rewrite, and `Promise.allSettled` across 3 endpoints). Needs internet access
  (calls jsonplaceholder.typicode.com):
  ```
  node daily-challenges.js
  ```

- **`lesson12-user-directory/`** — Task 12.1–12.4: fetches users from
  JSONPlaceholder, renders cards in the DOM, live search, sort A–Z/Z–A, city
  filter, and a POST form to create a new post. Open `index.html` in a browser.

- **`weather-dashboard/`** — The mini-project. Open `index.html` in a browser.
  **Before it will work, add your free OpenWeatherMap API key** at the top of
  `app.js`:
  ```js
  const API_KEY = "your_api_key_here"; // <-- put your key here
  ```
  Get a key at https://openweathermap.org/api (the free tier is enough).

  Implements all required features plus every bonus:
  - Search by city, loading/error states
  - Full current-conditions display (temp, feels-like, humidity, wind, pressure)
  - 5-day forecast (bucketed from the 3-hourly forecast endpoint)
  - °C/°F toggle
  - Geolocation button (📍) for weather at your current position
  - Background theme shifts with the current sky condition (clear/cloudy/rain/
    snow/storm/mist, day vs night)
  - Recent searches (last 5) saved in `localStorage`, clickable to re-search
  - Signature UI element: an instrument-panel style dial gauge showing the
    temperature reading, styled like an old weather-station barometer

## Notes

- All exercises were run and verified where they don't require a live network
  connection (the sandbox that produced this has no internet, so the fetch
  calls in `daily-challenges.js` were verified for logic/error-handling only —
  they'll work normally in a browser or a Node environment with internet
  access and, for the dashboard, a valid API key).



