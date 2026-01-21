# MLB Wins Predictor & Team Stats Analysis

Python project that cleans and merges MLB team-season data, explores which batting stats relate to winning, and trains a Ridge Regression model to predict team wins.

## Goals
- Build an end-to-end data workflow (load → clean → merge → analyze → visualize → conclude)
- Identify which team stats are most associated with wins
- Train and evaluate a baseline model to predict wins

## What I Did
- Cleaned and prepared data (handled missing values, fixed data types, standardized team identifiers)
- Merged datasets using team + season keys and validated joins
- Engineered features (rates/percentages) and created summary tables (groupby/agg)
- Performed EDA using correlation checks and visualizations (scatter plots + heatmap)
- Trained a Ridge Regression model and evaluated performance with MAE/RMSE/R²
- Interpreted top coefficients to explain what metrics mattered most (and limitations)

## Results
Test-set performance:
- MAE: ~7.67 wins  
- RMSE: ~9.75 wins  
- R²: ~0.39

Key takeaway: The model captures real patterns from batting stats, but wins are also influenced by pitching, defense, injuries, schedule strength, and randomness.

## Tech Stack
Python, pandas, NumPy, scikit-learn, Matplotlib (Seaborn optional)

## How to Run
1. Open the notebook: `mlb_project.ipynb`
2. Install dependencies if needed:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn


