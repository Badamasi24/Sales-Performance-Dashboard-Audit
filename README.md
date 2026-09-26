# Sales-Performance-Dashboard-Audit
# Sales Performance & Dashboard Audit

## 📊 Data Analytics Audit Project

A comprehensive data analytics audit project focused on validating an existing sales dashboard, identifying data-quality issues, correcting inaccurate calculations, challenging management conclusions, and developing a reliable dashboard for data-driven decision-making.

This project was completed as part of the **DSN AI Bootcamp 2026 – Data Analytics Track** using **Microsoft Excel and Power Query**.

---

## 🎯 Project Overview

The objective of this project was to determine whether the insights presented in an existing sales dashboard were supported by the underlying data.

Rather than simply accepting the original dashboard findings, I conducted a structured audit involving:

- Data cleaning and standardization
- Missing-value treatment
- Data validation
- Revenue and profit recalculation
- Business claim validation
- Discount-band analysis
- Market and product-category analysis
- Return-rate analysis
- Monthly sales analysis
- Dashboard redesign
- Business recommendations

The audit revealed several discrepancies between the original dashboard and the corrected analysis, demonstrating the importance of data quality and validation before using business dashboards for decision-making.

---

## 🛠️ Tools & Technologies

- **Microsoft Excel**
- **Power Query**
- Excel PivotTables
- Data Cleaning & Transformation
- Data Validation
- Business Analysis
- Dashboard Development
- Data Visualization
- Data Storytelling

---

## 🧹 Data Cleaning & Quality Issues

During the audit, I identified several data-quality issues.

### 1. Inconsistent State Names

The dataset contained inconsistent capitalization, such as:

- `LAGOS`
- `Lagos`

These values were standardized to ensure that the same state was correctly grouped during analysis.

### 2. Inconsistent Product Categories

Product category values contained spelling and capitalization variations, including:

- `Accesory`
- `accessories`
- `Accessories`

These values were standardized to ensure accurate category-level analysis.

### 3. Missing Unit Product Cost

The `Unit Product Cost` column contained missing values.

To resolve this issue, I:

1. Identified the missing values.
2. Created a product-cost reference dataset.
3. Selected the Product and Unit Product Cost fields.
4. Removed duplicates.
5. Merged the reference data with the main dataset.
6. Used the matching product information to fill the missing costs.

This was particularly important because Unit Product Cost is required for accurate **COGS and profit calculations**.

---

## 🔍 Most Important Data-Quality Finding

The missing Unit Product Cost values had the greatest impact on the analysis.

Without correcting these values, COGS could be understated and profit could be overstated or misleading.

Correcting the missing costs allowed the analysis to produce more reliable:

- Cost of Goods Sold (COGS)
- Profit
- Profit Margin
- Product profitability insights

---

# 📈 Original Dashboard Audit

I tested eight major conclusions from the original dashboard against the cleaned and validated data.

| Original Dashboard Claim | Audit Verdict | Corrected Finding |
|---|---|---|
| Abuja is the most profitable market | ❌ Misleading | Lagos is the most profitable market |
| Electronics is the strongest-performing category | ✅ Correct | Electronics is the strongest-performing category by revenue |
| Higher discounting improves profitability | ❌ Incorrect | Profit declines as discount levels increase |
| Online has the lowest return rate | ❌ Incorrect | In-store has the lowest return rate |
| August is the strongest sales month | ❌ Misleading | May is the strongest sales month |
| Lagos is underperforming | ❌ Misleading | Lagos is the strongest market by revenue and profit |
| Reported revenue can be used directly | ❌ Incorrect | Revenue requires validation and reconciliation |
| Dashboard is reliable without further cleaning | ❌ Misleading | Further cleaning and validation are required |

---

# 💰 Major Financial Finding

One of the most important findings was the difference between the originally reported financial figures and the audited figures.

### Revenue

**Original reported revenue:** approximately **$47M**

**Audited revenue:** approximately **$44.34M**

**Difference:** approximately **$2.66M**

**Reduction:** approximately **5.66%**

### Profit

**Original reported profit:** approximately **$16M**

**Audited profit:** approximately **$11.50M**

**Difference:** approximately **$4.50M**

**Reduction:** approximately **28.13%**

This demonstrates how data-quality problems can materially affect business performance reporting and decision-making.

---

# 📊 Corrected Dashboard KPIs

After cleaning and validating the data, the corrected dashboard reported:

| KPI | Result |
|---|---:|
| Net Revenue | **$44.34M** |
| Total Profit | **$11.50M** |
| Profit Margin | **25.93%** |
| Transactions | **420** |
| Return Rate | **9.05%** |
| Average Discount | **7.99%** |

---

# 📌 Key Business Insights

## 1. Electronics is the strongest-performing product category

Electronics generated approximately:

- **$27.99M Revenue**
- **$7.17M Profit**

This represents approximately:

- **63.1% of total revenue**
- **62.3% of total profit**

Electronics therefore represents the largest contributor to overall business performance in the audited dataset.

---

## 2. Lagos is the strongest-performing market

The corrected market analysis showed:

