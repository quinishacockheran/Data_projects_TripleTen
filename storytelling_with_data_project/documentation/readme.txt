--------------------
README: Superstore Return Analysis - Storytelling with Data: Project
--------------------

Project Overview:
-----------------
This project investigates the root causes behind the high number of returned orders at the Superstore. Designed for the CEO, the analysis aims to uncover customer return behaviors and identify actionable strategies to reduce returns. Using the Superstore dataset (Superstore.xls), various visualizations were developed in Tableau to explore correlations between returns, sales, customer segments, geography, and time.

Project Components:
-------------------
1. **Data Files:**
   - **Superstore.xls:** Contains multiple tables including Orders, Returns, and supplementary data such as product and customer details.
   - *Note:* The Returns table was left-joined onto the Orders table to capture both “Yes” and null values in the Returned column. A calculated field was then created to convert null values to 0 and “Yes” to 1, where the average of this field represents the return rate.

2. **Visualizations & Analysis:**
   - **What is Causing Returns?**
     - **Scatterplot:** Correlates total sales with total returns, aggregated by product subcategory, to assess if higher sales always lead to higher returns.
     - **Bar Chart:** Displays the return rate by product category.
     - **Customer Analysis:** Visualizes the return rate by customer (filtering out those with only 1 order) to identify high-risk segments.
     - **Geographic Analysis:** A map showing return rates by a geographic measure (e.g., state or city) to detect regional patterns.
     - **Time Series Analysis:** Examines return rates over time (by month or week) to uncover any seasonal effects.
     - **Composite Charts:** Combines multiple factors (such as date, geography, and product category) to further explore the drivers of returns.
   
   - **Dashboard for Monitoring Returns:**
     - **Low-Fidelity Mock-Ups:** Pen-and-paper sketches (3 variations) were created and refined into a dashboard template in Tableau.
     - **Final Dashboard:** The dashboard integrates all key visualizations and is designed to clearly present insights and facilitate interactive exploration.
   
   - **Presentation & Storytelling:**
     - A draft story arc with captions outlining the key points of the analysis.
     - A finalized Tableau Story incorporating the visualizations, interactive filters, and narrative captions.
     - A recorded (or PDF) presentation summarizing the analysis, interpretation of the dashboard, and recommended next steps.

3. **Documentation:**
   - This README file.
   - Storytelling with Data Rubric

Methodology:
------------
1. **Data Preparation:**
   - Imported the Superstore dataset into Tableau.
   - Joined the Returns table onto the Orders table using a LEFT JOIN.
   - Created a calculated field for the Returned column (null → 0; "Yes" → 1) to measure return rates.

2. **Analysis:**
   - Developed multiple worksheets to analyze return rates from different perspectives (product, customer, geography, and time).
   - Aggregated and visualized data to identify correlations between sales volume and returns.
   - Constructed composite charts to explore the interplay between various factors influencing return rates.
   - Built a cohesive dashboard template that integrates all individual analyses into a comprehensive narrative.

Key Insights & Recommendations:
-------------------------------
- **Sales vs. Returns:** While higher sales volumes tend to correlate with higher returns, certain product subcategories exhibit disproportionately high return rates.
- **Customer & Product Analysis:** Specific customer segments and product categories are identified as having elevated return rates, signaling potential areas for operational review.
- **Geographic & Seasonal Trends:** Significant regional concentrations and seasonal patterns in returns were observed, indicating targeted opportunities for intervention.
- **Strategic Actions:** Recommendations include discontinuing problematic products, refining return policies, and enhancing customer service to address high return rates.

How to View the Project:
-----------------------------
- **Tableau Public Dashboard:**
  1. Click the following link to access the interactive dashboard: [https://public.tableau.com/app/profile/quinisha.cockheran/viz/storytelling_with_data_project/SuperstoreReturnAnalysis]
- **Project Files:**
  - Download files.
  - The provided visualizations and documentation offer a detailed walkthrough of the analysis and findings.

Future Improvements:
--------------------
- Integrate additional dimensions and predictive analytics to forecast future return trends.
- Enhance the dashboard with further interactive features and drill-down capabilities.
- Refine calculated fields and data transformations to further improve analysis accuracy.

Contact Information:
--------------------
Project Lead: Quinisha Cockheran  
LinkedIn: [Quinisha Cockheran](https://www.linkedin.com/in/quinisha-cockheran)

--------------------
End of README
--------------------
