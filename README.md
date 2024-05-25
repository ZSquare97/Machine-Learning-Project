# Machine Learning for Predicting Reviews for an E-Commerce Business
Machine Learning for Predicting Reviews for an E-Commerce Business - Master's Course Project

Project Flow:
1.	**Data Acquisition and Exploration:**
    o	The project utilized a dataset provided by the instructor, containing information about reviews and their associated "shares".
    o	We explored the data to identify missing values, inconsistencies, and potential relationships between features.
2.	**Feature Engineering:**
    o	Association Rule Mining: This technique helped us understand how features interacted and identify potential patterns related to review sentiment (positive/negative).
    o	One-Hot Encoding: Categorical features were converted into numerical representations suitable for machine learning models.
    o	Feature Selection: We employed a two-stage approach: 
        	Correlation Analysis: This identified initially important features.
        	Association Rule Mining: We further refined the selection based on the most significant association rules for predicting sentiment.
3.	**Model Training and Evaluation:**
    o	We experimented with various regression models and feature combinations to achieve the lowest Mean Absolute Error (MAE).
    o	Several strategies were explored: 
        	Full Feature Set: This initial run used all available features to identify the best performing models.
        	Selected Features with Outlier Removal: We then focused on a subset of features identified through the selection process, further refined by removing outliers using One-Class SVM.
        	Model Exploration with PyCaret: The PyCaret library streamlined the process of identifying the best performing regression model for our data.     Through this process, Gradient Boosting emerged as the most effective model.
4.	**Model Interpretation:**
    o	SHAP (SHapley Additive exPlanations) values and beeswarm plots were used to understand which features had the strongest influence on model predictions (most significant features).
5.	**Recommendations and Limitations:**
    o	Based on the findings, the project recommended leveraging the most significant features to improve sentiment analysis.
    o	This could involve developing guidelines for users to manage review sentiment on the platform.
    o	It's important to acknowledge the limitations of the project. The pre-processed nature of the data, and restricted context influenced the model development process.

