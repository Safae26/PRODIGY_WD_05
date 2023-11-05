# PRODIGY_WD_05
# Weather App

This is a simple weather app that allows you to check the current weather for a specific city. To use this app, you need to obtain an API key from the OpenWeather website.

## Getting an OpenWeather API Key

Before you can use this app, you will need to get an API key (appid) from OpenWeather. Follow these steps to obtain your API key:

1. Visit the OpenWeather website: [https://openweathermap.org/](https://openweathermap.org/)

2. Sign up for a free or paid account and log in.

3. Once you are logged in, go to your account dashboard and look for the section where you can generate an API key.

4. Generate an API key (appid). Make sure to keep it secure as it will be used in the application code.

## Using the API Key in the Application

After obtaining your OpenWeather API key, you will need to use it in the application code. Open the `script.js` file and find the following lines of code:

```javascript
// Our API URL
const apiUrl = "https://api.openweathermap.org/data/2.5/weather?&units=metric&q=";

// Define your API key
const apiKey = "YOUR_OPENWEATHER_API_KEY"; // Insert your API key here

async function checkWeather(city) {
  const response = await fetch(apiUrl + city + '&appid=${apiKey}');
  // ...
}
```
And finally replace "YOUR_OPENWEATHER_API_KEY" in the apiKey variable with your apiKey value.
