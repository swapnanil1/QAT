# Alligation Rule Concept

#quant #mixtures_and_alligations #alligation_rule #ratio_concepts #formula #shortcut

## Definition

Alligation (or the Rule of Alligation) is a rule that enables us to find the ratio in which two or more ingredients at given prices (or concentrations, speeds, etc.) must be mixed to produce a mixture of a desired price (or concentration, speed, etc.).

It's essentially a visual technique to solve problems related to weighted averages, expressed in terms of ratios. It helps determine the proportion in which two quantities with different characteristics must be mixed to obtain a mixture with a characteristic that lies between the two.

## The Rule

Suppose we have two ingredients:
*   Ingredient 1 (Cheaper/Lower Quantity): Characteristic `C` (e.g., cost price, concentration)
*   Ingredient 2 (Dearer/Higher Quantity): Characteristic `D` (e.g., cost price, concentration)
*   Desired Mixture: Mean Characteristic `M` (e.g., mean price, final concentration)

**Condition:** `C < M < D`. The mean characteristic must lie between the characteristics of the two ingredients being mixed.

The Alligation Rule states that the ratio in which Ingredient 1 and Ingredient 2 must be mixed is:

`(Quantity of Cheaper) / (Quantity of Dearer) = (D - M) / (M - C)`

**Graphical Representation:**

```text
 Ingredient 1                    Ingredient 2
 (Cheaper/Lower)                 (Dearer/Higher)
      C                             D
       \                           /
        \                         /
         Mean Characteristic (M)
        /                         \
       /                           \
    (D - M)                      (M - C)
      |                             |
      v                             v
Ratio Part for                Ratio Part for
Ingredient 1                  Ingredient 2

Ratio Part for Ingredient 1 Ratio Part for Ingredient 2
```
So, the required ratio is `(D - M) : (M - C)`.

## Key Points for Application

1.  **Uniform Characteristic:** All three values (`C`, `D`, `M`) must represent the same characteristic (e.g., all cost prices per unit, all percentage concentrations, all speeds).
2.  **Unit Consistency:** Ensure all values are in the same units (e.g., cost per kg, percentage strength).
3.  **Characteristic Type:**
    *   If `C`, `D`, `M` are **cost prices**, the resulting ratio is the ratio of **quantities** mixed.
    *   If `C`, `D`, `M` are **concentrations** (e.g., % milk), the resulting ratio is the ratio of the **amounts** (volumes/weights) of the solutions mixed.
4.  **Selling Price vs. Cost Price:** If the problem involves Selling Price (SP) and a profit/loss percentage for the mixture, you *must* first calculate the Cost Price (CP) of the mixture before applying the Alligation Rule. Alligation works on cost prices or inherent characteristics, not selling prices that include profit/loss. `CP = SP / (1 + Profit%)` or `CP = SP / (1 - Loss%)`. See [[03 - Profit and Loss/02 - Finding SP CP given Profit Loss %.md]].

## Application Examples

*   Mixing two varieties of rice/wheat/tea with different costs to get a mixture with a desired cost.
*   Mixing two solutions with different concentrations (e.g., acid, milk, alcohol) to achieve a target concentration.
*   Finding the ratio of cheaper and dearer items sold to achieve an average price.
*   Sometimes used metaphorically in average speed or weighted average problems. See [[08 - Averages/03 - Weighted Average.md]].

## Related Concepts

*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]] (The result of alligation is a ratio)
*   [[08 - Averages/01 - Basic Average Formula.md]]
*   [[08 - Averages/03 - Weighted Average.md]] (Alligation is a method to solve weighted average problems)
*   [[02 - Percentages/01 - Basic Concepts and Conversions.md]] (Used when dealing with concentrations)
*   [[03 - Profit and Loss/01 - Basic Terminology (CP, SP, Profit, Loss).md]] (Important when dealing with prices)