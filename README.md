# customer-churn-prediction
Customer Churn Prediction Using Logistic Regression

Project Description:
Customer retention is difficult in the telecommunications industry. This project develops a machine learning solution that predicts whether customers are likely to discontinue their services (churn) based on demographic, service usage, and account information. Using the dataset, a logistic regression model was trained and evaluated to identify what factors contribute the most to customer churn.

Installation: 
https://github.com/RobertKresser/customer-churn-prediction

Usage Example:
Train Model
Run the notebook cells sequentially to train the logistic regression model.

Load Saved Model
import joblib

model = joblib.load('customer_churn_model.pkl')
Predict New Customer
prediction = model.predict(new_customer_df)
print(prediction)

Key Findings:
Contract Type Impact - Month-to-month contracts show the highest churn.
Service Type Risk - Fiber optic customers churn more than others.
Tenure Effect - New customers )low tenure) are high risk.
Pricing Correlation - Higher monthly charges correlate with churn.
Model Performance - Accuracy: 80%
                    No Churn Precision: 85%
                    No Churn Recall: 89%
                    Churn Precision: 65%
                    Churn Recall: 57%
                    Weighted F1-Score: 80%

Dependencies:
pandas
numpy
matplotlib
seaborn
scikit-learn
joblib
kagglehub
