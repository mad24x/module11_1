Link to Notebook
https://github.com/mad24x/module11_1/blob/main/used_cars_notebook.ipynb


Used Car Price Prediction
Summary of Findings
This project analyzes the factors that influence the price of used cars, focusing on a subset of data from the state of Georgia. Multiple regression models were developed to predict car prices based on features such as condition, mileage, and manufacturer.

Key Insights:
Manufacturer Influence: Initially, the "manufacturer" column dominated feature importance due to OneHotEncoding. However, after excluding this column, more meaningful insights emerged, with car condition becoming the leading predictor.  This was tested outside the notebook provided and was more for curiosity purposes.
Car Condition: After refining the models, it was found that the condition of the car is one of the most significant factors in determining its price.
Data Quality: The dataset contained many missing or nonsensical entries, requiring extensive cleaning. Further review and improvement of the dataset would likely enhance model performance.
Profit Margin Analysis: Further analysis is recommended to explore the profit margin on each vehicle. This would enable dealerships to identify the most profitable cars and optimize their inventory accordingly.
Model Performance:
Best Ridge Model MSE: 6.83
Best Lasso Model MSE: 6.84
Linear Regression MSE: 6.87
These results demonstrate a high level of accuracy, offering valuable insights into the drivers of used car prices in the Georgia region.

Modeling Approach
Use of Multiple Regression Models
Multiple regression models, including Linear Regression, Ridge Regression, and Lasso Regression, were utilized to capture different aspects of the relationship between car features and price. Each model was trained and evaluated on the same dataset for consistent comparison.

Cross-Validation
Cross-validation was applied to assess model performance across different folds of the data, ensuring robustness and reducing the risk of overfitting.

Hyperparameter Tuning
A grid search was performed for both Ridge and Lasso models to optimize hyperparameters, particularly the regularization strength (alpha). This process ensured the best trade-off between bias and variance.

Interpretation of Coefficients
The coefficients of each model were examined to understand the impact of various features (such as car condition and mileage) on the predicted price. Categorical variables were processed using OneHotEncoding, and the influence of each category was interpreted based on its corresponding coefficient.

Evaluation Metric
Mean Squared Error (MSE) was selected as the primary evaluation metric across all models. MSE effectively penalizes larger errors, making it suitable for price prediction, where outliers could disproportionately affect the results. This metric was used to evaluate how well the models predicted car prices with minimal error.

Best Ridge Model MSE: 6.83
Best Lasso Model MSE: 6.84
Linear Regression MSE: 6.87
Rationale for MSE
MSE was chosen as it emphasizes larger errors, which is particularly important in pricing predictions. By penalizing larger deviations more heavily, MSE helps identify models that minimize significant pricing discrepancies.

Next Steps
Future work should include expanding the analysis to additional regions and incorporating profit margin data to better inform dealership inventory management decisions.




