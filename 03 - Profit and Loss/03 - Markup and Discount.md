# Markup and Discount

Tags: #quant #profit_and_loss #markup #discount #marked_price #list_price #concepts

## Introduction

In retail scenarios, items are often tagged with a price higher than their cost price, and then a reduction (discount) is offered on this tag price to attract customers. This introduces two key terms: Marked Price and Discount.

## Definitions

### 1. Marked Price (MP)

*   **Also known as:** List Price, Tag Price, Advertised Price.
*   **Definition:** The price printed or tagged on an article by the seller. This is the price *before* any discount is applied.
*   It is usually set higher than the Cost Price (CP) to allow for discounts while still potentially making a profit.

### 2. Markup

*   **Definition:** The amount added to the Cost Price (CP) to arrive at the Marked Price (MP). It can be expressed as an absolute value or as a percentage of the CP.
*   **Formula (Amount):** `Markup = MP - CP`
*   **Formula (Percentage):** `Markup % = (Markup Amount / CP) * 100 %`
*   **Relationship:** `MP = CP + Markup Amount = CP * (1 + Markup % / 100)`

### 3. Discount

*   **Definition:** A reduction offered by the seller on the Marked Price (MP) of an article. It is usually expressed as a percentage of the MP.
*   **Purpose:** To attract customers, clear stock, or compete with other sellers.
*   **Crucial Point:** Discount is **always calculated on the Marked Price (MP)**, unless explicitly stated otherwise.
*   **Formula (Amount):** `Discount Amount = (Discount % / 100) * MP`
*   **Relationship:** `Selling Price (SP) = Marked Price (MP) - Discount Amount`

## Relationship between CP, MP, and SP

These three prices are linked through Markup and Discount:

1.  **CP to MP:** The seller adds a Markup to the CP.
    `MP = CP * (1 + Markup % / 100)`
2.  **MP to SP:** The seller offers a Discount on the MP.
    `SP = MP * (1 - Discount % / 100)`

Combining these, we can express the Selling Price directly in terms of the Cost Price, Markup Percentage, and Discount Percentage: 
```SP = [ CP * (1 + Markup % / 100) ] * (1 - Discount % / 100)```
Alternatively, writing the factors using the 100 base:*`
```SP = CP * [(100 + Markup %) / 100] * [(100 - Discount %) / 100]```
Both formulas are mathematically equivalent.

## Calculating Overall Profit or Loss
Even after giving a discount, the seller might make a profit or a loss. This overall profit or loss is still calculated by comparing the **final Selling Price (SP)** with the **initial Cost Price (CP)**.

- Overall Profit / Loss = SP - CP
    
- Overall Profit / Loss % = [(SP - CP) / CP] * 100 %
    

**Important Note:** The Markup Percentage is not the Profit Percentage, and the Discount Percentage is not the Loss Percentage. Profit/Loss depends on the final SP relative to the initial CP.
## Key Takeaway

Markup is the increase from CP to MP. Discount is the decrease from MP to SP. Profit/Loss is the final comparison between SP and CP. The entire process (Markup followed by Discount) is an application of [[02 - Percentages/03 - Successive Percentage Change]].

## Related Concepts

- [[03 - Profit and Loss/01 - Basic Terminology (CP, SP, Profit, Loss)]]
    
- [[03 - Profit and Loss/02 - Finding SP CP given Profit Loss %]]
    
- [[02 - Percentages/03 - Successive Percentage Change]] (The CP -> MP -> SP transition follows this pattern)
    
- [[03 - Profit and Loss/04 - Successive Discounts]] (Extends the discount concept)