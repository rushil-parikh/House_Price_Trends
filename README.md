# Understanding House Price Trends: A Data-Driven Exploration

## Project Objective

The goal of this project was to analyze housing price trends and predict house prices based on significant features in the data. By exploring the King County House Sales dataset, we aimed to:

1. Develop a predictive model to estimate house prices accurately.
2. Identify key factors that influence housing prices, providing actionable insights for stakeholders such as homeowners, real estate agents, and investors.

---

## Dataset Description

The dataset used for this project is the **King County House Sales dataset**, sourced from Kaggle. It includes:

- **Records**: 21,613 house sales.
- **Features**: 21 attributes, including:
  - `bedrooms`: Number of bedrooms.
  - `bathrooms`: Number of bathrooms.
  - `sqft_living`: Interior living space in square feet.
  - `grade`: Construction and design quality.
  - `sqft_above`: Square footage excluding the basement.
  - `sqft_living15`: Average living space of 15 nearest neighbors.

The dataset provides comprehensive information, enabling a detailed analysis of the factors affecting housing prices.

---

## Methodology

### 1. Data Preprocessing

- **Outlier Handling**:
  - Removed unrealistic entries, such as houses with 0 bathrooms or bedrooms > 8.
  - Performed log transformation on skewed features like price and square footage to stabilize variance.
- **Feature Selection**:
  - Conducted correlation analysis to select key features strongly associated with house prices: `sqft_living`, `grade`, `bathrooms`, `sqft_above`, and `sqft_living15`.
- **Normalization**:
  - Normalized all features to ensure consistency in model training.

### 2. Model Training

- **Linear Regression**:
  - Served as the baseline model due to its simplicity and interpretability.
  - Identified the impact of each feature on house prices through regression coefficients.
- **K-Nearest Neighbors (KNN)**:
  - Captured non-linear relationships in the data.
  - Determined the optimal value of `k` (10) using cross-validation to balance bias and variance.

### 3. Evaluation Metrics

- **Mean Absolute Error (MAE)**: Measures average prediction error.
- **Root Mean Squared Error (RMSE)**: Penalizes larger errors more heavily.
- **R² Score**: Represents the proportion of variance explained by the model.

---

## Key Findings

### 1. Predictive Model Performance

- **Best Model**: K-Nearest Neighbors (KNN) with `k=10`:

  - **R²**: 0.5789 (explains \~58% of price variance).
  - **MAE**: \$144,292.28 (lowest prediction error).
  - **RMSE**: \$224,531.33 (lowest overall error).

- Linear Regression performed slightly worse than KNN but provided interpretable insights into feature importance.

### 2. Feature Importance

- `sqft_living`: Strongest positive correlation with price.
- `grade`: Significant predictor of price variations across construction quality categories.
- `bathrooms` and `sqft_living15`: Moderate correlation but valuable for understanding property functionality and neighborhood influences.

### 3. Data Insights

- **Price Distribution**:
  - Positively skewed with most houses priced in the lower range.
  - High-value properties formed a long tail, requiring normalization.
- **Outliers**:
  - Large properties and high-value transactions influenced the variance in predictions but were critical for understanding market extremes.

---

## Conclusion

This project highlighted the complexity of predicting house prices due to the diverse factors at play. By comparing models, we found that **KNN with k=10** was the most effective, offering:

- Accurate predictions (lowest MAE and RMSE).
- Better handling of non-linear relationships between features and price.

While Linear Regression was less accurate, it provided valuable insights into how individual features impact prices. The importance of `sqft_living` and `grade` as key predictors was reaffirmed, emphasizing their role in real estate pricing.

This project demonstrates:

1. How to preprocess and analyze real-world datasets.
2. The application of machine learning models for predictive analysis.
3. The importance of balancing model complexity with interpretability.

---

This project serves as a step towards understanding housing market dynamics and showcases the power of data-driven decision-making in real estate. Feel free to explore the code and replicate the analysis!

