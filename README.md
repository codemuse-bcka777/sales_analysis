# Supermarket Sales Performance Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue) ![pandas](https://img.shields.io/badge/pandas-2.0-green) ![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow) ![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## Overview

This project analyzes two years of sales transaction data to uncover regional performance gaps, seasonal trends, and high-value customer segments. The goal is to deliver actionable business recommendations — not just charts.

All analysis is done in Python (pandas), with a final interactive dashboard built in Power BI.

---

## Business Questions Answered

| # | Question | Method |
|---|---|---|
| 1 | Which product category generate the most revenue? | Grouped aggregation + bar chart |
| 2 | Which regions perform best and worst? | Multi-metric regional comparison |
| 3 | What are the monthly sales trends? | Time series analysis + MoM growth |
| 4 | Which customers contribute the most revenue? | Pareto / 80-20 analysis |
| 5 | Which product categories need improvement? | Revenue vs profit margin comparison |

---

## Key Findings

- **Top 20% of customers drive 45.1% of total revenue** — a near-perfect Pareto distribution, indicating that customer retention of the top tier should be the company's highest priority.
- **Naypyitaw city outperforms all others**, not by volume but by average order value (2× the company average), suggesting a premium customer segment concentrated there.
- **Food and beverage items contribute 17.38% in gross income**, but is not that significantly higher than other categories. Number of sales and sum of gross income is almost similar for all categories.

---

## Project Structure

```
sales-analysis-project/
├── data/
│   └── sales.csv        # Cleaned and feature-engineered dataset
├── notebooks/
│   ├── 01_data_cleaning.ipynb # Null handling, type fixes, feature engineering
│   ├── 02_eda.ipynb           # Exploratory analysis for all 6 business questions and Mean/median, Pareto, MoM growth rates
├── dashboard/
│   └── sales_dashboard.pbix   # Power BI dashboard (requires Power BI Desktop)
├── insights/
│   └── business_insights_summary.pdf  # 1-page written recommendations report
└── README.md
```

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core analysis language |
| pandas | Data cleaning and aggregation |
| matplotlib / seaborn | Exploratory charts in notebooks |
| Power BI Desktop | Interactive business dashboard |
| Jupyter Notebook | Analysis environment |

---

## Dashboard Preview

The Power BI dashboard includes:

- **KPI Cards** — Total Revenue, Total Orders, Average Order Value, Top Region
- **Monthly Trend Line** — Sales over time with month-over-month growth
- **Top 10 Products** — Horizontal bar chart sorted by revenue
- **Regional Comparison** — Grouped bar showing revenue vs profit by region
- **Category Breakdown** — Pie chart for sales share by category
- **Slicers** — Filter by City


---

## How to Run the Notebooks

**1. Clone the repository**
```bash
git clone https://github.com/your-username/sales-analysis-project.git
cd sales-analysis-project
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn  jupyter
```

**3. Run notebooks in order**
```bash
jupyter notebook
```
Open and run `01_data_cleaning.ipynb` → `02_eda.ipynb` 

> The notebooks are self-contained. Each one saves its output so the next one can load it.

---

## Skills Demonstrated

- Data cleaning and preprocessing with pandas
- Feature engineering (extracting time-based columns from dates)
- Exploratory data analysis with groupby aggregations
- Statistical analysis (mean, median, growth rates, Pareto)
- Business insight generation from raw data
- Dashboard design and layout in Power BI
- DAX measures for calculated KPIs
- Written communication of findings for a non-technical audience

---
