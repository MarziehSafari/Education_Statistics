# Educational Data Analytics: From Macro-Drivers to Institutional Insights

## 🎯 Strategic Goal
My objective is to bridge the gap between raw educational data and actionable institutional strategy. By leveraging machine learning and time-series forecasting, I aim to provide leadership with the diagnostic tools to understand current spending drivers and the predictive frameworks necessary for robust long-term budgeting and decision-making.

## 🔍 Phase 1: Diagnostic Analysis (State-Level Expenditure)
This phase utilized Ridge Regression to identify the demographic and institutional factors influencing state-wide educational spending.

## *Key Technical Specs*
Model: Ridge Regression (Alpha=100)

## *Variance Explained:* 
R2=0.3829 (Approx. 38% of variance)

## *Key Findings:*
Drivers: Specific demographics (Non-Resident Aliens, Private Non-Profit enrollments) were identified as significant cost influencers.

The 62% Gap: The remaining variance suggests that factors like regional economic conditions and legislative priorities are critical external drivers.

Efficiency Mapping: Residual plots identified states like Pennsylvania (high-cost outlier) and Idaho (low-cost outlier), highlighting areas where local policy overrides national trends.

## 📈 Phase 2: Predictive Forecasting (Institutional Expense Projection)
Building on the diagnostic phase, I developed an ARIMAX (1, 1, 0) model to project institutional expenses for the 2025–2027 fiscal period in COTC, specifically testing how enrollment shifts impact the bottom line.

## *Why ARIMAX?*
While simpler models (like Holt’s Linear Trend) track momentum, the ARIMAX model incorporates Full-Time Equivalent (FTE) enrollment as an external driver.

## *Accuracy:*
88.3% historical accuracy (MAPE=11.73%).

## *Statistical Efficiency:*
Achieved a lower AIC (345.38) than simpler ARIMA models, ensuring a better fit without overfitting to noise.

## *Scenario Analysis:*
The model quantifies the "What-If"—for example, a drop of 100 students is predicted to increase the cost-per-student by $1,081.90 by 2027.

### 💡 Institutional Impact & Decision-Making
By combining these methodologies, I provide a two-tier framework for educational leadership:

*Baseline Budgeting:* Use the ARIMAX "Mean Forecast" for standard planning while maintaining a contingency reserve based on the 11% historical variance.

*Resource Allocation:* Understanding that enrollment is a moderate—but not sole—driver allows for more nuanced discussions regarding fixed costs like faculty salaries and facility maintenance.

*Future Investigation:* My ongoing goal is to incorporate the external "regional" factors identified in Phase 1 into institutional models to further reduce volatility and increase predictive power.

### 🛠️ Tools & Technologies
Python: Scikit-learn (Ridge Regression), Statsmodels (ARIMAX).

Data Science: Standardization, Cross-Validation, AIC/MAPE Evaluation.

Visualization: Coefficient Plots, Residual Plots, Confidence Interval Forecasting.
