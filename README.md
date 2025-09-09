# Day Count Convention
This is a lightweight Python implementation of financial day count conventions, providing an alternative to QuantLib for calculating days and years between dates in financial applications.

## Functions
- `day_count()`: Calculates the actual number of days between two dates
- `year_count()`: Calculates the fraction of years between two dates

## Supporting Type
- 0: actual/actual
- 1: 30/360 (SIA)
- 2: actual/360
- 3: actual/365
- 4: 30/360 (PSA)
- 5: 30/360 (ISDA)
- 6: 30/360 (European)
- 7: actual/365 (Japanese)
  
## Reference
https://www.mathworks.com/help/fininst/day-count-basis.html
