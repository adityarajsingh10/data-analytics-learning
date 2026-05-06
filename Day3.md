# Day 3 — Advanced Data Cleaning
**Date:** 6 May 2026
**Topic:** TRIM, PROPER+TRIM, SUBSTITUTE, Remove Duplicates

---

## What I worked on today
Built a data cleaning sheet with intentionally messy data —
extra spaces, inconsistent casing, duplicate cities.
Cleaned it using 3 formulas and 1 Excel feature.

---

## Formulas used

### TRIM — Remove extra spaces
=TRIM(A2)
Removes leading, trailing and double spaces from text.
"  Aditya Singh  " → "Aditya Singh"

### PROPER + TRIM — Combined cleaning
=PROPER(TRIM(A2))
Fixes case AND removes spaces in one formula.
"ARYAN SINGH" → "Aryan Singh"
This is the version analysts actually use in production.

### SUBSTITUTE — Find and replace inside formula
=SUBSTITUTE(A3,"VIVEK","Vivek")
Replaces specific text without touching the rest.
Useful when PROPER gives wrong results (e.g. McDonald's)

---

## Technique — Remove Duplicates
Data tab → Remove Duplicates → select column → OK
Mumbai appeared twice (as "Mumbai" and "mumbai")
Excel treated both as same — case insensitive
Result: 3 unique cities from 5 rows

---

## Key insight today
TRIM is always step one before any text analysis.
Invisible spaces cause VLOOKUP failures, wrong COUNTIFs,
broken pivot tables — all because of a space you can't see.
Clean first. Always.

---

## Skills practised
- TRIM for whitespace removal
- PROPER+TRIM combined formula
- SUBSTITUTE for targeted replacement
- Remove Duplicates feature
- Understanding case-insensitive deduplication

---

## Tomorrow — Day 4
- Building the Excel Sales Dashboard from scratch
- Charts, slicers, dynamic summaries
- First real project upload to GitHub
