&#x20;**Customer Churn Analysis Dashboard**



**📊 Project Overview**



This project analyzes customer churn for a telecommunications company using Power BI. The goal is to understand why customers leave, identify high-risk customer segments, evaluate the financial impact of churn, and provide actionable business recommendations.



The analysis transforms customer-level data into an interactive Power BI dashboard that helps management understand customer behavior and make data-driven retention decisions.





&#x20;**🎯 Business Problem**



Customer churn can significantly affect revenue and long-term business growth.



The business wants to understand:



* How many customers are churning?
* What is the overall churn rate?
* Which customer segments have higher churn?
* Are newer customers more likely to leave?
* Which contract types have the greatest churn?
* Which internet service segments have higher churn?
* What is the historical revenue associated with churned customers?
* What actions can the company take to improve customer retention?







&#x20;**📁 Dataset**



The project uses the **Telco Customer Churn** dataset.



The dataset contains customer demographic information, account information, services, charges, tenure, and churn status.



Key columns include:



* CustomerID
* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Contract
* Internet Service
* Payment Method
* Monthly Charges
* Total Charges
* Churn







**🛠️ Tools \& Technologies**



* **Power BI Desktop**
* **Power Query**
* **DAX**
* **Data Cleaning**
* **Data Visualization**
* **Data Analysis**
* **Microsoft Excel / CSV**
* **GitHub**







&#x20;📊 **Dashboard Pages**



**1. Executive Overview**



Provides a high-level view of customer churn and business performance.



Key metrics:



* Total Customers: **7,043**
* Active Customers: **5,174**
* Churned Customers: **1,869**
* Churn Rate: **26.5%**



Visuals include:



* Churn by Contract Type
* Churn by Internet Service
* Churn by Payment Method
* Churn by Tenure



**2. Customer Analysis**



Analyzes customer characteristics associated with churn.



Visuals include:



* Churn by Gender
* Churn by Senior Citizen
* Churn by Tenure Group
* Churn by Partner
* Churn by Dependents



A custom tenure grouping was created:



* 0–12 Months
* 13–36 Months
* 37+ Months



**3. Revenue Analysis**



Examines the financial characteristics of churn.



Key metrics:



* Total Revenue: **$16.06M**
* Churned Revenue: **$2.86M**
* Average Monthly Charges: **$64.76**
* Churned Revenue Share: **17.8%**



Visuals include:



* Revenue by Churn Status
* Revenue by Contract Type
* Churned Revenue by Contract
* Average Monthly Charges by Churn
* Revenue by Internet Service
* Churned Revenue by Internet Service



**4. Recommendations**



Summarizes the major findings and translates the analysis into business actions.



**💡 Key Findings**



**1. New Customers Are at Higher Risk**



Customers with **0–12 months of tenure** have the highest churn count.



**Recommendation**: Strengthen onboarding and provide additional support during the first year.



**2. Month-to-Month Customers Require Attention**



Month-to-month customers have the highest churned revenue in the analysis.



**Recommendation**: Explore retention incentives and encourage customers to consider longer-term contracts.



**3. Fiber Optic Is a High-Value Risk Segment**



Fiber optic customers generate the highest total historical revenue and also have the highest churned revenue.



**Recommendation**: Investigate fiber-optic pricing, service quality, customer satisfaction, and support.



**4. Churned Customers Have Higher Average Monthly Charges**



Customers who churned have a higher average monthly charge than customers who stayed.



**Recommendation**: Review pricing, plan value, and customer expectations among higher-charge customers.





&#x20;📈 **DAX Measures**



Examples of DAX measures created for the analysis include:



**Total Revenue =**

SUM(Churn\_Data\[TotalCharges])



**Churned Revenue =**

CALCULATE(

&#x20;   SUM(Churn\_Data\[TotalCharges]),

&#x20;   Churn\_Data\[Churn] = "Yes"

)





**Average Monthly Charges =**

AVERAGE(Churn\_Data\[MonthlyCharges])







**Churned Revenue % =**

DIVIDE(

&#x20;   \[Churned Revenue],

&#x20;   \[Total Revenue],

&#x20;   0

)





A calculated tenure group was also created to segment customers by relationship length.







🎯 **Business Recommendations**



Based on the analysis, the company should:



1\. Strengthen onboarding for new customers.

2\. Develop targeted retention strategies for month-to-month customers.

3\. Investigate the customer experience of fiber-optic users.

4\. Review pricing and plan value for higher-charge customers.

5\. Monitor churn rates across customer segments regularly.

6\. Use customer segmentation to identify high-risk customers earlier.



\-



🖼️ **Dashboard Screenshots**



**Executive Overview**



Executive\_Overview.png



**Customer Analysis**



Customer\_Analysis.png



**Revenue Analysis**



Revenue\_Analysis.png



**Recommendations**



Recommendations.png







📌 **Skills Demonstrated**



This project demonstrates practical experience with:



* Data cleaning and preparation
* Power Query
* DAX
* KPI development
* Data modeling
* Customer segmentation
* Churn analysis
* Revenue analysis
* Business intelligence
* Data visualization
* Business storytelling
* Translating data insights into recommendations







**🚀 Project Outcome**



The analysis identified key customer segments associated with churn and highlighted areas where the business can focus its retention efforts.



The project demonstrates an end-to-end analytics workflow:



**Raw Data → Data Cleaning → DAX → Analysis → Visualization → Business Insights → Recommendations**

