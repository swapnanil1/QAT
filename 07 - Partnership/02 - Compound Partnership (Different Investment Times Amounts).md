# Compound Partnership (Different Investment Times / Amounts)

#quant #partnership #compound_partnership #profit_sharing #ratio_concepts #formula

## Definition

A **compound partnership** is a partnership where:
1.  Partners invest their capital for **different durations**, OR
2.  Partners change their investment amounts (add or withdraw capital) during the partnership period.

This contrasts with simple partnership, where all partners invest for the same duration with constant investments.

## Core Principle: Ratio of Equivalent Capitals

In compound partnerships, the profit or loss is distributed in the ratio of the partners' **equivalent capitals** (also called effective investments).

Equivalent Capital = Investment × Time Period

The profit-sharing ratio is:
`Profit_A : Profit_B : Profit_C = (Equivalent Capital_A) : (Equivalent Capital_B) : (Equivalent Capital_C)`
`Profit_A : Profit_B : Profit_C = (I_A * T_A) : (I_B * T_B) : (I_C * T_C)`

Where `I` represents the investment and `T` represents the time period for which that investment was active.

## Scenarios and Calculation

**Scenario 1: Different Investment Durations**

*   Partners invest their capital at the start but remain invested for different lengths of time.
*   **Example:** A starts a business with ₹50k. B joins after 3 months with ₹60k. They make a profit after 1 year.
    *   A's Time (`T_A`) = 12 months
    *   B's Time (`T_B`) = 12 - 3 = 9 months
    *   Profit Ratio (A : B) = `(50000 * 12) : (60000 * 9)`
    *   Ratio = `600000 : 540000` = `60 : 54` = `10 : 9`

**Scenario 2: Variable Investments**

*   Partners add or withdraw capital during the partnership period.
*   The equivalent capital for such a partner must be calculated by summing the product of each investment amount and the duration it was held.
*   **Calculation:** If Partner A invests `I_1` for time `T_1`, then changes investment to `I_2` for time `T_2`, and then to `I_3` for time `T_3`, their total equivalent capital is:
    `Equivalent Capital_A = (I_1 * T_1) + (I_2 * T_2) + (I_3 * T_3)`

*   **Example:** A starts with ₹20k. After 4 months, A withdraws ₹5k. After another 4 months, A adds ₹10k. The partnership lasts for 1 year (12 months).
    *   Period 1: Investment = ₹20k, Duration = 4 months. Contribution = `20000 * 4 = 80000`.
    *   Period 2: Investment = ₹(20k - 5k) = ₹15k, Duration = 4 months. Contribution = `15000 * 4 = 60000`.
    *   Period 3: Investment = ₹(15k + 10k) = ₹25k, Duration = 12 - 4 - 4 = 4 months. Contribution = `25000 * 4 = 100000`.
    *   A's Total Equivalent Capital = 80000 + 60000 + 100000 = 240000.
    This value (240000) would then be used in the ratio calculation against other partners' equivalent capitals.

## Key Considerations

*   **Time Units:** Always use consistent time units (usually months) for all partners and all investment periods.
*   **Careful Calculation:** When investments change, carefully track the amount invested during *each specific period* and the *duration* of that period.
*   **Total Duration:** Determine the total duration of the partnership to correctly calculate the time periods for partners who join late or leave early, or for the final investment period of a partner with variable investments.

## Related Concepts

*   [[07 - Partnership/01 - Basic Concepts (Investment, Time, Profit Ratio).md]] (Foundation for partnership)
*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]]
*   [[05 - Ratio and Proportion/04 - Applications (Division, Coins).md]] (Profit distribution)
*   [[07 - Partnership/03 - Working and Sleeping Partners.md]] (Further complexity involving salaries/commissions)