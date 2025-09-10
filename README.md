# Day Count Convention
This is a lightweight Python implementation of financial day count conventions, providing an alternative to QuantLib for calculating days and years between dates in financial applications.

## Features
- Functions:
  - `day_count()`: Calculates the number of days between two dates
  - `year_count()`: Calculates the fraction of years between two dates
- No dependencies: Uses only `pandas` library

## Supporting Type
- 0: actual/actual
- 1: 30/360 (SIA)
- 2: actual/360
- 3: actual/365
- 4: 30/360 (PSA)
- 5: 30/360 (ISDA)
- 6: 30/360 (European)
- 7: actual/365 (Japanese)

## Examples
t1 = pd.to_datetime("2025-09-10") \\
t2 = pd.to_datetime("2027-12-15") \\
No_days = day_count(t1, t2, basis=6) \\
No_years = year_count(t1, t2, basis=6)

## Reference
https://www.mathworks.com/help/fininst/day-count-basis.html
