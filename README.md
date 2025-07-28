# Real Estate Value Prediction

This project uses machine learning to predict real estate values based on housing and geographic data from California.

## Dataset Features

- `longitude`, `latitude`, `housing_median_age`, `total_rooms`, `total_bedrooms`, `population`, `households`, `median_income`, `ocean_proximity`
- Target: `median_house_value`

## Preprocessing Steps

- Data shuffling
- Log-transform on skewed features
- Normalization (StandardScaler)
- One-hot encoding (`ocean_proximity`)
- Missing value handling (`total_bedrooms` → median fill)

## Models Implemented

| Model                     | Type                  | MAE   | MSE   |
|--------------------------|-----------------------|-------|-------|
| Perceptron               | Binary classification | 0.35  | 0.70  |
| LMS (Least Mean Squares) | Linear regression     | 0.42  | 0.34  |
| Neural Network (3-layer) | Non-linear regression | 0.31  | 0.22  |

> All models evaluated using 10-fold cross-validation.

## Tools & Libraries

- Python, Jupyter Lab
- pandas, numpy, matplotlib, seaborn
- scikit-learn, tensorflow

