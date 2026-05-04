# Day 2 — Excel for Data Analytics
**Date:** 4 May 2026
**Topic:** VLOOKUP vs XLOOKUP + Data Cleaning

---

## What I worked on today
Built a LOOKUP practice sheet and a Data Cleaning sheet using 
real employee data from the Day 1 HR project.

---

## Formulas I used

### VLOOKUP — Search and Return
=VLOOKUP(A2,RAW_DATA!A:C,3,0)
- Searched EMP IDs and returned Department from RAW_DATA sheet
- Limitation: requires column number (fragile if columns shift)

### XLOOKUP — Modern Alternative
=XLOOKUP(A2,RAW_DATA!A:A,RAW_DATA!C:C)
- Same result, cleaner syntax
- No column number needed — directly references return column
- Works in both directions
- Industry standard in 2026

### Both returned identical results:
| EMP ID | Department |
|--------|------------|
| 101 | Marketing |
| 105 | Sales |
| 112 | Sales |
| 117 | Sales |
| 120 | Finance |

---

## Data Cleaning techniques practised

### PROPER — Fix inconsistent text casing
=PROPER(A2)
Converts: "aditya raj singh" → "Aditya Raj Singh"
Converts: "VIVEK SINGH" → "Vivek Singh"
Use case: Names, city names, department names in real datasets

### PROPER on departments
=PROPER(C2)
Converts: "MARKETING", "sales", "FINANCE" → consistent Proper Case
Real world: Same department written 5 different ways in exports

### COUNTA — Catch missing data instantly
=COUNTA(A2:A6) → returned 4 instead of 5
Instantly revealed one blank row in the dataset
Key insight: Always run COUNTA before analysing any dataset

---

## Key insight from today
Real company data is always messy.
HR exports, CRM dumps, ERP reports — inconsistent cases,
blank rows, duplicate entries. 
Clean first. Analyse second. That's the analyst's first rule.

---

## VLOOKUP vs XLOOKUP — Summary
| Feature | VLOOKUP | XLOOKUP |
|---------|---------|---------|
| Column reference | Number (fragile) | Direct (clean) |
| Direction | Left to right only | Both directions |
| Error handling | Manual IFERROR needed | Built-in |
| Industry usage | Legacy | Current standard |

---

## Skills practised today
- VLOOKUP with exact match
- XLOOKUP modern syntax
- PROPER function for text standardisation
- COUNTA for missing data detection
- Cross-sheet referencing (RAW_DATA!A:C)

---

## Tomorrow — Day 3
- Advanced data cleaning: TRIM, SUBSTITUTE, Remove Duplicates
- Conditional Formatting deep dive
- Start building the Excel Sales Dashboard project
