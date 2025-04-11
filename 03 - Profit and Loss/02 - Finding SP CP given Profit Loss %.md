# Finding Selling Price (SP) and Cost Price (CP) Given Profit/Loss Percentage

Tags: #quant #profit_and_loss #selling_price #cost_price #profit_percentage #loss_percentage #concepts #formula

## Introduction

A common type of Profit and Loss problem involves calculating either the Selling Price (SP) or the Cost Price (CP) when the other price and the profit or loss percentage are provided. These calculations rely on the fundamental relationships established in [[03 - Profit and Loss/01 - Basic Terminology (CP, SP, Profit, Loss)]].

## Formulas

Remember that Profit% and Loss% are calculated on the Cost Price (CP).

### 1. Finding Selling Price (SP)

*   **Given CP and Profit %:**
    If an item is sold at a profit of `P%`, the Selling Price is `P%` *more* than the Cost Price.
    `SP = CP + Profit`
    `SP = CP + (P/100 * CP)`
    `SP = CP * (1 + P/100)`
    **Formula:**
    ```
    SP = CP * [(100 + Profit %) / 100]
    ```

*   **Given CP and Loss %:**
    If an item is sold at a loss of `L%`, the Selling Price is `L%` *less* than the Cost Price.
    `SP = CP - Loss`
    `SP = CP - (L/100 * CP)`
    `SP = CP * (1 - L/100)`
    **Formula:**
    ```
    SP = CP * [(100 - Loss %) / 100]
    ```

*   **Unified Approach (Using Multiplication Factor):**
    This combines both scenarios, derived from the percentage increase/decrease concept [[02 - Percentages/02 - Percentage Increase and Decrease]].
    *   For Profit P%: Factor = `(1 + P/100)`
    *   For Loss L%: Factor = `(1 - L/100)`
    ```
    SP = CP * Multiplication_Factor
    ```

### 2. Finding Cost Price (CP)

These formulas are derived by rearranging the SP formulas above.

*   **Given SP and Profit %:**
    If an item was sold at a profit of `P%`, the SP represents `(100 + P)%` of the CP.
    From `SP = CP * [(100 + Profit %) / 100]`, we get:
    **Formula:**
    ```
    CP = SP * [100 / (100 + Profit %)]
    ```
    Alternatively:
    ```
    CP = SP / (1 + Profit % / 100)
    ```

*   **Given SP and Loss %:**
    If an item was sold at a loss of `L%`, the SP represents `(100 - L)%` of the CP.
    From `SP = CP * [(100 - Loss %) / 100]`, we get:
    **Formula:**
    ```
    CP = SP * [100 / (100 - Loss %)]
    ```
    Alternatively:
    ```
    CP = SP / (1 - Loss % / 100)
    ```

*   **Unified Approach (Using Multiplication Factor):**
    ```
    CP = SP / Multiplication_Factor
    ```
    Where the Multiplication Factor is `(1 + P/100)` for profit or `(1 - L/100)` for loss.

## Key Takeaway

The multiplication factor method (`SP = CP * Factor` and `CP = SP / Factor`) provides a consistent way to handle all these calculations, directly linking them to basic percentage increase/decrease concepts. Understanding this relationship is often more efficient than memorising four separate formulas.

## Related Concepts

*   [[03 - Profit and Loss/01 - Basic Terminology (CP, SP, Profit, Loss)]] (Foundation)
*   [[02 - Percentages/02 - Percentage Increase and Decrease]] (Core concept for factors)
*   [[03 - Profit and Loss/03 - Markup and Discount]] (Extends these calculations)