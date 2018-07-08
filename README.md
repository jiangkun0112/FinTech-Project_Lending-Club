# FinTech-Project_Lending-Club

# PROJECT SUMMARY

This project is implemented using Python on the Jupyter Notebook platform. Data processing and machine learning packages such as Pandas and Sci-kit Learn are utilized. The modeling is trained based on the Lending Club's historic loan data from year 2014.

The target is to predict the default rate of the new loans listed on Lending Club. The workflow of the project consists of 6 steps:

Loading Data
Exploratory Analysis
Feature Engineering
Model Building
Model Integration
Model Evaluation
Data cleaning are performed to uniform the features used in the training set and the target set. Categorical variables are extracted into meaningful features for model input via feature engineering. XGBoost (Extreme Gradient Boost) is used as the modeling algorithm. As an advanced Gradient Boosted Regression Trees (GBRT) algorithm, XGBoost adopted several advantages of GBRT such as: natural handling of data of mixed type , predictive power, robustness to outliers in output space (via robust loss functions). Combining both Random Forest and Adaptive Gradent Boosting algorithms, XGBoost exhibited high efficiency and flexibility in modeling large datasets with ease of implementation.

The model is then autotuned to optimize its performance using Bayesian Optimization and Cross Validation. The tuned model is tested using the Area Under Curve (AUC) of the Receiver Operating Characteristics (ROC) as the performance metrics. The overall AUC score reaches above 73% on the testing set. Finally, the tuned model is saved using Pickle and integrated into an interactive web-application built with Flask Framework.

The total runtime for model building and model tuning may take 4-5 hours, depending on computer hardware.

Required Libraries
This notebook uses several standard Python packages and special packages for model building and model tuning. The primary libraries that we'll be using are:

requests: request data from API servers.
pandas: and numpy: numeric paneled data operation.
matplotlib and seaborn: data visualization.
bayes_opt: Bayesian Optimization.
sklearn: Sci-kit Learn for model buidling and evaluation.
xgboost: XGBoost algorithm.
