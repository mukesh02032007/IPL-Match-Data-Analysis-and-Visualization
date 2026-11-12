# IPL Match Data Analysis and Visualization

Exploratory data analysis (EDA) of Indian Premier League match and ball-by-ball data using Python. The project cleans the data, computes descriptive statistics, and builds visualizations to study scoring patterns, toss impact, venues, and season trends.

## Dataset

- Source: Kaggle, IPL Complete Dataset
- `matches.csv`: one row per match (teams, venue, toss, winner, result margin, season)
- `deliveries.csv`: ball-by-ball data (batter, runs, extras, etc.)

> The CSV files are not included in this repo. Download them from Kaggle and place them in the same folder as the notebook.

## What the project does

- Loads and inspects both datasets
- Handles duplicates and missing values (e.g. missing `city` filled with `Unknown`)
- Converts dates and explores matches, seasons, teams, and venues
- Computes descriptive statistics (mean, median, mode, variance, quartiles, IQR outliers)
- Builds visualizations:
  - Histogram: total runs per match
  - Bar charts: wins by team, top venues, top run scorers, Player of the Match awards
  - Pie chart: toss decisions (bat vs field)
  - Box plot: winning margins
  - Scatter plot: fours vs sixes
  - Line chart: total runs per season
  - Heatmap: correlation of total runs, fours, and sixes

## Key findings

- Most teams choose to field first after winning the toss.
- Winning the toss gives only a small edge in winning the match.
- Sixes and fours both correlate positively with total match runs.
- Total runs per season trend upward in recent seasons.

## Tech stack

Python 3, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## How to run

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook IPL_Analysis.ipynb
```

## Repository contents

```
├── IPL_Analysis.ipynb                        # Full analysis code
├── IPL_Match_Data_Analysis_Mini_Project.pdf  # Lab record / report
└── README.md
```

## SDG mapping

SDG 9: Industry, Innovation and Infrastructure (data-driven decision making in sports).

## Author

Mukesh P, B.Tech Artificial Intelligence and Data Science, Rajalakshmi Institute of Technology (Anna University)
