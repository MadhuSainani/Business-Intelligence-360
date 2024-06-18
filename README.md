# Business Insights 360
Live Dashboard Link: https://app.powerbi.com/view?r=eyJrIjoiZWU1MmExZDQtMGUzMC00Mjg3LTk1NzUtMGM3ZmI2NjVkNGQ2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=ReportSectionb0ed72eebc8562dcce4a
## Problem Statement:
AtliQ Technologies is a company that sells hardware such as PCs, network and storage devices, and peripherals to various customers across the world.
Their customers are served through three different channels: Retailer, Direct, and Distributor. While they have grown substantially in recent years, 
the company has experienced significant losses in Latin America due to decisions based on limited surveys and intuition. 
Additionally, AtliQ faces intense competition from Dell. Previously, the company relied on large Excel files for data analysis. 
To address these challenges and improve data transparency, AtliQ has decided to hire a dedicated data analysis team.

## Task:
- Create a dashboard tool for business review meetings and decision-making processes such as customer negotiations, marketing promotions, inventory management, and finance budgeting.
- Enable quick insights for the business across various customers to facilitate data-driven decision making.

## Project Implementation:
The project execution includes various steps:
- Connecting the MySQL database to Power BI for importing the dataset.
- Creating the required dimention table (dim_date) in Power Query using M language.
- Performing data transformation through Power Query.
- Data Modelling (Creating relationship between diffrent entities).
- Creating calculated columns and Measures using more than 45 DAX formulas.
- utlizing appropriate visuals as per the business requirement.
- Using Field Parameters and Bookmarks to switch between two visulas.
- creating dynamic titles based on applied filters.
- Creating tooltip to show sales trend analysis.
- Optimizing the report using DAX Studio.
- Utilizing Bookmarks to create a Filter Pane, which also shows the number of selected filters and provides a tooltip that shows selected filters when you hover your mouse over the button.
- Publishing the report to Power BI services.
- setting up the personal gateway to enable automatic data refresh.
## Data Model:
The data model is designed to efficiently manage and analyze business data using a combination of star and snowflake schemas. It includes 8 fact tables: fact_actual_estimates, fact_forecast_monthly, manufacturing_cost, freight_cost, operational_cost, post_invoice_deduction, NsGmTarget, and Marketshare. These fact tables includes the transactional data and are placed at the center of the model. The fact tables are surrounded by 4 dimension tables: dim_customer, dim_product, dim_date, and dim_market, which provide descriptive attributes related to the facts, forming a star schema structure. Additionally, a snowflake schema is utilized to normalize certain dimensions for more efficient data organization and storage. This involves connecting tables such as fiscal_year, sub_zone, and category to the relevant dimension tables, thus optimizing the data model for complex queries and reducing redundancy. 

![Data Model](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/DataModel_BI360.png)

## Building The Dashboard:
For Business Insights 360, I have created 5 multi-view dashboards, which serves the requirements of various stakeholders. Let's have a look at each them.

![Home Page](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Home%20Page.png)
### Finance View:
- The finance view indicates clear picture of organization's financial growth. This view includes KPIs such as Net sales, Gross Margin %, and Net Profit %.
- The Profit & Loss statement shows the progress of each metric, which allows users to filter by factors such as fiscal year, year-to-date, and year-to-go, etc.
- The Area chart displays the comparison of selected measure in P&L statement with Benchmark numbers ( LY or Target).
  
![Finance View](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Finance%20View.png)
### Sales View: 
- The sales view access organization's growth at the customer level using Net Sales and Gross Margin metrics.
- The scatter plot assist the stakeholders to identify customers that contribute significantly to organization's growth by displaying a comparison of Net sales and Gross MArgin.
- Donot chart displays the proportion of pre-invoice deductions, post-invoice deductions, and Gross Margin.
  
![Sales View](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Sales%20View.png)
### Marketing View: 
- The marketing view access organization's growth at the product level using Net Sales, Gross Margin, and Net Profit metrics.
- The scatter plot assist stakeholders in comparing Net sales with GM% or NP%.
- The Donut chart displays the proportion of Gross MArgin and Total COGS (Cost of Goods Sold).
  
![Marketing View](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Marketing%20View.png)
### Supply Chain View:
- Supply chain view examines Net Error and Absolute Error by assesing key metrics based on actual sales quantity and forecasted sales quantity.
- The column chart illustrates a comparison between the present Forecast Accuracy and that of the previous year for each month, showing the Net Error.
  
![Supply Chain View](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Supply%20Chain%20View.png)
### Executive View:
- Customized for top level executives, showcasing top 5 customers & products by revenue contribution, along with yearly trends in Revenue, GM%, NP%, & Market Share %.
- The Ribbon chart designed to analyze the market share % of top-level manufacturers for each fiscal year.
  
![Executive View](https://github.com/MadhuSainani/Business-Intelligence-360/blob/main/Executive%20View.png)



