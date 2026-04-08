📊 Superstore Analytics Dashboard — Power BI

An end-to-end business intelligence dashboard built on the 
Superstore Sales dataset, designed to track sales performance, 
profitability, and customer behavior across 2020–2023.

---

📸 Dashboard Preview

![Dashboard Preview](https://github.com/anidata3099/superstore-analytics-powerbi/blob/main/Screenshot%20(180).png)

---

🎯 Project Objective

To analyze retail business performance by building an interactive 
Power BI dashboard that helps stakeholders monitor KPIs, 
identify trends, and make data-driven decisions.

---

📌 Key KPIs

| Metric              | Current Year | Previous Year | YOY Change |
|---------------------|-------------|---------------|------------|
| Total Sales         | €2.33M      | €1.58M        | -0.53      |
| Total Profit        | €292.30K    | €196.37K      | -0.51      |
| Total Orders        | 5K          | 7K            | -0.75      |
| Avg Order Value     | €455.20     | €466.64       | -0.02      |
| % Returned Orders   | 5.81%       | 0.06          | +0.03      |

---

📊 Dashboard Features

- ✅ KPI Cards — Sales, Profit, Orders, Avg Order Value, Return Rate
- ✅ YOY & PY Comparison — DAX time intelligence measures
- ✅ Sales vs Previous Year — Trend line chart (2020–2023)
- ✅ Profit by Product — Bar chart by category & sub-category
- ✅ Profit by State — US geographic heatmap
- ✅ Sales by Segment — Donut chart (Consumer, Corporate, Home Office)
- ✅ Monthly Profit & Sales Analysis — Horizontal bar chart
- ✅ Dynamic Year Slicer — Filter by 2020, 2021, 2022, 2023

---

🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| Power BI Desktop | Dashboard design & visualization |
| DAX | KPI measures, YOY, PY calculations |
| Power Query (M) | Data cleaning & transformation |

---

🧮 DAX Measures Used

```dax
-- Previous Year Sales
PY Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))

-- Year-Over-Year Growth
YOY Sales = DIVIDE([Total Sales] - [PY Sales], [PY Sales])

-- Total Profit
Total Profit = SUM(Orders[Profit])



📁 Dataset

- Source:[Superstore Sales Dataset — Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- Records: ~10,000 orders
- Fields: Order ID, Sales, Profit, Category, Sub-Category, 
  Region, State, Segment, Ship Mode, Return Status

---

 📂 Repository Structure
