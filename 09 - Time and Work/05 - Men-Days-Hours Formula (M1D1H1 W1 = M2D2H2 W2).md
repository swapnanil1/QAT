# Men-Days-Hours Formula (M1*D1*H1/W1 = M2*D2*H2/W2)

**Concept:**

This formula, often called the **MDH formula** or the **Chain Rule** in the context of Time and Work, relates the number of workers (Men), the number of days they work (Days), the number of hours they work per day (Hours), and the amount of work done (Work). It's used to solve problems where two different scenarios involving these variables are compared.

**The Formula:**

If `M1` workers working `D1` days for `H1` hours per day complete `W1` amount of work, and `M2` workers working `D2` days for `H2` hours per day complete `W2` amount of work, then the relationship between these quantities is given by:

`(M1 * D1 * H1) / W1 = (M2 * D2 * H2) / W2`

**Explanation of Variables:**

*   **M:** Number of workers (Men, women, machines, etc. - representing the workforce units).
*   **D:** Number of days the work is done for.
*   **H:** Number of hours worked per day.
*   **W:** Amount of work done (e.g., number of items produced, length of wall built, area painted, or often just considered '1 unit' if the job is singular).

**Underlying Principle - Proportionality:**

The formula is based on the concept of **Man-Hours** or **Man-Days**, representing the total effort required to complete a certain amount of work.

*   The amount of work done (`W`) is directly proportional to the number of workers (`M`), the number of days (`D`), and the hours worked per day (`H`).
    *   `W ∝ M` (More workers, more work done, assuming constant time/hours)
    *   `W ∝ D` (More days, more work done, assuming constant workers/hours)
    *   `W ∝ H` (More hours per day, more work done, assuming constant workers/days)
*   Combining these, `W ∝ M * D * H`.
*   This can be written as `W = k * M * D * H`, where `k` is a constant of proportionality (representing work done per man-hour or per man-day-hour).
*   Rearranging, `(M * D * H) / W = 1/k = Constant`.
*   Therefore, for two different scenarios (1 and 2), the ratio `(M * D * H) / W` must be the same:
    `(M1 * D1 * H1) / W1 = (M2 * D2 * H2) / W2`

**Variations and Simplifications:**

*   **If hours per day are constant or not mentioned:** The formula simplifies to `(M1 * D1) / W1 = (M2 * D2) / W2`.
*   **If the amount of work is the same (`W1 = W2`):** The formula simplifies to `M1 * D1 * H1 = M2 * D2 * H2`.
*   **If both hours and work are the same:** The formula simplifies to `M1 * D1 = M2 * D2`. This shows the inverse relationship between the number of workers and the days required for the same job.

**Efficiency Factor (Optional Inclusion):**

Sometimes, the efficiency (`E`) of the workers might differ between the two groups. Efficiency acts as a multiplier for the workforce. The formula can be extended to:

`(M1 * D1 * H1 * E1) / W1 = (M2 * D2 * H2 * E2) / W2`

Where `E1` and `E2` are the relative efficiencies of workers in group 1 and group 2, respectively.

**Example Application:**

If 10 men working 6 hours a day can build a wall in 15 days, how many days will 20 men take to build the same wall working 5 hours a day?
*   M1=10, H1=6, D1=15, W1=1 (same wall)
*   M2=20, H2=5, W2=1, D2=?
*   Formula (since W1=W2): `M1 * D1 * H1 = M2 * D2 * H2`
*   `10 * 15 * 6 = 20 * D2 * 5`
*   `900 = 100 * D2`
*   `D2 = 9` days.
*   **See Example:** [[09 - Time and Work/05.E01 - Applying MDH Formula Example.md]]

**Related Concepts:**

*   [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]] (Efficiency is implicitly handled here as a group)
*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]] (Direct and Inverse Proportion)

#quant #time_and_work #mdh_formula #chain_rule #work_rate #proportionality #formula