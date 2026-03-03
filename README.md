# IPL Data Analysis & Match Insights

## Project Overview

This project is an Exploratory Data Analysis (EDA) of Indian Premier League (IPL) cricket matches, utilizing a comprehensive dataset. The primary objective is to process historical match data and extract descriptive analytical insights regarding player performances, team scoring trends, and seasonal run accumulations. 

The analysis is conducted through a Jupyter Notebook environment, leveraging Python's core data science libraries to clean the data, perform match-level aggregations, and generate structured visualizations.

## Dataset Description

The analysis uses a granular ball-by-ball dataset containing delivery-level records of IPL matches spanning 18 seasons (from 2008 to the present).

*   **Size:** Approximately 278,200 rows and 64 columns.
*   **Granularity:** Each row represents a single legal or illegal delivery bowled in a match.
*   **Key Features:** Includes match identifiers, dates, batting and bowling team names, striker and non-striker names, bowler names, runs scored off the bat, extras, over and ball numbers, and dismissal events.

## Key Features of the Project

*   **Data Cleaning & Preprocessing:** Handles missing values and fixes data types across numeric and categorical features.
*   **Feature Engineering:** Extracts the IPL `season` (year) from raw match dates to allow for temporal analysis.
*   **Data Aggregation:** Utilizes `pandas` to group large-scale delivery data into concise match-level and season-level statistics.
*   **Player Performance Analysis:** Ranks individual players to identify the top historical run-scorers and top wicket-takers.
*   **Data Visualization:** Employs standard formatting and color palettes to plot trends and distributions.
*   **Defensive Programming:** Implements column-checking logic to ensure code continuity even if certain expected columns are absent in future dataset updates.

## Exploratory Analysis Performed

The notebook performs descriptive analytics to answer several historical questions about the IPL:
*   Total runs scored per season across the history of the league.
*   Identification of the top 10 highest run-scorers in IPL history.
*   Identification of the top 15 most successful bowlers based on career wickets.
*   Match volume analysis per season.

## Tech Stack

The project relies on the standard Python data science ecosystem:
*   **Python**
*   **Pandas** (Data manipulation and aggregation)
*   **NumPy** (Numerical operations)
*   **Matplotlib** (Static plotting)
*   **Seaborn** (Statistical data visualization)
*   **Jupyter Notebook** (Interactive development environment)

## Project Classification

This is an **Exploratory Data Analysis (EDA)** project focused exclusively on descriptive analytics. It aggregates past events to summarize "what happened." It currently does not employ machine learning algorithms to predict future events such as match winners or player scores.

## Future Improvements

To elevate this project from descriptive analytics to predictive machine learning, several enhancements can be implemented:
*   **Advanced Feature Engineering:** Calculate rolling averages, player strike rates, bowler economy rates, and venue-specific metrics.
*   **Predictive Modeling:** Build regression models (e.g., XGBoost, Random Forest) to predict first-innings totals based on the state of the game at the 10-over mark.
*   **Player Clustering:** Apply K-Means clustering on metrics like Strike Rate and Average to segment players into specific tactical archetypes (e.g., "Anchors", "Power-hitters").
*   **Interactive Dashboard:** Convert the static notebook visualizations into a dynamic web application using Streamlit or Dash.

## How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd IPL-Data-Analysis
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
   *Open `notebooks/ipl_analysis.ipynb` and execute the cells sequentially.*



