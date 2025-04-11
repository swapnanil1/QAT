# Quant ## Simple Interest (SI) Formula and Concepts

#quant #simple_and_compound_interest #simple_interest #formula #concepts

## Definition

Simple Interest (SI) is a method of calculating the interest charge on a loan or investment based *only* on the original **Principal** amount. Unlike compound interest, the interest earned or paid in each period is *not* added back to the principal for calculating the interest of subsequent periods. Hence, the interest amount remains constant for each period, assuming the rate and principal don't change.

## Key Terms

*   **Principal (P):** The initial sum of money borrowed, lent, or invested.
*   **Rate (R):** The percentage at which interest is calculated on the principal. It's typically expressed *per annum* (p.a.), meaning per year.
*   **Time (T):** The duration for which the money is borrowed, lent, or invested. **Crucially, for formula use, time must be expressed in years.**
*   **Interest (SI):** The monetary charge for borrowing money or the earnings from an investment, calculated using the simple interest method.
*   **Amount (A):** The total sum due at the end of the time period. It's the sum of the Principal and the Simple Interest. A = P + SI.

## Core Formulas

### 1. Calculating Simple Interest (SI)

```SI = (P * R * T) / 100```

*   P: Principal amount
*   R: Annual Rate of Interest (in %)
*   T: Time duration (in **years**)

### 2. Calculating Amount (A)

```A = P + SI```

Substituting the SI formula:
```
A = P + (P * R * T) / 100
A = P * (1 + (R * T) / 100)
```
### 3. Finding Principal (P) when SI, R, T are known

```P = (SI * 100) / (R * T)```
### 4. Finding Rate (R) when SI, P, T are known

```R = (SI * 100) / (P * T)```
*   The result will be the rate in % per annum.

### 5. Finding Time (T) when SI, P, R are known

```T = (SI * 100) / (P * R)```
*   The result will be the time in years.

## Important Considerations & Shortcuts for Exams

*   **Time Unit Conversion:** Always convert the given time into **years** before using the formulas.
    *   If Time is in months: T (in years) = Number of Months / 12
    *   If Time is in days: T (in years) = Number of Days / 365 (Unless a leap year is specified, use 365 for standard calculations in aptitude tests).
*   **Rate Period:** Ensure the rate period matches the time unit (usually per annum rate and time in years).
*   **"Amount becomes n times":** If it's stated that a sum P becomes 'n' times itself (Amount A = n*P) in T years at simple interest, then the Simple Interest earned is SI = A - P = n*P - P = (n-1)P.
    *   **Shortcut for Rate:** Substitute SI in the rate formula: R = ((n-1)P * 100) / (P * T) => R = ((n - 1) / T) * 100 %
    *   **Shortcut for Time:** Substitute SI in the time formula: T = ((n-1)P * 100) / (P * R) => T = ((n - 1) / R) * 100 years
*   **Variable Rates:** If the interest rate changes over the total duration (e.g., R1% for the first T1 years, R2% for the next T2 years, R3% for the period beyond T1+T2 years up to a total time T), the total Simple Interest is the sum of interests calculated for each period:
    ```Total SI = [ (P * R1 * T1) / 100 ] + [ (P * R2 * T2) / 100 ] + [ (P * R3 * T3) / 100 ] + ...```
    
    ```Total SI = P * ( (R1*T1) + (R2*T2) + (R3*T3) + ... ) / 100```
    
    Where T1, T2, T3... are the duration for which rates R1, R2, R3... apply respectively.
## Related Concepts

*   The core idea builds upon [[02 - Percentages/01 - Basic Concepts and Conversions.md]].
*   It's crucial to distinguish SI from [[04 - Simple and Compound Interest/02 - Compound Interest (CI) Formula and Concepts.md]].
*   Understanding the [[04 - Simple and Compound Interest/03 - Difference between CI and SI.md]] is a common exam topic.
*   Concepts might be combined with [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]] (e.g., splitting an amount and investing at different SI rates).

## Example Links

*   [[04 - Simple and Compound Interest/01.E01 - Calculating Simple Interest Example.md]]
*   [[04 - Simple and Compound Interest/01.E02 - Finding Principal Rate Time in SI Example.md]]