# Work and Wages

**Concept:**

Work and Wages problems deal with the distribution of payment (wages) among individuals based on the amount of work they perform, either individually or together. The fundamental principle is that **wages are distributed in proportion to the work done by each individual.**

**Core Principle:**

*   `Ratio of Wages = Ratio of Work Done`

**Calculating Work Done:**

The 'work done' by each individual can be determined in a few ways, often related to their efficiency and the time they worked:

1.  **Based on Efficiency (if time worked is the same):** If all individuals work for the same duration to complete the job together, their wages are proportional to their individual efficiencies (rate of work).
    *   `Ratio of Wages = Ratio of Efficiencies`
    *   This is the most common scenario in basic problems.

2.  **Based on Total Work Units Completed:** Using the LCM method from [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]], calculate the total work units completed by each person (`Work Done = Efficiency * Time Worked`). The ratio of these work units determines the ratio of wages.
    *   This method is applicable even if individuals work for different durations or if they work together for only part of the job.

3.  **Based on Fraction of Work Done:** Calculate the fraction of the total work completed by each person. The wages are divided in the ratio of these fractions.
    *   If A completes `1/x` of the work, B completes `1/y`, and C completes `1/z` such that `1/x + 1/y + 1/z = 1` (total work), then the ratio of their wages is `1/x : 1/y : 1/z`.

**Steps for Solving:**

1.  **Calculate Individual Efficiencies:** Use the time taken by each individual to complete the work alone to find their efficiencies (using the LCM method is often easiest). Let efficiencies be `Eff_A`, `Eff_B`, `Eff_C`, etc.
2.  **Determine the Ratio of Work Done:**
    *   If they all work together for the entire duration, the ratio of work done is simply the ratio of their efficiencies: `Eff_A : Eff_B : Eff_C`.
    *   If they work for different times, calculate work units done by each: `Work_A = Eff_A * Time_A`, `Work_B = Eff_B * Time_B`, etc. The ratio is `Work_A : Work_B : ...`.
3.  **Calculate Individual Shares:** Divide the total wages according to the calculated ratio.
    *   A's Share = `(A's part in the ratio / Sum of ratio parts) * Total Wages`.

**Example:**

A takes 10 days, B takes 15 days. They work together and earn Rs. 500.
1.  LCM(10, 15) = 30 (Total Work).
2.  Eff(A) = 30/10 = 3 units/day. Eff(B) = 30/15 = 2 units/day.
3.  Ratio of efficiencies (since they work together for the whole time) = Eff(A) : Eff(B) = 3 : 2.
4.  Sum of ratio parts = 3 + 2 = 5.
5.  A's Share = (3 / 5) * 500 = Rs. 300.
6.  B's Share = (2 / 5) * 500 = Rs. 200.
*   **See Example:** [[09 - Time and Work/04.E01 - Dividing Wages Based on Work Done Example.md]]

**Important Note:** Wages depend on *work done*, not just time spent. If someone less efficient works for longer, they might still do less work than a highly efficient person working for a shorter time.

**Related Concepts:**

*   [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]]
*   [[09 - Time and Work/02 - Efficiency Comparison.md]]
*   [[05 - Ratio and Proportion/04 - Applications (Division, Coins).md]] (Dividing amounts in a ratio)

#quant #time_and_work #work_and_wages #efficiency #ratio #wages_distribution