# Housing Sale Price Prediction (Austin, Texas)

## Project Overview

This project focuses on predicting housing sale prices in Austin, Texas using multiple linear regression techniques.

The objective is to analyze property features and build a predictive model capable of estimating housing prices. The project also explores relationships between housing characteristics and sale prices through statistical analysis and data visualization.

This work was originally implemented in **R as part of an academic assignment**, and is now being **reimplemented in Python** to demonstrate data science and machine learning workflow using Python libraries.

---

## Business Problem

The real estate market in Austin, Texas has experienced significant price fluctuations, particularly during the post-COVID housing boom. Predicting housing prices can help:

- Buyers avoid overpaying
- Investors estimate property value
- Developers understand market drivers
- Real estate analysts forecast trends

---

## Dataset

Austin Housing Dataset

The dataset contains property-level information including:

- living_area
- lot_area
- bedrooms
- bathrooms
- school_rating
- student_teacher_ratio
- parking_features
- waterfront_features
- school_dist
- heating availability
- association features
- patio/porch features

Target variable:
sale_price


---

## Project Workflow

### 1. Problem Understanding
Define the objective: predicting house sale prices based on property characteristics.

### 2. Data Cleaning & Preprocessing

Steps performed:

- Handling missing values
- Removing duplicates
- Converting categorical variables
- Standardizing feature values
- Handling outliers using the **IQR method**
- Replacing extreme values to reduce skewness

---

### 3. Exploratory Data Analysis (EDA)

EDA techniques included:

- Histograms
- Boxplots
- Correlation analysis
- Distribution analysis
- Skewness detection

Correlation analysis showed strong relationships between sale price and:

- Living area
- School rating
- Lot area

---

### 4. Feature Engineering

Categorical variables were transformed and numerical variables were normalized where necessary.

---

### 5. Model Development

Multiple **Linear Regression models** were built iteratively by adding more explanatory variables.

| Model | Variables | R² |
|------|------|------|
| Model 1 | 4 variables | 0.316 |
| Model 2 | 8 variables | 0.344 |
| Model 3 | 10 variables | 0.345 |
| Model 4 | 11 variables | 0.417 |
| Model 5 | 12 variables | **0.423** |

Model 5 was selected as the **best performing model**.

---

## Model Evaluation

Evaluation metrics used:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

Best Model Performance:
R² = 0.423
RMSE = 175,347
MAE = 119,999


The model explains **42.3% of the variance in housing prices**.

---

## Model Diagnostics

The following regression assumptions were tested:

### Multicollinearity
Variance Inflation Factor (VIF) showed **low multicollinearity**.

Mean VIF ≈ 1.70

### Residual Analysis

Checked for:

- Linearity
- Normality
- Homoscedasticity

Some heteroscedasticity and deviation from normality were observed.

### Influential Observations

Cook’s Distance was used to detect influential data points.

### Autocorrelation

Durbin-Watson test suggested possible **positive autocorrelation**.

---

## Key Insights

- **Living area** has the strongest correlation with sale price.
- **School rating** significantly impacts property value.
- Adding more relevant features improved model performance.
- Real estate price prediction is sensitive to outliers and skewed data.

---

## Limitations

- Linear regression assumes linear relationships.
- Outliers significantly affect predictions.
- The model could be improved using advanced algorithms such as:

- Random Forest
- Gradient Boosting
- XGBoost

---

## Technologies Used

Python (Reimplementation)

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

Original Implementation:

- R
- dplyr
- caret
- car
- lmtest

---

## Repository Structure
housing-price-prediction
│
├── data
├── notebooks
├── images
├── models
├── src
└── README.md


---

## Author

Dinesh Dhanseelan  
MSc Business Analytics  
Queen's University Belfast
