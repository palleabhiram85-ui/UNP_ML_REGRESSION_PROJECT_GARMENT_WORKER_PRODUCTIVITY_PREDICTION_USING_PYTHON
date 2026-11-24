# UNP_ML_REGRESSION_PROJECT_GARMENT_WORKER_PRODUCTIVITY_PREDICTION_USING_PYTHON


This project was completed as part of the United Network of Professionals (UNP) Machine Learning Academic Internship Program.

The project focuses on tracking, analyzing, and predicting the continuous productivity of garment manufacturing teams (actual_productivity, ranging from 0.0 to 1.0) using an end-to-end machine learning and deep learning regression pipeline. It aims to understand how operational factors, workflow delays, and team attributes influence production output in a labor-driven manufacturing environment.

Project Overview

Analyzed the Garment Worker Productivity dataset containing 1,197 records and 15 attributes, exporting a finalized 13-feature cleaned dataset.
Conducted exploratory data analysis (EDA) using consolidated box plots for outlier detection across 10 numerical attributes (targeted_productivity, smv, wip, over_time, incentive, idle_time, idle_men, no_of_style_change, no_of_workers, actual_productivity), along with count plots and pie charts for categorical and proportional breakdowns.
Performed missing-value diagnostics, identifying 506 missing records (42.27%) in Work-in-Progress (wip) and imputing them with 0 to reflect zero unfinished inventory between shifts.
Applied domain-driven preprocessing, including dropping non-predictive identifiers (date, team), normalizing department string inconsistencies, aggregating days of the week into weekdays and weekends, and clipping actual_productivity upper bounds at 1.0.
Encoded quarter sequentially (1 through 5) and applied one-hot dummy encoding (drop_first=True) to department and day to prevent multicollinearity.
Machine Learning Implementation

Applied Variance Inflation Factor (VIF) analysis using statsmodels to evaluate multicollinearity, and prepared features using StandardScaler, train_test_split, and fixed random seeds (SEED = 42) for reproducibility.
Developed regression models using Linear Regression, K-Nearest Neighbors (KNeighborsRegressor), and Support Vector Regression (SVR).
Implemented tree-based and ensemble regression algorithms, including Decision Tree, Random Forest, AdaBoost, Gradient Boosting, and XGBoost (XGBRegressor).
Built a deep learning regression pipeline using TensorFlow to predict continuous team productivity.
Model Evaluation

Assessed predictive performance using standard regression evaluation metrics, including 
R
2
 Score, Mean Squared Error (MSE), and Mean Absolute Error (MAE).
Compared traditional machine learning, ensemble, and deep learning architectures to evaluate their effectiveness on manufacturing productivity data.
Project Outcome

The project provided hands-on experience in end-to-end data cleaning, domain-specific imputation, exploratory data analysis, multicollinearity diagnostics, ensemble regression modeling, and deep learning with TensorFlow. It demonstrates how supervised machine learning and neural networks can be applied to manufacturing datasets to forecast team productivity and support data-driven operational analysis.

Google collab link :https://drive.google.com/file/d/1q5JcjTAy4bvb5NdMeVZ53B7XBOMZYQyc/view?usp=sharing 
Presentation Link :https://docs.google.com/presentation/d/1p-TsGxv82h4zdcxPxp08Jv3ipfyongRW/edit?usp=sharing&ouid=102073202992785711567&rtpof=true&sd=true
