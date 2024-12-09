# Microcredit Churn Classifier

Customer behaviour analysis for Ironhack Payment, a financial services provider, to uncover insights into retention, revenue trends, and transaction success. Using Python, Pandas, and Plotly, I created cohort-based views that highlight customer lifecycle patterns and seasonal trends to support strategic growth.

![cohort_analysis_wallpaper](https://github.com/user-attachments/assets/e9fa25e2-33eb-4a1a-bd85-058d3717982b)

## Key Findings

- **Revenue by Cohort**: October 2020 cohort led in revenue, with strong seasonal growth patterns in spring and summer.
  
  ![income_users_cohort](https://github.com/user-attachments/assets/14189e28-ded7-4830-a8a9-61b18739de14)

- **Retention Analysis**: May 2020 cohort showed the highest early retention, visualized through heatmaps.
  
  ![image](https://github.com/user-attachments/assets/19ab6a89-041d-4792-b13b-c8c941d42258)

- **Transaction Success**: Post-June 2020, transaction failures decreased, while October 2020 cohort generated the highest revenue.
  
  ![image](https://github.com/user-attachments/assets/2f72f493-8063-4ef4-9031-9027eba6d8d0)

- **Loan Amount & Frequency**: Positive correlation found, with larger loans linked to higher borrowing frequency.

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
