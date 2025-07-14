# 📘 Finance Dashboard - Documentation

## 📊 Project Objective

To visualize personal finance data over time using Power BI. The goal is to track **income**, **expenses**, and **savings**, and understand financial habits better.

---

## 📁 Data Source

- **File Name**: `financial_data.csv`
- **Format**: CSV
- **Fields Included**:
  - Year
  - Month
  - Income
  - Expenses (Groceries, Rent, EMI, Health, etc.)
  - Savings (FD, Mutual Fund, etc.)
  
---

## 📈 Dashboard Overview

### 🔹 Summary Cards
- **Income**: Total income received over the years.
- **Savings**: Total money saved.
- **Expenses**: Total money spent.
- **Expense %**: Calculated as `(Total Expenses / Total Income) * 100`.

### 🔹 Time Filters
- Filters by **year** (2018 to 2021) and **month** (Jan to Jun).

### 🔹 Line Graph
**Title**: Do I save/spend according to what I earn?
- **Expense %**
- **Savings %**
- **Income change MoM**
- **Saving target (100%)**

Helps you compare actual savings/expenses against targets and observe income fluctuations.

### 🔹 Bar Chart - Where Do I Spend?
Breakdown of key spending categories:
- House Rent
- Groceries
- EMIs
- Health
- Leisure
- Shopping

### 🔹 Bar Chart - Where Do I Save?
Breakdown of savings distribution:
- Mutual Funds
- Emergency Fund
- Fixed Deposit
- Liquid Cash

### 🔹 Detailed Table
Year-wise breakdown of all components (both income and expenses).

---

## 🧠 DAX Measures Used

- `Total Expense` = SUM([Expense])
- `Expense %` = DIVIDE([Total Expense], [Total Income]) * 100
- `Savings %` = DIVIDE([Total Savings], [Total Income]) * 100
- `Income Change MoM` = ([Current Month Income] - [Previous Month Income]) / [Previous Month Income]

---

## 📊 Key Insights

- Most expenses go into **House Rent** and **Groceries**.
- **Mutual Funds** dominate savings.
- Expense % remains around 78.41%, leaving ~21.59% saved.
- Notable income fluctuations seen in 2020.

---

## 🛠 Tools Used

- Power BI (Data Modeling, DAX, Visualization)
- Excel / CSV data file

---

## 📌 Notes

- Dashboard supports dynamic filtering.
- Ideal for personal or family budgeting analysis.

---
