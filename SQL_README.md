# 🛒 Superstore Sales Analysis — SQL Business Intelligence

> **End-to-end SQL analysis of 4 years of U.S. retail sales data (2015–2018), featuring an RFM customer segmentation model built entirely in SQL.**

---

## 📌 Business Problem

A U.S. retail superstore operating across four regions wants to better understand its sales performance, customer loyalty, and shipping operations. This project uses **SQL inside a Jupyter notebook** to answer 14 business questions across five themes — and goes beyond standard analysis by implementing a full **RFM scoring model in SQL**, a technique used by real retail analytics teams.

---

## ⭐ What Makes This Project Different

Most Superstore analyses stop at revenue by region and top products. This project goes further by implementing a **full RFM (Recency, Frequency, Monetary) customer segmentation model entirely in SQL** using multi-step CTEs, `NTILE(4)` window functions, and `CASE WHEN` classification logic — producing 6 actionable customer segments with a concrete marketing action plan for each.

---

## 🎯 Key Results

| Finding | Insight |
|---|---|
| West region leads in total revenue | Consistent growth across all 4 years |
| Top 6 sub-categories account for ~80% of revenue | Pareto principle confirmed |
| Champions generate 3x avg revenue of Lost customers | Strong case for retention investment |
| Standard Class used for 60%+ of orders | Upgrade upsell opportunity exists |

---

## 📊 Analysis Structure

**Section 1 — Sales Performance:** Revenue by region, MoM growth with `LAG()`, YoY comparison with `CASE WHEN` pivot, segment analysis

**Section 2 — Product Performance:** Revenue by sub-category, Top 10 products, Pareto 80/20 analysis with cumulative `SUM() OVER()`, `DENSE_RANK()` within categories

**Section 3 — Customer Analysis:** Top 10 customers, New vs. Returning customers by year

**Section 4 — RFM Segmentation *(Differentiator)*:** Full 3-step CTE model using `NTILE(4)` to score Recency, Frequency, Monetary — classifies 793 customers into Champions, Loyal, Potential Loyalists, New, At Risk, and Lost with marketing actions per segment

**Section 5 — Shipping & Operations:** Mode performance with `SUM() OVER()`, Region × Mode heatmap

---

## 🔧 SQL Concepts Demonstrated

`SELECT/WHERE/GROUP BY/ORDER BY/HAVING` · `INNER JOIN/LEFT JOIN` · Multi-step CTEs · `DENSE_RANK() OVER (PARTITION BY)` · `LAG()` · `SUM() OVER()` · `NTILE(4)` · `CASE WHEN` · `julianday()` · `strftime()`

---

## 🗄️ Dataset

**Source:** [Superstore Sales Dataset — Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) | 9,800 line items | 793 customers | 1,861 products | 2015–2018

---

## 🔧 Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat)

---

## 📁 Repository Structure

```
superstore-sql-analysis/
├── Superstore_SQL_Analysis.ipynb   # Full analysis notebook
├── superstore.db                    # SQLite database
├── train.csv                        # Source dataset
└── README.md
```

---

## 🚀 How to Run

```bash
git clone https://github.com/YOUR_USERNAME/superstore-sql-analysis.git
cd superstore-sql-analysis
pip install pandas matplotlib seaborn jupyter
jupyter notebook Superstore_SQL_Analysis.ipynb
```

> `superstore.db` is included — no database setup required.

---

## 💡 Top Recommendations

1. **Protect Champions** — reward with exclusives, ask for reviews, offer early access
2. **Win back At Risk / Lost customers** — targeted campaigns for high-spend customers gone quiet
3. **Concentrate on Technology** — highest revenue per order; expand accessories and phones
4. **Focus inventory on the top 80% sub-categories** — confirmed by Pareto analysis
5. **Upsell Standard Class to First Class** — majority of customers default to the slowest option

---

## 🔮 Future Work

Cohort analysis · Market basket analysis · Predictive CLV model · Power BI executive dashboard

---

## 👤 Author

**Siddhant Bhandari** | MS Business Analytics | Available for DA / BI Analyst roles (OPT)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_PROFILE)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/YOUR_USERNAME)
