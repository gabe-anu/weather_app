# Weather App
Submitted by: **Gabriel Anurum-Anyanwu**

Live Demo: [weather_app](https://weather-app-sepia-xi-81.vercel.app/)

Weather app to run on **Vercel** with a **serverless function**.

## Overview

- Enter a city, get the weather.
- The OpenWeather API key is stored as a **Vercel environment variable**.
- A **serverless function** handles API requests, keeping the key secure.

This application utilizes a RESTful architecture both on the frontend and backend. When the user enters a city name and clicks "Search," a GET request is made to a custom API endpoint (/api/weather). This endpoint is implemented using a serverless function (in Next.js), which acts as a middleware between the frontend and the external OpenWeatherMap REST API.

The serverless function:

Receives the city name via query parameters (?city=London)

Sends a GET request to OpenWeatherMap’s Geocoding API to retrieve the latitude and longitude

Then sends another GET request to OpenWeatherMap’s Weather API using those coordinates

Finally returns the combined weather data back to the frontend in JSON format

On the frontend, the JavaScript code parses the JSON and dynamically updates the UI with weather details such as temperature, city name, and description. This architecture follows REST principles: stateless communication, use of HTTP methods (GET), resource-based URIs, and JSON-formatted responses.



## Changes from Codédex

- Serverless function for weather data requests.
- Secure API key storage via Vercel environment variables.
- Deployed to Vercel.

## Project Structure

- `index.html`: Main web interface.
- `script.js`: Handles the UI and fetch requests.
- `api/weather.js`: Serverless function for weather data.
