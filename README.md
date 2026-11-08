<img width="1599" height="1399" alt="Dashboard 1 (1)" src="https://github.com/user-attachments/assets/84466cd9-9703-49ee-82b6-f7a61d78cc19" />🇭🇰 Hong Kong Trading Sector — Industry & Business Performance Analysis
An industry analytics project using Python and Tableau to analyse Hong Kong's Import/Export, Wholesale and Retail Trades Sector (2015–2024), identify structural and productivity trends, and translate the findings into practical banking insights.

<p align="center">
  <img ![Uploading Dashboard 1 (1).png…]()
 alt="Hong Kong Trading Sector Performance Tableau Dashboard" width="100%" />
</p><p align="center">
  <a href="https://public.tableau.com/app/profile/man.yin.yeung/viz/Hk_tradefinalv/Dashboard?publish=yes"><strong>↗ Open the Interactive Tableau Dashboard</strong></a>
</p><p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/NumPy-Analytics-013243?logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/Tableau-Visualization-E97627?logo=tableau&logoColor=white" alt="Tableau" />
  <img src="https://img.shields.io/badge/Data-C%26SD-1F4E79" alt="C&SD data" />
  <img src="https://img.shields.io/badge/Period-2015--2024-555" alt="2015–2024" />
</p>📊 2024 Dashboard Results
The dashboard brings together the sector's financial scale, business population, workforce, industry mix, productivity and cost structure.
2024 KPI	Result	Change vs. 2023
Total revenue / receipts	HK$5.29 trillion	+4.7%
Industry value added	HK$581.3 billion	+3.5%
Number of companies	125,139	−6%
Number of persons engaged	637,357	−4%


<sub>Financial amounts are converted from the source dataset's HK$ million unit for readability. Percentage changes are based on the dashboard's year-on-year comparison; displayed KPI percentages are rounded.</sub>
Key findings at a glance
1. Import/Export dominates revenue. The dashboard's industry breakdown shows that Other import/export trade alone generated approximately 77.6% of total sector receipts in 2024 (HK$4,102,536 million).
2. Import/Export has the strongest employee-based productivity profile. In the productivity comparison, it sits above the other two trade activities in value added per employee and also records higher revenue per employee.
3. The business population and workforce contracted year-on-year. The number of companies fell by 6% and persons engaged fell by 4% in 2024, despite increases in receipts and industry value added.
4. Revenue per person increased as the workforce index declined. The 2015–2024 trend view shows revenue per person rising while the workforce index moves down. This is a descriptive pattern, not proof of a particular cause.
5. The sector has different business-size and cost profiles. The dashboard compares companies and employment by establishment-size band and breaks down receipts into cost of goods sold, operating expenses and value added.
📌 Project Overview
Hong Kong's Import/Export, Wholesale and Retail Trades Sector contains businesses with very different levels of scale, productivity, workforce structure and operating costs.

This project uses 2015–2024 Hong Kong Census and Statistics Department (C&SD) data to build a structured industry-analysis framework that moves from:

Market Scale → Business Structure → Productivity → Cost Structure → Industry Trends → Banking Opportunities

The objective is not simply to visualise economic statistics, but to turn public-sector data into a business-facing industry screening tool.
🎯 Business Questions
Question	What the analysis looks at
🏢 Where is economic activity concentrated?	Revenue, value added, companies and employment
📈 Which industries are more productive?	Revenue per employee and value added per employee
👥 How is the market structured?	Company and workforce distribution by establishment size
💰 How do operating economics differ?	COGS, operating expenses and value-added margins


💡 Key Insights & Business Implications
1️⃣ Import/Export is the main revenue contributor
Import/Export generates the largest share of receipts among the three trade activities. The 2024 industry breakdown also shows that Other import/export trade contributes approximately 77.6% of total sector receipts.

Potential banking applications
- Trade finance and import/export financing
- Working-capital facilities
- FX solutions and hedging
- Cash and liquidity management
2️⃣ The sector requires a segmented customer approach
The establishment-size analysis shows a fragmented business population, with many smaller establishments and a different distribution of employment across size bands. Business needs are therefore unlikely to be uniform across the sector.

Potential banking applications
- SMEs: digital cash management, trade finance and working-capital facilities
- Larger businesses: corporate lending, structured working capital, treasury / FX and supply-chain finance
3️⃣ Productivity differs across trade activities
The employee-based productivity comparison places Import/Export above Wholesale and Retail in value added per employee, with a higher revenue-per-employee profile as well. These measures provide a descriptive comparison of business output and value creation relative to workforce size.

Potential banking applications
- Compare financing needs alongside productivity and operating scale
- Explore technology and process investment opportunities
- Use sector and sub-sector benchmarks as an initial screening tool
4️⃣ Receipts and value added increased while headcount declined
In 2024, total receipts reached HK$5.29 trillion (+4.7%) and industry value added reached HK$581.3 billion (+3.5%). Over the same year, the number of companies fell 6% and persons engaged fell 4%. The longer-term indexed trend also shows revenue per person increasing while the workforce index declines.

