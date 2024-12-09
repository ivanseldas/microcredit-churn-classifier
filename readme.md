# Microcredit Churn Classifier

Welcome to my Churn Prediction project, where I explored the challenge of identifying customers at risk of leaving a business. By applying machine learning techniques, I built a pipeline capable of delivering accurate predictions and valuable insights to support decision-making.

![cohort_analysis_wallpaper](https://github.com/user-attachments/assets/e9fa25e2-33eb-4a1a-bd85-058d3717982b)

1. **Exploratory Data Analysis (EDA):**
   - Identify cohorts by first transaction and retention rate:
   ![image](https://github.com/user-attachments/assets/e4950aec-4658-4ff4-8982-2a87f413ff7b)

2. **Feature Engineering:**
   - Designed meaningful features, including recency and lifetime metrics, to improve model performance.
   - Processed and transformed raw data into a structured format suitable for machine learning.
   - Create a Dataframe from transactional data to analytical data for churn prediction with the following correlation between features:
   ![image](https://github.com/user-attachments/assets/e4b39298-67ad-4339-a83e-930059ed27d7)

3. **Machine Learning Models:**
   - Developed and evaluated a LogisticRegression and RandomForestClassifier models, 
   - Achieved over 90% accuracy in both of them measure by F1-Score, ROC-AUC-Curve and Confusion Matrix

   RandomForestClassifier Confusion Matrix:
![image](https://github.com/user-attachments/assets/5597ef0a-f1f8-4d66-adc7-17b913c64edf)

   ROC Curve:
![image](https://github.com/user-attachments/assets/0dbedae6-ea8e-4c0d-8695-b031bfae1146)

## Results

1. **Model Comparison**:
   - The **RandomForestRegressor** performs slightly better, with both models achieving over **95% accuracy**.

2. **Data Limitations**:
   - Despite the **high accuracy**, the models do not appear to be **overfitting**, suggesting they are well-generalized.
   - However, the dataset covers only **1 year**, which may limit capturing long-term churn trends.

3. **Feature Importance**:
   - **`Recency`** strongly correlates with churn, aligning with the 90-day threshold.

4. **Cohort Impact**:
   - Customer **cohorts** from first transactions significantly affect churn predictions, highlighting the importance of segmentation.

## Files

- **Churn Prediction** - [churn_prediction.ipynb](./churn_prediction.ipynb)


