# 🍎 Apple Sales Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-teal?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

---

## 📌 Project Overview

This is my **Project 2** as part of my Data Science learning journey.

This project analyzes an Apple Sales Dataset to identify **sales trends**, **top-performing products**, and **high-revenue markets** across 13 countries, 7 apple varieties, and 4 market channels — covering the years **2024 and 2025**.

The entire analysis was performed using **Python** with no Machine Learning algorithms — focusing on Data Cleaning, Exploratory Data Analysis (EDA), and Visualization.

---

## 🎯 Objective

- Identify which months have the highest and lowest apple sales
- Discover the most popular apple varieties and quality grades
- Analyze which countries generate the most revenue
- Compare sales performance across different market channels
- Understand year-over-year revenue growth trends

---

## 📁 Project Structure

```
Apple-Sales-Analysis/
│
├── 📓 Apple_Sales_Analysis.ipynb   # Main Jupyter Notebook
├── 📊 apple_sales_data.csv         # Dataset
├── 📄 Report/
│   └── Apple_Sales_Report_Ali.docx # Full Analysis Report
└── 📝 README.md                    # Project Documentation
```

---

## 🗂️ Dataset Information

| Attribute        | Details                                      |
|-----------------|----------------------------------------------|
| Dataset Name     | apple_sales_data                             |
| Total Records    | 500 rows × 11 columns                        |
| Time Period      | 2024 – 2025                                  |
| Missing Values   | 0 (Clean Dataset)                            |
| Duplicate Rows   | 0                                            |

### Columns

| Column             | Type     | Description                          |
|--------------------|----------|--------------------------------------|
| record_id          | int64    | Unique record identifier             |
| country            | str      | Country of sale (13 countries)       |
| apple_variety      | str      | Apple type (7 varieties)             |
| quality_grade      | str      | Premium / Standard / Economy         |
| market_type        | str      | Supermarket / Wholesale / Online / Local |
| month_name         | str      | Month of transaction                 |
| year               | int32    | Year (2024 or 2025)                  |
| price_per_kg_usd   | float64  | Price per KG in USD                  |
| quantity_sold_kg   | int64    | Quantity sold in KG                  |
| revenue_usd        | float64  | Revenue generated in USD             |
| calculated_revenue | float64  | Verified revenue (price × quantity)  |

---

## 🧹 Data Cleaning Steps

- ✅ Checked and confirmed **zero null values**
- ✅ Checked and confirmed **zero duplicate rows**
- ✅ Converted `Date` column to `datetime64` format
- ✅ Standardized all column names to **snake_case**
- ✅ Verified `revenue_usd` accuracy — matched `price × quantity` at **100%**
- ✅ Extracted `year` and `month_name` from Date column
- ✅ Reordered columns for better readability

---

## 📊 Exploratory Data Analysis (EDA)

### 📅 Insight 1 — Monthly Sales
| Month     | Qty Sold (KG) |
|-----------|--------------|
| October   | 57,254 ⬆️ Highest |
| February  | 53,953       |
| September | 50,527       |
| July      | 31,413 ⬇️ Lowest |

### 🍏 Insight 2 — Variety-wise Sales
| Apple Variety    | Qty Sold (KG) |
|-----------------|--------------|
| Fuji             | 81,241 🥇    |
| Pink Lady        | 78,318 🥈    |
| Honeycrisp       | 77,317 🥉    |
| Golden Delicious | 55,999 ⬇️   |

### 🏪 Insight 3 — Market Type Performance
| Market Type      | Qty Sold (KG) | Revenue (USD)   |
|-----------------|--------------|-----------------|
| Wholesale Market | 141,762       | $358,325        |
| Supermarket      | 137,178       | $366,895 💰 #1  |
| Local Market     | 133,572       | $350,371        |
| Online Store     | 97,717        | $255,336        |

### 🌍 Insight 4 — Top Countries by Revenue
| Country   | Revenue (USD) |
|-----------|--------------|
| China     | $149,149 🥇   |
| Germany   | $124,117 🥈   |
| UAE       | $110,790 🥉   |
| USA       | $79,858 ⬇️   |

### 📈 Insight 5 — Year-wise Revenue Growth
| Year | Revenue (USD)  |
|------|---------------|
| 2024 | $655,125.65   |
| 2025 | $675,800.80 (+3.15% 📈) |

---

## 💡 Key Insights

1. **October** is the peak sales month (57,254 KG | $142,502 revenue)
2. **Fuji** is the most popular apple variety with 81,241 KG sold
3. **China** leads in both quantity (53,233 KG) and revenue ($149,149)
4. **Supermarket** generates the highest revenue ($366,895) among all channels
5. **Standard quality** dominates total sales (179,153 KG)
6. Revenue grew **+3.15%** from 2024 to 2025
7. Strong correlation of **0.749** between Quantity Sold and Revenue
8. **Online Store** is the weakest channel — high growth opportunity
9. **Gala** is the most expensive variety at $2.87 avg/KG
10. **USA** has the lowest sales despite being a major market

---

## 🛠️ Tools & Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 🚀 How to Run

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/Apple-Sales-Analysis.git
```

2. **Install required libraries**
```bash
pip install pandas numpy matplotlib seaborn
```

3. **Open the Jupyter Notebook**
```bash
jupyter notebook Apple_Sales_Analysis.ipynb
```

---

## 📌 Project Roadmap

| Step | Description | Status |
|------|-------------|--------|
| 1    | Problem Statement | ✅ Done |
| 2    | Data Loading | ✅ Done |
| 3    | Data Overview | ✅ Done |
| 4    | Data Cleaning | ✅ Done |
| 5    | EDA + Visualization | ✅ Done |
| 6    | Insights & Recommendations | ✅ Done |
| 7    | Report & Dashboard | ✅ Done |
| 8    | Conclusion & Future Scope | ✅ Done |

---


## 👤 Author

**Alikaif**
---

⭐ **If you found this project helpful, please give it a star!** ⭐
