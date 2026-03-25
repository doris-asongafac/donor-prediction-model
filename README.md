# Donor-prediction-model
Predictive modeling project to identify likely donors using Logistic Regression, Random Forest, and SVM to optimize fundraising campaigns.
Donor Prediction Model

📊 Overview

This project focuses on building a predictive model to identify individuals who are most likely to donate to a fundraising campaign.

A national veterans’ organization faces a low response rate (~5.1%) and high mailing costs. This project uses machine learning techniques to improve targeting and maximize campaign profitability.

🎯 Objective

The goal is to develop a classification model that predicts whether a person will donate, allowing the organization to:

Reduce unnecessary mailing costs
Target high-probability donors
Increase overall return on investment (ROI)
📁 Dataset

The dataset contains historical donor information including:

Demographics (income, home value, family income)
Donation behavior (last gift, average gift, lifetime gifts)
Engagement metrics (number of promotions, months since last donation)

Target variable:

Donor vs No Donor
🧹 Data Preprocessing
Converted categorical variables to factors
Converted integer variables to numeric
Checked multicollinearity (VIF < 5 → no major issues)
Handled feature selection using stepwise regression
🤖 Models Used

Three classification models were implemented:

1. Stepwise Logistic Regression
Feature selection using AIC
Combines forward and backward selection
Automatically selects significant predictors
2. Random Forest
Ensemble learning method
Uses multiple decision trees
Reduces overfitting through bagging
3. Support Vector Machine (SVM)
Kernel: Radial Basis Function (RBF)
Effective for non-linear classification problems
📈 Model Performance
Model	AUC
Logistic Regression	0.550
Random Forest	0.527
SVM (RBF)	0.500
Logistic Regression performed best based on AUC
Random Forest provided strong practical predictions
🏆 Best Model

The Random Forest model was selected as the best model due to its ability to better predict actual donors with lower error rates.

🔍 Key Insights

Significant predictors include:

months_since_donate → strongest predictor
last_gift → higher previous donations increase likelihood
income → lower income groups more likely to donate
home_value → higher values reduce donation likelihood
📊 Results
Balanced predictions between donors and non-donors
Improved targeting strategy compared to random mailing
Enables cost-effective marketing decisions
🛠️ Tools & Technologies
R (glm, randomForest, e1071)
Data preprocessing & feature engineering
Model evaluation (ROC, AUC, confusion matrix)
Visualization (ggplot2)
🚀 How to Run
Clone the repository
Load the dataset
Run the R script or notebook
Train models and evaluate performance
📌 Future Improvements
Hyperparameter tuning
Feature engineering improvements
Try XGBoost / Gradient Boosting
Deploy model as a dashboard (Tableau or Streamlit)
👤 Author

Doris Mbitazi Asongafac
