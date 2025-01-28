# Data Analysis Expressions (DAX)

This repository provides basic examples of Data Analysis Expressions (DAX) used for creating calculated columns and measures in Power BI, Excel, and other Microsoft tools.

## DAX Expressions

### SUM_SCORE
This DAX expression calculates the total score by summing values from multiple columns (`A1`, `A2`, `A3`, `A4`, `A5`) in a given table.

```DAX
SUM_SCORE = Table[A1] + Table[A2] + Table[A3] + Table[A4] + Table[A5]


# DAX Grade Calculation Example

This repository contains an example of using Data Analysis Expressions (DAX) to calculate grades based on scores in Power BI, Excel, or other Microsoft tools.

## DAX Expression: GRADE

The following DAX expression is used to calculate the grade of a student based on their score in column `A2` of a table.

### Expression

```DAX
GRADE = 
SWITCH(TRUE(),
    'Table'[A2] >= 90, "A",    // If score in A2 is 90 or above, return "A"
    'Table'[A2] >= 80, "B",    // If score in A2 is 80 or above, return "B"
    'Table'[A2] >= 70, "C",    // If score in A2 is 70 or above, return "C"
    'Table'[A2] >= 60, "D",    // If score in A2 is 60 or above, return "D"
    'Table'[A2] < 60, "F"      // If score in A2 is below 60, return "F"
)
