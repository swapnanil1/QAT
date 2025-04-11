# Applications of Percentage Change: Population and Depreciation

Tags: #quant #percentages #applications #population_change #depreciation #successive_change #concepts

## Overview

Percentage changes, particularly successive percentage changes, have direct applications in modeling real-world scenarios like population growth/decay and the depreciation of assets. Understanding these applications often involves recognizing the pattern of repeated percentage change over time periods.

## 1. Population Growth/Decay

Population changes are typically expressed as an annual percentage rate (increase or decrease).

### Formula (Using Successive Change Logic)

Let:
*   `P0` = Initial Population
*   `R` = Annual rate of change (as a percentage)
*   `r` = Annual rate of change (as a decimal: r = R/100)
    *   Use `+r` for growth (increase)
    *   Use `-r` for decay (decrease)
*   `n` = Number of years
*   `P_n` = Population after `n` years

The calculation involves applying the percentage change `n` times successively. This leads to a formula very similar to compound interest:

**Formula:** ```P_n = P0 * (1 + r)^n```
*   If the population **increases** at R% per annum: `P_n = P0 * (1 + R/100)^n`
*   If the population **decreases** at R% per annum: `P_n = P0 * (1 - R/100)^n`

**Finding Past Population:** If you know the current population (`P_n`) and want to find the population `n` years ago (`P0`), rearrange the formula: P0 = P_n / (1 + r)^n

**Variable Rates:** If the rate changes each year (e.g., R1% in year 1, R2% in year 2, R3% in year 3), use the multiplication factor method:
P_n = P0 * (1 + R1/100) * (1 + R2/100) * (1 + R3/100) * ...```(Use 1 - R/100 for decreases).```

## 2. Depreciation
Depreciation refers to the decrease in the value of an asset (like a car, machine, etc.) over time due to use, wear and tear, or obsolescence. It's commonly calculated as a fixed percentage of the asset's value at the beginning of each year (similar to population decay or compound interest calculated in reverse).

### Formula (Using Successive Decrease Logic)

Let:

- V0 = Original Value (or Value at the beginning)
    
- R = Annual rate of depreciation (as a percentage)
    
- n = Number of years
    
- V_n = Value after n years (Scrap Value, Depreciated Value)
    

**Formula:** 
```V_n = V0 * (1 - R/100)^n```
**Finding Original Value:** If you know the depreciated value (`V_n`) and want to find the original value `n` years ago (`V0`):

```V0 = V_n / (1 - R/100)^n```
**Variable Depreciation Rates:** If the depreciation rate changes each year (e.g., R1% in year 1, R2% in year 2), use multiplication factors:

```V_n = V0 * (1 - R1/100) * (1 - R2/100) * ...```
Final formula calculates the final value `V_n` after `n` years, where the rate of depreciation changes from year to year.
## Key Connection

Both population change (at a constant rate) and depreciation (at a constant rate) are applications of **successive percentage change**. The formulas are essentially derived from repeatedly multiplying by the factor `(1 + R/100)` for growth or `(1 - R/100)` for decrease/depreciation. This mathematical structure is identical to the calculation of Compound Amount in [[04 - Simple and Compound Interest/02 - Compound Interest (CI) Formula and Concepts]].

## Related Concepts

*   [[02 - Percentages/03 - Successive Percentage Change]] (The underlying principle)
*   [[04 - Simple and Compound Interest/02 - Compound Interest (CI) Formula and Concepts]] (Identical mathematical structure for growth/compounding)
*   [[12 - Algebra/04 - Indices and Surds]] (Handling the exponent 'n' in calculations)