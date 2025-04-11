# Successive Discounts

Tags: #quant #profit_and_loss #discount #successive_discounts #marked_price #selling_price #successive_change #concepts

## Definition

Successive discounts occur when **two or more discounts** are applied one after the other to the Marked Price (MP) of an article.

**Example Scenario:** An item has a Marked Price of ₹1000. The seller offers a 20% discount, and then an *additional* 10% discount on the reduced price.

**Crucial Point:** Each subsequent discount is calculated on the price **after** the previous discount has been applied, not on the original Marked Price.

---

## Why Discounts are Not Additive (Common Pitfall)

A common mistake is to simply add the discount percentages. Using the example above (20% then 10% off ₹1000):

*   **Incorrect Assumption:** Total Discount = 20% + 10% = 30%. This is **wrong**.
*   **Correct Calculation:**
    1.  **First Discount (20%):**
        *   Discount Amount 1 = 20% of ₹1000 = ₹200
        *   Price after 1st Discount = ₹1000 - ₹200 = **₹800**
    2.  **Second Discount (10% on the reduced price):**
        *   Discount Amount 2 = 10% of **₹800** = ₹80
        *   Final Selling Price (SP) = ₹800 - ₹80 = **₹720**
*   **Analysis:**
    *   Total Discount Amount = ₹200 + ₹80 = ₹280
    *   Net Equivalent Discount Percentage = (Total Discount / Original MP) * 100 = (280 / 1000) * 100 = **28%**

Successive discounts result in a lower *total discount amount* than simply adding the percentages because subsequent discounts apply to a smaller base price.

---

## Calculating Final Selling Price (SP)

### Method 1: Step-by-Step Calculation

Calculate the price after each discount sequentially, as demonstrated in the example above. This method is accurate but can be time-consuming for multiple discounts.

### Method 2: Using Multiplication Factors (Recommended)

This is generally the most efficient method. A discount of D% corresponds to a multiplication factor of `(1 - D/100)`, representing the remaining portion of the price.

**Formula:**
```
SP = MP * Factor1 * Factor2 * Factor3 * ...  
SP = MP * (1 - D1/100) * (1 - D2/100) * (1 - D3/100) * ...
```

*   **Example (20% then 10% on MP=1000):**
    *   Factor 1 (20% off) = `1 - 20/100 = 0.80`
    *   Factor 2 (10% off) = `1 - 10/100 = 0.90`
    *   Calculation:
        ```
        SP = 1000 * 0.80 * 0.90
        SP = 1000 * 0.72
        SP = ₹720
        ```

---

## Calculating Net Equivalent Single Discount

This is the single discount percentage that yields the same final Selling Price.

### Method 1: Using the Final SP

1.  Calculate the final SP (using either method above).
2.  Calculate the total discount amount:
    ```
    Total Discount Amount = MP - SP
    ```
3.  Calculate the net discount percentage:
    ```
    Net Discount % = (Total Discount Amount / MP) * 100 %
    ```
*   **Example:** SP = 720, MP = 1000. Total Discount = 280.
    `Net Discount % = (280 / 1000) * 100 = 28%`

### Method 2: Using Net Multiplication Factor

1.  Calculate the Net Multiplication Factor by multiplying the individual factors:
    ```
    Net Factor = Factor1 * Factor2 * Factor3 * ...
    ```
2.  The net discount percentage `D_net` is related to the net factor:
    `Net Factor = 1 - D_net / 100`
3.  Solve for `D_net`:
    ```
    D_net = (1 - Net Factor) * 100 %
    ```
*   **Example:** Net Factor = 0.80 * 0.90 = 0.72.
    `D_net = (1 - 0.72) * 100 % = 0.28 * 100 % = 28%`

### Method 3: Formula for Net Discount (For Two Discounts Only)

This formula directly calculates the net discount for exactly **two** successive discounts, D1% and D2%. It derives from the successive percentage change formula `a + b + ab/100` with negative values for discounts.

**Formula:** ```Net Equivalent Discount % = [ D1 + D2 - (D1 * D2 / 100) ] %```
*   **Example (20% and 10%):**
    ```
    Net Discount % = [ 20 + 10 - (20 * 10 / 100) ] %
    Net Discount % = [ 30 - (200 / 100) ] %
    Net Discount % = [ 30 - 2 ] %
    Net Discount % = 28 %
    ```
**Caution:** Do not use this formula for more than two discounts. Use Method 1 or 2 instead.

---

## Order Doesn't Matter

Since multiplication is commutative (`Factor1 * Factor2 = Factor2 * Factor1`), the **order** in which successive discounts are applied does **not** affect the final Selling Price or the Net Equivalent Single Discount.

---

## Related Concepts

*   [[03 - Profit and Loss/03 - Markup and Discount]] (Introduces single discount)
*   [[02 - Percentages/03 - Successive Percentage Change]] (The underlying mathematical principle)