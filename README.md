# **Customer Growth Analytics: An End-to-End Analysis**

This repository contains an end-to-end data analytics project focused on analyzing customer purchase activity to identify key drivers for strategic growth. The core objective was to move beyond descriptive reporting to uncover actionable insights that can optimize marketing, product, and customer engagement strategies for a leading retail enterprise.

This project demonstrates a full analytical workflow, from initial data engineering in Python to advanced database querying in SQL, culminating in an interactive Power BI dashboard.

## **🎯 Business Problem & Objectives**

The primary business challenge was to understand shifting consumer purchasing patterns to maintain a competitive edge. The project aimed to move from *what* was happening to *why* it was happening by identifying the causal factors (like discounts, product ratings, and payment methods) that drive consumer decisions and repeat purchases.

The analysis was guided by key business questions:

* Which customer segments (by gender, age group, location) are the most profitable?  
* What is the real impact of the subscription program on revenue and customer spending?  
* Which products are top performers (by sales, rating) and which are under-performers?  
* How do shipping preferences and payment methods correlate with customer loyalty and purchase frequency?

## **🛠️ Tech Stack**

* **Python:** Used for data cleaning, transformation, and feature engineering (primarily using Pandas).  
* **PostgreSQL (SQL):** Employed for data storage and executing 17 advanced analytical queries to segment data and extract insights.  
* **Power BI:** Used to build the final interactive dashboard and visualize key findings.  
* **Jupyter Notebook:** Served as the environment for the Python-based ETL process and Exploratory Data Analysis (EDA).

## **🗂️ Project Workflow**

1. **Project Initiation:** Defined the business problem, objectives, and analytical roadmap.  
   * *See: Project Initiation Brief.pdf*  
2. **Data Engineering (ETL):** The raw purchase\_activity.csv dataset (3,900 records, 18 columns) was loaded into a Jupyter Notebook (CLV\_Analysis.ipynb). The data was cleaned and transformed using Pandas, which involved:  
   * Handling missing values (imputing Review Rating with the category median).  
   * Standardizing column names (to snake\_case).  
   * Engineering new features, such as age\_group, for better segmentation.  
   * Checking for data consistency and dropping redundant columns.  
3. **Database & SQL Analysis:** The cleaned DataFrame was loaded into a PostgreSQL database named clv\_analysis (in a table named consumer). All 17 advanced SQL queries were written and executed (CLV\_Analysis.sql) to answer the core business questions.  
4. **Visualization & Insights:** Key findings and query results were consolidated into an interactive Power BI dashboard (consumer\_insights\_dashboard.pbix) for stakeholder exploration.  
5. **Reporting & Recommendations:** A comprehensive report (Consumer Growth Analytics.pdf) and presentation (Project Presentation.pdf) were created to summarize the findings and provide actionable business recommendations.

## **💡 Key Insights & Recommendations**

The analysis uncovered several high-impact insights:

* **High-Value Segments:** Male customers account for **68% of total revenue**, and the **"Young Adult"** demographic is the highest-earning age group.  
  * **Recommendation:** Develop targeted marketing campaigns and product bundles for these high-value segments.  
* **Subscription Paradox:** Non-subscribers ($170.4K revenue) generate significantly **more revenue** than subscribers ($62.6K).  
  * **Recommendation:** Re-evaluate the subscription program's value proposition. It is currently not a key driver for high-value customers.  
* **Loyalty Drivers:** Customers using modern payment methods (PayPal, Credit/Debit) average more lifetime purchases than those using cash, indicating higher digital engagement.  
  * **Recommendation:** Promote and incentivize the use of digital payment methods to encourage repeat purchases.  
* **Product Performance:** The "Clothing" category is the top performer in both sales and revenue.  
  * **Recommendation:** Investigate low-rated products to address quality or expectation gaps and prevent customer churn.

## **📂 Repository Artifacts**

* CLV\_Analysis.ipynb: Jupyter Notebook containing the full Python ETL and data cleaning process.  
* CLV\_Analysis.sql: Contains all 17 advanced SQL queries used for the analysis.  
* purchase\_activity.csv: The raw, unprocessed dataset used as the project's foundation.  
* consumer\_insights\_dashboard.pbix: The final, interactive Power BI dashboard file.  
* Project Initiation Brief.pdf: The original document outlining the project's problem statement, goals, and scope.  
* Consumer Growth Analytics.pdf: The final, detailed project report summarizing the methodology, findings, and recommendations.  
* Project Presentation.pdf: An executive-level presentation of the project's key insights.  
* LICENSE: MIT License.

## **👨‍💻 Connect with the Author**

This project was created by **Arnav Bhomia**.

Feel free to connect on [LinkedIn](http://www.linkedin.com/in/arnavbhomia) to discuss this project, data analytics, or potential opportunities\!
