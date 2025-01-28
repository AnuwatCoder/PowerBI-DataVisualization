# Data Analysis Expressions (DAX)

This repository provides basic examples of Data Analysis Expressions (DAX) used for creating calculated columns and measures in Power BI, Excel, and other Microsoft tools.

## DAX Expressions

### SUM_SCORE
This DAX expression calculates the total score by summing values from multiple columns (`A1`, `A2`, `A3`, `A4`, `A5`) in a given table.

```DAX
SUM_SCORE = Table[A1] + Table[A2] + Table[A3] + Table[A4] + Table[A5]
