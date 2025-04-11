## Compound Interest (CI) Formula and Concepts

#quant #simple_and_compound_interest #compound_interest #formula #concepts

## Definition

Compound Interest (CI) is the interest calculated on the initial Principal *and* also on the accumulated interest from previous periods. Essentially, the interest earned in one period is added back to the principal, forming a new, larger principal for the next calculation period. This leads to exponential growth of the investment or loan amount over time. It's often referred to as "interest on interest".

## Key Terms

*   **Principal (P):** The initial amount of money.
*   **Rate (R):** The interest rate per compounding period (usually expressed annually, p.a., but needs adjustment based on compounding frequency).
*   **Time (T or n):** The total duration of the investment/loan, usually in years. Often represented by 'n' in formulas, especially when dealing with the number of compounding periods.
*   **Compounding Frequency (k):** The number of times interest is calculated and added to the principal *per year*.
    *   Annually: k = 1
    *   Half-yearly (or Semi-annually): k = 2
    *   Quarterly: k = 4
    *   Monthly: k = 12
*   **Amount (A):** The final amount after time T, including the principal and the accumulated compound interest.
*   **Compound Interest (CI):** The total interest earned or paid. CI = A - P.

## Formulas

### 1. Calculating Amount (A) when compounded annually (k=1)
```A = P * (1 + R/100)^T```
*   Where:
    *   A = Amount
    *   P = Principal
    *   R = Annual Rate of Interest (in %)
    *   T = Time (in years)

### 2. Calculating Amount (A) when compounded 'k' times per year
```A = P * (1 + (R/k) / 100)^(k*T)```
*   Or sometimes written as: `A = P * (1 + r)^n`
    *   Where `r = R / (k * 100)` is the interest rate per compounding period.
    *   And `n = k * T` is the total number of compounding periods.

**Adjustments based on Compounding Frequency:**

*   **Half-yearly (k=2):** Amount `A = P * (1 + (R/2)/100)^(2*T)` (Rate is halved, Time is doubled)
*   **Quarterly (k=4):** Amount `A = P * (1 + (R/4)/100)^(4*T)` (Rate is quartered, Time is quadrupled)
*   **Monthly (k=12):** Amount `A = P * (1 + (R/12)/100)^(12*T)` (Rate divided by 12, Time multiplied by 12)

### 3. Calculating Compound Interest (CI)
```
CI = Amount (A) - Principal (P)  
CI = [ P * (1 + (R/k) / 100)^(kT) ] - P  
CI = P * [ (1 + (R/k) / 100)^(kT) - 1 ]
```

### 4. When Rates are different for different years (Compounded Annually)

If the annual interest rates are R1%, R2%, R3%... for the 1st, 2nd, 3rd... year respectively:
```
A = P * (1 + R1/100) * (1 + R2/100) * (1 + R3/100) * ... 
```
## Important Considerations & Shortcuts for Exams

*   **Compounding Frequency:** Pay close attention to how often the interest is compounded (annually, half-yearly, quarterly). This significantly affects the calculation. **This is a very common trap in MCQs.** Adjust the Rate (R) and Time (T) in the formula accordingly:
    *   Divide the annual rate R by the number of compounding periods per year (k).
    *   Multiply the time T (in years) by the number of compounding periods per year (k).
*   **Time in Fractions:** If the time is a fraction (e.g., 2 years and 3 months = 2 1/4 years), apply the formula carefully.
    *   For T = a (b/c) years (e.g., 2 3/4 years), compounded annually:
        Calculate the amount for the whole number of years ('a') using the standard CI formula. Then, calculate Simple Interest on *this amount* for the fractional part of the year ('b/c') at the given annual rate R.
        The formula combines these steps:
        ```
        A = P * (1 + R/100)^a * (1 + ((b/c) * R)/100)
        ```
*   **Successive Percentage Change:** Compound interest is essentially an application of [[02 - Percentages/03 - Successive Percentage Change.md]]. For 2 years at R%, the amount is `P*(1+R/100)*(1+R/100)`. For 3 years, multiply by `(1+R/100)` again. This perspective can be useful for quick calculations or estimations, especially for 2 or 3 periods.
*   **Rule of 72 (Approximation):** To *estimate* the number of years (T) it takes for an investment to double at a given annual compound interest rate R:
    ```
    Years to Double (T) ≈ 72 / R
    ```
    This is a useful mental shortcut, most accurate for rates between 5% and 15%. For example, at 8% CI, it takes approx 72/8 = 9 years to double.

## Related Concepts

*   Directly contrasts with [[04 - Simple and Compound Interest/01 - Simple Interest (SI) Formula and Concepts.md]].
*   The [[04 - Simple and Compound Interest/03 - Difference between CI and SI.md]] is a key concept derived from SI and CI.
*   Installment calculations often use CI principles: [[04 - Simple and Compound Interest/04 - Installments.md]].
*   Builds heavily on [[02 - Percentages/01 - Basic Concepts and Conversions.md]] and [[02 - Percentages/03 - Successive Percentage Change.md]].

## Example Links

*   [[04 - Simple and Compound Interest/02.E01 - Calculating Compound Interest (Yearly) Example.md]]
*   [[04 - Simple and Compound Interest/02.E02 - Calculating CI (Half-Yearly Compounding) Example.md]]
*   [[04 - Simple and Compound Interest/02.E03 - Finding Amount in CI Example.md]]