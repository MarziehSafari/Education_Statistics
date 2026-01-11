# Education_Statistics

## Executive Summary: 
The optimized Ridge Regression model (Alpha=100) explained approximately 38% of the variance in state education expenditure. The model favored a linear approach (Degree 1), suggesting that while demographics like [% Non-Resident Alien Students, % Private Post-baccalaureate Non-Profit 4-Year, % Full-Time Male Students, and % Asian Students] influence costs, they are not the sole drivers. The remaining 62% of variance likely stems from factors outside of enrollment data, such as regional economic conditions and specific state legislative priorities.

While a complex polynomial model (Degree 2) was tested, the validation curve confirms it suffered from high variance at low penalty levels. The simpler linear model (Degree 1) proved more stable across cross-validation folds, reaching its optimal performance at an Alpha of 100. This suggests that a more conservative, linear interpretation of the data provides the most reliable predictions for unseen state-level expenditures.


### Drivers of State Education Expenditure
This analysis examined how state-level enrollment demographics and institutional types influence educational spending per student. By using Machine Learning, I moved beyond simple averages to identify the specific factors that have the most significant impact on State Education Expenditure.

**1. Methodology: The Ridge Regression Model**  
I used a Ridge Regression model to analyze the data. This model is specifically designed to handle "interconnected" data (where factors like race, sex, and school type often overlap).

Standardization: All data was "scaled" so we could compare different categories.

Predictive Power: The model achieved an R-squared score of 0.3829, meaning it successfully explains 38.29% of the differences in spending between states.

**2. Key Findings (The Coefficient Plot)**  
The Coefficient Plot visualizes the "weight" or "influence" of each category.

Positive Drivers: Categories with bars pointing to the right are associated with higher per-student costs. This often indicates specialized resource needs or higher operational costs for those institutions.

Negative Drivers: Categories with bars pointing to the left are associated with lower per-student costs, representing areas where states might achieve greater "economies of scale."

**3. State Performance (The Residual Plot)**  
The Residual Plot identifies states that do not follow the national trend.

High-Cost Outliers: States like Pennsylvania and Connecticut spend significantly more than the model predicts. This suggests unique local factors such as high cost-of-living or specific state policies that aren't captured by enrollment numbers alone.

Efficient/Low-Cost Outliers: States like Idaho spend less than expected, which may indicate highly efficient resource allocation or, conversely, a potential under-investment relative to their student demographic needs.

### Final Thoughts:
**This model provides a baseline for "expected" spending. For future policy planning, the state should investigate the outlier states identified in the residual plot to understand the specific local programs or economic conditions that cause them to deviate so significantly from the national average.**
