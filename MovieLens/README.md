# MovieLens Rating Prediction System

## Project Overview

This project uses the MovieLens 100K dataset to predict user movie ratings using machine learning techniques.

The objective is to understand user preferences and movie characteristics by creating meaningful features from historical ratings and comparing multiple regression models.

---

## Dataset

Dataset: MovieLens 100K

https://grouplens.org/datasets/movielens/100k/

The dataset contains:

- User ID
- Movie ID
- Rating (1–5)
- Timestamp

Each record represents a user's rating for a particular movie.

---

## Project Workflow

### 1. Data Preparation

- Loaded MovieLens 100K dataset
- Processed user and movie rating information
- Created structured training data

### 2. Feature Engineering

Generated statistical features including:

#### User Features

- user_mean
- user_std
- user_count

#### Movie Features

- movie_mean
- movie_std
- movie_count

#### Additional Features

- user_enc
- movie_enc
- global_mean

These features help capture user behaviour and movie popularity.

---

### 3. Exploratory Data Analysis

Performed:

- Rating distribution analysis
- Correlation analysis
- Heatmap visualisation
- Feature relationship inspection

### Key Observation

No severe multicollinearity was observed among the engineered features.

---

## Models Evaluated

The following baseline models were trained and compared:

1. Linear Regression
2. Ridge Regression
3. Decision Tree Regressor
4. Random Forest Regressor
5. Gradient Boosting Regressor
6. XGBoost Regressor

---

## Evaluation Metrics

Models were evaluated using:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)

Lower values indicate better predictive performance.

---

## Results

| Model | RMSE | MAE |
|---------|---------|---------|
| Linear Regression | 0.9285 | 0.7344 |
| Ridge Regression | 0.9285 | 0.7344 |
| Decision Tree | 0.9322 | 0.7335 |
| Random Forest | 0.9359 | 0.7326 |
| Gradient Boosting | 0.9194 | 0.7261 |
| XGBoost | **0.9126** | **0.7180** |

### Best Model

**XGBoost Regressor**

- RMSE: 0.9126
- MAE: 0.7180

---

## Conclusion

Feature engineering successfully transformed raw user and movie identifiers into meaningful predictive features.

Correlation analysis indicated low multicollinearity among the engineered variables.

Among all evaluated models, XGBoost achieved the best performance and demonstrated the strongest ability to capture user–movie rating patterns.

The project highlights the importance of feature engineering and model comparison in building effective recommendation systems.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## Author

**Niranjan Nandam**
