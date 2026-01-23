# Education Statistics - Budget Forecasting

## *Author: Marzieh Safari*

Source for data:
IPEDS - NCES

Objectives:

1. Forecasting total expenses for Public University i.e. Central Ohio Technical College (COTC)
2. Indication of factors influencing total expenses

Executive Summary of Forecast Methodology and Results:

To project institutional expenses for the 2025–2027 fiscal period, I utilized an ARIMAX (1, 1, 0) model, which incorporates Full-Time Equivalent (FTE) enrollment
as a critical external driver. By prioritizing statistical efficiency (AIC) and operational relevance over simple historical trends, this approach enables precise
"what-if" scenario analysis regarding how enrollment shifts impact cost-per-student. The model achieved an 88.3% historical accuracy, providing leadership with a
robust, data-driven framework for baseline budgeting and contingency planning.

"If FTE drops by 100 students per year, the model predicts the Total Expense-per-student will increase by $1081.9 by 2027."

Why ARIMAX was Selected Over Simpler Models:
While the simple ARIMA model showed a slightly lower historical error (Mean Absolute Percentage Error (MAPE) of 10.57% vs. 11.73%), I have prioritized the ARIMAX
model for the following reasons:

Statistical Efficiency (AIC): The ARIMAX model achieved a lower Akaike Information Criterion (AIC) score (345.38 vs. 347.18). In statistical modeling, a lower AIC
indicates a more efficient model that better captures the underlying drivers of the data while avoiding "overfitting" to historical noise.

Operational Relevance: Unlike univariate models (Holt’s Linear Trend) that only look at "momentum," ARIMAX acknowledges that enrollment is a primary driver of 
institutional costs. Including FTE enrollment allows the model to adjust forecasts based on admissions projections.

Scenario Versatility: The selected model allows leadership to perform "what-if" analysis. We can specifically demonstrate how a decline or increase in student 
population directly impacts the "Expense per Student" metric, a capability missing from simpler trend-line models.

Interpretation of Model Accuracy:
The model’s Adjusted In-Sample MAPE of 11.73% indicates that while the long-term trend is robust, there is a natural year-over-year volatility in institutional 
spending. To account for this, the forecast includes a 95% Confidence Interval.

Recommendation:
Use the "Mean Forecast" for baseline budgeting but maintaining a contingency reserve up to the "Upper Bound" to account for the ~11% historical variance 
in non-trend related expenses.

Final remarks:
"I didn't just look at where the budget was going; I looked at how student counts drive those costs. That makes this a more reliable tool for planning."

There is a moderate relationship between enrollment and cost-per-student, but it isn't the only thing driving costs, which makes sense, as faculty salaries 
and facilities costs are often fixed.
