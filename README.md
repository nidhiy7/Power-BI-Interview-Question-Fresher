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
- Time Intelligence Functions: DAX offers a set of specialized functions for time intelligence analysis. These functions, such as TOTALYTD, SAMEPERIODLASTYEAR, and DATESBETWEEN, allow for calculations based on specific time periods, year-to-date analysis, and comparisons across different time frames.

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


 ## Power BI  — Power Pivot
 
### 21) What is Power Pivot?
Ans: - Power Pivot is an add-in for Microsoft Excel 2010 that enables you to import millions of rows of data from multiple data sources into a single Excel workbook.   
- It helps you build a data model, relationships, creating formulas, calculated columns, Pivot Tables, and Pivot Charts from multiple resources.

### 22) How many active relations can we have between two tables in Power Pivot? 

We can only have one active relationship between tables at a time. When a relationship is active (represented with a continuous line), all other relationships will be inactive (represented with a dotted line).

### 23)  What is xVelocity in-memory analytics engine used in Power Pivot?
The xVelocity in-memory analytics engine, used in Power Pivot, is a highly optimized columnar database engine designed to provide fast and efficient data processing capabilities.


### 23)  What is the limitation of Power Pivot over Power Query?

Power Query is an ETL (Extract, Transform & Load) tool that allows extracting data from various sources and manipulate data based on your need. In contrast, Power Pivot can load data but can not manipulate or transform.


 ## Power BI  — Power Query 
 
### 24) What is Power Query?

Power Query is a tool for ETL (Extract, Transform & Load) data with a simple GUI. It allows users to extract data from multiple sources, transform data with their needs and load the final data in the system

### 25)  What are the destinations for output in Power Query?

There are two destinations for Power Query output: load to a table in the worksheet and load to an excel data model

### 26) What is some common Power Query/Editor Transforms?
 Changing Data Types, Filtering Rows, Choosing/Removing Columns, Grouping, Splitting a column into multiple columns, Adding new Columns, etc.

### 27)  Which language is used in Power Query?
A new programming language is used in a power query called M-Code. It is easy to use and similar to other languages. M-code is case sensitive language. 


 ## Power BI  — Power  Map

### 28) What is Power Map?

Power Map is a tool for the geographical representation of data in a Bing map. It also supports 3D representation with a collection of millions of geo-coded data points. It gives users the ability to create geographical visualization of data.

### 29) What are the primary data requirements for using Power Map?

The table loaded in Power Map should have location-based information like latitude, longitude, country, region, state, province, city, zip/pin code, etc.

 ## Power BI  — Power  View

 ### 30) What is Power View?
 Power View is a data visualization technology to create interactive graphs, charts, maps, and many other visuals. It helps in analyzing the data patterns and generating meaningful insights. Power View is 
 available for multiple tools and platforms like Excel, SharePoint, SQL Server, and Power BI.
 The following pages provide details about different visualizations available in Power View:

 The following pages provide details about different visualizations available in Power View:

- Charts
- Line charts
- Pie charts
- Maps
- Tiles
- Cards
- Tables
- Multiples Visualizations
- Bubble and scatter charts
- Key performance indicators (KPIs)

## 31) How to compare target and actual value in Power BI?
Using Gauge charts, we can compare two different measures, including the target and actual value.

## 32) What are the types of visualizations in Power BI?
Visualization is a graphical representation of data. We can use visualizations to create reports and dashboards. The kinds of visualizations available in Power BI are Bar charts, Column charts, Line chart, Area chart, Stacked area chart, Ribbon chart, Waterfall chart, Scatter chart, Pie chart, Donut chart, Treemap chart, Map, Funnel chart, Gauge chart, Cards, KPI, Slicer, Table, Matrix, R script visual, Python visual, etc.

## 33) What are the different views available in Power BI Desktop? 
- Report View - In this view, users can add visualizations and additional report pages and publish the same on the portal.

- Data View - In this view, data shaping can be performed using Query Editor tools.

- Model View - In this view, users can manage relationships between complex datasets.

## 34)  What is a Slicer?
- A slicer in Power BI is an interactive visual control that allows users to filter data by selecting specific values from a list.
- When applied, slicers dynamically update other visualizations on the report page to display data relevant to the chosen filters, enabling easy data exploration and analysis.
## Power BI - Advanced Question

## 35) What do we understand by Power BI services?
Power BI is a business analytics tool developed by Microsoft that provides interactive visualizations and business intelligence capabilities. Power BI Services, also known as Power BI cloud or Power BI Online, refers to the cloud-based platform where users can publish, share, collaborate on, and access Power BI reports and dashboards.

Power BI Services offers several key features and functionalities:

