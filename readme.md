# Ironhack Payments: Cohort Analysis Project

![Ironhack Logo](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

[Google Slides Presentation](https://docs.google.com/presentation/d/1_L4GUAM97lEYs5Hsi1Z-n9deOiAW1OBkdNPWSkRmq7s/edit?usp=sharing)

## Project Background and Goals

This project is a cohort analysis for Ironhack Payment, a financial services company providing cash advance solutions since 2020. My objective was to analyze customer behavior over time and offer insights into patterns like user retention, revenue trends, and transaction success rates. By exploring these data-driven insights, Ironhack Payment can better understand customer lifecycle and refine its business strategy.

I used Python as the primary tool, with Pandas for data manipulation and Plotly for visualizations. Cohorts were defined by each customer’s first transaction month, allowing a month-by-month look into specific customer behaviors.

## Project Files

- **Exploratory Analysis** - [Exploratory_Analysis.ipynb](./Exploratory_Analysis.ipynb): Code for data cleaning and initial exploratory analysis.
- **Main Analysis** - [Main.ipynb](./Main.ipynb): Code for the main cohort analysis, including calculations and visualizations.
- **Detailed Report** - [Detailed Report](https://docs.google.com/document/d/1x_SGMHIXYSq7ZKbDT0LDCKbsVLg8nutCPDme0G9rrhA/edit?usp=sharing)
- **Presentation** - [Google Slides Presentation](https://docs.google.com/presentation/d/1_L4GUAM97lEYs5Hsi1Z-n9deOiAW1OBkdNPWSkRmq7s/edit?usp=sharing)

## Key Steps and Insights

### Data Cleaning and Preparation
To prepare for analysis, I focused first on organizing and cleaning the data in `Exploratory_Analysis.ipynb`. I removed duplicates, filled missing values, and standardized date formats to build the cohort structure. This preparation laid the groundwork for a detailed cohort analysis.

### Main Analysis

In the main analysis, documented in `Main.ipynb`, I created cohorts based on each client’s first transaction month and calculated specific metrics to track trends over time. Here are some of the insights I found:

1. **Total Revenue by Cohort**  
   Analyzing revenue by cohort highlighted trends in customer growth and seasonal behaviors. For instance:
   - The January 2019 cohort led in revenue and total users.
   - The October 2020 cohort saw the highest increase in new users month-over-month.
   - A seasonal pattern was observed, with significant user growth during spring, peaking in summer and fall.

2. **Retention Rate by Cohort**  
   Using a retention heatmap, I found that the May 2020 cohort had the highest retention rate after the first month. Visualizing retention rates provided insight into customer loyalty over time.

3. **Incident Rate by Cohort**  
   By examining transaction success rates, I noticed that failed transactions decreased after June 2020. Additionally, the October 2020 cohort generated the highest revenue, despite a high volume of transactions.

4. **RFM (Recency, Frequency, Monetary) Analysis**  
   I applied the RFM model to segment customers based on recency (time since the last transaction), frequency (purchase frequency), and monetary value (spending). This segmentation highlighted high-value customer groups for potential retention strategies.

5. **Correlation Between Loan Amount and Transaction Frequency**  
   Lastly, I explored the correlation between loan amount and transaction frequency, finding a positive relationship—customers who borrowed larger amounts tended to borrow more frequently over time.

## Conclusions and Reflections

Through this analysis, I gained valuable experience in cohort analysis, data visualization, and RFM modeling. This project not only provided actionable insights for Ironhack Payment but also reinforced my skills in structuring and interpreting data to inform business decisions.

I hope these findings and recommendations help Ironhack Payment in their strategy, and I appreciate your time in reviewing my project!

Thank you!

---

Feel free to reach out if you have any questions or feedback.

