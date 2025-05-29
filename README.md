# Student-Performance-Predictor
## About this Notebook

This notebook analyzes study performance data stored in a CSV file (`study_performance.csv`). 

---

## Data File

The dataset `study_performance.csv` must be located in the **same folder** as the notebook for it to load correctly.

---

### 📊 Features (Independent Variables)
- **gender**: Male or Female  
- **race/ethnicity**: Categorical groupings (e.g., group A, B, C...)  
- **parental level of education**: Highest education level of parents  
- **lunch**: Type of lunch (standard or free/reduced)  
- **test preparation course**: Whether the student completed a prep course  
- **reading score**: Numerical score representing reading performance  

### 🎯 Target Variable (Dependent)
- **math score**: The main variable we aim to predict using linear regression.

---

## Model: Linear Regression

Linear regression is used to identify how the independent variables (including both categorical and numerical features) relate to the target variable (`math score`). Among the features, `reading score` is a continuous variable, while others are categorical and will be encoded accordingly before training.


---

## Overfitting vs Underfitting

### ⚠️ Overfitting
Occurs when the model learns the training data *too well*, including noise and fluctuations. It performs well on training data but poorly on unseen (test) data.



### ⚠️ Underfitting
Occurs when the model is *too simple* to capture underlying patterns in the data.


---

## How to Use

1. **Clone or download this repository**, making sure both the notebook (`student_evaluator(1).ipynb`) and the data file (`study_performance.csv`) are in the same directory.

2. **Run the notebook** using any Jupyter environment or Google Colab.

3. The notebook reads the dataset directly using:

   ```python
   import pandas as pd
   df = pd.read_csv('study_performance.csv')
   df.head(10)
