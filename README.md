# 🇭🇰 Hong Kong Trading Sector — Industry & Business Performance Analysis

> **Industry analytics project using Python + Tableau to analyse Hong Kong's Import/Export, Wholesale and Retail Trades Sector (2015–2024), identify structural and productivity trends, and translate them into practical banking insights.**

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python\&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas\&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Analytics-013243?logo=numpy\&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-Visualization-E97627?logo=tableau\&logoColor=white)
![Data](https://img.shields.io/badge/Data-C%26SD-1F4E79)
![Period](https://img.shields.io/badge/Period-2015--2024-555)

</p>

---

## 📌 Project Overview

Hong Kong's **Import/Export, Wholesale and Retail Trades Sector** contains businesses with very different levels of scale, productivity, workforce structure and operating costs.

This project uses **2015–2024 Hong Kong Census and Statistics Department (C&SD) data** to build a structured industry-analysis framework that moves from:

**Market Scale → Business Structure → Productivity → Cost Structure → Industry Trends → Banking Opportunities**

The objective is not simply to visualise economic statistics, but to turn public-sector data into a **business-facing industry screening tool**.

---

## 🎯 Business Questions

| Question                                        | What the analysis looks at                               |
| ----------------------------------------------- | -------------------------------------------------------- |
| 🏢 **Where is economic activity concentrated?** | Revenue, value added, companies and employment           |
| 📈 **Which industries are more productive?**    | Revenue per employee and value added per employee        |
| 👥 **How is the market structured?**            | Company and workforce distribution by establishment size |
| 💰 **How do operating economics differ?**       | COGS, operating expenses and value-added margins         |

---

# 💡 Key Insights

### 1️⃣ Import/Export is the strongest overall contributor

Import/Export generates the highest revenue among the three major trade activities and is concentrated in the **high-revenue / high-value-added** region of the productivity analysis.

**Potential banking applications**

* Trade finance
* Working-capital facilities
* FX solutions
* Cash management

---

### 2️⃣ The market combines a fragmented SME base with larger establishments

Smaller establishments represent a large share of the company population, while employment is more distributed across larger establishments.

This suggests that **one banking strategy should not be applied uniformly across the sector**.

**Potential banking applications**

**SME segment**

* Working-capital facilities
* Trade finance
* Digital cash management

**Larger businesses**

* Corporate lending
* Structured working capital
* Treasury / FX
* Supply-chain finance

---

### 3️⃣ Different cost structures create different risk exposures

Industries display different combinations of **COGS intensity** and **operating-expense intensity**.

A high-COGS / lower-operating-expense structure can indicate greater sensitivity to goods prices and input-cost shocks.

**Risk areas to monitor**

* Gross-margin sensitivity
* Inventory requirements
* Working-capital needs
* Input-price volatility

---

### 4️⃣ Workforce declines while productivity improves in some areas

Overall workforce levels declined over the period, with Import/Export showing a particularly strong reduction while employee-based productivity increased.

This may indicate structural changes in how the sector generates output and revenue.

**Potential banking applications**

* Automation financing
* Technology investment
* Business transformation
* Productivity-related capital expenditure

---

# 🧰 Tech Stack

## 🐍 Python

### Data Wrangling

* Pandas
* NumPy
* Data cleaning and restructuring
* Multi-level hierarchy reconstruction
* Missing-value treatment
* Feature engineering

### Exploratory Data Analysis

* Distribution analysis
* Outlier investigation
* Correlation analysis
* Time-series exploration
* Hypothesis generation

---

## 📊 Tableau

* Interactive dashboards
* KPI reporting
* Parent → child drill-down
* Scatter plots
* Reference lines
* Trend analysis
* Industry comparisons
* Trade-activity comparisons

---

# 🔄 Data Pipeline

```text
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
```

---

# 🗂️ Dataset

**Source:** Hong Kong Census and Statistics Department (C&SD)

**Dataset:** [Table 630-76002 — Principal statistics for all companies by industry grouping and number of persons engaged](https://www.censtatd.gov.hk/en/web_table.html?id=630-76002)

**Source page:** [C&SD — Import/Export and Wholesale Trades](https://www.censtatd.gov.hk/en/scode550.html)

### Coverage

**2015–2024**

### Main Variables

| Category               | Measures                  |
| ---------------------- | ------------------------- |
| 🏢 Business population | Number of companies       |
| 👥 Employment          | Number of persons engaged |
| 💵 Revenue             | Total receipts            |
| 👨‍💼 Labour cost      | Compensation of employees |
| 🧾 Operating cost      | Operating expenses        |
| 📦 Direct cost         | Cost of goods sold        |
| 📈 Value creation      | Industry value added      |

> Financial measures are reported in **HK$ million**.

---

# 🧹 Data Cleaning & Preparation

The source dataset contains a multi-level industry structure and partially reported observations.

Key preparation steps included:

* Reconstructing the multi-level industry hierarchy
* Separating parent and child industry groups
* Preserving establishment-size bands and `Total` observations
* Converting `*` and `N.A.` to missing values rather than zero
* Checking duplicate analytical keys
* Checking negative and zero values
* Converting analytical and financial fields to numeric types
* Preserving partially reported records where valid variables remain available
* Keeping financial analysis primarily at the complete `Total` level
* Using company and employment measures for detailed size-band analysis

### Missing-Data Principle

> A missing value is excluded only from analyses that require that specific measure. An entire industry or observation is **not automatically removed** because one financial variable is unavailable.

---

# 🧠 Analytical Framework

The dataset is analysed at two main levels.

## 1. Aggregate Financial Analysis

Uses:

```text
Scale Band = Total
```

This level is used for:

* Revenue comparison
* Industry value-added comparison
* Revenue per employee
* Value added per employee
* COGS ratio
* Operating expense ratio
* Value-added margin
* 2015–2024 financial trends

---

## 2. Segment Structure Analysis

Uses:

```text
Scale Band ≠ Total
```

Detailed size-band analysis focuses on:

* Number of companies
* Number of persons engaged
* Company-size composition
* Workforce composition
* Persons per company
* Industry × establishment-size structure

---

## 🌳 Industry Hierarchy

```text
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
```

> Parent and child rows are kept separate to avoid double counting.

---

# 📐 Key Derived Metrics

| Metric                          | Formula                                  | Business Interpretation                 |
| ------------------------------- | ---------------------------------------- | --------------------------------------- |
| 💵 **Revenue per employee**     | `Total receipts / persons engaged`       | Descriptive revenue productivity        |
| 📈 **Value added per employee** | `Industry value added / persons engaged` | Descriptive value creation per employee |
| 🏢 **Revenue per company**      | `Total receipts / number of companies`   | Establishment revenue scale             |
| 👥 **Persons per company**      | `Persons engaged / number of companies`  | Workforce structure                     |
| 📦 **COGS ratio**               | `Cost of goods sold / total receipts`    | Direct-cost intensity                   |
| 🧾 **Operating expense ratio**  | `Operating expenses / total receipts`    | Operating-cost intensity                |
| 📊 **Value-added margin**       | `Industry value added / total receipts`  | Value creation relative to revenue      |

> These are **descriptive business measures** used to compare operating characteristics across industries.

---

# 🔬 Python Exploratory Analysis

Python was used to validate the dataset, investigate distributions, identify unusual observations and compare productivity and operating characteristics across the Hong Kong trading sector.

---

# 1️⃣ 📊 Data Distributions & Outlier Analysis

The initial analysis examined the distribution and potential outliers of key business and financial metrics.

## 💵 Revenue per Company

Revenue per company shows a right-skewed distribution, with several higher-value observations appearing as potential outliers.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/9b84001e-9947-41e6-b619-aa66070ea852" />
</p>

---

## 👤 Revenue per Employee

Revenue per employee also shows substantial variation across observations, with several high-productivity observations identified as potential outliers.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/a65cb0de-5f63-4d15-bb11-a5b1d571b38d" />
</p>

---

## 📈 Value Added per Employee

The distribution of value added per employee is concentrated at lower levels with a smaller number of higher-value observations.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/849dca19-2c40-4912-a9fc-b76135ca6aaa" />
</p>

---

## 📦 COGS Ratio

The COGS ratio distribution highlights differences in direct-cost intensity across the observations.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/55852dd1-26aa-4d0b-a02f-fd3fdb750454" />
</p>

---

## 🧾 Operating Expense Ratio

The operating expense ratio shows a concentrated distribution with a smaller number of observations exhibiting relatively high operating-expense intensity.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/6b357856-3adb-4b57-9397-c5a0a47fbb2d" />
</p>

---

## 📊 Value-Added Margin

The value-added margin distribution provides an additional view of differences in value creation relative to total receipts.

<p align="center">
  <img width="90%" src="https://github.com/user-attachments/assets/b20cdf5b-8a23-43a2-929f-30b20d8bf6eb" />
</p>

---

# 2️⃣ 🔄 Trade-Activity Differences

The analysis compared **Import/Export, Wholesale and Retail** to examine differences in employee-based value creation across the three major trade activities.

## 💼 Value Added per Employee by Trade Type — Overall Comparison

Import/Export shows a noticeably higher value-added-per-employee profile compared with Wholesale and Retail.

<p align="center">
  <img width="75%" src="https://github.com/user-attachments/assets/f04b7f79-c377-46cf-9a59-0fc9d8ad95ec" />
</p>

---

## 💼 Value Added per Employee by Trade Type — Comparative View

A further trade-type comparison highlights the differences in the distribution of employee-level value creation across Import/Export, Wholesale and Retail.

<p align="center">
  <img width="75%" src="https://github.com/user-attachments/assets/3cc94053-c6cc-4c13-ab62-e542c5d885e5" />
</p>

---

# 💡 Key Observations from Python EDA

The exploratory analysis identified several patterns for further business analysis:

* Revenue per company increases strongly with establishment size.
* Revenue per employee and value added per employee vary substantially across observations.
* Import/Export shows a stronger employee-based productivity profile.
* Revenue productivity and value creation are related but not identical.
* COGS and operating-expense ratios show different operating-cost structures across observations.
* Some observations exhibit unusually high productivity or cost ratios and warrant further investigation.

These findings were subsequently used to guide the **Tableau business analysis and industry-screening framework**.


---

# 📊 Tableau Dashboard

The Python analysis was transformed into one interactive Tableau dashboard for business-facing exploration.

🖥️ Interactive Dashboard

<p align="center">

<a href="https://public.tableau.com/app/profile/man.yin.yeung/viz/Hk_tradefinalv/Dashboard?publish=yes">

<img src="https://img.shields.io/badge/📊%20Open%20Interactive%20Tableau%20Dashboard-E97627?style=for-the-badge&logo=tableau&logoColor=white" alt="Open Tableau Dashboard">

</a>

</p>

🔗 View the Dashboard

Open the interactive Tableau dashboard →

The dashboard provides a business-facing view of the Hong Kong trading sector and supports exploration of the project's key analytical themes, including:

📈 Industry and trade-activity performance

👥 Business and workforce structure

💵 Productivity and value creation

💰 Cost structure

🔎 Interactive comparison and exploration

🖼️ Dashboard Preview

Replace the placeholder below with a screenshot of your Tableau dashboard after uploading it to the repository.

![Tableau Dashboard](images/tableau_dashboard.png)

Note: The live Tableau dashboard is hosted on Tableau Public. The link above opens the interactive version rather than a static image.

# 💻 Code & Project Files

## 🐍 Main Python Notebook

The main analysis notebook contains the data-loading, cleaning, restructuring, feature-engineering and exploratory-analysis workflow.

**Notebook:**

```text
HK_Trading_Business_Analysis_Professional_v2.ipynb
```

👉 [Open Python Notebook](./HK_Trading_Business_Analysis_Professional_v2.ipynb)

---

## 📁 Suggested Repository Structure

```text
HK-Trading-Business-Analysis/
│
├── README.md
│
├── HK_Trading_Business_Analysis_Professional_v2.ipynb
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── tableau/
│   └── HK_Trading_Business_Analysis.twbx
│
├── images/
│   ├── dashboard_executive_overview.png
│   ├── dashboard_productivity.png
│   ├── dashboard_business_structure.png
│   ├── dashboard_cost_structure.png
│   └── dashboard_time_trends.png
│
└── docs/
    └── project_documentation.pdf
```

> **Tip:** Do not upload confidential data, credentials, personal information, or unnecessary raw files to a public repository.

---

# 🏦 Banking Takeaway

The project demonstrates how economic data can be transformed into a **first-stage industry-screening framework** for banking.

```text
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
```

The analysis can help identify:

### 🎯 Where to focus attention

Which trade activities and industries contribute the most economic value?

### 👥 Which customer segments may need different products

SME businesses and larger establishments may have different financing, working-capital and treasury requirements.

### ⚠️ Which industries require closer monitoring

Cost intensity, workforce contraction and structural changes may indicate different operating and risk profiles.

---

# 🚀 How to Run the Project

## 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/HK-Trading-Business-Analysis.git
cd HK-Trading-Business-Analysis
```

## 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

## 3. Open the notebook

```bash
jupyter notebook
```

Then open:

```text
HK_Trading_Business_Analysis_Professional_v2.ipynb
```

## 4. Update the data path

Inside the notebook, replace the local file path with the location of your dataset.

```python
DATA_PATH = "path/to/your/data.xlsx"
```

---

# 📚 Data Source

**Hong Kong Census and Statistics Department (C&SD)**

* [Table 630-76002](https://www.censtatd.gov.hk/en/web_table.html?id=630-76002)
* [Import/Export and Wholesale Trades](https://www.censtatd.gov.hk/en/scode550.html)

---

# 👤 Author

**Your Name**

🎓 BBA in Information Management (Business Intelligence)
🏫 City University of Hong Kong
📍 Hong Kong

### 🔗 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?logo=linkedin\&logoColor=white)](YOUR_LINKEDIN_URL)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github\&logoColor=white)](https://github.com/YOUR_USERNAME)

---

<p align="center">
  <sub>Built with Python 🐍 • Tableau 📊 • C&SD Open Data 🇭🇰</sub>
</p>
