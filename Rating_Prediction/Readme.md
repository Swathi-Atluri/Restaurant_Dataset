#  Predict Restaurant Ratings:

This task compares the performance of **Linear Regression** and **Decision Tree Regressor** models on the restaurant dataset. The objective is to predict restaurant ratings and evaluate model performance using both numerical metrics and visualisation.

---

##  Models Used
1. **Linear Regression**  
   A simple linear model that tries to fit data using straight-line relationships.

2. **Decision Tree Regressor**  
   A non-linear model that splits data into regions and predicts using tree-based decisions.

---

## 📝 Observations

-  **Linear Regression**
  - Shows significant scatter around the diagonal line.
  - Underfits the data, especially at lower actual values.
  - Tends to predict mid-range values even when actuals are low.
  
-  **Decision Tree**
  - Predictions closely follow the actual values.
  - Distinct "steps" visible due to tree splits (normal behavior).
  - Outperforms linear regression in this case but may slightly overfit.

---

##  Performance Metrics (Example)
| Model            | MSE  | R² Score |
|------------------|------|----------|
| Linear Regression| 1.34 | 0.44     |
| Decision Tree    | 0.06 | 0.97     |


---

## 💻 Requirements
- Python
- `scikit-learn`
- `matplotlib`
- `numpy`
- `pandas`

