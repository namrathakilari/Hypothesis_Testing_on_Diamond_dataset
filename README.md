# Hypothesis_Testing_on_Diamond_dataset
Statistical analysis of the Diamonds dataset using OLS regression, hypothesis testing, and ANOVA to examine how physical and categorical attributes affect price. Includes full-model evaluation, significance testing, and predictive insights.

##  Project Overview

The goal of this project is to understand and quantify the relationship between **diamond features** and **diamond price**. We use statistical modeling techniques to evaluate how strongly each attribute influences the price and how effectively the full model predicts pricing.

**Key Questions:**
- Can diamond price be predicted using physical attributes?
- Which features significantly contribute to price?
- How do reduced models compare with the full model?
- Does adding more features meaningfully improve prediction accuracy?

---

##  Tools & Libraries Used

- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Statsmodels  
- SciPy  
- Scikit-learn  

---

##  Analysis Performed

### **1. Data Preparation**
- Loaded the Diamonds dataset from Seaborn.
- Encoded categorical columns (`cut`, `color`, `clarity`) using `LabelEncoder`.
- Built a final dataset containing 9 predictors.

### **2. Correlation Analysis**
- Generated a heatmap to identify relationships between features and price.
- Found **carat** and **dimensions (x, y, z)** to be the strongest correlated with price.

### **3. Full OLS Regression Model**
Model used:
price ~ carat + depth + table + x + y + z + cut + color + clarity

- All coefficients had **p-values < 0.05**.
- Model achieved a **high R²**, indicating strong predictive power.
- Actual vs. Predicted plots showed excellent fit.

### **4. Hypothesis Testing**
Performed:
- **t-tests** for each regression coefficient  
- **Z-tests** (large-sample approximation)  
- **Z-test for mean price**  
- All tests confirmed that each predictor significantly influences price.

### **5. ANOVA (F-Test)**
Compared reduced vs. expanded models:
- Found adding more physical dimensions (y, z) significantly improves prediction.
- Very high F-statistics and extremely low p-values.

---

##  Key Findings

- **Yes — diamond price can be predicted very accurately from physical attributes.**
- All nine features (carat, depth, table, x, y, z, cut, color, clarity) are **statistically significant**.
- **Carat** is the strongest predictor; dimensions also play a major role.
- Adding more features significantly improves model performance.
- The full model provides the highest prediction accuracy.

---

##  Conclusion

This project shows that **statistical modeling can reliably predict diamond prices** using both physical and categorical attributes. The full regression model captures most of the variability in price and demonstrates strong statistical significance for all predictors.

---

##  Future Improvements

- Implement machine learning models (Random Forest, XGBoost).
- Compare statistical vs. ML performance.
- Create a price prediction web app or API.
- Explore feature interactions and higher-order terms.

---

##  Author

Created by **Namratha Kilari**

If you like this project, feel free to ⭐ the repository!
