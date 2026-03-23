#Austin Housing Price Prediction

This project focuses on predicting housing sale prices in Austin, Texas using regression-based machine learning techniques. The study combines statistical analysis (R) and machine learning (Python) to build and evaluate predictive models.

---

## Problem Overview

The real estate market in Austin, Texas is highly dynamic, with fluctuating prices influenced by multiple factors such as property size, location, and amenities. 

The objective of this project is to:

- Predict house sale prices using regression models  
- Identify key features influencing housing prices  
- Compare multiple models to improve prediction accuracy  
- Support better decision-making for buyers, sellers, and investors  

This work builds upon prior statistical analysis conducted in R, where multiple linear regression models were developed and evaluated. :contentReference[oaicite:0]{index=0}

---

## Objectives

- Perform data cleaning and preprocessing  
- Conduct exploratory data analysis (EDA)  
- Build multiple regression models with increasing complexity  
- Evaluate model performance using R² and RMSE  
- Improve prediction accuracy through feature engineering  

---

## 📊 Methodology

1. **Data Preprocessing**
   - Handled missing values  
   - Converted categorical variables  
   - Treated outliers using IQR method  
   - Standardized and cleaned dataset  

2. **Exploratory Data Analysis**
   - Distribution analysis (histograms, boxplots)  
   - Correlation analysis  
   - Feature relationships  

3. **Model Building**
   - Split dataset into training (80%) and testing (20%)  
   - Built multiple regression models with incremental features  

4. **Model Evaluation**
   - R² (explained variance)  
   - RMSE (prediction error)  

---

## Models Implemented

- **Model 1** – Basic regression (core features)  
- **Model 2** – Added additional relevant predictors  
- **Model 3** – Optimized feature set (best-performing model)  
- **Model 4** – Alternative feature combination  

---

## Model Performance (Updated Results)

| Metric        | Model 1 | Model 2 | Model 3 | Model 4 |
|--------------|--------|--------|--------|--------|
| **Train R²** | 0.3175 | 0.3673 | **0.5668** | 0.4072 |
| **Test R²**  | 0.3151 | 0.3633 | **0.5464** | 0.4056 |
| **Train RMSE** | 0.4510 | 0.4343 | **0.3593** | 0.4204 |
| **Test RMSE**  | 0.4589 | 0.4424 | **0.3734** | 0.4274 |

---

 Key Insights

- **Model 3 is the best-performing model**
  - Highest Test R²: **0.546**
  - Lowest Test RMSE: **0.373**

- Adding more relevant features significantly improves performance compared to the baseline model

- The gap between training and testing performance is small → indicates **good generalization**

- Feature engineering and variable selection played a critical role in improving model accuracy

---

##Insights from R Analysis

- Living area shows the strongest positive correlation with sale price  
- Moderate correlation observed with:
  - Lot area  
  - Bathrooms  
  - School rating  

- Model assumptions revealed:
  - Low multicollinearity (VIF ≈ 1.7)  
  - Presence of heteroscedasticity  
  - Slight deviation from normality  

- Best R model achieved:
  - R² ≈ **42.3%**  
  - RMSE ≈ **175,347**

 The Python model (Model 3) improves performance significantly beyond the R baseline.

---

##Tech Stack

- **Python** (Scikit-learn, Pandas, NumPy)   
- Jupyter Notebook  
- Data Visualization libraries  

---

---

## Future Improvements

- Apply advanced models (Random Forest, XGBoost)  
- Perform hyperparameter tuning  
- Deploy model using Streamlit or Flask  
- Improve handling of outliers and skewed data  

---

## Conclusion

This project demonstrates a complete end-to-end machine learning workflow, integrating statistical analysis and predictive modelling. 

While the R-based regression model provided a strong baseline, the Python implementation improved performance significantly, achieving better predictive accuracy and generalization.

The study highlights the importance of:
- Feature selection  
- Data preprocessing  
- Model evaluation  

in building effective real-world predictive systems.

---
