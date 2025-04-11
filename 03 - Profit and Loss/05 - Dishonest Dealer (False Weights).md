# Dishonest Dealer (Using False Weights)

Tags: #quant #profit_and_loss #dishonest_dealer #false_weights #profit_calculation #concepts #tricky_question

## Introduction

A common type of "tricky" profit and loss problem involves a dishonest dealer who uses faulty weights or measures. They might claim to sell goods at Cost Price (CP) or a nominal profit/loss, but their actual profit comes from manipulating the *quantity* of goods delivered.

## The Core Concept: Profit from Quantity Manipulation

The fundamental principle is that the dealer charges the customer for a certain weight (the *Professed Weight* or *True Weight*, e.g., 1 kg = 1000g) but actually delivers a lesser quantity using a faulty weight (the *Actual Weight* or *False Weight*, e.g., 900g).

The dealer's **Cost Price (CP)** corresponds to the **Actual Weight** they deliver.
The dealer's **Selling Price (SP)** corresponds to the **Professed Weight** they charge for.

Even if they *claim* to sell at the same price per gram as they bought it (i.e., professing to sell at Cost Price), they make a profit because they are selling *less product* than the customer pays for.

## Calculating Profit Percentage (When Professing to Sell at CP)

Let:
*   `TW` = True Weight (the weight the dealer professes to sell, e.g., 1000g for 1kg)
*   `FW` = False Weight (the weight the dealer actually delivers, e.g., 900g)

Assume the dealer professes to sell at Cost Price. This means the Selling Price charged for `TW` is equal to the Cost Price of `TW`.

*   **Dealer's Cost:** The cost incurred by the dealer is for the `FW` they actually provide. Let the cost per unit weight be 'C'. So, `Dealer's CP = FW * C`.
*   **Dealer's Revenue:** The revenue received by the dealer is the price they charge for the `TW`. Since they profess to sell at CP, this price is `TW * C`. So, `Dealer's SP = TW * C`.
*   **Dealer's Profit:** `Profit = Dealer's SP - Dealer's CP = (TW * C) - (FW * C) = (TW - FW) * C`.
*   **Profit Percentage:** This is calculated based on the dealer's actual cost (`Dealer's CP`).
    ```
    Profit % = (Profit / Dealer's CP) * 100 %
    Profit % = [ (TW - FW) * C / (FW * C) ] * 100 %
    ```
    Cancel 'C':
    ```
    Profit % = [ (True Weight - False Weight) / False Weight ] * 100 %
    ```
    Alternatively, let `Error = True Weight - False Weight`.
    ```
    Profit % = (Error / False Weight) * 100 %
    Profit % = (Error / (True Weight - Error)) * 100 %
    ```

**Simplified View:** The dealer effectively buys `FW` grams but sells them as if they were `TW` grams (at the cost price rate). The gain is on the difference (`TW - FW`), calculated over the actual cost base (`FW`).

**Formula:**
```
Gain % = [ (Amount Gained) / (Amount Used) ] * 100 %  
Gain % = [ (True Weight - False Weight) / False Weight ] * 100 %
```

*   **Example:** A dealer uses a 900g weight instead of a 1000g (1kg) weight and professes to sell at CP.
    *   True Weight (TW) = 1000g
    *   False Weight (FW) = 900g
    *   Gain % = [(1000 - 900) / 900] * 100 %
    *   Gain % = (100 / 900) * 100 %
    *   Gain % = (1 / 9) * 100 % = 11.11... % or 11 1/9 %

## Scenarios with Additional Profit/Loss Claims

Sometimes, a dealer might use false weights *and* claim to sell at a certain profit or loss percentage. In such cases, you need to combine the effect of the false weight with the claimed profit/loss percentage. This usually involves calculating the SP based on the false weight quantity and the claimed profit/loss, and comparing it to the actual cost of the false weight quantity. (Examples will clarify this).

## Key Takeaway

Profit in false weight problems arises from the difference between the quantity charged for and the quantity delivered. Always calculate the profit percentage based on the **actual cost** incurred by the dealer, which corresponds to the **false weight** delivered.

## Related Concepts

*   [[03 - Profit and Loss/01 - Basic Terminology (CP, SP, Profit, Loss)]]
*   [[02 - Percentages/01 - Basic Concepts and Conversions]]
*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc)]] (Understanding the ratio of true weight to false weight can be helpful)