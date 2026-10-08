Hong Kong Trading Sector — Industry & Business Performance Analysis
1. Executive Summary
Background
Hong Kong's import/export, wholesale and retail trades show different patterns in business scale, productivity, workforce structure and cost composition.
This project analyses 2015–2024 C&SD data to turn public economic statistics into a practical industry-screening view for banking and business analysis.
Objective
The project aims to identify:
•	where economic activity is concentrated;
•	which trade activities and industries show stronger revenue and value-creation productivity;
•	how companies and employment are distributed by establishment size; and
•	which industries show distinctive cost structures or structural changes.
________________________________________
2. Dataset Used
Source: Hong Kong Census and Statistics Department (C&SD)
Dataset: Table 630-76002 — Principal statistics for all companies by industry grouping and number of persons engaged, covering the Import/Export, Wholesale and Retail Trades Sector.
Source page: C&SD — Import/Export and Wholesale Trades
Period
2015–2024
Main measures
•	Number of companies
•	Number of persons engaged
•	Total receipts
•	Compensation of employees
•	Operating expenses
•	Cost of goods sold
•	Industry value added
Financial measures are reported in HK$ million.
________________________________________
3. Quick Highlights
1. Import/export is the strongest overall contributor
Import/export generates the most revenue among the three major trade activities and is concentrated largely in the high-revenue / high-value-added region of the productivity analysis.
Recommended action: Prioritise import/export for deeper sector coverage and targeted financing opportunities, such as trade finance, working-capital facilities, FX solutions and cash-management services.
2. The market has a fragmented SME base and a larger-establishment segment
Small establishments account for a large share of the company population, while employment is more distributed across larger establishments.
Recommended action: Use different approaches for the two segments. For smaller businesses, consider SME working-capital lines, trade finance and digital cash-management solutions. For larger businesses, consider corporate lending, structured working capital, treasury/FX and supply-chain finance.
3. Different cost structures create different risk exposures
Industries show different combinations of COGS and operating-expense intensity. A high-COGS / lower-operating-expense structure can increase sensitivity to input-cost or goods-price shocks.
Recommended action: When assessing credit exposure, consider gross-margin sensitivity, inventory and working-capital requirements, and input-price volatility. Relevant financing and risk-management tools may include revolving working-capital facilities, trade finance, inventory financing and FX/commodity risk-management solutions.
4. Workforce is declining while productivity improves in some areas
Overall workforce levels declined over the period, with Import/export showing a particularly strong reduction while employee-based productivity increased.
Recommended action: Monitor workforce contraction as a structural risk while exploring financing needs related to automation, technology investment and business transformation.
________________________________________
4. Technologies
Python
Data Wrangling
•	Pandas
•	NumPy
•	Data cleaning and restructuring
•	Hierarchy reconstruction
•	Missing-value treatment
•	Feature engineering
Data Exploration
•	Distribution analysis
•	Outlier investigation
•	Correlation analysis
•	Initial hypothesis generation
Tableau
EDA / Business Analysis
•	Interactive dashboards
•	Parent → child drill-down
•	KPI reporting
•	Scatter plots
•	Reference lines
•	Trend analysis
•	Industry and trade comparisons
________________________________________
5. Data Pipeline Architecture
C&SD Open Data
      ↓
Raw data extraction
      ↓
Python — Data Wrangling
      ↓
Data validation & cleaning
      ↓
Hierarchy reconstruction
      ↓
Feature engineering
      ↓
Python — Initial Data Exploration
      ↓
Export cleaned analytical dataset
      ↓
Tableau — EDA & Business Analysis
      ↓
Business insights
      ↓
Banking recommendations
________________________________________
6. Analytical Structure
The analysis separates the dataset into two main analytical levels.
Aggregate financial analysis
Uses:
Scale Band = Total
This is the main level for financial analysis because the Total rows provide complete financial measures in the analysed dataset.
Used for:
•	revenue and value-added comparison;
•	revenue per employee;
•	value added per employee;
•	COGS ratio;
•	operating expense ratio;
•	value-added margin; and
•	2015–2024 financial trends.
Segment structure analysis
Uses:
Scale Band ≠ Total
For detailed size-band analysis, the consistently available measures are:
•	Number of companies
•	Number of persons engaged
Used for:
•	company-size composition;
•	workforce composition;
•	persons per company; and
•	industry × size structure.
Parent and child hierarchy
Import/export trade
├── Food, alcoholic drinks and tobacco
├── Clothing, footwear and allied products
└── Other import/export trade

