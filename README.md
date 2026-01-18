# 📊 Bank Loan Analysis Dashboard (Power BI)

## 📌 Project Overview
This project is an end-to-end **Bank Loan Analysis Dashboard** built using **Power BI**.  
The objective is to analyze loan performance from multiple perspectives — **business growth, operational details, credit risk, and profitability** — using well-defined KPIs, time intelligence (MTD, PMTD, MoM), and structured visual storytelling.

The dashboard is designed to answer four critical questions:
1. How is the loan business performing overall?
2. What drives loan applications and funding?
3. Where is the credit risk concentrated?
4. Is the bank being adequately compensated for the risk taken?

---

## 🎯 Business Objectives
- Track **loan demand and funding trends**
- Monitor **approval efficiency**
- Identify **high-risk segments**
- Measure **profitability and unit economics**
- Support **data-driven credit and pricing decisions**

---

## 🧩 Dataset Description
The dataset contains historical loan-level data with the following key attributes:
- Loan ID
- Application Date
- Loan Amount
- Funded Amount
- Total Payment Received
- Loan Purpose
- Loan Grade
- Employment Length
- Debt-to-Income Ratio (DTI)
- Interest Rate
- Loan Status (Good / Bad)

A **Date Table** is used to enable time intelligence calculations.

---

## 🏗️ Dashboard Structure

### 1️⃣ Summary Page
**Purpose:** High-level snapshot for executives.

**KPIs:**
- Total Loan Applications
- Total Funded Amount
- Total Amount Received
- Average Interest Rate

This page answers: *“What is the overall size and pricing of the loan portfolio?”*

---

### 2️⃣ Overview Page
**Purpose:** Portfolio health and momentum.

**KPIs:**
- Total Loan Applications
- Total Funded Amount
- Approval Rate (%)
- Month-over-Month Loan Application Growth (%)

This page answers: *“Is demand growing, and how efficiently are applications converted into funded loans?”*

---

### 3️⃣ Details Page
**Purpose:** Understand volume drivers and borrower composition.

**KPIs:**
- Average Loan Amount  
- Applications per Borrower  
- Top Loan Purpose Share (%)  
- Stable Employment Share (%)  

This page answers: *“Who is borrowing, for what purpose, and how concentrated is the portfolio?”*

---

### 4️⃣ Risk Page
**Purpose:** Credit quality and exposure analysis.

**KPIs:**
- Bad Loan % (based on loan applications)
- Bad Loan Exposure (Funded Amount)
- Average DTI
- High-Risk Grade Exposure (%)

This page answers: *“How risky is the portfolio, and where is the risk concentrated?”*

---

### 5️⃣ Profit Page
**Purpose:** Measure financial return versus risk.

**KPIs:**
- Net Profit
- Profit Margin (%)
- Average Interest Rate
- Profit per Loan

This page answers: *“Is the bank earning enough to justify the risk taken?”*

---

## 📐 Key Measures & Logic

### Core Measures
- **Total Loan Applications** = Count of Loan IDs  
- **Total Funded Amount** = Sum of Loan Amount  
- **Total Amount Received** = Sum of Total Payments  
- **Average Interest Rate** = Average of Interest Rate  
- **Average DTI** = Average of DTI  

---

### Risk Measures
- **Bad Loan %** = Bad Loan Applications ÷ Total Loan Applications  
- **Bad Loan Exposure** = Funded Amount of Bad Loans  
- **High-Risk Exposure %** = Funded Amount (Grades D–G) ÷ Total Funded Amount  

---

### Profit Measures
- **Net Profit** = Total Amount Received − Total Funded Amount  
- **Profit Margin %** = Net Profit ÷ Total Funded Amount  
- **Profit per Loan** = Net Profit ÷ Total Loan Applications  

---

## ⏱️ Time Intelligence (MTD, PMTD, MoM)

### Month-to-Date (MTD)
Used to analyze current month performance up to the selected date.

**Example:**
- MTD Loan Applications
- MTD Bad Loan %
- MTD Approval Rate
- MTD Stable Employment %

### Previous Month-to-Date (PMTD)
Used for comparison against the previous month.

### Month-over-Month (MoM)
Calculated as:
- **Absolute Change** for ratios (e.g., Bad Loan %, Avg DTI)
- **Percentage Change** for amounts (e.g., Funded Amount, Exposure)

This ensures mathematically correct and interpretable trends.

---

## 📊 Visualization Techniques
- KPI Cards with MTD values and MoM indicators
- Horizontal and Vertical Bar Charts for ranking
- Highlight-based interaction for cross-filtering
- Scatter plots for Interest Rate vs Default Risk
- Trend lines for monthly performance tracking

All visuals follow consistent color coding:
- Blue → Primary metrics
- Red → Risk indicators
- Green → Positive performance

---

## 🧠 Key Insights Enabled
- Identification of high-risk loan grades and purposes
- Early warning signals using DTI and Bad Loan %
- Understanding whether growth is volume-driven or quality-driven
- Clear separation between **growth**, **risk**, and **profit** narratives

---

## 🛠️ Tools & Technologies
- **Power BI**
- **DAX (Data Analysis Expressions)**
- **Date Table & Time Intelligence**
- **GitHub for version control**

---

## ✅ Best Practices Followed
- Ratios calculated using aggregated values (not averaged ratios)
- Clear separation of KPIs by business objective
- Consistent MTD / PMTD / MoM logic
- Risk and profit metrics never mixed without context
- Dashboard pages designed with a single, clear question in mind

---

## 📌 Conclusion
This Bank Loan Analysis Dashboard provides a **holistic, business-ready view** of loan performance.  
It balances **growth, risk, and profitability** and is suitable for **executive reviews, credit committees, and operational teams**.

The project demonstrates strong skills in:
- Data modeling
- DAX time intelligence
- KPI design
- Financial and risk analysis
- Dashboard storytelling

---

📁 **This repository contains:**
- Power BI report file
- Supporting documentation
- DAX logic embedded in the model

Feel free to explore, fork, or adapt this project for learning and professional use.
