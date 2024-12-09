# Microcredit Churn Classifier

Welcome to my Churn Prediction project, where I explored the challenge of identifying customers at risk of leaving a business. By applying machine learning techniques, I built a pipeline capable of delivering accurate predictions and valuable insights to support decision-making.

![cohort_analysis_wallpaper](https://github.com/user-attachments/assets/e9fa25e2-33eb-4a1a-bd85-058d3717982b)

1. **Exploratory Data Analysis (EDA):**
   - Conducted detailed analyses to uncover key churn drivers and customer behaviour patterns.
   - Leveraged visualizations to make data insights actionable.

2. **Feature Engineering:**
   - Designed meaningful features, including recency and frequency metrics, to improve model performance.
   - Processed and transformed raw data into a structured format suitable for machine learning.

3. **Machine Learning Models:**
   - Developed and evaluated several models, with Random Forest achieving over 95% accuracy.
   - Focused on interpretability and reliability by benchmarking multiple approaches.

4. **Results:**
   - Delivered a robust model to predict churn effectively.
   - Identified actionable insights to guide retention strategies, emphasizing business impact.

## Files

- **Churn Prediction** - [churn_prediction.ipynb](./churn_prediction.ipynb)

## Conclusion

1. **Model Comparison**:
   - The **RandomForestRegressor** performs slightly better, with both models achieving over **95% accuracy**.

2. **Data Limitations**:
   - Despite the **high accuracy**, the models do not appear to be **overfitting**, suggesting they are well-generalized.
   - However, the dataset covers only **1 year**, which may limit capturing long-term churn trends.

3. **Feature Importance**:
   - **`Recency`** strongly correlates with churn, aligning with the 90-day threshold.

4. **Cohort Impact**:
   - Customer **cohorts** from first transactions significantly affect churn predictions, highlighting the importance of segmentation.
