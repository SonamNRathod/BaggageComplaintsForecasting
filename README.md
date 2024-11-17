# Baggage Complaints Analysis

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
   - Validated the assumptions of linear regression

