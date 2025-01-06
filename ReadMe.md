# Weather App

This Weather App allows users to get weather information for their current location or any city they search for. The app uses the Geolocation API to get the user's current location and fetches weather data from a weather API.

## Features

- Get weather information for the current location using Geolocation.
- Search for weather information by city name.
- Display weather details including temperature, sky condition, wind speed, humidity, and air quality.

## How to Use

### Getting Weather for Current Location

1. Open the app in your browser.
2. Click the "Locate Me" button.
3. The app will request permission to access your location.
4. If permission is granted, the app will display the weather information for your current location.

### Searching for Weather by City Name

1. Enter the name of the city in the input field with the placeholder "Enter city name".
2. Click the "Search" button.
3. The app will display the weather information for the entered city.

### Storing and Displaying Searched Cities

- The app stores all the city names entered in the search field using local storage.
- The list of previously searched cities is displayed in the console on page load.

## Code Overview

### HTML

The main HTML structure includes:
- An input field for entering the city name (`<input id="searchcity">`).
- A button for searching by city name (`<button id="search">Search</button>`).
- A button for getting the current location (`<button id="locateme">Locate Me</button>`).
- Elements to display weather information (`<div id="tempc">`, `<div id="sky">`, etc.).

### JavaScript

The main JavaScript functions include:
- `getlocation()`: Gets the user's current location using the Geolocation API.
- `success(position)`: Fetches and displays weather information for the given coordinates.
- `failed(error)`: Handles errors when getting the user's location.
- Event listeners for the "Locate Me" and "Search" buttons.
- Logic to store and retrieve city names from local storage.