- Dashboards: Users can create interactive dashboards by combining multiple visualizations, reports, and data sources.

- Reports: Power BI allows users to create detailed reports with interactive visualizations and data exploration capabilities.
- Data Connectivity: Power BI Services supports connectivity to a wide range of data sources, both on-premises and cloud-based. It offers native connectors for popular data sources such as Excel, SQL Server, SharePoint, Dynamics 365, Salesforce, and many others.

- Data Transformation: Power Query, a data transformation and mashup tool within Power BI, enables users to clean, shape, and combine data from different sources. It provides an intuitive interface for performing data preparation tasks, such as merging tables, filtering data, and applying transformations.

- Collaboration and Sharing: Power BI Services allows users to collaborate and share reports and dashboards with others in their organization. Users can control access permissions, publish content to specific workspaces, and collaborate in real-time by sharing and commenting on reports.

- Mobile Access: Power BI offers native mobile apps for iOS and Android devices, enabling users to access and interact with reports and dashboards on the go. The mobile apps provide a responsive and optimized experience for viewing and analyzing data on mobile devices.

- Data Refresh and Scheduled Refresh: Power BI Services supports automatic data refresh for reports and dashboards. Users can define data refresh schedules to keep the visualizations up-to-date with the latest data from the underlying data sources.

- Integration with Other Tools: Power BI integrates with other Microsoft tools and services such as Azure Data Factory, Azure Analysis Services, Excel, and SharePoint. It also supports embedding Power BI content into custom applications or websites using APIs and embedding capabilities.

## 33) What are some of the disadvantages or risks that we should look out for as we use Power BI?
- One of the biggest disadvantages of using Power BI is that their cloud-based solution (Power BI Service) is locked into the Microsoft ecosystem. Only those with a Microsoft 365 account and Power BI PRO subscription can access reports and dashboards.
- Power BI desktop only works on Windows and cannot be installed on machines that run MacOS or Linux
- Power BI cannot accept file sizes larger than 1 GB.

## 34)What is Power BI Q&A?
- Power BI Q&A is a feature that allows users to ask questions in natural language and get insights from their data.It uses advanced algorithms to interpret the user's intent and generates visualizations based on the queried data.Users can refine their queries and ask follow-up questions to explore the data further.Power BI Q&A makes data analysis more accessible and user-friendly, bridging the gap between non-technical users and data insights.

## 35) How can you integrate Power BI with other Microsoft products and services, such as Azure and SQL Server?
Integrating Power BI with other Microsoft products and services:

- Power BI integrates seamlessly with Azure services like Azure Data Factory, Azure SQL Database, and Azure Analysis Services.
- Integration with SQL Server allows direct connectivity to on-premises data sources.
- SharePoint integration enables embedding Power BI reports and dashboards within SharePoint sites.

## 36)What are the best practices for data modeling in Power BI?
- Create a star schema or snowflake schema to simplify relationships and optimize performance.
- Use descriptive naming conventions for tables, columns, and measures.
- Avoid circular dependencies and unnecessary relationships.
- Normalize or denormalize tables based on data usage patterns.

## 37) How can you optimize DAX calculations for better performance in Power BI?

- Minimize the use of calculated columns and prefer measures for aggregations.
- Use CALCULATE and CALCULATETABLE functions efficiently to filter and modify calculations.
- Use table variables or temporary tables to store intermediate results.
- Consider using query folding to push some calculations back to the data source.

##38) What are KPIs in Power BI?
- KPIs (Key Performance Indicators) in Power BI are visual elements that show the performance of specific metrics against predefined goals. \
- Examples :
1) Sales Revenue KPI: This KPI measures the total sales revenue against a target or goal. It may use a trend analysis to show the performance over time, indicating whether the revenue is above or below the target.



## 41) What is PowerBI Gateway ?
- The Power BI Gateway is a tool that facilitates the connection between on-premises data sources and the cloud-based Power BI service. It enables secure data transfer and ensures data freshness in Power BI reports and dashboards
-  There are two types of Power BI Gateways:
  
1)Power BI Personal Gateway:
- The Power BI Personal Gateway is designed for individual users and allows them to refresh their own datasets and reports.
- The Personal Gateway is installed on the user's computer and manages the data connectivity and refresh for their specific Power BI content.

2)  Power BI On-premises Data Gateway:
- The Power BI On-premises Data Gateway is designed for enterprise use and enables centralized management and shared dataset refreshes.
-  It is suitable for scenarios where multiple users or teams need to access on-premises data sources and ensure data consistency across Power BI content.
-  The On-premises Data Gateway is installed on a server within the organization's network and allows for scheduling and managing data refreshes for multiple datasets and reports.

## 42) 