| Market | Revenue | Profit |
|---|---:|---:|
| Lagos | $13.01M | $3.76M |
| Kano | $9.70M | $2.72M |
| Ibadan | $8.90M | $2.37M |
| Port Harcourt | $7.02M | $1.93M |
| Abuja | $5.71M | $0.72M |

Lagos recorded the highest revenue and profit among the markets analyzed.

Abuja recorded the lowest revenue and profit.

---

## 3. Higher discounting is not improving profitability

The discount-band analysis showed that profitability declined as discount levels increased.

| Discount Band | Revenue | Profit |
|---|---:|---:|
| No Discount | $16.39M | $5.84M |
| Low (1–5%) | $11.76M | $3.33M |
| Medium (6–10%) | $9.26M | $1.85M |
| High (11–15%) | $4.75M | $0.65M |
| Very High (16–25%) | $2.18M | **-$0.18M** |
| **Total** | **$44.34M** | **$11.50M** |

Approximately **79.8% of total profit ($9.18M)** was generated from transactions with **0–5% discounts**.

Most significantly, the **16–25% discount band generated approximately $2.18M in revenue but resulted in a loss of approximately $0.18M**.

This indicates that high discounting requires careful review because it can place significant pressure on profitability.

---

## 4. In-store has the lowest return rate

Return rate by channel:

| Channel | Return Rate |
|---|---:|
| In-store | **6%** |
| Online | **11%** |
| WhatsApp | **12%** |

The original dashboard incorrectly identified Online as the channel with the lowest return rate.

---

## 5. May is the strongest sales month

The corrected monthly analysis showed:

- **May:** approximately $6.98M revenue
- **January:** approximately $6.33M revenue
- **July:** approximately $6.26M revenue
- **August:** approximately $2.97M revenue

May was the strongest sales month, while August was the lowest-performing month in the analyzed period.

---

# ⚠️ Key Audit Finding

The most misleading conclusion in the original dashboard was:

> **"Abuja is the most profitable market."**

The audited data showed that:

- Lagos profit = **$3.76M**
- Abuja profit = **$0.72M**

If management relied on the original conclusion when allocating resources, it could result in disproportionate investment in a lower-profit market while overlooking stronger performance in Lagos.

---

# 🎯 Management Recommendations

Based on the corrected analysis, I developed three key recommendations.

### 1. Give greater attention to Electronics

Management should prioritize the Electronics category by:

- Maintaining product availability
- Monitoring customer demand
- Identifying opportunities for increased sales
- Monitoring category profitability

This recommendation is supported by Electronics' contribution of approximately **63.1% of total revenue**.

---

### 2. Maintain balanced market coverage while investigating Abuja

Management should maintain sales activities across the major markets while giving additional attention to Abuja's significantly lower profitability.

Further investigation should focus on:

- Product mix
- Operating costs
- Pricing
- Discounting
- Market-specific performance

---

### 3. Review high-discount strategies

Management should carefully review discount strategies, particularly discounts above 15%.

The analysis shows that:

- No discount → **$5.84M profit**
- 1–5% discount → **$3.33M profit**
- 6–10% discount → **$1.85M profit**
- 11–15% discount → **$0.65M profit**
- 16–25% discount → **-$0.18M loss**

Discounts should therefore be evaluated based on their impact on both sales volume and profitability rather than assuming that higher discounts automatically improve performance.

---

# 📊 Dashboard

The final dashboard provides management with an interactive view of:

- Net Revenue
- Total Profit
- Profit Margin
- Transactions
- Return Rate
- Average Discount
- Revenue and Profit by Market
- Revenue and Profit by Product Category
- Monthly Revenue and Profit Trend
- Return Rate by Channel
- Return Rate by Category
- Discount Band Performance

---

# 💡 Key Learning

The biggest lesson from this project is:

> **A professional-looking dashboard does not necessarily mean the underlying insights are reliable.**

Data cleaning, validation, and auditing are critical before business decisions are made.

This project strengthened my practical understanding of the complete analytics workflow:

**Raw Data → Data Cleaning → Data Validation → Analysis → Audit → Visualization → Business Insights → Recommendations**

It also reinforced the importance of challenging assumptions rather than simply accepting existing dashboard conclusions.

---

# 📁 Project Structure

```text
Sales-Performance-Dashboard-Audit/
│
├── README.md
│
├── data/
│   └── sales_dataset.xlsx
│
├── dashboard/
│   └── corrected_sales_dashboard.xlsx
│
├── report/
│   └── data_analytics_audit_report.pdf
│
└── screenshots/
    └── corrected_dashboard.png
👨‍💻 About the Project

Project: Sales Performance & Dashboard Audit
Track: Data Analytics
Program: DSN AI Bootcamp 2026
Participant: Muhammad Yunusa Badamasi
Tool: Microsoft Excel
Techniques: Data Cleaning, Power Query, Data Validation, Business Analysis, Dashboard Development, Data Storytelling

🔗 Connect With Me

I am interested in opportunities involving:

Data Analysis
Business Intelligence
Excel & Power BI
Data Visualization
Dashboard Development
Data Cleaning & Transformation
AI & Data Analytics

Feel free to explore the project and connect with me.

#DataAnalytics #Excel #PowerQuery #DataVisualization #BusinessIntelligence #DataCleaning #Dashboard #DataAnalyst #DSNAIBootcamp
