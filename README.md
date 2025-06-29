# Task-Management-Tool

This is a web-based Task Management Tool designed to help users organize their tasks efficiently, with an integrated weather planning feature to aid in scheduling outdoor activities based on real-time weather conditions and forecasts.

## Features

### Core Task Management
* **Add New Tasks:** Users can input a task title, optional deadline (date picker), and priority (Low, Medium, High) to add new tasks. Tasks can also be added by pressing "Enter" in the input field.
* **Mark Tasks as Completed:** Each task includes a checkbox to toggle its completion status. Completed tasks are visually distinguished with strikethrough text and a lighter background.
* **Filter Tasks:** Users can filter the task list by status: "All" (shows all tasks), "Active" (shows incomplete tasks), and "Completed" (shows completed tasks).
* **Sort Tasks:** Tasks can be sorted dynamically by:
    * **Added Date:** Default sorting, displaying newest tasks first.
    * **Deadline:** Tasks with earlier deadlines appear first (tasks without deadlines are at the end).
    * **Priority:** High priority tasks are listed first, followed by Medium, then Low.
* **Local Storage Persistence:** All tasks, including their status, deadline, and priority, are automatically saved to and loaded from the browser's local storage, ensuring data persists across browser sessions.
* **Dynamic Task Rendering:** The task list updates dynamically based on additions, completion status changes, and filter/sort selections.
* **"No Tasks" Message:** A user-friendly message appears when no tasks are present under the currently selected filter.

### Weather-Based Task Planning
* **Location Input:** An interactive front-end allows users to input a city name (e.g., "Secunderabad, IN") and retrieve weather information.
* **Current Weather Display:** Shows current temperature, conditions, humidity, wind speed, sunrise, and sunset times for the specified location.
* **24-Hour Forecast:** Displays a simplified 24-hour forecast in 3-hour intervals, including temperature, conditions, and weather icons.
* **Weather-Based Task Suggestions:** Provides suggestions for optimal times for outdoor tasks (e.g., moderate temperature, clear/mild weather, low wind) based on the 48-hour forecast.
* **Weather Alerts:** Flags and displays alerts for potentially disruptive weather conditions within the next 24 hours, such as heavy rain, thunderstorms, snow, strong winds, or extreme temperatures.

## Technologies Used

* **Frontend:**
    * HTML5
    * CSS3 (with Tailwind CSS framework)
    * JavaScript
* **Libraries:**
    * [Tailwind CSS](https://tailwindcss.com/) (for rapid UI development)
    * [Axios](https://axios-http.com/) (for making HTTP requests to the OpenWeatherMap API)
    * [Google Fonts - Inter](https://fonts.google.com/specimen/Inter)
* **API:**
    * [OpenWeatherMap API](https://openweathermap.org/api) (for weather data)

## Setup Instructions

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Samuel27-max/Task-Management-Tool.git](https://github.com/Samuel27-max/Task-Management-Tool.git)
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd Task-Management-Tool
    ```

3.  **Open `TaskMgmtTool.html`:**
    Simply open the `TaskMgmtTool.html` file in your preferred web browser.

4.  **OpenWeatherMap API Key:**
    * Obtain a free API key from [OpenWeatherMap](https://openweathermap.org/api).
    * Locate the line `const OPENWEATHER_API_KEY = "YOUR_OPENWEATHER_API_KEY";` in the `<script>` section of `TaskMgmtTool.html`.
    * Replace `"YOUR_OPENWEATHER_API_KEY"` with your actual API key.

    **Note:** For a production environment, it is highly recommended to proxy API calls through a backend server to secure your API key, rather than embedding it directly in client-side code.

## Live Demo

[Live Demo URL Here]()

## Example Screenshot Section

![Screenshot of Task Management Tool](https://github.com/Samuel27-max/Task-Mgmt-Tool/blob/5ff3cafd91335b67a4da57f1699aca8e9bf04342/preview.png)

---
