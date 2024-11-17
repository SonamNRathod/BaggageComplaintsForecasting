# README: Baggage Complaints Analysis

## Project Overview
This project aims to analyze the factors influencing baggage complaints in airline operations and develop a predictive regression model. By examining operational variables such as scheduled flights, canceled flights, and enplaned passengers, we aim to identify key drivers of complaints and assess the model's performance.

---

## Dataset Description
The dataset includes the following variables:

- **Airline**: Name of the airline.
- **Date**: Reporting date (monthly or yearly).
- **Scheduled**: Number of scheduled flights (independent variable).
- **Cancelled**: Number of canceled flights (independent variable).
- **Enplaned**: Number of passengers enplaned (independent variable).
- **Baggage**: Count of baggage complaints (dependent variable).

---

## Analysis Workflow
1. **Simple Linear Regression**:
   - Examined the relationship between baggage complaints and `Scheduled` flights.

2. **Multiple Linear Regression**:
   - Built a model using `Scheduled`, `Cancelled`, and `Enplaned` as predictors.
   - Assessed the model's goodness-of-fit and statistical significance.

3. **Residual Analysis**:
   - Validated the assumptions of linear regression:
     - Linearity
     - Normality of residuals
     - Homoscedasticity (equal variance of residuals)

4. **Model Diagnostics**:
   - Used diagnostic plots and statistical metrics to evaluate the model and identify potential improvements.

---

## Key Findings
1. **Model Performance**:
   - **Multiple \( R^2 = 0.8472\)**: The model explains 84.72% of the variance in baggage complaints.
   - **Adjusted \( R^2 = 0.8453\)**: The model generalizes well to unseen data.
   - Residual standard error: **3930** complaints.

2. **Predictor Significance**:
   - **Cancelled Flights**: Strongest predictor (\( \beta = 5.536\), \( p < 2e-16 \)).
   - **Scheduled Flights**: Moderate impact (\( \beta = 0.0864\), \( p = 0.00429 \)).
   - **Enplaned Passengers**: Small but significant impact (\( \beta = 0.0035\), \( p < 2e-16 \)).

3. **Residual Analysis**:
   - Residuals are generally well-distributed but show some large deviations (outliers) that warrant further investigation.

---

## Recommendations
1. **Address Outliers**:
   - Investigate large residuals to identify missing predictors or potential data errors.

2. **Enhance the Model**:
   - Incorporate additional variables, such as weather conditions or staffing levels, to explain the remaining variance.

3. **Model Refinement**:
   - Consider transformations (e.g., logarithmic) to address potential heteroscedasticity.

---

## Scripts and Tools
- **Scripts**:
  - `simple_regression.R`: Simple regression analysis with `Scheduled` flights.
  - `multiple_regression.R`: Multiple regression analysis using all predictors.
  - `residual_analysis.R`: Residual diagnostics and assumption validation.
  - `forecasting.R`: Forecast baggage complaints using the fitted model.

- **Tools**:
  - **R Packages**:
    - `ggplot2` for visualization.
    - `car` for multicollinearity analysis (VIF).
    - `forecast` for predictive modeling.

---

## Contact
For questions or feedback, contact the project author:
- **Name**: Smith Surendran
- **Email**: smith.surendran@rutgers.edu
