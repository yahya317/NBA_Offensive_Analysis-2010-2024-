# The Rise of NBA Offense (2010–2024)

This project analyzes the evolution of offensive scoring trends in the NBA from the 2010 to 2024 seasons. By isolating specific shooting and scoring features, the analysis investigates how modern basketball has shifted, focusing heavily on the **3-Point Revolution Era**.

## Data Source

The data is driven by `regular_season_totals_2010_2024.csv`, sourced from the [`NBA-Data-2010-2024`](https://github.com/NocturneBear/NBA-Data-2010-2024) public GitHub repository maintained by NocturneBear.

The dataset aggregates statistics from public NBA sources into a structured CSV format, updated bi-annually to allow analysis of player performance, team statistics, and game trends.

## Repository Structure

```text
├── data/
│   └── regular_season_totals_2010_2024.csv
│
├── notebooks/
│   ├── 01_Establish_Data.ipynb
│   ├── 02_Exploring_Data.ipynb
│   └── 03_Final_Product.ipynb
│
├── images/
│   └── Exported visualization assets
│
└── README.md

## Methodology

The analysis isolates the following key metrics to track the evolution of NBA offenses:

- `SEASON_START` / `SEASON_YEAR`
- `PTS` (Total points scored)
- `FG3A` & `FG3M` (Three-point field goals attempted and made)
- `FG3_PCT` & `FG_PCT` (Three-point percentage and field goal percentage)

To maintain data integrity, records with missing values in non-relevant columns (like `AVAILABLE_FLAG`) were left untouched, and the primary timeframe was formatted to aggregate by the starting year of the season.

## Dependencies

The codebase requires a standard Python data science stack:

- `pandas`
- `matplotlib`
- `seaborn`

## Project Goal

The goal of this project is to use historical NBA data to explore how offensive basketball has evolved between 2010 and 2024, with particular attention to the growth of three-point shooting and changes in overall scoring and shooting efficiency.
