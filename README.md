# Cincinnati Car Crash Forecasting

This project aims to forecast daily car crash counts in Cincinnati using various time series models. The goal is to evaluate and compare forecasting methods to identify the most accurate and reliable approach for predicting future crash counts.

## Dataset
- **File:** `cpd_crashes.csv`
- **Description:** Contains daily crash counts for Cincinnati. Columns:
  - `date`: Date of observation (YYYY-MM-DD)
  - `cpd_crashes`: Number of crashes reported on that day

## Notebooks
- `bana7050_assignment_2.ipynb`, `bana7050_assignment_3.ipynb`, `bana7050_assignment_4.ipynb`: Stepwise assignments exploring data, model selection, and evaluation.
- `Time_Series_4 2.ipynb`: Main notebook for advanced time series modeling and cross-validation.

## Methodology
1. **Data Preparation:**
   - Load and clean the crash data.
   - Set the date as the index and sort chronologically.
2. **Train/Test Split:**
   - Typically, 80% of the data is used for training and 20% for testing.
3. **Cross-Validation:**
   - Rolling window cross-validation is used to simulate real-world forecasting and assess model robustness.
4. **Models Evaluated:**
   - Naive and Seasonal Naive
   - ARIMA and SARIMA
   - Prophet (if available)
5. **Evaluation Metrics:**
   - RMSE, MAE, MAPE, MASE
   - Visual comparison of actual vs. predicted values

## How to Run
1. **Requirements:**
   - Python 3.8+
   - Jupyter Notebook or Quarto
   - Install dependencies:
     ```bash
     pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
     ```
2. **Usage:**
   - Open any notebook (e.g., `Time_Series_4 2.ipynb`) in Jupyter.
   - Run cells sequentially to reproduce the analysis and plots.
   - Modify parameters or models as needed for experimentation.

## Results & Insights
- SARIMA models generally outperform naive baselines, especially for multi-step forecasts.
- Rolling window cross-validation provides a realistic estimate of model performance.
- Forecast errors reveal both strengths and limitations of each approach.

## File Structure
- `cpd_crashes.csv`: Main dataset
- `*.ipynb`: Jupyter notebooks with code and analysis
- `*.html`: Rendered notebook outputs
- `Time_Series_4 2_files/`: Supporting files for HTML outputs

## Author
Siddhant Madan

---
Feel free to use or adapt this project for your own time series forecasting tasks!



