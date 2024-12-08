# Microcredit Churn Predictor

Customer behaviour analysis for Ironhack Payment, a financial services provider, to uncover insights into retention, revenue trends, and transaction success. Using Python, Pandas, and Plotly, I created cohort-based views that highlight customer lifecycle patterns and seasonal trends to support strategic growth.

![cohort_analysis_wallpaper](https://github.com/user-attachments/assets/e9fa25e2-33eb-4a1a-bd85-058d3717982b)

## Key Findings

- **Revenue by Cohort**: October 2020 cohort led in revenue, with strong seasonal growth patterns in spring and summer.
  
  ![income_users_cohort](https://github.com/user-attachments/assets/14189e28-ded7-4830-a8a9-61b18739de14)

- **Retention Analysis**: May 2020 cohort showed the highest early retention, visualized through heatmaps.
  
  ![retention_heatmap](https://github.com/user-attachments/assets/020a1480-e247-4b6e-9a09-eeab770ace2e)

- **Transaction Success**: Post-June 2020, transaction failures decreased, while October 2020 cohort generated the highest revenue.
  
  ![status_per_cohort](https://github.com/user-attachments/assets/df7e6194-f234-461e-a7e1-1c3adb1f57f8)

- **RFM Segmentation**: Identified high-value customer groups, providing insights for targeted retention strategies.
  
  ![user_ranking](https://github.com/user-attachments/assets/15e7531f-dfe6-4b45-9d71-6f31494ba0ff)

- **Loan Amount & Frequency**: Positive correlation found, with larger loans linked to higher borrowing frequency.

## Files

- **Exploratory Analysis** - [Exploratory_Analysis.ipynb](./Exploratory_Analysis.ipynb): Initial data cleaning and preparation.
- **Main Analysis** - [Main.ipynb](./Main.ipynb): Cohort analysis and visualizations.

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
