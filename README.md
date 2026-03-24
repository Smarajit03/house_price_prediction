# House Price Prediction — ML Project

A machine learning project to predict house prices based on various property features.
The dataset is from the Kaggle competition **"House Prices: Advanced Regression Techniques"**.

## Model Performance
- **Algorithm:** Gradient Boosting Regressor
- **Score:** 87.16% (R² Score)

## Project Structure

```
House-Price-Prediction/
├── ML_Model/
│   ├── data_set/
│   │   ├── train.csv               # Training dataset
│   │   ├── test.csv                # Test dataset
│   │   ├── sample_submission.csv   # Sample submission format
│   │   ├── submission.csv          # Final predictions
│   │   └── data_description.txt    # Feature descriptions
│   └── src/
│       ├── main.ipynb              # Main Jupyter Notebook
│       └── gbr.pkl                 # Trained model (pickle)
└── README.md
```

## Libraries Used

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

## Workflow

### 1. Data Loading & Analysis
- Training and test datasets are loaded from CSV files
- Exploratory data analysis (EDA) is done to understand feature distributions
- Visualizations: histograms, box plots, and heatmaps

### 2. Data Preprocessing
- Missing values handled via imputation or column removal
- Categorical variables encoded using one-hot encoding
- Numerical features standardized for uniform scaling

### 3. Model Selection & Training
Multiple regression models were evaluated:
- Linear Regression
- SVR
- SGDRegressor
- KNeighborsRegressor
- DecisionTreeRegressor
- RandomForestRegressor
- **GradientBoostingRegressor** ✅ (selected)
- XGBRegressor
- MLPRegressor

Cross-validation was used to compare models based on R² score.

### 4. Prediction & Output
- Final model trained on the full training set
- Predictions generated for the test set
- Results saved to `submission.csv`

## Dataset

From Kaggle: [House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

## Connect

**Smarajit** — [GitHub](https://github.com/Smarajit03)
