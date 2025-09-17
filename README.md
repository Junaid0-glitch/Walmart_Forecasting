# Walmart Sales Forecasting

This project aims to forecast weekly sales for Walmart stores using historical data and machine learning models. The workflow includes data cleaning, feature engineering, exploratory data analysis, and model training/evaluation.

## Project Structure
- `features.csv`: Store-level and date-level features
- `stores.csv`: Store type and size information
- `train.csv`: Weekly sales data for each store and department
- `Walmart_forecasting.ipynb`: Main notebook with all analysis and modeling steps

## Workflow
1. **Data Import & Merging**
   - Load all CSV files and merge them into a single DataFrame for analysis.
2. **Data Cleaning & Feature Engineering**
   - Remove unnecessary columns and handle missing values.
   - Convert `Date` to datetime and extract `year`, `month`, and `week` features.
   - Encode categorical variables (e.g., `Type`, `IsHoliday`).
3. **Exploratory Data Analysis (EDA)**
   - Visualize sales trends, feature distributions, and relationships.
   - Analyze feature importance using Random Forest.
4. **Modeling**
   - Train and evaluate multiple regression models:
     - Decision Tree Regressor
     - Random Forest Regressor
     - XGBoost Regressor
   - Use metrics like Mean Squared Error (MSE), Mean Absolute Error (MAE), and R2 Score to compare models.
   - XGBoost provided the best results (R2 ≈ 0.95).

## Results
- **Best Model:** XGBoost Regressor
- **Performance:**
  - R2 Score: ~0.95 (explains 95% of variance)
  - MAE: ~2,950 (average prediction error)
  - MSE: ~27,800,000

## How to Run
1. Install required packages:
   - pandas, seaborn, matplotlib, scikit-learn, xgboost
2. Open `Walmart_forecasting.ipynb` in Jupyter or VS Code.
3. Run all cells sequentially to reproduce the analysis and results.

## Author
- Project by [Your Name]

---
Feel free to reach out for questions or suggestions!
