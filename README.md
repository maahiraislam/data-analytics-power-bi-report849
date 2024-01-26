# data-analytics-power-bi-report849
## Description
Welcome to the Power BI Retail Insights project! In this initiative, my role was to enhance how a medium-sized international retailer utilizes data for decision-making. They've accumulated sales data from various sources across the globe, and my task was to transform it into valuable insights. The project involved aggregating sales data from diverse sources worldwide and crafting meaningful visualizations to aid decision-making.

### Project Overview:

The data has been meticulously gathered and organized from various sources, and a robust data model has been established to facilitate seamless analysis.

### Quarterly Report:

A user-friendly Quarterly report has been generated, providing executives with key insights for informed decision-making.

### Customer Insights:

In-depth analysis has been conducted to understand the retailer's top customers in different regions. Valuable insights have been gleaned, shedding light on customer preferences.

### Product Analysis:

Thorough examination of the performance of top-selling products against sales targets has been completed. Successful products have been identified, and areas for improvement have been highlighted.

### Geographic Performance Map:

An interactive map visualization has been developed, showcasing the performance metrics of retail outlets in different regions. This visual aid offers insights into geographic trends and opportunities.

## Tasks Accomplished During the Project:

1. Importing the Data into Power BI:
   - Loaded/Imported and transformed the following Tables:
     - Orders
     - Products
     - Stores
     - Customers
   - Used the following tools and features to clean/transform the data:
     -  Split Column Feature
     -  Removing missing/null values
     -  Renaming Columns
     -  Deleting Columns
     -  Merged Columns
     -  Column from Examples Feature
     -  Replacing Values
     -  Created new Calculated Columns
       
 2. Creating the Data Model:
      - In this analysis, a comprehensive date table was established in Power BI using DAX formulas to enhance time-based analytics:
         - This table, named "Dates" covers the earliest date in the Orders['Order Date'] to the latest in Orders['Shipping Date']. It's a handy tool for time-based analysis in our reports.
         - Added some key date-related info to make our analysis even more insightful. The "Day Of Week" column tells us the day of the week, "Month Number" gives the month in a number format, and "MonthName" tells us the full month name. "Quarter" helps us analyze data by quarters, and "Year" simply shows the year.
         - Also included columns for specific reference points in time. "Start Of Year" shows the beginning of each year, "Start Of Quarter" marks the start of each quarter, and "Start Of Month" pinpoints the start of each month. Lastly, "Start Of Week" gives a reference point at the beginning of each week.
         - This straightforward date table is like a time compass for our Power BI model, making it easier to explore and analyze data trends over time. These added date-related details makes the report more meaningful and user-friendly for everyone involved.
         - These DAX functions were used to create a date table and add various date-related columns to facilitate time-based analysis in the Power BI model:
      
            - ADDCOLUMNS
            - CALENDER
            - MIN
            - MAX
            - FORMAT
            - YEAR
            - QUARTER
            - MONTH
            - WEEKDAY
            - DATE
      - Established relationships between different tables to create a star schema in the Power BI model. The connections are as follows:
        ![image](https://github.com/maahiraislam/data-analytics-power-bi-report849/assets/148975841/04276fae-b1c3-4e17-966a-97c3a6e4dd13)
      - Have created a set of key measures that will serve as a starting point in building the report. The following DAX functions were used to create key measures and calculated columns:

        - DISTINCTCOUNT
        - TOTALYTD
        - COUNTROWS
        - SUMX
        - RELATED
          
   3. Building the Customer Detail Page:
      - Created a report page focusing on customer level analysis. The following visuals were created:
         - **Card visuals** for total distinct customers and revenue per customer
         - **Line chart** of weekly distinct customers
         - **Table** showing the top 20 customers by total revenue, showing the revenu per customer and the total orders for each customer
         - **Donut chart** showing number of customers by country
         - **Bar chart** showing number of customers by product category
         - **Three card visuals** showing the name, number of orders, and revenue for the top customer by revenue.
         - **Data Slicer**
         - The final layout is given as follows:
           
           ![image](https://github.com/maahiraislam/data-analytics-power-bi-report849/assets/148975841/df444112-25ec-4061-8944-c993d61d5017)
           
   4. Created a report page for the high-level executive summary. This gives an overview of the company peroformance as a whole. The following visuals were created:
      - Card visuals showing Total Revenue, Total Profit and Total Orders
      - Line graph of revenue against time
      - Donut charts showing orders and revenue by country
      - Bar chart of orders by category
      - KPI's for Quarterly revenue, customers and profit
      - Table of the top 10 products
      - The final layout is given as follows:
        
        ![image](https://github.com/maahiraislam/data-analytics-power-bi-report849/assets/148975841/c5365ea0-a8f5-4a0b-adf1-045ad8fa5c0e)
        
   5. Created a product detail page that provides insights for all products and regions combined. Provides an in-depth look at which prodcuts within the inventory are performing well, with the option to filter by product and region. The following visuals were created:
      - **Card visuals** to show which filters are curently selected.
      - **Gauge visuals** to show how the selected category's revenue, profit and number of orders are performing against a quarterly target
      - An **area chart** showing relative revenue performance of each category over time
      - **Table** showing the top 10 products by revenue in the selected context
      - A **scatter graph** of quantity ordered against profit per item for products in the current context
      - The final layout is given as follows:
        
        ![image](https://github.com/maahiraislam/data-analytics-power-bi-report849/assets/148975841/ff02abf1-3c88-4afe-97d3-698c5f19b145)
        
   6. Created a **map visual** that allows you to check easily check on the stores under the regional managers control, allowing you to see which of the stores they are responsible for, the most profitable, as well as which are on track to reach their quarterly profit and revenue targets.
   7. Created a stores drillthrough page that summarises each store's performance to check on the progress of a given store. The following visuals were created:
      - A **table** showing the top 5 products, with columns: Description, Profit YTD, Total Orders, Total Revenue
      - A **column chart** showing Total Orders by product category for the store
      - **Gauges** for Profit YTD against a profit target of 20% year-on-year growth vs. the same period in the previous year. 
      - A **card visual** showing the currently selected store
      - The final layout is given as follows:
        
        ![image](https://github.com/maahiraislam/data-analytics-power-bi-report849/assets/148975841/3d461321-7541-4560-bc57-e9aba9f92a2f)

   8. Cross filtered the visualsand set the following interactions:
      - **Executive Summary Page**:
        - Product Category bar chart and Top 10 Products table should not filter the card visuals or KPIs
      - **Customer Detail Page**:
        - Top 20 Customers table should not filter any of the other visuals - Total Customers by Product Donut Chart should not affect the Customers line graph - Total Customers by Country donut chart should cross-filter Total Customers by Product donut Chart
      - **Product Detail Page**:
        - Orders vs. Profitability scatter graph should not affect any other visuals - Top 10 Products table should not affect any other visuals 

   
