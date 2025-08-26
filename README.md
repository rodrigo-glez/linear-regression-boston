# Boston Housing Linear Regression Practice

This short project explores the Boston Housing dataset with the goal of applying simple and multiple linear regression models. It emphasizes strong linear relationships between variables and uses exploratory analysis to support modeling decisions.

## Project Goals

- Practice setting up a virtual environment for project isolation.
- Gain experience with loading and exploring a real-world dataset.
- Perform exploratory data analysis (EDA) and correlation analysis.
- Practice simple and multiple linear regression using statsmodels.
- Generate and interpret regression summary reports.
- Visualize model performance (e.g., actual vs. predicted values).

## Dataset

- Source: Scikit-learn's Boston Housing dataset (CSV version)
- Shape: 506 rows × 14 columns
- Target variable: medv (Median value of owner-occupied homes in $1000's)

## Steps

### 1. Environment Setup
- Created and activated a virtual environment using venv
- Installed necessary libraries:
pandas, matplotlib, seaborn, statsmodels, scikit-learn, ipykernel
- Created a requirements.txt file

### 2. Data Exploration
- Loaded dataset into a pandas DataFrame
- Confirmed no missing values using df.info()
- Generated correlation matrix and focused on variables most correlated with medv

### 3. Visualizations
- Heatmap of correlations (full and focused on medv)
- Scatter plots of medv vs:
rm (avg. rooms per dwelling),
lstat (% lower status population),
ptratio (pupil-teacher ratio),

### 4. Simple Linear Regression
- Target: medv
- Predictor: lstat
- Model: sm.OLS()
- R-squared: ~0.54

### 5. Multiple Linear Regression
- Predictors: lstat, rm, ptratio
- R-squared: ~0.68
- All predictors were statistically significant
- Model captured more variation than the simple model

### 6. Model Evaluation
- Plotted Actual vs. Predicted values for visual comparison
- Included a diagonal reference line to assess accuracy

## Disclaimer

This project was created as part of my personal learning journey. It’s a practice project, built from scratch on my own initiative. The goal is to experiment, try out ideas, and improve my skills.

Because of that, it may not have a clear practical use case, and some parts might be rough around the edges or not follow best practices yet. I’m sharing it here openly as a way to document my progress and keep learning.
