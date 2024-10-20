# Zeotap-application-2

This project is a **Real-Time Weather Monitoring System** that retrieves weather data from the OpenWeatherMap API for multiple cities. The system processes the data in real-time, performs rollups and aggregates (e.g., average temperature), and can trigger alerts based on user-defined thresholds for weather conditions.

### Features:
- **Real-Time Data Fetching**: Fetch weather data (temperature, humidity, wind speed, etc.) for multiple cities in real-time.
- **Weather Aggregation**: Perform rollups/aggregates such as average, minimum, and maximum temperatures, dominant weather conditions.
- **Alert System**: Trigger alerts when user-defined thresholds (e.g., temperature > 35°C) are breached.
- **Weather Visualization**: Display visualizations of weather trends using graphical charts.
  
### Technologies Used:
- **Backend**: Python (with SQLAlchemy for database management)
- **Database**: MySQL or any SQL-based database supported by SQLAlchemy
- **API**: OpenWeatherMap API for fetching real-time weather data
- **Visualization**: Matplotlib (or other Python plotting libraries)

### File Structure:
- **code.ipynb**: Main Python file for running the weather monitoring application, handling API calls, data processing, and alert management.
- **weather_data.sql**: SQL file for setting up the MySQL database to store weather data for each city.
- **weather_map.html**: A simple HTML file for demo purposes, showing output examples and visualizations.

### Installation:
1. Clone this repository.
2. Set up the MySQL database using the `weather_db.sql` file.
3. Install the necessary Python dependencies (see `requirements.txt`).
4. Modify `config.py` to add your OpenWeatherMap API key and database connection settings.
5. Run `app.py` to start fetching and processing weather data.

### How to Use:
1. Set up API access by adding your OpenWeatherMap API key in `config.py`.
2. Run the application (`app.py`) to start fetching weather data at configurable intervals.
3. Review real-time weather data, including average, minimum, and maximum temperatures, humidity, and wind speed.
4. Set threshold alerts in `config.py` (e.g., temperature > 35°C for consecutive updates) and monitor the console or email for alerts.

### Key Achievements:
- Successfully retrieved real-time weather data for six major cities (Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad).
- Implemented daily summaries of weather data, including average temperature calculation (30.85°C), humidity, and wind speed.
- Configured an alert system for extreme conditions, such as temperature exceeding thresholds, with successful alerts triggered during testing.
