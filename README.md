# 🛒 Superstore Sales Performance Analysis

An exploratory data analysis of ~10,000 Superstore orders (2014–2017), examining sales, profit, discount behavior, customer segments, shipping, and time-based trends to understand what actually drives — and drains — the business's performance.

---

## 📌 Overview

Raw totals can lie. A category can look like a top performer purely because it has more orders, not because each order is worth more.

This project digs past totals into **margin, discount behavior, and product-level profitability** to find where Superstore is genuinely winning — and where it's quietly losing money.

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🎯 Key Business Questions

1. Which categories and sub-categories actually drive sales *and* profit — not just one or the other?
2. How does discount behavior erode profitability, and does it differ by category?
3. Which customer segments and shipping modes matter most?
4. How do sales and profit trend over time — is growth accelerating, steady, or fragile?
5. Does a top-selling product always mean a top-profiting product?

---

## 🔥 Key Findings

| #Finding |                                                                                                                                                                                                                                                                                                                 |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1**    | **Technology leads on value, Office Supplies leads on volume.** Technology drives the most revenue on both a total and per-order basis (~$453 avg/order). Office Supplies' comparable total sales are largely a function of order count (6,026 orders vs. Technology's 1,847), not per-order value (~$119 avg). |
| **2**    | **Furniture has a structural margin problem.** Its profit margin (~0.025) is roughly **7× lower** than Office Supplies or Technology (~0.17 each), despite having comparable total sales (~$742K vs. ~$719K–$836K).                                                                                             |
| **3**    | **Discount hurts categories in different ways.** Furniture's losses are frequent but individually modest, spread across a broad 30–60% discount range. Technology's losses are rare but severe — one order at a 70% discount lost over **$6,600**, ~3.5× Furniture's worst loss.                                |
| **4**    | **2017's growth came with a margin cost.** Sales grew strongly in 2016–2017, but the growth rate slightly decelerated (29.5% → 20.4%). Profit growth outpaced sales growth in 2015–2016, but fell behind in 2017 (14.2% vs. 20.4%) — a sign of margin dilution that year.                                       |
| **5**    | **High sales ≠ high profit at the product level.** Cisco TelePresence ranks #3 by sales (~$22.6K) but is absent from the profit top 10, driven by an extreme 50% average discount. HON Task Chairs shows a similar gap, more likely tied to Furniture's thin category-level margins than to discounting alone.  |

---

## 💡 Recommendations

* **Review Furniture's discount policy**, especially in the 30–60% range where losses are most frequent, and investigate whether its costs are structurally thin-margin regardless of discount.

* **Introduce category-specific discount controls** rather than applying a uniform discount strategy across all categories. Technology and Furniture show very different relationships between discount and profitability.

* **Audit high-revenue, low-profit products** such as Cisco TelePresence and HON Task Chairs. High sales should not automatically be treated as a sign of strong product performance.

* **Investigate the 2017 margin slowdown** to understand why profit growth (14.2%) lagged behind sales growth (20.4%).

---

## 📂 Repository Structure

```text
.
│   README.md
│   requirements.txt
│
├───data
│       Superstore.csv
│
└───notebook
        Superstore_Sales_Analysis.ipynb
```

---

## 📊 Dataset

The dataset contains approximately **10,000 Superstore orders** covering **2014–2017**.

Key fields include:

* Order Date & Ship Date
* Customer & Segment
* Region
* Category & Sub-Category
* Product
* Sales
* Quantity
* Discount
* Profit

---

## 🔬 Methodology

The analysis follows a structured exploratory data analysis workflow:

```text
Raw Data
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Feature Creation
   ↓
Exploratory Data Analysis
   ↓
Visualization
   ↓
Business Insights
   ↓
Recommendations
```

Key steps included:

* Data inspection and cleaning
* Date conversion
* Shipping duration calculation
* Sales and profit analysis
* Discount analysis
* Customer and regional analysis
* Product-level analysis
* Time-based trend analysis

---

## 🚚 Shipping Analysis

A `Shipping Days` feature was created from the difference between **Order Date** and **Ship Date**.

This was used to analyze shipping performance across different shipping modes.

---

## ▶️ How to Run

Clone the repository:

```bash
git clone https://github.com/anushkauppin-dev/superstore-sales-analysis.git
```

Navigate into the project:

```bash
cd superstore-sales-analysis
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook notebook/Superstore_Sales_Analysis.ipynb
```

---

## 📝 Notes

This project focuses on **exploratory data analysis and business interpretation**, demonstrating practical use of Python, Pandas, NumPy, Matplotlib, and Seaborn to transform raw data into actionable insights.


---

## 👩‍💻 About

This project is part of my journey toward becoming an **AI/ML Engineer**, with a focus on strengthening my foundations in:

* Python
* Data Analysis
* Data Visualization
* Machine Learning
* Problem Solving

More projects and experiments will be added as the journey continues. 🚀🧠
