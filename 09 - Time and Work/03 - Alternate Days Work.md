# Alternate Days Work

**Concept:**

Alternate Days Work problems are a variation where individuals (or groups) do not work simultaneously every day but take turns working on consecutive days. Usually, the pattern specifies who starts the work.

**Key Idea:**

The core idea is to calculate the amount of work done in one **cycle** of the working pattern (typically 2 days if two people alternate, 3 days if three people alternate, etc.) and then determine how many full cycles are needed to get close to the total work. The remaining work is then completed by the person(s) whose turn it is.

**Steps for Solving (LCM Method):**

1.  **Assume Total Work:** Calculate the LCM of the individual times taken by each person to complete the work alone. This represents the Total Work units.
2.  **Calculate Individual Efficiencies:** Find the work done per day (efficiency) for each person: `Efficiency = Total Work / Time Taken`.
3.  **Identify the Work Cycle:** Determine the pattern of work (e.g., A works Day 1, B works Day 2). Calculate the total work done in one full cycle (e.g., in 2 days for A and B alternating).
    *   Work in one cycle = Work done by person 1 on their day + Work done by person 2 on their day + ...
4.  **Calculate Number of Full Cycles:** Divide the Total Work by the work done per cycle to find how many full cycles can be completed.
    *   `Number of Cycles = Floor(Total Work / Work per Cycle)`
    *   Calculate the total work done in these full cycles: `Work Done = Number of Cycles * Work per Cycle`.
    *   Calculate the time taken for these full cycles: `Time Taken = Number of Cycles * Days per Cycle`.
5.  **Calculate Remaining Work:** Subtract the work done in full cycles from the Total Work.
    *   `Remaining Work = Total Work - Work Done in Cycles`.
6.  **Complete Remaining Work:** Determine whose turn it is after the full cycles are complete (based on who started). Add the time taken by the appropriate person(s) to complete the remaining work.
    *   If Remaining Work <= Efficiency of the next person, Time added = `Remaining Work / Efficiency`.
    *   If Remaining Work > Efficiency, that person works a full day, subtract their work, and see whose turn is next for the rest.
7.  **Total Time:** Add the time taken for the full cycles and the time taken to complete the remaining work.

**Example Scenario:**

A takes 10 days, B takes 15 days. A starts the work. They work on alternate days.
1.  LCM(10, 15) = 30 units (Total Work).
2.  Eff(A) = 30/10 = 3 units/day. Eff(B) = 30/15 = 2 units/day.
3.  Cycle (2 days):
    *   Day 1 (A works): 3 units
    *   Day 2 (B works): 2 units
    *   Work per cycle (2 days) = 3 + 2 = 5 units.
4.  Number of Cycles = Floor(30 / 5) = 6 cycles.
    *   Work done in 6 cycles = 6 * 5 = 30 units.
    *   Time taken for 6 cycles = 6 * 2 days = 12 days.
5.  Remaining Work = 30 - 30 = 0.
6.  No remaining work.
7.  Total Time = 12 days.

*   **See Example:** [[09 - Time and Work/03.E01 - A and B Working on Alternate Days Example.md]]

**Important Considerations:**

*   **Who Starts:** Pay close attention to who begins the work, as this determines the work done on odd/even days.
*   **Remaining Work:** Be careful when calculating the time for the remaining work, ensuring the correct person is working.

**Related Concepts:**

*   [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]] (Foundation)
*   [[09 - Time and Work/02 - Efficiency Comparison.md]]

#quant #time_and_work #alternate_days #lcm_method #efficiency #work_cycle