# Understanding House Price Trends: A Data-Driven Exploration

## Project Objective

The goal of this project was to analyze housing price trends and predict house prices based on significant features in the data. By exploring the King County House Sales dataset, we aimed to:

1. Develop a predictive model to estimate house prices accurately.
2. Identify key factors that influence housing prices, providing actionable insights for stakeholders such as homeowners, real estate agents, and investors.

---

## Dataset Description

The dataset used for this project is the **King County House Sales dataset**, sourced from Kaggle. It includes:

- **Records**: 21,613 house sales.
- **Features**: 21 attributes, including:
  - `bedrooms`: Number of bedrooms.
  - `bathrooms`: Number of bathrooms.
  - `sqft_living`: Interior living space in square feet.
  - `grade`: Construction and design quality.
  - `sqft_above`: Square footage excluding the basement.
  - `sqft_living15`: Average living space of 15 nearest neighbors.

The dataset provides comprehensive information, enabling a detailed analysis of the factors affecting housing prices.

---

## Methodology

### 1. Data Preprocessing

- **Outlier Handling**:
  - Removed unrealistic entries, such as houses with 0 bathrooms or bedrooms > 8.
  - Performed log transformation on skewed features like price and square footage to stabilize variance.
- **Feature Selection**:
  - Conducted correlation analysis to select key features strongly associated with house prices: `sqft_living`, `grade`, `bathrooms`, `sqft_above`, and `sqft_living15`.
- **Normalization**:
  - Normalized all features to ensure consistency in model training.

### 2. Model Training

- **Linear Regression**:
  - Served as the baseline model due to its simplicity and interpretability.
  - Identified the impact of each feature on house prices through regression coefficients.
- **K-Nearest Neighbors (KNN)**:
  - Captured non-linear relationships in the data.
  - Determined the optimal value of `k` (10) using cross-validation to balance bias and variance.

### 3. Evaluation Metrics

- **Mean Absolute Error (MAE)**: Measures average prediction error.
- **Root Mean Squared Error (RMSE)**: Penalizes larger errors more heavily.
- **R² Score**: Represents the proportion of variance explained by the model.

---

## Key Findings

### 1. Predictive Model Performance

- **Best Model**: K-Nearest Neighbors (KNN) with `k=10`:

  - **R²**: 0.5789 (explains \~58% of price variance).
  - **MAE**: \$144,292.28 (lowest prediction error).
  - **RMSE**: \$224,531.33 (lowest overall error).

- Linear Regression performed slightly worse than KNN but provided interpretable insights into feature importance.

### 2. Feature Importance

- `sqft_living`: Strongest positive correlation with price.
- `grade`: Significant predictor of price variations across construction quality categories.
- `bathrooms` and `sqft_living15`: Moderate correlation but valuable for understanding property functionality and neighborhood influences.

### 3. Data Insights

- **Price Distribution**:
  - Positively skewed with most houses priced in the lower range.
  - High-value properties formed a long tail, requiring normalization.
- **Outliers**:
  - Large properties and high-value transactions influenced the variance in predictions but were critical for understanding market extremes.

---

## Conclusion

This project highlighted the complexity of predicting house prices due to the diverse factors at play. By comparing models, we found that **KNN with k=10** was the most effective, offering:

- Accurate predictions (lowest MAE and RMSE).
- Better handling of non-linear relationships between features and price.

While Linear Regression was less accurate, it provided valuable insights into how individual features impact prices. The importance of `sqft_living` and `grade` as key predictors was reaffirmed, emphasizing their role in real estate pricing.

This project demonstrates:

1. How to preprocess and analyze real-world datasets.
2. The application of machine learning models for predictive analysis.
3. The importance of balancing model complexity with interpretability.

---

This project serves as a step towards understanding housing market dynamics and showcases the power of data-driven decision-making in real estate. Feel free to explore the code and replicate the analysis!

