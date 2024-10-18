# Zeotap-application-2

# Real-Time Weather Monitoring System

## Overview

The Real-Time Weather Monitoring System fetches and stores weather data for major cities in India. It uses the OpenWeatherMap API to retrieve real-time weather information, calculates daily summaries, and triggers alerts based on temperature thresholds.

## Features

- **Real-Time Weather Data**: Fetches current temperature, humidity, weather conditions, and more for the following cities:
  - Delhi
  - Mumbai
  - Chennai
  - Bangalore
  - Kolkata
  - Hyderabad
- **Daily Weather Summary**: Calculates average, maximum, and minimum temperatures for each city at the end of the day.
- **Weather Alerts**: Triggers alerts when the temperature exceeds a specified threshold (default is 35°C).
- **SQLite Database**: Stores weather summaries in a local SQLite database.

## Requirements

- Python 3.x
- `requests` library
- `SQLAlchemy` library

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/weather-monitoring-system.git
   cd weather-monitoring-system
