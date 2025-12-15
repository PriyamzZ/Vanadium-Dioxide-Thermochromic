# ML-Based Optimization of VO₂ Thin Film Deposition

This project explores the use of ML models to analyze and optimize
magnetron sputtering parameters for fabricating high-purity monoclinic VO₂ (VO₂(M))
thermochromic thin films.

## Dataset
The dataset contains experimental sputtering parameters and includes:
- Power applied to the target (W)
- Substrate temperature (°C)
- O₂/Ar ratio
- Chamber pressure (Pa)
- Target material
- Substrate material

The target variable indicates whether the resulting film is pure-phase VO₂(M).

## Methods
- Exploratory data analysis (histograms, boxplots, correlations)
- Preprocessing with scaling and one-hot encoding
- Supervised classification:
  - K-Nearest Neighbors
  - Logistic Regression
  - Random Forest
- Hyperparameter tuning using GridSearchCV

## Model Interpretation
- Logistic regression coefficients for directional insight
- Random forest feature importance
- Partial dependence plots to identify optimal parameter ranges
- 2D decision boundary visualizations

## Key Observations
- Temperature and oxygen ratio are dominant factors in VO₂(M) formation
- Random forest captures nonlinear interactions better than linear models
- Decision boundaries suggest threshold-driven phase behavior

## Tools
Python, pandas, scikit-learn, seaborn, matplotlib

## Applications
This workflow demonstrates how ML can guide experimental parameter selection
in materials synthesis, reducing trial-and-error.
