# Titanic Visual Story

Exploratory Data Analysis (EDA) of the Titanic dataset to understand the factors that influenced passenger survival using Python, pandas, Matplotlib, and Seaborn.

## What I Did

- Loaded and explored the Titanic dataset.
- Cleaned missing values in the Age and Embarked columns.
- Removed the Cabin column due to excessive missing values.
- Created six publication-quality visualizations.
- Added a one-line takeaway below each chart.
- Summarized the findings in a 200-word conclusion.

## Charts Included

1. Age Distribution
2. Fare Distribution (Boxplot)
3. Passenger Survival Count
4. Survival by Gender
5. Survival by Passenger Class
6. Correlation Heatmap

## Key Findings

- Most passengers were between 20 and 40 years old.
- Female passengers had a much higher survival rate than male passengers.
- First-class passengers survived more often than passengers in lower classes.
- Ticket fares contained several high-value outliers.
- Passenger class and fare showed a relationship with survival.

## How to Run

1. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

2. Open Jupyter Notebook:

```bash
jupyter notebook visual_story.ipynb
```

3. Ensure `Titanic-Dataset.csv` is in the same folder as the notebook.

## Dataset

- Titanic Dataset (`Titanic-Dataset.csv`)

## Tech Stack

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
