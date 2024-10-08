# Fitness-plan-generator

## Overview
The Dynamic Fitness Plan Generator is designed to create personalized workout plans using real-time data from wearable devices such as Fitbit. It dynamically adjusts the user's workout routine based on their performance data, such as steps taken, calories burned, sleep patterns, and nutrition intake. The system leverages Fitbit's API for retrieving fitness data and Google Generative AI for generating customized workout plans based on user goals, preferences, and available data.

## Features
- **Wearable Device Integration**: Fetch real-time fitness data (steps, calories burned, sleep duration) via the Fitbit API.
- **Dynamic Workout Plan Generation**: Google Generative AI generates workout routines tailored to user fitness data and goals.
- **Customizable Plans**: Users can specify their goals (e.g., weight loss, muscle gain), workout preferences, available equipment, and dietary preferences.
- **PDF Export**: Automatically generates a downloadable PDF of the workout plan.

## Files overview
- fitbit_data_check.py : this script is responsible for verfiying and validating data recieved from fitbit API
- relevant_data_fetch.py : this scrip handles the fetching relevant real-time user fitbit data that is required for the task
- workout_generator.py : the cofe file that generated personalized workout plans using Gen AI
- Documentation.pdf : this file contains the overview, functionality, workflow and tech stack of the task. It also explains the challenges and assumptions taken.
- working video.mp4 : a demonstration of the working code and the generated output


## Prerequisites
- Python 3.12.5
- Fitbit account with access token
- Google Generative AI API key

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sirisujala30/fitness-plan-generator.git
```

## Configuration
1. Replace your Fitbit API token in the code:
```python
TOKEN = "your_fitbit_api_token"
```

2. Set up your Google Generative AI API key:
```python
os.environ["API_KEY"] = "your_google_api_key"
```

## Usage
```bash
streamlit run workout_generator.py
```
