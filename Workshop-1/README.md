# Data Analysis Expressions (DAX) Examples

This repository contains basic examples of Data Analysis Expressions (DAX) used to create calculated columns and measures in Power BI, Excel, and other Microsoft tools. Below are examples of common DAX expressions for summing values and calculating grades.

## 1. `SUM_SCORE`: Calculate Total Score

This DAX expression calculates the total score by summing values from multiple columns (`A1`, `A2`, `A3`, `A4`, `A5`) in a given table.

### Expression

```DAX
SUM_SCORE = 
Table[A1] + Table[A2] + Table[A3] + Table[A4] + Table[A5]
