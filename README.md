---
# **Business Intelligence project: Strategic Insights for a Bike Share Company**
Business intelligence analysis of a Bike share company bike usage using ETL, SQL, and dashboards to generate actionable insights.



### 
<div style="text-align: center;"><img src="Bike_Share.jpg" alt="Example Image" width="800"/></div>

---
### **Project Overview**
This project aims to enhance Cyclistic’s strategic decision-making by analyzing rider behavior using Business Intelligence (BI) tools. The analysis follows a structured five-phase approach, covering data extraction and preparation, exploratory data analysis (EDA), key performance indicator (KPI) development, dashboard creation, and actionable insights. By leveraging trip data, user demographics, and ride patterns, this project provides a data-driven approach to optimize marketing strategies and increase member conversion rates.

### **Business Understanding**
Cyclistic, a bike-share program in Chicago, aims to convert casual riders into annual members by understanding usage patterns and user behavior. The stakeholders in this project include Cyclistic’s marketing team and executive leadership, who can use the insights generated to inform targeted marketing campaigns and operational improvements.

### **Data Understanding**
- The dataset consists of trip records, including start and end times, ride duration, start and end stations, user type (casual or member), and bike type.
- The analysis covers multiple months of data to capture seasonal trends and user behaviors.
- Key data challenges included missing values, inconsistent timestamps, and data standardization, which were addressed during preprocessing.
- Exploratory Data Analysis (EDA) revealed differences in trip durations, station popularity, and peak usage times between casual riders and members.

### **BI Process and Analysis**
- **Phase 1: Data Preparation** – Extracting, cleaning, and transforming raw trip data for structured analysis.
- **Phase 2: Exploratory Data Analysis (EDA)** – Identifying trends in ride duration, station usage, and user segmentation.
- **Phase 3: KPI Development** – Defining key metrics such as average trip duration, most popular stations, peak usage hours, and member conversion rates.
- **Phase 4: Dashboard Creation** – Building interactive visualizations in Tableau/Power BI to provide stakeholders with real-time insights.
- **Phase 5: Strategic Insights** – Recommending marketing strategies based on data-driven findings, such as targeting high-usage areas for membership promotions.

#### **1 -Project Documents**
The Project requirements document describes the overall purpose of the Cyclistic project, including its goals and key dependencies. The Stakeholder requirements document outlines key stakeholder needs for developing a BI dashboard. It focuses on understanding customer usage patterns and demand at bike stations to guide strategic decisions for expansion and improvement. The Strategy document details the BI dashboard development plan, including data sources, user profiles, and dashboard features. It outlines access restrictions, data scope, and key metrics like heat maps and area charts to analyze bike usage, seasonal trends, and weather impacts. The document is in draft and has to be reviewed before implementation.

- [Project requirements document (here)](Project_Documents/Cyclistic_Bike_share_Project_requirements.pdf)
- [Stakeholder requirements document (here)](Project_Documents/Cyclistic_Bike_Share_Sakeholders_req.pdf)
- [Strategy document (here)](Project_Documents/Cyclistic_Bike_share_Strategy_Document.pdf)

#### **2 -ETL code and SQL documents**
I created the queries for this scenario using BigQuery and leveraged BigQuery’s public datasets to develop the analysis. This approach allowed me to utilize large datasets for comprehensive insights and effective scenario modeling. Also, i uploaded an additional file with the zip codes in NYC. 
The annual query was designed to retrieve annual relevant data; but i had a problem, the zip codes coordinates were not recognized by Tableau, so i had to include them in que query. However, including variables such as stations and coordinates resulted in an excessively large file size that was impractical for download. Therefore, the coordinates were included in a second query to manage the data more efficiently.
Finnaly, the summer query was performed without problems.

- [Zip codes data (here)](ETL_SQL/Cyclistic_NYC_zip_codes.csv)
- [Annual Query (here)](ETL_SQL/Cyclistic_query_2022_2023.txt)
- [Zip code coordinates Query (here)](ETL_SQL/Cyclistic_year_end_lat_long_query.txt)
- [Summer Query (here)](ETL_SQL/Cyclistic_summer_query.txt)

#### **3- Dashboards**
Before creating the dashboards, some calculations were first performed in Tableau

[Relationships (here)](Tableau_doc/Data_relationships_tableau.pdf)

[Dashboards in Tableau (here)](https://public.tableau.com/app/profile/francisco.navarro7243/viz/CyclisticBike-ShareTrends/Story1)

#### **4 - Business Sumary**
This summary highlights how subscribers and non-subscribers differ in their usage, seasonal trends in bike usage, and the impact of weather conditions. It also provides actionable insights for strategic bike station placement, congestion management, operational adjustments, marketing, and service optimization to enhance overall performance and customer experience. Please follow the link for the full Business Summary

[Business Sumary (here) ](business_summary/Cyclistic_business_summary.pdf)

### **Conclusion**
This BI project provides Cyclistic with actionable insights into rider behavior, enabling data-driven decision-making to enhance user engagement and increase membership conversions. Future improvements may include integrating additional data sources (e.g., weather patterns, event calendars) and refining segmentation models to optimize targeted campaigns further.

