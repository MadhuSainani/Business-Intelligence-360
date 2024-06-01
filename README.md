# Business-Intelligence-360
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