This pattern may reflect changes in business scale, operating models or workforce composition. The dashboard identifies the trend, but the aggregate data alone does not establish its cause.

Potential banking applications
- Automation and technology financing
- Business transformation and productivity-related capital expenditure
- Further investigation of labour, operating-cost and investment needs
5️⃣ Cost structures create different operating sensitivities
The dashboard compares cost of goods sold, operating expenses and value added as components of receipts. Differences in these proportions can indicate different exposure to inventory, input-price and operating-cost pressures.

Risk areas to monitor
- Gross-margin sensitivity
- Inventory and working-capital requirements
- Input-price volatility
- Operating-expense pressure
🧰 Tech Stack
🐍 Python
Data Wrangling
- Pandas
- NumPy
- Data cleaning and restructuring
- Multi-level hierarchy reconstruction
- Missing-value treatment
- Feature engineering
Exploratory Data Analysis
- Distribution analysis
- Outlier investigation
- Correlation analysis
- Time-series exploration
- Hypothesis generation
📊 Tableau
- Interactive dashboards
- KPI reporting
- Parent → child drill-down
- Scatter plots
- Reference lines
- Trend analysis
- Industry comparisons
- Trade-activity comparisons

🔄 Data Pipeline
┌──────────────────────────────┐
│ 🇭🇰 C&SD Open Data            │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 📥 Raw Data Extraction        │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 🐍 Python Data Wrangling      │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 🧹 Data Validation & Cleaning │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 🌳 Hierarchy Reconstruction   │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ ⚙️ Feature Engineering        │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 🔎 Python Initial EDA         │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 📤 Clean Analytical Dataset   │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 📊 Tableau Business Analysis  │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 💡 Business Insights          │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│ 🏦 Banking Recommendations    │
└──────────────────────────────┘

🗂️ Dataset
Source: Hong Kong Census and Statistics Department (C&SD)

Dataset: Table 630-76002 — Principal statistics for all companies by industry grouping and number of persons engaged

Source page: C&SD — Import/Export and Wholesale Trades
Coverage
2015–2024
Main Variables
Category	Measures
🏢 Business population	Number of companies
👥 Employment	Number of persons engaged
💵 Revenue	Total receipts
👨‍💼 Labour cost	Compensation of employees
🧾 Operating cost	Operating expenses
📦 Direct cost	Cost of goods sold
📈 Value creation	Industry value added


Financial measures are reported in HK$ million.

🧹 Data Cleaning & Preparation
The source dataset contains a multi-level industry structure and partially reported observations.

Key preparation steps included:
- Reconstructing the multi-level industry hierarchy
- Separating parent and child industry groups
- Preserving establishment-size bands and Total observations
- Converting * and N.A. to missing values rather than zero
- Checking duplicate analytical keys
- Checking negative and zero values
- Converting analytical and financial fields to numeric types
- Preserving partially reported records where valid variables remain available
- Keeping financial analysis primarily at the complete Total level
- Using company and employment measures for detailed size-band analysis
Missing-Data Principle
A missing value is excluded only from analyses that require that specific measure. An entire industry or observation is not automatically removed because one financial variable is unavailable.

🧠 Analytical Framework
The dataset is analysed at two main levels.
1. Aggregate Financial Analysis
Uses:
Scale Band = Total
This level is used for:
- Revenue comparison
- Industry value-added comparison
- Revenue per employee
- Value added per employee
- COGS ratio
- Operating expense ratio
- Value-added margin
- 2015–2024 financial trends
2. Segment Structure Analysis
Uses:
Scale Band ≠ Total
Detailed size-band analysis focuses on:
- Number of companies
- Number of persons engaged
- Company-size composition
- Workforce composition
- Persons per company
- Industry × establishment-size structure
🌳 Industry Hierarchy
Import / Export Trade
├── Food, alcoholic drinks and tobacco
├── Clothing, footwear and allied products
└── Other import / export trade

Wholesale Trade
├── Food, alcoholic drinks and tobacco
├── Clothing, footwear and allied products
└── Other wholesale trade

Retail Trade
├── Food, alcoholic drinks and tobacco
├── Fuel
├── Clothing, footwear and allied products
├── Transport equipment
└── Other retail trade
Parent and child rows are kept separate to avoid double counting.

📐 Key Derived Metrics
Metric	Formula	Business Interpretation
💵 Revenue per employee	Total receipts / persons engaged	Descriptive revenue productivity
📈 Value added per employee	Industry value added / persons engaged	Descriptive value creation per employee
🏢 Revenue per company	Total receipts / number of companies	Establishment revenue scale
👥 Persons per company	Persons engaged / number of companies	Workforce structure
📦 COGS ratio	Cost of goods sold / total receipts	Direct-cost intensity
🧾 Operating expense ratio	Operating expenses / total receipts	Operating-cost intensity
📊 Value-added margin	Industry value added / total receipts	Value creation relative to revenue


