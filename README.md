# Project 1: Reproducing *The Virtue of Complexity in Return Prediction*

This project is part of DSA5205 (Data Science for Quantitative Finance).  
The goal is to reproduce and critically analyze the findings of Kelly, Malamud, and Zhou (2024), *Journal of Finance*.

## Structure
- **Report.pdf**: Final report (including Tasks 1–3, discussion, and references).
- **notebook.ipynb**: Jupyter notebook with complete implementation (simulation, Ridge, Lasso, cross-validation, figures, and outputs).
- **outputs/**: Generated predictions for datasets A, B, and C, following naming convention `A0333405N_predictions_X.csv`.
- **figures/**: Diagnostic plots such as SR vs z.

## Tasks
1. **Task 1**: Simulation under misspecification with Ridge regression.
2. **Task 2**: Extension with Lasso and comparison to Ridge.
3. **Task 3**: Application to real datasets A/B/C with rolling block split cross-validation.

## Key Results
- Ridge regression exhibits the "virtue of complexity" and performs better than Lasso in this setting.
- Lasso quickly degenerates to zero predictions as the penalty grows, highlighting its limitations for return prediction.
- On real datasets, empirically optimal z from cross-validation performs better than the simplified theoretical z*.

## How to Run
1. Install dependencies from `requirements.txt`.
2. Open `notebook.ipynb` in Jupyter Lab/Notebook.
3. Run all cells to reproduce figures and generate predictions.
4. Final outputs will be saved under `outputs/`.

## Reference
- Kelly, B. T., Malamud, S., & Zhou, K. (2024). The virtue of complexity in return prediction. *Journal of Finance, 79*(1), 459–503. https://doi.org/10.1111/jofi.13298.  
- James, G., Witten, D., Hastie, T., & Tibshirani, R. (2021). An Introduction to Statistical Learning: with Applications in R (2nd ed.). Springer. (See Section 6.2)