Wholesale trade
├── Food, alcoholic drinks and tobacco
├── Clothing, footwear and allied products
└── Other wholesale trade

Retail trade
├── Food, alcoholic drinks and tobacco
├── Fuel
├── Clothing, footwear and allied products
├── Transport equipment
└── Other retail trade
Parent and child rows are kept separate to avoid double counting.
________________________________________
7. Cleaning
Key cleaning steps included:
•	Reconstructing the multi-level industry structure.
•	Separating parent and child industry groups.
•	Preserving company-size bands and Total observations.
•	Converting * and N.A. to missing values rather than zero.
•	Checking duplicate analytical keys.
•	Checking negative and zero values.
•	Converting financial and analytical fields to appropriate numeric types.
•	Preserving partially reported records where valid variables remain available.
•	Keeping financial analysis primarily at the complete Total level.
•	Using company and employment measures for detailed size-band analysis.
Missing-data principle
Missing values are excluded only from analyses that require the missing measure. The entire industry or row is not removed simply because one financial measure is unavailable.
________________________________________
8. Key Derived Metrics
Revenue per employee
Total receipts / persons engaged
A descriptive indicator of revenue productivity.
Value added per employee
Industry value added / persons engaged
A descriptive indicator of value creation per employee.
Revenue per company
Total receipts / number of companies
Used to describe establishment revenue scale.
Persons per company
Persons engaged / number of companies
Used to describe workforce structure.
COGS ratio
Cost of goods sold / total receipts
Operating expense ratio
Operating expenses / total receipts
Value-added margin
Industry value added / total receipts
These are descriptive business measures used to compare operating characteristics across industries.
________________________________________
9. Python Initial Exploration
Python was used to validate the dataset and identify patterns that could be investigated further in Tableau.
Main exploration areas
1.	Data distributions
2.	Outliers
3.	Time trends
4.	Trade-activity differences
5.	Industry differences
6.	Establishment-size structure
7.	Productivity relationships
8.	Cost structure
9.	Hypothesis generation
Selected observations
•	Revenue per company increases strongly with establishment size.
•	Revenue per employee and value added per employee are highly heterogeneous across industries.
•	Import/export shows a distinctly higher employee-based productivity profile.
•	Revenue productivity and value creation are positively related but not identical.
•	COGS ratio and operating-expense ratio show a strong inverse relationship.
•	Some industries show distinctive cost structures and value-added margins.
•	Workforce levels decline over the period while some productivity measures improve.
________________________________________
10. Tableau Dashboard
The Tableau workbook turns the Python findings into a business-facing analytical interface.
Dashboard 1 — Executive Overview
Question: Where is economic activity concentrated?
•	Total revenue
•	Industry value added
•	Number of companies
•	Persons engaged
•	Revenue by major trade activity
•	Value added by major trade activity
Dashboard 2 — Industry & Productivity
Question: Which industries show distinctive productivity and value-creation profiles?
•	Revenue per employee
•	Value added per employee
•	Productivity scatter plot
•	Parent → child drill-down
•	Industry comparison
Dashboard 3 — Business Structure
Question: How is the business population distributed by establishment size?
•	Share of companies by size band
•	Share of persons engaged by size band
•	Persons per company
•	Industry × scale analysis
Dashboard 4 — Cost Structure
Question: How do industries differ in operating economics?
•	COGS ratio
•	Operating expense ratio
•	Value-added margin
•	COGS ratio vs operating expense ratio
•	Industry drill-down
Dashboard 5 — Time Trends
Question: How have the sector's characteristics changed over 2015–2024?
•	Revenue trends
•	Workforce trends
•	Productivity trends
•	Cost-ratio trends
•	Value-added margin trends
•	2021–2022 subsidy annotation
________________________________________
Banking Takeaway
The analysis provides a first-stage industry-screening view for a bank:
Market scale
     ↓
Business structure
     ↓
Productivity
     ↓
Cost structure
     ↓
Industry trend
     ↓
Prioritise deeper banking analysis
The practical objective is to help identify where to focus attention, which customer segments may need different products, and which industries require closer monitoring of cost and operating risks.


