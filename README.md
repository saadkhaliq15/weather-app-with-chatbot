# Weather and Chat Bot Website

This project is a dynamic weather and chat bot web application that uses the **OpenWeather API** for current weather and forecast data, and the **Google Gemini API** for natural language chat responses. It allows users to search for the weather conditions of any city and also interact with a chatbot that handles general queries.

## Features

- **Weather Data:**
  - Fetch current weather conditions (temperature, weather description) and display them dynamically.
  - Fetch and display a 5-day weather forecast for a city, presented in a table with pagination for easy navigation.
  - Real-time background color changes based on weather conditions (e.g., sunny, rainy, cloudy).
  - Responsive charts (bar, line, doughnut) that visualize temperature trends and weather conditions using the Chart.js library.
  - **Filtering and Sorting Features**:
    - **Sort Temperatures Ascending**: Sort the displayed temperatures in ascending order.
    - **Sort Temperatures Descending**: Sort the displayed temperatures in descending order.
    - **Filter Rainy Days**: Display only the days with rain in the forecast.
    - **Show Day with Highest Temperature**: Display the day with the highest temperature from the forecast.
    - These features maintain pagination, allowing users to navigate through filtered or sorted results seamlessly.

- **Chat Bot:**
  - Handles weather-related and general queries.
  - If the user asks for weather or forecast, it will automatically fetch the relevant data for the provided city.
  - For non-weather-related questions, the bot uses the **Google Gemini API** to generate responses.

## Prerequisites

To run this project locally, you will need:

- A text editor or IDE (such as VSCode).
- A modern web browser (Google Chrome, Firefox, Edge, etc.).
- A local development server (optional, but can be used for better experience, such as **Live Server** in VSCode).

## API Keys

Before running the project, make sure to add your API keys for the OpenWeather API and Gemini API in the script.

- **OpenWeather API Key**: You can get it from [OpenWeatherMap](https://openweathermap.org/).
- **Gemini API Key**: Obtain the API key from [Google Cloud](https://ai.google.dev/aistudio).

You will need to insert your keys in the appropriate place in the JavaScript file:

```js
const apiKey = 'YOUR_OPENWEATHER_API_KEY';
const geminiApiKey = 'YOUR_GOOGLE_GEMINI_API_KEY';
```

## How to Run Locally

Follow these steps to run the project on your local machine:

1. **Clone or download the project**:
   ```bash
   git clone https://github.com/saadkhaliq15/weather-app-with-chatbot.git
   cd weather-app-with-chatbot
   ```

2. **Insert API Keys**:
   Open JavaScript files and replace the placeholders with your **OpenWeather API** and **Gemini API** keys.

   ```js
   const apiKey = 'YOUR_OPENWEATHER_API_KEY';
   const geminiApiKey = 'YOUR_GOOGLE_GEMINI_API_KEY';
   ```

3. **Open the project**:
   You can open the `index.html` file in your browser by double-clicking it. Alternatively, you can use a live server (such as the **Live Server** extension in VSCode) for auto-refresh during development.

4. **Search for Weather**:
   - Enter a city name in the search bar and click the "Search" button, or press Enter.
   - The current weather and 5-day forecast will be displayed, along with visualizations.

5. **Chat with the Bot**:
   - Enter a question or message in the chat input box and click "Send", or press Enter.
   - The bot will reply with weather-related info if the message contains terms like "weather" or "forecast," or it will use the **Gemini API** to respond to general questions.

6. **Use Filtering and Sorting Features**:
   - You can sort the forecast temperatures in ascending or descending order.
   - Filter the forecast to display only rainy days.
   - Show the day with the highest temperature.
   - Pagination will remain intact when using these features.

## Project Structure

```bash
weather-chat-bot/
├── index.html           # Main HTML file
├── chatbot.html         # Chatbot HTML file
├── weather-dashboard.js  # JavaScript logic for main dashboard
├── weather-chatbot.js    # JavaScript logic for chatbot and weather forecast table
├── README.md            # Project documentation (this file)
└── assets/              # Static assets (images, icons, etc.)
```

## Dependencies

- **Chart.js**: Used for rendering interactive charts.
- **Fetch API**: Native JavaScript API for making HTTP requests to the OpenWeather and Gemini APIs.
- **Google Gemini API**: For natural language processing in chatbot responses.

## Future Improvements

- Add more robust error handling.
- Implement a more advanced chat conversation history feature.
- Add more interactive chart features and animations.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
