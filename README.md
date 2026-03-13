# house-price-prediction
Machine learning regression project that predicts Bangalore house prices using data cleaning, feature engineering, EDA, and models like Linear Regression, Decision Tree, and Random Forest.
#  Bangalore House Price Prediction

This project builds a **machine learning regression model** to predict housing prices in Bangalore based on various features such as location, square footage, number of bedrooms (BHK), bathrooms, and balconies.  
The project demonstrates a complete **data science workflow**, including data cleaning, exploratory data analysis, feature engineering, model training, and evaluation.

---

#  Dataset

The dataset used for this project is the **Bangalore Housing Price Dataset**.

Features include:

- Area Type  
- Availability  
- Location  
- Total Square Feet  
- Number of Bathrooms  
- Number of Balconies  
- Size (BHK)  
- Price  

Dataset source: Kaggle

---

#  Project Workflow

The project follows the standard **data science pipeline**:

### 1. Data Loading and Exploration
- Loaded dataset using **Pandas**
- Inspected dataset structure, data types, and missing values
- Identified numerical and categorical features

### 2. Data Cleaning & Preprocessing
- Handled missing values
- Removed columns with excessive missing data
- Converted `total_sqft` to numeric values
- Extracted **BHK values from the size column**

### 3. Exploratory Data Analysis (EDA)
Performed multiple visualizations to understand relationships between variables, including:

- Price vs Total Square Feet
- Price vs BHK
- Distribution of prices
- Correlation heatmap
- Feature relationship plots

### 4. Feature Engineering
- Created new features for better model performance
- Removed redundant or inconsistent data
- Converted categorical variables using **One-Hot Encoding**

### 5. Model Building
Three regression models were trained:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 6. Model Evaluation
Models were evaluated using:

- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)**
- **R² Score**

---

#  Model Performance

| Model | RMSE | MAE | R² Score |
|------|------|------|------|
| Linear Regression | 109.43 | 37.50 | 0.44 |
| Decision Tree | 34.77 | 3.98 | 0.94 |
| Random Forest | **31.60** | **2.85** | **0.95** |

**Random Forest Regressor achieved the best performance**, explaining approximately **95% of the variance in housing prices**.

---

#  Key Insights

- **Total square footage** is one of the most influential factors affecting house prices.
- Houses with higher **BHK and bathroom counts** generally have higher prices.
- **Location significantly impacts housing prices**.
- Ensemble models like **Random Forest perform better** than simple linear models for this dataset.

---

#  Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-Learn  
- Jupyter Notebook

Jupyter Notebook
