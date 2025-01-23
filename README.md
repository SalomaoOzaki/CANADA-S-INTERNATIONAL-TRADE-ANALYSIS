# CANADA-S-INTERNATIONAL-TRADE-ANALYSIS

Overview
This project analyzes Canada’s international trade performance from 2019 to November 2024 using data from Statistics Canada (Table 12-10-0175-01). It involved building a seamless data pipeline utilizing Python, AWS, SQL, and Power BI to transform raw trade data into actionable insights. The analysis focuses on three types of trade: Import, Domestic Export, and Re-Export, with the latter two combined into a single variable, Export, for comprehensive reporting. Additionally, Re-Export data is only available at the national level and is not broken down for provinces.
Workflow
1. Data Extraction with Python
Connected to Statistics Canada’s API to extract international trade data in CSV format.

2. Data Storage in AWS using Python
Uploaded the extracted dataset to an S3 bucket in AWS for secure storage and accessibility.

3. Data Transformation with AWS Athena
Used SQL queries in AWS Athena to create structured tables from CSV files for further analysis.

4. Data Visualization in Power BI
Connected Power BI to AWS using ODBC for real-time data visualization.
Built interactive dashboards to provide insights at both national and provincial levels.
Utilized Power Query for data transformation tasks.
Implemented advanced DAX measures to calculate key metrics, such as percentage growth, export-to-import ratios, etc, enabling dynamic and detailed analysis.

Key Insights and Visualizations
1. National View
Trade Value Over Time: Analyze trends in Canada’s total imports and exports.
Top 15 Trading Partners: Visualize Canada’s major trade partners and their contributions to trade volumes.
Trade Values by Commodities: Highlight key commodities driving Canada’s trade performance.
Percentage Change Over Time: Dynamically track trade value growth. This metric is calculated either year-over-year or month-over-month. The level of comparison can be adjusted by changing the hierarchy in the chart. If the current year is incomplete, the comparison is made with the same period of the previous year, rather than the entire year.
Top 10 Trading Partners with Highest Growth: Identify rapidly growing markets and highlight growth in dollar value. Identify the fastest-growing markets and highlight their growth in dollar value. If the year and month are not selected, the metric will calculate the Compound Annual Growth Rate (CAGR), which represents the average annual growth rate over the entire period. If a specific period is selected, it will show the percentage growth compared to the previous period. Δ Value: If the current year is incomplete, the comparison will be made to the same period of the previous year rather than the entire year.

2. Provincial Insights
Trade Value Over Time: Examine import and export trends for each province.
Top 15 Partners: Highlight the main trading partners for each province.
Percentage Change Over Time: Assess growth trends at the provincial level.
Top 5 Commodities: Identify the most traded commodities by value.
Top 10 Trading Partners with Highest Growth: Highlight emerging markets for individual provinces.

3. National and Provincial Export-Import Ratios
Compare export-to-import ratios at both national and provincial levels to evaluate trade balances.

4. Partner Insights
Trade Value Over Time: Analyze trends in Canada’s total imports and exports.
Trade Values by Commodities: Highlight key commodities driving Canada’s trade performance.
Percentage Change Over Time: Dynamically track trade value growth (e.g., year-over-year or month-over-month).

Enhancements
This project incorporates Python scripts, SQL queries, and Power BI dashboards, supported by visuals that showcase the data transformation process and insights. Advanced DAX measures and calculations provide in-depth analysis, enhancing the storytelling aspect of the dashboards.

Citation
Statistics Canada. Table 12-10-0175-01 International merchandise trade by province, commodity, and Principal Trading Partners (x 1,000).
