# ML Classification and Clustering on Real-World Dataset

This repository contains a Jupyter Notebook exploring machine learning classification and clustering techniques on a real-world dataset.

## Contents
- `ML_classifications.ipynb` – Main Jupyter Notebook
- `SeoulBikeData.csv` – Dataset used for modeling and analysis

## Project Overview

This project applies machine learning regression techniques to predict bike rental demand based on weather and seasonal data from Seoul.

The notebook explores:
- Data preprocessing and visualization
- Supervised learning with:
  - **Linear Regression** – a baseline model assuming linear relationships
  - **Random Forest Regression** – an ensemble model capable of handling non-linearity and feature interactions
- Model evaluation using:
  - **R² score** – to assess variance explained
  - **RMSE** – to evaluate prediction error

### Key Findings

- **Random Forest Regression consistently outperformed Linear Regression** across both the full feature set and a reduced set of selected features.
- Using the full dataset, Random Forest achieved an **R² of ~0.844** and **RMSE of ~63,015**, highlighting its ability to model complex relationships and resist outliers.
- With selected features, its **R² was ~0.827** and **RMSE ~69,894**, showing that meaningful accuracy can still be achieved even with fewer inputs.
- Linear Regression underperformed due to its assumption of linearity and sensitivity to outliers.

These results emphasize the importance of non-linear models in real-world prediction tasks and suggest that while more features often improve performance, a well-chosen subset can still deliver reliable results.

## Technologies Used
- python_version == 3.12.7
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook

## How to Run
1. Clone this repository:
```bash
git clone https://github.com/yourusername/ml-classification-clustering.git
cd ml-classification-clustering
