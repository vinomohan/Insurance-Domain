# Insurance-Domain
INSURANCE CLAIM PREDICTION MODEL

Data Overview
1] Dataset Size:	
58,592 rows and 44 columns of car policy and claim data.
2] Key Features:
Policy and customer details (e.g., policy tenure, policyholder’s age).
Vehicle attributes (e.g., age of car, fuel type, engine specifications).
Safety and feature indicators (e.g., airbags, electronic stability control).
3] Target Variable:
is_claim: Binary variable (1 for claim, 0 for no claim

Data Preprocessing
Handling Missing Values:
Verified completeness of data; no imputation was required.

Data Type Conversions:
Converted binary features (e.g., is_esc, is_parking_camera) to integers.

Encoding Categorical Features:
Applied one-hot encoding for variables like segment, fuel_type, and transmission_type for model compatibility.

Exploratory Data Analysis (EDA)
Distribution Analysis:
Visualized distributions of key variables, including policy_tenure, age_of_car, and ncap_rating, revealing patterns and guiding feature selection.


Correlation Analysis:
Analyzed correlations among numerical features, identifying potential predictors for claim probability.

Feature Importance Exploration:
Investigated the influence of features like airbags, ncap_rating, and safety features on claim likelihood.

Model Selection
Linear Models:
Logistic Regression as a baseline classifier.
Tree-Based Models:
Random Forest to capture non-linear patterns.
Advanced Model:
Gradient Boosting Classifier for high predictive power, given its potential to improve recall for claim detection.

Model Training and Evaluation
Data Splitting:
80% of data used for training, 20% reserved for testing.
Class Imbalance Handling:
Experimented with random oversampling and undersampling techniques to balance claim and non-claim classes.
Performance Metrics:
Evaluated models with a focus on Recall for claim detection, alongside accuracy and F1 score.

Key Findings and Feature Importance
Top Features Impacting Claims:
airbags, ncap_rating, and safety features collectively influenced claim probability significantly.
Model Insights:
The Gradient Boosting model was able to capture complex relationships in the data, particularly beneficial for identifying high-risk cases.
Recall-Oriented Approach:
By focusing on recall, the model prioritizes detecting potential claims, aligning with the goal of minimizing missed claims.

