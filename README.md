# Simple Weather App

This is a minimalist web application that fetches and displays the current temperature and humidity for the user's current location. It leverages the browser's Geolocation API to determine the user's coordinates and then uses the OpenWeatherMap API to retrieve weather information.

## Features

*   **Geolocation-Based Weather**: Automatically detects your location to provide relevant weather data.
*   **Current Temperature**: Displays the current temperature in Celsius.
*   **Current Humidity**: Shows the current humidity percentage.
*   **Responsive Design**: Built with Tailwind CSS for a seamless experience across various devices.
*   **Error Handling**: Provides user-friendly messages for geolocation denials, API errors, and unsupported browsers.

## Technologies Used

*   **HTML5**: For the basic structure of the web page.
*   **Tailwind CSS**: A utility-first CSS framework for rapid and responsive UI development.
*   **JavaScript**: For handling geolocation, API calls, and dynamic content updates.
*   **Geolocation API**: Browser API to get the user's current geographical position.
*   **OpenWeatherMap API**: A third-party service used to fetch weather data based on latitude and longitude.

## Setup and Installation

To get this project up and running, follow these simple steps:

1.  **Clone the Repository (or download `index.html`):**

    If this project were in a repository, you would clone it:
    ```bash
    git clone <repository-url>
    cd simple-weather-app
    ```
    For this standalone `index.html` file, simply save the provided HTML content into a file named `index.html` on your local machine.

2.  **Obtain an OpenWeatherMap API Key:**

    *   Go to [OpenWeatherMap](https://openweathermap.org/api).
    *   Sign up for a free account.
    *   Once logged in, navigate to your API keys section and generate a new API key.

3.  **Configure the API Key:**

    *   Open the `index.html` file in a text editor.
    *   Locate the JavaScript section (within the `<script>` tags).
    *   Find the line `const API_KEY = 'YOUR_OPENWEATHERMAP_API_KEY';`.
    *   Replace `'YOUR_OPENWEATHERMAP_API_KEY'` with your actual API key obtained from OpenWeatherMap.

    _Note: It can take a few minutes for a newly generated API key to become active._

4.  **Open in Browser:**

    *   Simply open the `index.html` file in your preferred web browser.
    *   Your browser will likely prompt you to allow location access. Grant permission for the app to function correctly.

## Usage

Upon opening the `index.html` file in your browser, the application will:

1.  Request permission to access your current location.
2.  If permission is granted, it will use your latitude and longitude to make a request to the OpenWeatherMap API.
3.  Once the data is received, it will display the current temperature (in Celsius) and humidity for your area.
4.  If location access is denied or if there's an issue fetching data, an appropriate error message will be shown.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.