# Concrete-Strength-Prediction-Using-Regression-Analysis
## Project Workflow: Concrete Strength Prediction

### 1. Dataset Overview
- **Dataset Size**: 1030 rows and 9 columns.  
- **Features**:  
  - Independent Variables: 'Cement', 'Blast Furnace Slag', 'Fly Ash', 'Water', 'Superplasticizer', 'Coarse Aggregate', 'Fine Aggregate', 'Age'.  
  - Dependent Variable: 'CCS' (Compressive Strength of Concrete).

---

### 2. Data Preprocessing
- **Descriptive Analysis**:  
  - Summarized the dataset to understand distributions and relationships.  
- **Data Cleaning**:  
  - Identified and removed duplicate rows.  
- **Outlier Treatment**:  
  - Capped outliers using the Interquartile Range (IQR) method.  

---

### 3. Regression Analysis Workflow

#### A. Assumptions Check for Linear Regression
- Verified key assumptions:  
  1. Linearity  
  2. Homoscedasticity  
  3. Independence of errors  
  4. Normality of residuals  
  5. Absence of multicollinearity (treated using Variance Inflation Factor).

#### B. Linear Regression Model
- **Performance**:  
  - R² (Train): 0.71  
  - R² (Test): 0.69  

#### C. Regularization Techniques
- **Ridge Regression**:  
  - R² (Train): 0.71  
  - R² (Test): 0.69  
- **Lasso Regression**:  
  - R² (Train): 0.71  
  - R² (Test): 0.69  
- **Elastic Net Regression**:  
  - R² (Train): 0.70  
  - R² (Test): 0.69  

#### D. Hyperparameter Tuning
- Performed grid search to optimize hyperparameters for Ridge, Lasso, and Elastic Net models.  

#### E. Gradient Descent
- Fitted Gradient Descent model for optimization.  
- **Performance**:  
  - R² (Train): 0.69  
  - R² (Test): 0.67  

---

### 4. Key Results
- Ridge, Lasso, and Elastic Net demonstrated similar performance with slight variations.  
- Gradient Descent showed slightly lower performance compared to regularization models.  

---

### 5. Conclusion
- Regularized models (Ridge, Lasso, Elastic Net) achieved the best results with R² values of 0.71 (Train) and 0.69 (Test).  
- The project provides insights into the factors influencing concrete compressive strength and demonstrates the effectiveness of regularization in linear regression.
