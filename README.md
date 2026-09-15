# IPL Cricket Statistics Dashboard – Moneyball Predictor

## Project Overview

This project is an IPL Cricket Statistics Dashboard combined with a Machine Learning based "Moneyball" predictor.

The project analyzes IPL match and ball-by-ball data to understand player and team performance. It also uses machine learning to estimate how many runs a player may score in their next simulated match.

The project contains two main parts:

1. IPL Cricket Statistics Dashboard
2. Machine Learning based Player Run Prediction

The analysis is performed using Python and Jupyter Notebook, while the final dashboard is created using Microsoft Power BI.

---

## Project Objectives

The main objectives of this project are:

- Analyze IPL cricket match data.
- Analyze player batting and bowling performance.
- Calculate player statistics such as runs and strike rate.
- Analyze team performance.
- Calculate player momentum using recent performance.
- Predict a player's runs in their next simulated match.
- Compare different regression models.
- Export processed data for Power BI.
- Build an interactive cricket statistics dashboard.
- Provide useful insights from IPL historical data.

---

## Dataset

The project uses IPL match and ball-by-ball cricket data from Cricsheet.

### Data Source

Cricsheet provides structured cricket match data, including ball-by-ball information and match-level information.

Source:

Cricsheet

The data source provides match information and detailed delivery-level information that can be used for player, team, batting, bowling, and match analysis.

---

## Dataset Files

The project uses two main input files:

### matches.csv

This file contains match-level information.

Examples of information include:

- Match ID
- Season
- Date
- Teams
- Venue
- Match result
- Winning team
- Other match-level information

### deliveries.csv

This file contains ball-by-ball information.

Examples of information include:

- Match ID
- Innings
- Batting team
- Bowling team
- Batter
- Bowler
- Runs scored
- Extra runs
- Total runs
- Wickets
- Delivery information

The match-level and delivery-level datasets are combined during the analysis to create player and match statistics.

---

## Project Structure

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
│
├── Dashboard_IPL.pbix
│
├── IPL_trophy.png
├── ipl.png
├── Logo.png
│
├── requirements.txt
│
└── README.md
