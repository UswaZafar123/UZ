                                                    README
SkyCast Weather Application:
SkyCast is a weather application that provides real-time weather updates and forecasts using the OpenWeather API. The application displays weather information based on the user's current location or a city input. Users can view temperature data, weather conditions, and additional information such as humidity and wind speed. The app also includes sorting and filtering capabilities for the forecast data, and a chatbot feature for querying weather information.
1.Features
•	Fetch and display real-time weather data based on the user's input (city or latitude/longitude).
•	Geolocation support: Automatically fetches weather data based on the user’s current location if no input is provided.
•	Displays weather conditions using images for a visual experience (e.g., clear sky, clouds, rain, haze, etc.).
•	Toggle between Celsius and Fahrenheit temperature units.
•	Displays a weather forecast for the next 5 days, which can be sorted or filtered (e.g., by temperature, weather condition).
•	Interactive charts (bar, doughnut, and line) to visualize temperature data and weather counts.
•	Chatbot support using the Gemini API, which responds to user queries about the weather and other topics.
2.Technologies Used
•	HTML, CSS, and JavaScript: Front-end technologies for building the user interface.
•	Bootstrap: For responsive design and layout.
•	OpenWeather API: To fetch real-time weather data and forecasts.
•	Chart.js: For rendering interactive charts to visualize weather data.
•	Gemini API: To provide chatbot responses based on user queries.
3. Run the Application Locally
•	You can open the index.html file directly in your browser to run the app. Alternatively, you can use a local server (e.g., with VSCode Live Server or Node.js) to host it:
o	Using VSCode Live Server:
	Open the project folder in VSCode.
	Right-click weatherapp.html and select Open with Live Server.


4. Using the Application
The SkyCast Weather Application provides an interactive way for users to explore and view weather information. Below is a detailed guide on how to use the various features:
4.1 Enter a City Name or Latitude and Longitude for Weather Data
•	In the input fields located at the top of the page, you have the following options:
o	City Name: Enter the name of the city for which you want to check the weather (e.g., "New York", "London"). The application will fetch and display the current weather information for the city you input.
o	Latitude and Longitude: If you prefer to be more precise, you can enter the latitude and longitude coordinates of a location. For example:
	Latitude: 40.7128
	Longitude: -74.0060 This will fetch the weather data for the exact location specified by these coordinates.
o	Fetch Weather Button: Once you have entered either the city name or coordinates, click the "Get Weather Update" button. The application will fetch and display the weather data in the weather widget below.
•	Note: You can enter either the city name or coordinates. If both are provided, the application will prioritize the coordinates.
4.2 Automatic Location Detection (Geolocation Support)
•	If no city name or coordinates are entered, the application will automatically attempt to use your device’s location to provide weather information for your current location. This feature uses the browser's Geolocation API to detect your location.
•	Permission Prompt: When you open the app, you may receive a prompt requesting permission to access your location. You must allow access for this feature to work.
o	Accept the Permission: If you accept, the app will retrieve your latitude and longitude and fetch the weather data for your current location.
o	Deny the Permission: If you deny access, the application will not be able to fetch your location automatically. You will need to manually enter a city name or coordinates to retrieve weather data.
4.3 Viewing the Weather Information
•	The weather information is displayed in a widget that includes:
o	The name of the city or location.
o	A description of the weather (e.g., "clear sky", "rain", "haze").
o	The temperature in either Celsius or Fahrenheit (toggle available—see below).
o	Humidity percentage.
o	Wind speed (in meters per second or miles per hour, depending on the temperature unit).
•	A weather icon corresponding to the weather condition is also displayed for easy visualization.
4.4 Toggling Temperature Units (Celsius / Fahrenheit)
•	Below the weather information, you will see a button labeled "Toggle to Fahrenheit" or "Toggle to Celsius".
•	Click the button to switch the temperature unit between Celsius and Fahrenheit. The weather data will be refreshed in the chosen unit.
•	The application will dynamically update the displayed temperature and wind speed values based on your selection.
4.5 Viewing and Sorting the 5-Day Weather Forecast
•	The application displays a 5-day weather forecast, showing the temperature and weather conditions for each time interval (typically every 3 hours) over the next 5 days.
•	This data is displayed in the Tables section:
o	You can navigate between pages if the forecast data exceeds 10 entries per page using the pagination controls at the bottom of the table.
o	Each row shows the date/time, temperature, and weather condition for that time slot.
•	Sorting and Filtering Forecast Data:
o	There is a dropdown menu located above the table where you can select various options to sort or filter the data:
	Ascending Temperature: Sorts the forecast data from the lowest to the highest temperature.
	Descending Temperature: Sorts the forecast data from the highest to the lowest temperature.
	Rainy Days Only: Filters and shows only the forecast entries where rain is predicted.
	Hottest Temperature: Highlights the day or time interval with the highest temperature forecasted over the next 5 days.
o	Select any option from the dropdown menu to apply the sort or filter. The table will update automatically based on your selection.
4.6 Visualizing Weather Data with Charts
•	The application uses Chart.js to render interactive charts that visually represent the weather data:
o	Bar Chart: Displays temperatures over the next 5 intervals (typically within a day). This shows the temperature variation in bar format.
o	Doughnut Chart: Visualizes the proportion of weather conditions (e.g., rain, clouds, clear skies) over the forecast period. The chart dynamically shows the percentage each weather condition occupies.
o	Line Chart: Shows the temperature trend for the next 5 intervals in a line format, allowing you to observe changes over time.
•	These charts are located in the Dashboard section and update automatically when you fetch new weather data.
4.7 Chatbot Feature
•	The SkyCast application includes a chatbot powered by the Gemini API, which responds to user queries:
o	Querying Weather Information:
	In the chat input field, you can type a question such as "What is the weather in Paris?" or "Show me the weather in New York".
	The chatbot will respond with the current weather information for the location specified, including the description and temperature.
o	Interacting with the Chatbot:
	The chatbot can only respond to weather-related queries at this time. If you ask something unrelated to weather (e.g., "Tell me a joke"), it will inform you that it can only respond to weather questions.
o	Enter Key: Press the Enter key to send your query. The chatbot's response will appear below the input field.
By following these instructions, you will be able to explore all the features and functionality of SkyCast. The app is designed to be intuitive, and you can experiment with different inputs and filters to see how the information updates dynamically.
