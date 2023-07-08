# Top 50 Question - Power BI Fresher


 ## General Question
### 1)What is Power BI and how does it differ from other business intelligence tools?
-Power BI is a business analytics tool developed by Microsoft that allows users to visualize and analyze data from various sources. It differs from other BI tools with its user-friendly interface, seamless integration with other Microsoft products, and strong self-service capabilities.

#### Power BI features allow you to:
 - Pre-built dashboards and reports for SaaS Solutions.
 - Power BI allows real-time dashboard updates.
 - Share presentations and queries with your colleagues.
 - Update your Excel file from data sources that can be on-site or in the cloud.
  -Display the output on multiple devices. This includes PCs, tablets, and HTML 5-enabled mobile devices that use the Power BI app.
 - Query your data using natural language processing (or Q&A, as it is known).

### 2)What data sources can Power BI connect to?
Power BI can connect to the following types of data sources:

- Databases: Microsoft SQL Server, Oracle, MySQL, PostgreSQL, etc.
- Files: Excel workbooks, CSV, XML, JSON, text files, etc.
- Online Services: SharePoint, Dynamics 365, Salesforce, Google Analytics, etc.
- Big Data Sources: Apache Hadoop, Apache Spark, Azure HDInsight, etc.
- Azure Services: Azure SQL Database, Azure Data Factory, Azure Cosmos DB, etc.
- Web Content: Web pages for web scraping data.
- Streaming Data: Azure Stream Analytics, Azure Event Hubs, PubNub, etc.
- APIs: Custom-built or third-party applications and services.
- On-Premises Data Gateways: Securely connect to on-premises databases and file servers.
Power BI offers a wide range of connectivity options, enabling users to extract and analyze data from various sources, both on-premises and in the cloud.

### 3)What is Building Blocks in Power BI?
- Visualizations: Visual representations of data, such as pie charts, line graphs, and maps.
- Datasets: Collections of data from various sources like Excel sheets or SQL databases.
- Reports: Collections of visualizations organized on one or more pages.
- Dashboards: Single-page presentations of multiple visualizations for a consolidated view.
- Tiles: Individual visualizations within a report or on a dashboard.
These building blocks enable users to analyze and present data effectively in Power BI.

### 4)What are the different types of filters in Power BI Reports?
n Power BI Reports, there are several types of filters available:

- Visual-level filters: These filters are applied to individual visualizations and affect only the data displayed within that specific visual.
- Page-level filters: These filters are applied to an entire page within the report and impact all the visualizations on that page.
- Report-level filters: These filters are applied to the entire report and affect all the pages and visualizations within it.
- Drillthrough filters: These filters allow users to navigate from one page to another, passing specific filter values to the target page for more detailed analysis.
- 
### 5)What are the content packs in Power BI?

### 6) Name the types of Power BI tools and components ?

A)The Power BI tools available are:

- Power BI Desktop – The desktop tool for computers.
- Power BI Service – Online SaaS tool that can be accessed using any browser.
- Power BI Mobile – Portable tool for mobile users with Android and iOS operating systems.
- Power BI Report Builder – Special tool for creating paginated reports.

 B) ****Some important components in the Power BI toolkit are:****

  **- Power Query – It allows to load and transform data from various sources.
- Power Pivot – It is a data modelling tool in Power BI.
- Power View – It is a presentation tool for creating tables, charts, and many more.
- Power Map – It allows the creation of geospatial data representations.
- Power Q/A –  It allows the use of natural language to get answers.**

*** 7)

 ## Power BI  — DAX

 ### 11) What is DAX?
 -DAX (Data Analysis Expressions) is a formula language used in Power BI to create custom calculations and aggregations. It enables users to define measures, calculated columns, and tables to perform complex calculations and build advanced analytical models.
 - It is a collection of constants, operators, and functions to create an expression for calculating values.
- DAX works on column values.
- DAX can not modify or insert data.
- We can create calculated columns and measures with DAX but we can not calculate rows using DAX.

- Here is a basic sample for DAX expression.

Total Sales = SUM(Sales[SalesAmount])

- Total Sales – It is the measure name that will take the calculated values.
- SUM – It is the DAX function for summing up the values.
- Parenthesis () – This is the parenthesis from which the function takes the argument (value passed to the function).
- Sales – It is the table name from where we want to pick the values.
- SalesAmount – It is the column name of the table where the values are present.

### 12) Name some common DAX functions

Here are some common DAX functions that are used frequently.

- Aggregation Functions: SUM, MIN, MAX, AVG, COUNTROWS, DISTINCTCOUNT
- Logical Functions: IF, AND, OR, SWITCH
- Information Functions: ISBLANK, ISFILTERED, ISCROSSFILTERED
- Filter Functions: VALUES, ALL, FILTER, CALCULATE, TOPN
- Date & Time Functions: DATEDIFF, DATEVALUE
- Statistical Functions: GEOMEAN, MEDIAN
- Other Functions: UNION, INTERSECT, EXCEPT, NATURALINNERJOIN, NATURALLEFTEROUTERJOIN,
SUMMARIZECOLUMNS, ISEMPTY, VAR

### 13) What is special or unique about the CALCULATE and CALCULATETABLE functions?
 These are the only functions that allow you to modify the filter context of measures or tables.

- Add to the existing filter context of queries.
- Override filter context from queries.
- Remove existing filter context from queries.

### 14) What are calculated columns and measures?

- Calculated columns are the additional column that we create and calculate using DAX expressions.
- On the other hand, measures are also calculated using DAX expressions but do not add up in the data tables in any form. Calculated columns are evaluated at each row, and measures are only evaluated at the level of granularity where they are plotted.

### 15) What is the difference between SUM and SUMX functions in DAX?
- The SUM function calculates the sum of a column or expression within a given context, while the SUMX function iterates over a table and performs a sum calculation for each row.
- SUMX is useful when you need to perform calculations on a row-by-row basis or when working with virtual tables created by DAX functions.

1) TotalQuantitySold = SUM(Sales[QuantitySold])
2) TotalSalesAmount = SUMX(Sales, Sales[QuantitySold] * Sales[UnitPrice])

