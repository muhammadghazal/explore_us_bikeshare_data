# Interactive Python CLI for U.S. Bikeshare Insights

This project is an interactive command-line application that allows users to explore and analyze U.S. bikeshare data. It enables filtering by city, month, and day, then computes key usage statistics such as the most frequent travel times, popular stations, trip duration metrics, and user demographics.

## Features

- **User Input Filters:** Prompts for city (Chicago, New York City, Washington), month, and day.
- **Data Loading & Preprocessing:** Reads data from CSV files, converts date columns to datetime, and extracts month, day, and hour.
- **Time Statistics:** Identifies the most common month, day, and hour of usage.
- **Station Statistics:** Finds the most frequent start and end stations and their combinations.
- **Trip Duration Analysis:** Computes total and average trip durations.
- **User Statistics:** Summarizes counts of user types, genders, and birth year insights.

## Installation

1. Ensure you have Python 3.x installed.
2. Install required libraries:
   ```bash
   pip install pandas numpy
   ```
3. Place the CSV data files (e.g., `chicago.csv`, `new_york_city.csv`, `washington.csv`) in the project directory or update the `CITY_DATA` paths as needed.

## Usage

Run the program from the command line:
```bash
python your_script_name.py
```
Follow on-screen prompts to select a city, month, and day for analysis. The application will display the calculated statistics and performance metrics.

## Project Structure

- **main() function:** Orchestrates the CLI workflow.
- **get_filters():** Gets user input with input validation.
- **load_data():** Loads and filters the data based on user choices.
- **time_stats(), station_stats(), trip_duration_stats(), user_stats():** Compute and display the relevant statistics.
