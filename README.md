# Education_Statistics

## Executive Summary: Drivers of State Education Expenditure
This analysis examined how state-level enrollment demographics and institutional types influence educational spending per student. By using Machine Learning, I moved beyond simple averages to identify the specific factors that have the most significant impact on State Education Expenditure.

--*1. Methodology: The Ridge Regression Model*--
We used a Ridge Regression model to analyze the data. This model is specifically designed to handle "interconnected" data (where factors like race, sex, and school type often overlap).

Standardization: All data was "scaled" so we could compare different categories (like percentages vs. student counts) on a level playing field.

Predictive Power: The model achieved an R-squared score of 0.3829, meaning it successfully explains 38.29% of the differences in spending between states.

*2. Key Findings (The Coefficient Plot)*
The Coefficient Plot visualizes the "weight" or "influence" of each category.

Positive Drivers: Categories with bars pointing to the right are associated with higher per-student costs. This often indicates specialized resource needs or higher operational costs for those institutions.

Negative Drivers: Categories with bars pointing to the left are associated with lower per-student costs, representing areas where states might achieve greater "economies of scale."

*3. State Performance (The Residual Plot)*
The Residual Plot identifies states that do not follow the national trend.

High-Cost Outliers: States like Pennsylvania and Connecticut spend significantly more than the model predicts. This suggests unique local factors such as high cost-of-living or specific state policies that aren't captured by enrollment numbers alone.

Efficient/Low-Cost Outliers: States like Idaho spend less than expected, which may indicate highly efficient resource allocation or, conversely, a potential under-investment relative to their student demographic needs.

#### Final Thoughts:
This model provides a baseline for "expected" spending. For future policy planning, the state should investigate the outlier states identified in the residual plot to understand the specific local programs or economic conditions that cause them to deviate so significantly from the national average.