These are descriptive business measures used to compare operating characteristics across industries.

🔬 Python Exploratory Analysis
Python was used to validate the dataset, investigate distributions, identify unusual observations and compare productivity and operating characteristics across the Hong Kong trading sector.
1️⃣ 📊 Data Distributions & Outlier Analysis
The initial analysis examined the distribution and potential outliers of key business and financial metrics.
💵 Revenue per Company
Revenue per company shows a right-skewed distribution, with several higher-value observations appearing as potential outliers.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/9b84001e-9947-41e6-b619-aa66070ea852" />
</p>👤 Revenue per Employee
Revenue per employee also shows substantial variation across observations, with several high-productivity observations identified as potential outliers.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/a65cb0de-5f63-4d15-bb11-a5b1d571b38d" />
</p>📈 Value Added per Employee
The distribution of value added per employee is concentrated at lower levels with a smaller number of higher-value observations.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/849dca19-2c40-4912-a9fc-b76135ca6aaa" />
</p>📦 COGS Ratio
The COGS ratio distribution highlights differences in direct-cost intensity across the observations.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/55852dd1-26aa-4d0b-a02f-fd3fdb750454" />
</p>🧾 Operating Expense Ratio
The operating expense ratio shows a concentrated distribution with a smaller number of observations exhibiting relatively high operating-expense intensity.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/6b357856-3adb-4b57-9397-c5a0a47fbb2d" />
</p>📊 Value-Added Margin
The value-added margin distribution provides an additional view of differences in value creation relative to total receipts.
<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/b20cdf5b-8a23-43a2-929f-30b20d8bf6eb" />
</p>2️⃣ 🔄 Trade-Activity Differences
The analysis compared Import/Export, Wholesale and Retail to examine differences in employee-based value creation across the three major trade activities.
💼 Value Added per Employee by Trade Type — Overall Comparison
Import/Export shows a noticeably higher value-added-per-employee profile compared with Wholesale and Retail.
<p align="center">
  <img width="75%" src="https://github.com/user-attachments/assets/f04b7f79-c377-46cf-9a59-0fc9d8ad95ec" />
</p>💼 Value Added per Employee by Trade Type — Comparative View
A further trade-type comparison highlights the differences in the distribution of employee-level value creation across Import/Export, Wholesale and Retail.
<p align="center">
  <img width="75%" src="https://github.com/user-attachments/assets/3cc94053-c6cc-4c13-ab62-e542c5d885e5" />
</p>💡 Key Observations from Python EDA
The exploratory analysis identified several patterns for further business analysis:
- Revenue per company increases strongly with establishment size.
- Revenue per employee and value added per employee vary substantially across observations.
- Import/Export shows a stronger employee-based productivity profile.
- Revenue productivity and value creation are related but not identical.
- COGS and operating-expense ratios show different operating-cost structures across observations.
- Some observations exhibit unusually high productivity or cost ratios and warrant further investigation.
These findings were subsequently used to guide the Tableau business analysis and industry-screening framework.
📊 Tableau Dashboard
The interactive Tableau dashboard combines the analysis into a business-facing industry brief.

↗ Open the Interactive Tableau Dashboard

The dashboard includes:
- Headline KPIs: total receipts, industry value added, number of companies and persons engaged
- Ten-year trends: trade-activity revenue, revenue per person and workforce indices
- Industry composition: revenue breakdown by trade activity and sub-industry
- Business structure: company and workforce distribution by establishment-size band
- Cost structure: cost of goods sold, operating expenses and value added
- Productivity comparison: revenue per employee versus value added per employee, with average reference lines
The dashboard is designed for initial industry screening and comparison. It does not replace detailed company-level due diligence or a governed financial report.
🏦 Banking Takeaway
The project demonstrates how economic data can be transformed into a first-stage industry-screening framework for banking.
        MARKET SCALE
              ↓
      BUSINESS STRUCTURE
              ↓
         PRODUCTIVITY
              ↓
        COST STRUCTURE
              ↓
        INDUSTRY TREND
              ↓
   DEEPER BANKING ANALYSIS
The analysis can help identify:
🎯 Where to focus attention
Which trade activities and industries contribute the most economic value?
👥 Which customer segments may need different products
SME businesses and larger establishments may have different financing, working-capital and treasury requirements.
⚠️ Which industries require closer monitoring
Cost intensity, workforce contraction and structural changes may indicate different operating and risk profiles.
📚 Data Source
Hong Kong Census and Statistics Department (C&SD)
- Table 630-76002
- Import/Export and Wholesale Trades
