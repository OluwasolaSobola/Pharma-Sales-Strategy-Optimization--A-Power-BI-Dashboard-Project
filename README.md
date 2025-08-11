<img width="847" height="470" alt="image" src="https://github.com/user-attachments/assets/cfa2991e-c388-43a9-951a-a2ff0a45edd8" />

### Table of Content
---

- [Description](#description)
- [Business Introduction](#business-introduction)
- [Problem Statement](#problem-statement)
- [Aim of this Project](#aim-of-this-project)
- [Processes / Methodologies Used](#processes--methodologies-used)
- [Data Modeling](#data-modeling)
- [Visualization](#visualization)
  - [KPIs](kpis)
  - [Area Chart](#area-chart)
  - [Clustered Bar Chart](#clustered-bar-chart)
  - [Clustered Column Charts](#clustered-column-charts)
  - [Donut Chart](#donut-chart)
  - [Map](#map)
  - [Stacked Area Chart](#stacked-area-chart)
- [Dashboard Review](#dashboard-review)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Tools & Techniques Used](#tools--techniques-used)
- [Techniques](#techniques)

### Description
---
This Power BI dashboard provides a comprehensive analysis of NovaMed Solutions’ sales data (2022–2026), uncovering trends in revenue, profitability, drug performance, and customer demographics. It enables data-driven decision-making in sales strategy, inventory management, and targeted marketing.

### Business Introduction
---
NovaMed Solutions is a leading pharmaceutical distributor committed to the timely delivery of essential medications to healthcare providers across diverse markets. With a focus on operational excellence, NovaMed bridges the gap between manufacturers and medical institutions through reliable distribution, strategic inventory management, and responsive customer service. Leveraging data-driven practices, the company optimizes supply chain performance, adapts to evolving market demands, and ensures consistent access to high-quality pharmaceutical products—supporting better health outcomes.
### Problem Statement
---
NovaMed Solutions encountered challenges in enhancing sales performance and customer engagement, driven by limited visibility into product-level trends, inaccurate demand forecasting, and fragmented customer data. These obstacles resulted in inefficient inventory management, lost revenue potential, and difficulty pinpointing critical growth opportunities. To overcome these issues, the company required a centralized, data-driven solution to track performance, gain deeper customer insights, and support informed strategic decision-making.
### Aim of this project
---
The primary objectives of this project are as follows: 

- Develop a centralized and interactive Power BI dashboard to streamline sales analysis 
- Track trends in revenue, profit, and costs across different products and time periods
- Identify top and bottom-performing drugs through dynamic ranking features 
- Analyze customer demographics, including age, gender, and country
- Enhance visibility into overall market performance and customer behavior
- Support data-driven decision-making in sales strategy and inventory planning
  
### Processes / Methodologies Used
---
**Business Understanding:** The project was initiated to analyze NovaMed Solutions’ sales performance, product profitability, and customer demographics with the goal of uncovering actionable trends, reducing operational inefficiencies, and enabling data-driven decision-making.

**KPI Development:** Key performance indicators were defined and implemented, including Revenue, Profit, Profit Margin, Quantity Sold, COGS, and Average Revenue per Customer. Dynamic DAX measures were developed to support month-over-month (MoM) trend analysis and identify top/bottom-performing products.

**Data Understanding:** Conducted an in-depth review of sales, product, and customer datasets spanning 2022 to 2026 to understand key metrics such as revenue, profit, quantity sold, buyer segments, and demographic distributions.

**ETL Process:** Executed a full ETL process by extracting raw data, transforming it in Power Query (including removing duplicates, changing data types, and generating time-based columns), and loading the cleansed data into Power BI for modeling and analysis.

**Data Modeling:** Built a robust star schema data model consisting of fact and dimension tables, defined relationships, and created calculated columns and DAX measures to enable dynamic KPI computation and performance ranking.

**Visualization & Insight Generation:** Designed interactive Power BI dashboards to showcase top and bottom product performance, MoM sales trends, and customer insights by gender, age, and region. Enhanced user experience through intuitive filters and slicers, enabling deep-dive analysis and strategic insights.

### Data Modeling
---
The project adopts a star schema architecture to ensure efficient, scalable, and high-performance analysis within Power BI. At the center of the model is a comprehensive Fact Table capturing transactional sales data, including key metrics such as Revenue, Quantity Sold, Cost of Goods Sold (COGS), and Profit. It also includes relevant fields like buyer type, sales date, drug names and IDs, sales IDs, and customer IDs.

This Fact Table is linked to several Dimension Tables using unique identifiers:

**Customer Dimension:** Stores attributes such as customer name, customer ID, gender, age group, buyer type, and country.

**Product/Drug Dimension:** Contains details about each drug, including drug ID, drug name, unit sales price, unit production cost, and associated treatment information.

**Calendar Dimension:** Provides a structured time hierarchy (Year, Quarter, Month) to support time-series and month-over-month (MoM) analysis.

This relational model enables advanced filtering, slicing, and drill-down functionality within the dashboards. It supports accurate KPI aggregation and comparison across various customer segments, product categories, and time periods, driving deeper data exploration and more impactful business insights.

<img width="1916" height="930" alt="image" src="https://github.com/user-attachments/assets/304662d1-9a6c-4ab0-b2c7-a880779659cc" />


### Visualization

---

- KPIs
- Area Chart
- Clustered Bar Charts
- Clustered Column Charts
- Donut Chart
- Map
- Stacked Area Chart
  
### Data Analysis
---
**KPIs**

This dashboard highlights key performance indicators (KPIs) for Total Revenue, Total Profit, Cost of Goods Sold (COGS), Profit Margin, and Quantity Sold for NovaMed Solutions. From 2022 to 2026, the company generated $71.31 million in total revenue, achieving a total profit of $58.45 million, with COGS totaling $12.85 million. The overall profit margin was approximately 82% (81.97%), reflecting strong operational efficiency and effective pricing strategies. These KPIs underscore NovaMed’s solid sales performance, disciplined cost management, and its growing market presence over the five-year period.

<img width="1017" height="167" alt="KPI" src="https://github.com/user-attachments/assets/a29d128d-a599-4c38-bfdf-683a5a93372c" />

### Area Chart
---
**Monthly Revenue and Profit Analysis (2023 - 2026)**

NovaMed demonstrated strong overall financial performance from 2022 to 2026, with clear seasonal fluctuations in both revenue and profit throughout each year.

**Peak Performance Periods**: The months of January, July, and September consistently recorded the highest revenue and profit, indicating strong sales momentum. These spikes may be attributed to new product launches, bulk purchasing cycles, or strategically timed marketing campaigns.

**Underperforming Periods**: In contrast, the months of February, June, and October showed recurring declines in both revenue and profit, suggesting seasonal slowdowns, weaker demand, or potential operational inefficiencies during these periods.

<img width="506" height="283" alt="MONTHLY R   P PERFORMANCE COMPARISON" src="https://github.com/user-attachments/assets/391e0616-8858-4f2f-84ab-73909375e376" />

### Clustered Bar Chart
---
**Top & Bottom 10 Drugs Analysis by Revenue and Profit (Clustered Bar Chart)**

This clustered bar chart showcases the top and bottom 5 performing drugs based on both total revenue and total profit. It offers a clear side-by-side comparison of drug names with their corresponding revenue and profit values, making it easy to identify high performers such as Doxycycline and Ergocalciferol, as well as underperformers like Montelukast and Warfarin.

The visual enables quick ranking and comparison, supporting evidence-based decision-making in inventory planning, pricing strategies, and overall sales optimization.

<img width="512" height="275" alt="5 TOP   BOTTOM DRUG R AND P" src="https://github.com/user-attachments/assets/9eea68fa-9d0a-404a-886d-6cfc964cdaf0" />

### Clustered Column Charts
---
**Top 5 Performing Customers by Total Revenue and Contributions(Clustered Column Chart)**

This chart highlights NovaMed’s top 5 customers, ranked by their total revenue contributions. David Johnson leads the group, contributing $3.9 million in revenue, followed by other high-value clients such as Bob Williams, Jane Brown, and Bob Smith.

The visualization offers critical insights into NovaMed’s most profitable customer relationships, supporting targeted strategies in customer retention, personalized service delivery, and strategic upselling—especially among the highest spenders.

<img width="505" height="288" alt="image" src="https://github.com/user-attachments/assets/c702ae13-b24f-4620-93ec-bb21c618b56b" />

**Bottom 5 Performing Customers (Clustered Column Chart)**

This chart identifies the lowest performing customers based on total revenue and individual contributions. These clients exhibit minimal impact on sales despite remaining active in the system.

The visual plays a key role in uncovering engagement gaps, prompting a reevaluation of account strategies, and assessing whether these customers require targeted sales support, reactivation campaigns, or should be deprioritized to enable more efficient resource allocation.

<img width="512" height="288" alt="Underperformng Customers" src="https://github.com/user-attachments/assets/dc94894d-a635-45df-a61c-ffc479fb700c" />


**Customer Demographic by Age Group(Clustered Column Chart)**

This clustered column chart highlights customer engagement across demographic segments, showing that the Elderly Male group, aged 60+, is the most engaged segment with 3,283 customers. In contrast, the Children Female group, aged 18–25, is the least engaged segment, with only 166 customers. These insights enable NovaMed to tailor outreach, product offerings, and services to better serve its most active demographics while identifying opportunities to improve engagement among less represented groups.

<img width="465" height="257" alt="CUSTOMER DEMOGRAPHY" src="https://github.com/user-attachments/assets/276eceba-0b0b-42bb-a52e-a69cc804b365" />

### Donut Chart
**Average Revenue Per Customer Segment(Donut Chart)**

This donut chart illustrates that the Preferred Customers segment generates an average revenue of $4.69K per customer and contributes 35.76% of total revenue. As the most financially impactful segment, this insight helps NovaMed prioritize resources, enhance customer loyalty, and drive sustained revenue growth through targeted retention and engagement strategies.

<img width="518" height="265" alt="AVERAGE REVENUE PER CUSTOMER SEGMENT" src="https://github.com/user-attachments/assets/5515c34a-7f90-482b-8824-808ef708a4d7" />

### Clustered Bar Chart
**Revenue Distribution by Country and Customer Type**

This clustered bar chart displays revenue by country, revealing that Canada leads with $13.4 million, accounting for 31.67% of total revenue. Additionally, Preferred Customers dominate the revenue share across regions. The visualization highlights where NovaMed’s revenue is most concentrated, offering valuable insights for regional market prioritization, customer engagement planning, and resource allocation. This view enables decision-makers to focus retention and expansion strategies in countries with strong existing demand.

<img width="456" height="236" alt="REVENUE DISTRIBUTION BY COUNTRY AND CUSTOMER TYPE" src="https://github.com/user-attachments/assets/c1919289-6269-4da9-a191-0a9f0cd2da24" />

### Stacked Area Chart
**Revenue Trend by Gender and Age Group**

This stacked area chart reveals clear purchasing patterns by age and gender. The Elders (60+) Male segment shows the highest trend, generating $14.8 million in revenue. In contrast, the Children (18–25) Other segment has the lowest trend, contributing only $1.2 million. These insights highlight distinct customer behaviors, enabling NovaMed to tailor marketing and sales strategies to key demographic groups.

<img width="521" height="433" alt="REVENUE TREND BY AGE AND GENDER" src="https://github.com/user-attachments/assets/3e545f1d-d48c-4d8c-892c-c16913d9ce9c" />

### Map
**Geographical Insights - Top 2 Countries by Revenue(Map)**

This map highlights Canada and Australia as the top two revenue-generating countries. Canada leads, contributing 31.67% of total revenue, followed by Australia, which accounts for 15.25%. The geographic distribution offers strategic insight into NovaMed’s strongest markets, supporting region-specific planning and expansion efforts.

<img width="457" height="201" alt="Two Top Countries" src="https://github.com/user-attachments/assets/8bb1596f-3995-4bcd-bb17-2d67d58b8b5f" />

### Dashboard Review
---
The two interactive dashboards provide a comprehensive overview of NovaMed Solutions’ sales performance from 2022 to 2026. They uncover key trends in revenue, profit, and quantity sold across top and bottom-performing drugs, highlight monthly fluctuations, and deliver demographic and geographic insights into the customer base.

From identifying high-value drugs like Doxycycline and Ergocalciferol, and analyzing customer segments by age, gender, and country, to tracking sales by buyer type and visualizing profit trends over time, these dashboards support data-driven decision-making across marketing, inventory planning, and strategic initiatives.

Together, they serve as a dynamic tool for identifying growth opportunities, addressing inefficiencies, and optimizing overall commercial performance.

**Top/Bottom Sales Analysis**

<img width="1120" height="742" alt="TOP AND BOTTOM SALES ANALYSIS" src="https://github.com/user-attachments/assets/6db8d5ff-5456-4f4b-b02f-b8cb15a9c2f6" />


**Customer Analysis**

<img width="1086" height="743" alt="CUSTOMER ANALYSIS DASHBOARD" src="https://github.com/user-attachments/assets/5d40b31b-688a-48f3-8c75-b643ac179769" />

###  Key Insights
---

- **Top-Performing Products:** Doxycycline leads as the top-performing drug, generating the highest revenue and profit, making it a critical product for business growth. The top 5 drugs collectively account for a significant portion of total revenue, while several underperforming drugs deliver minimal returns—highlighting an opportunity to streamline NovaMed’s product portfolio.

- **Seasonal Trends:** January consistently records peak revenue and profit, indicating strong seasonal performance at the start of each year. In contrast, February, June, and October show noticeable dips, signaling the need for further analysis and potential seasonal strategy adjustments.

- **Customer Value:** High-value customers like David Johnson and Bob Williams contribute millions in revenue, emphasizing the importance of customer retention and personalized engagement strategies.

- **Geographic Performance:** Canada’s Preferred Customer segment leads with $13.7M in revenue, followed by Australia, positioning both as NovaMed’s strongest geographic markets.

- **Demographic Insights:** Male customers aged 60+ dominate the customer base and purchasing behavior, generating $14.76M in revenue alone. This demographic represents NovaMed’s most valuable segment, driving the highest revenue and requiring tailored engagement strategies.

- **Buyer Type Behavior:** In key markets like Canada and Australia, seller-type customers account for the majority of revenue, with minimal contribution from end-users. This reveals distinct purchasing patterns and highlights the need for differentiated go-to-market strategies by buyer type.

- **Financial Performance:** NovaMed achieved a strong profit margin of 82%, reflecting excellent operational efficiency and an effective pricing strategy across its portfolio. Over the five-year period, total revenue reached $71.31M, with 269K units sold, signaling robust overall performance and continued growth potential.

### Recommendations
---
**Strategic Insights & Recommendations**

Based on a comprehensive analysis of financial KPIs, customer demographics, regional trends, and product-level performance, the following strategic recommendations are proposed to help NovaMed Solutions drive revenue growth, enhance customer retention, and improve operational efficiency.

**Key Financial Metrics (2022–2026)**
- Total Revenue: $71.31M
- Total Profit: $58.45M
- Profit Margin: 82%
- Cost of Goods Sold (COGS): $12.85M
- Quantity Sold: 269,000

**Sales Strategy: Accelerate Revenue Growth**
- Prioritize high-performing drugs such as Doxycycline, Ergocalciferol, and Lisinopril, which deliver strong revenue and profitability.
- Reevaluate low-margin, high-volume drugs like Warfarin and Montelukast for pricing adjustments, cost control, or portfolio   optimization.
- Capitalize on monthly sales trends to strategically time promotions, campaigns, and seasonal inventory planning.
- Use the dashboard’s segmentation tools to uncover emerging revenue drivers by product, region, or buyer type, enabling more targeted   decision-making.

**Customer Strategy: Enhance Retention & Engagement**
- Prioritize high-value demographics, particularly elderly male customers, who represent the top-spending segment.
- Launch targeted campaigns to engage underperforming customer groups, such as female children, to boost inclusivity and growth.
- Expand Preferred Customer programs, which currently contribute 35.76% of total revenue, to further strengthen customer loyalty.
- Leverage customer insights to personalize loyalty offers, communications, and onboarding experiences, enhancing long-term retention.

**Operational Strategy: Boost Efficiency**
- Maintain focus on cost discipline to preserve the strong 82% profit margin.
- Optimize inventory planning using drug demand trends and seasonal sales patterns to reduce waste and improve availability.
- Implement automated alerts and exception reporting to quickly identify and respond to underperforming drugs or lagging regional markets, supporting proactive decision-making.

### Tools & Techniques Used
---

**Data was analyzed using Power BI, leveraging the following techniques:**
**Tools:**
- **Excel –** Used as the raw data source (sales, customer, and product data).
- **Power BI –** Main platform for data transformation, modeling, and visualization.
- **Power Query –** For cleaning and preparing data directly within Power BI.
- **DAX (Data Analysis Expressions) –** For creating dynamic KPIs, calculations, and ranking logic.

### Techniques
---

- Data Transformation & Cleaning
- Organized raw Excel data using Power Query (e.g., removing nulls, renaming fields,merging tables)
- Data Modeling
- Established relationships across tables (Sales, Drugs, Customers) for interactive slicing and filtering
- KPI & Metric CalculationsDeveloped key measures like Quantity Sold, Revenue, COGS, Profit, and Profit Margin
- Top N / Bottom N Ranking
- Applied DAX to dynamically rank drugs and customers by revenue and profit
- Segmentation
- Grouped customers by Age Range, Gender, and Buyer Type for targeted analysis
- Time Intelligence
- Used Month-over-Month comparisons to track performance trends over time
- Geospatial Visualization
- Used map visuals to display revenue distribution across countries
- Root Cause Analysis (5 Whys)Applied root cause thinking to uncover underlying issues in low-performing areas

<img width="838" height="477" alt="image" src="https://github.com/user-attachments/assets/53130ccb-ee54-42a6-80d9-6db82fd0741b" />
