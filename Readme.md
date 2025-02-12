# AgriSpeech: Agriculture Optimization App

## Overview
AgriSpeech is a Streamlit-based application designed to assist farmers by providing real-time weather-based optimization techniques. It collects input from farmers, fetches real-time weather data, and offers suggestions for improving agricultural practices.

## Features
- **Multi-language support** for farmer interactions.
- **Speech synthesis** for optimization recommendations.
- **Weather API integration** for real-time weather data.
- **Smart agricultural suggestions** based on weather conditions and farmer inputs.

## Dependencies
The application requires the following Python libraries:
```bash
pip install streamlit requests speechrecognition pyttsx3
```

## How It Works
1. **Farmer Input:**
   - The farmer enters their location, crops grown, years of experience, soil type, and farm size.
2. **Weather Fetching:**
   - The app fetches real-time weather data from WeatherAPI.
3. **Optimization Suggestions:**
   - The app provides customized suggestions based on the weather and farming parameters.
4. **Text-to-Speech Output:**
   - Optimization messages are converted to speech using `pyttsx3`.

## Configuration
- The application fetches weather data using an API key:
  ```python
  weather_api_key = "your_weather_api_key_here"
  ```
  Replace this key with a valid API key from [WeatherAPI](https://www.weatherapi.com/).

## Running the Application
Run the following command in your terminal:
```bash
streamlit run agrispeech.py
```

## Functions
### `take_farmer_input(language)`
Collects input from the farmer, including location, crop details, and farming experience.

### `fetch_realtime_weather(location)`
Fetches real-time weather data using the WeatherAPI.

### `generate_optimization_techniques(farmer_input, weather_data, language)`
Generates customized farming recommendations based on weather conditions and farming parameters.

### `get_welcome_message(language)`
Returns a welcome message in the selected language.

### `text_to_speech(text, language)`
Converts the given text into speech using `pyttsx3`.

## Supported Languages
- English
- Hindi
- Tamil
- Telugu
- Marathi
- Bengali
- Gujarati
- Kannada
- Malayalam
