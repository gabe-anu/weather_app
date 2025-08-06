# Weather App
Submitted by: **Gabriel Anurum-Anyanwu**

Live Demo: [weather_app](https://weather-app-sepia-xi-81.vercel.app/)

Weather app to run on **Vercel** with a **serverless function**.

## Overview

- Enter a city, get the weather.
- The OpenWeather API key is stored as a **Vercel environment variable**.
- A **serverless function** handles API requests, keeping the key secure.

## Changes from Codédex

- Serverless function for weather data requests.
- Secure API key storage via Vercel environment variables.
- Deployed to Vercel.

## Project Structure

- `index.html`: Main web interface.
- `script.js`: Handles the UI and fetch requests.
- `api/weather.js`: Serverless function for weather data.
