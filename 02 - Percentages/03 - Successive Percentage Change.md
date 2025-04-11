# Successive Percentage Change

Tags: #quant #percentages #successive_change #percentage_change #concepts

## Definition

Successive percentage change occurs when a value is subjected to multiple percentage changes one after the other. The key is that each subsequent percentage change is calculated on the **new value** obtained after the previous change, not on the original value.

**Example Scenario:** The price of an item is first increased by 10% and then decreased by 20%. The 20% decrease is applied to the price *after* the 10% increase.

## Methods for Calculation

### 1. Step-by-Step Calculation

Calculate the result after each percentage change sequentially.

*   **Example:** If a value of 100 is increased by 10% and then decreased by 20%:
    1.  **First Change (10% Increase):**
        New Value = 100 * (1 + 10/100) = 100 * 1.10 = 110
    2.  **Second Change (20% Decrease on the *new* value):**
        Final Value = 110 * (1 - 20/100) = 110 * 0.80 = 88
    3.  **Net Change:** The value changed from 100 to 88, a net decrease of 12 or 12%.

### 2. Using Multiplication Factors (Recommended for >2 changes)

This is often the most efficient method, especially for multiple changes. Multiply the original value by the multiplication factors corresponding to each change.

*   **Multiplication Factor for x% Increase:** `(1 + x/100)`
*   **Multiplication Factor for y% Decrease:** `(1 - y/100)`

**Formula:**
Final Value = Original Value * Factor1 * Factor2 * Factor3 * ...

*   **Example (Same as above):** 10% increase (Factor = 1.10), 20% decrease (Factor = 0.80)
    Final Value = 100 * 1.10 * 0.80 = 100 * 0.88 = 88
    Net Multiplication Factor = 1.10 * 0.80 = 0.88

*   **Net Percentage Change from Net Factor:**
    Net Factor = 0.88
    This means the final value is 88% of the original value.
    The decrease is `1 - 0.88 = 0.12`, which corresponds to a **12% decrease**.
    *General:* Net % Change = (Net Factor - 1) * 100% (Result is positive for increase, negative for decrease).

### 3. Formula for Net Percentage Change (For Two Changes Only)

A common shortcut formula exists for calculating the net percentage change after **exactly two** successive changes.

Let the two percentage changes be `a%` and `b%`.
*   Use positive values for `a` and `b` if they are increases.
*   Use negative values for `a` and `b` if they are decreases.

**Formula:** Net Percentage Change = [ a + b + (a * b / 100) ] %

*   **Example (Same as above):** 10% increase (a = +10), 20% decrease (b = -20)
    Net % Change = [ 10 + (-20) + (10 * (-20) / 100) ] %
    Net % Change = [ 10 - 20 + (-200 / 100) ] %
    Net % Change = [ -10 - 2 ] %
    Net % Change = -12 %
    This indicates a net decrease of 12%.

**Caution:** While quick, this formula is only for two changes. For three or more changes, use the multiplication factor method or apply the formula iteratively (find net change for first two, then combine that result with the third change, etc., which can be tedious).

## Key Takeaway

Successive percentage changes are **not additive**. A 10% increase followed by a 10% decrease does *not* result in a 0% net change.
Using the formula: `Net % Change = [ 10 + (-10) + (10 * -10 / 100) ] % = [ 0 - 1 ] % = -1%` (a net 1% decrease).
Using factors: `Original * 1.10 * 0.90 = Original * 0.99`. Final value is 99% of original, hence a 1% decrease.

## Related Concepts

*   [[02 - Percentages/02 - Percentage Increase and Decrease]]
*   [[02 - Percentages/04 - Applications (Population, Depreciation)]] (Population growth/decay and depreciation are often modeled using successive changes)
*   [[03 - Profit and Loss/04 - Successive Discounts]] (A direct application of successive percentage decreases)
*   [[04 - Simple and Compound Interest/02 - Compound Interest (CI) Formula and Concepts]] (Compound interest is essentially successive percentage increase)