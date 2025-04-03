# FRAUD-DETECTION-USING-MACHINE-LEARNING-MODEL
**1. Introduction**

     The goal of this project is to detect fraudulent financial transactions in a dataset using machine learning models. 
     Fraudulent transactions lead to financial losses for businesses and individuals. 
     Detecting fraud early helps prevent fraudsters from exploiting the system.

**2. Data Understanding**

     **Dataset Overview:**
     Dataset Link: https://www.kaggle.com/datasets/jaiminmukeshjariwala/fraud-csv-dataset
     The dataset contains 6,362,620 transactions with 10 features.

     **Key Features:**

     Transaction Type (e.g., PAYMENT, TRANSFER, CASH_OUT)

     **Transaction Amount**

     Source & Destination Account Balances

     Fraud Label (0 = Non-fraud, 1 = Fraud)

     **Challenges:**

     Fraud cases are rare, making the dataset highly imbalanced, which can affect model performance.

**3. Data Preprocessing **

     **Handling Missing Values & Outliers:**

     Checked for missing values—there were none.

     Detected outliers in transaction amounts but kept them as they are important for fraud detection.

     **Feature Engineering:**

     Converted categorical transaction types into numerical form using One-Hot Encoding.

     **Handling Data Imbalance:**

     Since fraud cases were very few, we used SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

**4. Model Building**

     **Algorithms Used:**

     We experimented with multiple models: Logistic Regression, Random Forest, and XGBoost.

     **Best Model:**

     Random Forest performed the best due to its ability to handle complex patterns and imbalanced data.

     **Model Training:**

     We split the dataset into train (80%) and test (20%) and trained the model using optimized hyperparameters.

**5. Model Evaluation**

     **Performance Metrics:**

     We used Accuracy, Precision, Recall, F1-score, and ROC-AUC to evaluate the model.

     Recall (Sensitivity) is the most important metric because detecting fraud is more important than avoiding false alarms.

     **Confusion Matrix Analysis:**

     Our model correctly identifies most fraud cases but sometimes misclassifies genuine transactions as fraud.

**6. Key Findings **

     **Feature Importance:**

     Transaction amount and account balance changes were the most significant indicators of fraud.

     **Insights:**

     Fraudulent transactions often involve high amounts and unusual transaction patterns.

**7. Fraud Prevention Strategies**

     **Based on the model's findings, companies can improve fraud detection by:** 
     Implementing real-time monitoring with AI models. Setting transaction limits for high-risk activities.
     Using multi-factor authentication (MFA) for high-value transfers.

**8. Future Improvements

     To improve the model, we can:"** Use Deep Learning (LSTMs or Autoencoders) for anomaly detection. 
     Apply real-time fraud detection using cloud-based AI. Improve feature selection for better accuracy.

**9. Conclusion**

     This project successfully built a fraud detection model using machine learning.
     By improving fraud detection, financial institutions can reduce losses and enhance security. 
     Future enhancements include real-time fraud detection and integrating the model into banking systems.

