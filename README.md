# Data Analytics Learning Journey

This repository documents my step-by-step progress in learning data analytics.

---

## 📚 Topics Covered

* Excel
* Data Cleaning
* Statistics
* SQL (upcoming)

---

## 📈 Progress

I will continuously update this repository as I learn and apply new concepts.

---

## 🎯 Objective

To build strong fundamentals and transition into real-world data analytics projects.

---

## 🗓️ Daily Progress Log

# Day 1 — Excel for Data Analytics
**Date:** 3 May 2026
**Topic:** Data Analysis with Excel — Formulas, Pivot Tables & Dashboards

---

## What I worked on today
Built an Employee HR Analysis project from scratch using real business data (20 employees across Sales, Marketing and Finance departments).

---

## Formulas I used

### IF — Status Classification
=IF(F2>=75,"ACTIVE","REVIEW")
Logic: Attendance above 75% = Active employee, below = Under Review

### Nested IF — Performance Tiers
=IF(F2>=90,"HIGH",IF(F2>=75,"AVERAGE","LOW"))
Logic: 3-tier performance system based on attendance percentage

### AVERAGEIF — Department-wise Salary
=AVERAGEIF(C:C,"SALES",D:D)
Result: Marketing ₹78,333 | Sales ₹75,625 | Finance ₹63,333

### INDEX + MATCH — Top Performer
=INDEX(B2:B21,MATCH(MAX(F2:F21),F2:F21,0))
Result: ADITYA GUPTA (100% attendance)

### COUNTIF — Summary Metrics
=COUNTIF(G2:G21,"ACTIVE") → 14 Active Employees
=COUNTIF(G2:G21,"REVIEW") → 6 Under Review

---

## Key Insights from the data
- Sales department has the highest total salary bill (₹6,05,000)
- Finance is the lowest paid department on average (₹63,333)
- 13 out of 20 employees are HIGH performers
- 6 employees are under review — all have attendance below 75%

---

## Skills practised today
- IF and Nested IF logic
- AVERAGEIF, COUNTIF, INDEX+MATCH
- Conditional Formatting (color scale)
- Pivot Tables and Pivot Charts
- Building a summary dashboard

---

## Tomorrow — Day 2
- Advanced Excel: VLOOKUP vs XLOOKUP
- Data cleaning techniques
- More complex dashboard building

