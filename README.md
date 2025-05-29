# Student-Performance-Predictor
## About this Notebook

This notebook analyzes study performance data stored in a CSV file (`study_performance.csv`). 

---

## Data File

The dataset `study_performance.csv` must be located in the **same folder** as the notebook for it to load correctly.

---

## How to Use

1. **Clone or download this repository**, making sure both the notebook (`student_evaluator(1).ipynb`) and the data file (`study_performance.csv`) are in the same directory.

2. **Run the notebook** using any Jupyter environment or Google Colab.

3. The notebook reads the dataset directly using:

   ```python
   import pandas as pd
   df = pd.read_csv('study_performance.csv')
   df.head(10)
