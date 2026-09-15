# IPL Cricket Statistics Dashboard & Moneyball Predictor

## Project Overview

This project is an **IPL Cricket Statistics Dashboard and Machine Learning based Moneyball Predictor**.

The project analyzes historical IPL match and ball-by-ball data to understand player and team performance. It also uses machine learning to estimate how many runs a player may score in their next simulated match.

The project combines:

- IPL cricket data analysis
- Data cleaning and preprocessing
- Player and team performance analysis
- Feature engineering
- Player momentum analysis
- Regression-based machine learning
- Player run prediction
- Data visualization
- Power BI dashboard

### Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Microsoft Power BI

---

# Project Objectives

The project has two main objectives.

### IPL Statistics Analysis

Analyze IPL data to understand:

- Player batting performance
- Player bowling performance
- Runs and wickets
- Strike rate
- Recent player form
- Player momentum
- Opponent-specific performance
- Team performance
- Season performance

### Moneyball Predictor

Build a machine learning system that uses historical player performance and engineered features to predict the number of runs a player may score in their next simulated match.

---

# Dataset

The project uses IPL cricket data from **Cricsheet**.

The dataset contains match-level and ball-by-ball information that can be used to calculate player and team statistics.

## Data Source

**Cricsheet:**  
https://cricsheet.org/

**Downloads:**  
https://cricsheet.org/downloads/

**Dataset:** Indian Premier League match and ball-by-ball data

**Extraction Date:** September 2026

> Update the extraction date if the dataset was downloaded on a different date.

---

# Dataset Files

The project uses two main input datasets:

### `matches.csv`

Contains match-level information such as:

- Season
- Teams
- Match results
- Winning team
- Venue
- Match information

Used for team and season-level analysis.

### `deliveries.csv`

Contains ball-by-ball information such as:

- Batter
- Bowler
- Runs
- Wickets
- Balls faced
- Match information

Used for player statistics, feature engineering, and prediction.

---

# Project Structure

```text
Cricket_Analysis/
│
├── dataFiles/
│   ├── matches.csv
│   ├── deliveries.csv
│   ├── player_match.csv
│   └── player_predictions.csv
│
├── IPL_Moneyball_Dashboard_Jupyter.ipynb
├── Dashboard_IPL.pbix
│
├── IPL_trophy.png
├── ipl.png
├── Logo.png
│
├── requirements.txt
└── README.md

# Project Workflow
IPL Match & Ball-by-Ball Data
            ↓
      Data Cleaning
            ↓
    Player-Match Dataset
            ↓
    Statistical Analysis
            ↓
     Feature Engineering
            ↓
     Player Momentum
            ↓
   Next-Match Target Creation
            ↓
     Machine Learning
            ↓
       Prediction
            ↓
     CSV Data Export
            ↓
      Power BI Dashboard


## **Machine Learning Models:**

Three regression models are compared.

# 1. Linear Regression

Used as a baseline model to identify a simple relationship between player features and next-match runs.

# 2. Random Forest Regressor

Used to capture non-linear relationships between player performance features and predicted runs.

# 3. Gradient Boosting Regressor

Used to capture complex patterns by sequentially improving predictions.

After model comparison and feature engineering, Gradient Boosting Regressor is used as the final prediction model.

Model Evaluation

The regression models are evaluated using appropriate regression metrics.

The models are compared to determine which approach performs better for predicting next-match runs.

The project also performs feature importance analysis to identify which player-performance features contribute most to the prediction.

Player Prediction

The notebook includes a prediction function that uses the player's historical and engineered features to estimate their expected runs in the next simulated match.

Prediction results are exported as:

player_predictions.csv
Actual vs Predicted Analysis

The project includes an Actual vs Predicted Runs visualization.

It compares:

Actual Runs
     vs
Predicted Runs

A regression line is also included to visualize the relationship between actual and predicted values.

Feature Importance

Feature importance is analyzed to understand which variables have the greatest influence on the final prediction.

This helps determine the importance of factors such as:

Recent form
Player momentum
Historical runs
Strike rate
Previous performance
Opponent information
Power BI Dashboard

The project includes an interactive Power BI dashboard:

Dashboard_IPL.pbix

The dashboard uses the processed CSV files generated from the Python analysis.

Important data files include:

player_match.csv
player_predictions.csv

The dashboard allows users to interactively explore IPL statistics.

Dashboard Features

The dashboard includes analysis of:

Player Statistics
Total runs
Runs per match
Strike rate
Recent performance
Player rankings
Predicted runs
Wickets
Team Statistics
Matches played
Matches won
Win percentage
Team performance
Season performance
Season Analysis

Users can explore player and team performance across different IPL seasons.

Interactive Filters

The dashboard provides filters such as:

Season
Team
Player
Other available dashboard fields
Required Dashboard Visualizations

The dashboard includes the main required cricket statistics:

Runs Per Match

A time-series visualization showing changes in scoring performance over time.

Top 10 Run Scorers

Shows the players with the highest total runs.

Top 10 Wicket Takers

Shows the players with the highest number of wickets.

Team Win Percentage

Compares teams based on their percentage of matches won.

Win Percentage = (Matches Won / Matches Played) × 100
Moneyball Prediction

Shows player performance trends and machine learning-based predicted runs.

Moneyball Concept

The Moneyball approach focuses on using data and statistics to evaluate player performance.

Instead of considering only total runs, this project also considers:

Recent form
Historical performance
Strike rate
Player momentum
Opponent information
Machine learning predictions

The overall process is:

Historical IPL Data
        ↓
Player Statistics
        ↓
Feature Engineering
        ↓
Player Momentum
        ↓
Machine Learning
        ↓
Predicted Next-Match Runs
Output Files
player_match.csv

Contains processed player-match statistics.

Used for:

Player analysis
Statistical analysis
Power BI
player_predictions.csv

Contains machine learning prediction results.

Used for:

Predicted runs analysis
Player comparison
Power BI prediction visuals
Installation

Install the required Python packages using:

python -m pip install -r requirements.txt
How to Run
Step 1 - Clone or Download the Repository

Download the project from GitHub.

Step 2 - Install Dependencies
python -m pip install -r requirements.txt
