# Global Freelance Earnings Analysis
## Compensation Drivers, Regional Disparities & Income Stability


### 🔎 Project Overview

This project analyzes global freelance earnings to identify the key factors influencing compensation across different countries, skills, and experience levels. Using a dataset of freelance professionals, the analysis explores how geography, skill specialization, education, and experience impact income levels.

The project focuses on uncovering meaningful patterns in the freelance labor market while ensuring data reliability through appropriate statistical techniques and data quality filtering.

Interactive visualizations were developed using Tableau to present insights through an executive-style analytical dashboard.


------------
## Business Questions


This analysis explores several key questions about the global freelance market:

• What regions offer the highest freelance compensation?

• Does education level significantly impact freelancer income?

• How does income stability vary across developed and emerging markets?

• Which factors drive the largest differences in freelance earnings?

--------------
## Interactive Dashboard

View the full interactive dashboard [here](https://public.tableau.com/app/profile/xhavide.zymberi/viz/GlobalFreelanceMarketAnalysisCompensationDriversRegionalDisparitiesIncomeStability/GlobalFreelanceEarningsAnalysisdashboard)




## 🖥️ Tableau Dashboard Preview

### Executive Overview

This section provides a high-level summary of global freelance earnings including key KPIs such as average annual income, median hourly rate, total freelancers analyzed, and the highest-paying region.

![Executive Overview](https://github.com/Xhavide/Global-Freelance-Earnings-Analysis-Compensation-Drivers-Regional-Disparities-Income-Stability/blob/6444efe48ee37ded3babccb5539efe3e89801a0a/Screenshot%202026-03-12%20231424.png)

### Market Comparison

Regional comparison of freelance markets highlighting top paying region and global income distribution.

![Market Comparison](https://github.com/Xhavide/Global-Freelance-Earnings-Analysis-Compensation-Drivers-Regional-Disparities-Income-Stability/blob/13c6cd3e83f7bb9ed511dda751155b5e57199f08/Screenshot%202026-03-12%20231624.png)



### Income Stability Analysis

Statistical measures such as Coefficient of Variation (CV) and Interquartile Range (IQR) are used to analyze income dispersion and stability across countries.

![Income Stability](https://github.com/Xhavide/Global-Freelance-Earnings-Analysis-Compensation-Drivers-Regional-Disparities-Income-Stability/blob/b6c08911b481ba9aa933acfe75bc2513e95ab1ed/Screenshot%202026-03-12%20231747.png)



🧠## Key Insights

• **Years of experience show minimal impact on freelance earnings.**

• **Education level does not significantly influence freelancer income.**

• **Skill specialization is the strongest driver of higher earnings.**

• **Western Europe ranks as the highest-paying region, with Switzerland leading the market in median hourly compensation.**

• **Emerging markets exhibit higher income dispersion relative to developed markets.**

------------
## Data Preparation

Several data quality checks and preprocessing steps were performed:

- Countries with **sample size < 15 were filtered** to improve statistical reliability.
- Extreme outliers were removed when necessary to avoid distortion of income metrics.
- Median values were used instead of averages for certain comparisons to reduce outlier influence.
 
--------------
## Key Metrics Used

To analyze compensation levels and income stability across markets, the following statistical measures were used:

• **Median Hourly Rate** – chosen to represent typical earnings while minimizing the effect of extreme outliers.

• **Coefficient of Variation (CV)** – used to measure income volatility relative to average compensation levels.

• **Interquartile Range (IQR)** – used to evaluate income dispersion within the middle 50% of the dataset.

These metrics allow meaningful comparisons between markets with different compensation levels.


-----------
## Key Calculated Fields (Tableau)

- **Median Hourly Rate per Country**

{ FIXED [Country] : MEDIAN([Hourly Rate Usd]) }

Used to measure the typical compensation level within each country.

- **Coefficient of Variation (CV)per country**

[Country StdDev] / [Country Mean]

Used to measure relative income volatility across markets.

CV allows comparison of compensation stability across countries with different income levels.


- **Interquartile Range (IQR) per country**

{ FIXED [Country] : PERCENTILE([Hourly Rate Usd], 0.75)} -
{ FIXED [Country] : PERCENTILE([Hourly Rate Usd], 0.25)}

Measures dispersion within the middle 50% of earnings.

IQR helps identify income dispersion while reducing the influence of extreme values.



- **% Difference from Country Median**


([Hourly Rate Usd] - [Country Median Rate])
/ [Country Median Rate]

Used to evaluate how far individual freelancer earnings deviate from the typical country compensation level.

This metric highlights income inequality within freelance markets.

----------

## Limitations

Several limitations should be considered when interpreting the analysis:

• The dataset size (~500 records) represents a sample rather than the entire freelance market.

• Some countries had small sample sizes and were filtered to improve statistical reliability.

• Outliers may still exist in certain markets and could slightly influence some aggregated metrics.

Future analysis could include larger datasets and additional variables such as industry specialization and project type.

------
## Repository Structure


global-freelance-earnings-analysis
│
├── data
│ └── freelance_dataset.csv
│
├── tableau
│ └── freelance_earnings_dashboard.twbx
│
├── dashboard-preview
│ └── dashboard_overview.png
│ └── market_comparison.png
│ └── statistical_analysis.png
│
└── README.md

------

## Skills Demonstrated

- Data analysis
- Data visualization
- Tableau dashboard design
- Statistical analysis
- Market analysis
- Data storytelling

  ------

## Business Relevance

This analysis highlights how freelance labor markets function differently from traditional employment markets.

Organizations and platforms can use similar analyses to:

- Understand global compensation benchmarks

- Identify emerging freelance markets

- Optimize pricing strategies

- Improve talent sourcing strategies across regions

  -------

**Author**

**Xhavide Zymberi**
Data Analytics | SQL | Tableau | Marketing Analytics

LinkedIn:
https://www.linkedin.com/in/xhavide-zymberi/

GitHub:
([https://github.com/Xhavide](https://github.com/Xhavide))

Tableau: ([https://public.tableau.com/app/profile/xhavide.zymberi/vizzes](https://public.tableau.com/app/profile/xhavide.zymberi/vizzes))






















