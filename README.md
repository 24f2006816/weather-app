# Readiness Route Tester

This project provides a simple, single-page web application designed to test a `POST` readiness endpoint. It's ideal for quickly verifying the operational status of a service or component that exposes a `/readiness` or similar endpoint expecting a POST request.

## Features

*   **Single File:** All HTML, CSS (Tailwind CSS), and JavaScript are contained within `index.html` for easy deployment and sharing.
*   **Customizable URL:** Easily change the target readiness endpoint URL directly within the UI.
*   **POST Request:** Explicitly sends a `POST` request, simulating a common readiness probe or health check pattern.
*   **Real-time Feedback:** Displays the request status (loading, success, error) and the raw response from the server.
*   **Responsive Design:** Built with Tailwind CSS for a mobile-first, responsive user interface.

## Getting Started

To use this readiness tester, simply follow these steps:

1.  **Clone the repository** (or copy the `index.html` content).
2.  **Open `index.html`** in your web browser.
3.  (Optional) **Adjust the 'Readiness Endpoint URL'** input field if your endpoint is different from `/readiness`.
4.  **Click the "Test POST /readiness" button.**
5.  **Observe the Status Message and Response Display** sections for the outcome of your request.

## Technical Details

*   **HTML5:** Semantic markup for the application structure.
*   **Tailwind CSS:** Used via CDN for rapid and efficient styling, ensuring a clean and responsive UI.
*   **JavaScript (ES6+):** Utilizes the `fetch` API to perform asynchronous `POST` requests and handles DOM manipulation for displaying results.
    *   The POST request sends a basic JSON body `{"timestamp": "...", "message": "Readiness probe"}` with a `Content-Type: application/json` header.
    *   It attempts to parse the response as JSON; if that fails, it displays the raw text.

## Development

No build step is required for this project. Simply edit the `index.html` file directly.

## License

This project is open-sourced under the MIT License. See the `LICENSE` file for more details.