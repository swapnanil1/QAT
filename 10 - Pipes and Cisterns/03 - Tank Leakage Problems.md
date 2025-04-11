# Tank Leakage Problems

**Concept:**

Tank leakage problems are a specific type of Pipes and Cisterns problem where an outlet is described as a 'leak'. Functionally, a leak acts exactly like an **outlet pipe**, causing the tank to empty. Therefore, the work done by a leak is considered **negative (-)**.

**Key Principles:**

1.  **Leak as an Outlet:** Treat the leak as just another outlet pipe with a certain emptying efficiency (rate).
2.  **Negative Work:** The rate/efficiency of the leak is subtracted when calculating the net efficiency of the system if inlets are also active.
3.  **Calculating Leak Efficiency:** Often, the problem doesn't directly state the time the leak takes to empty the tank alone. Instead, it provides:
    *   The time an inlet pipe takes to fill the tank *without* the leak (`T_inlet`).
    *   The time the inlet pipe takes to fill the tank *with* the leak present (`T_combined`).
    *   Since the leak slows down the filling, `T_combined` will always be greater than `T_inlet`.
    *   Using the LCM method:
        *   Find Total Capacity (LCM of `T_inlet` and `T_combined`).
        *   Calculate `Eff_inlet = Capacity / T_inlet` (Positive).
        *   Calculate `Eff_combined = Capacity / T_combined` (Positive, but smaller than `Eff_inlet`).
        *   The leak's efficiency is found by subtraction: `Eff_leak = Eff_combined - Eff_inlet`. This result will be negative, representing the emptying rate. `Eff_leak = Eff_inlet - Eff_combined` is also used to find the magnitude.
        *   `Eff_leak = Eff_inlet + Eff_leak`

4.  **Finding Time to Empty:** Once the leak's efficiency (`Eff_leak`) is found (as a negative value), the time it takes for the leak *alone* to empty a full tank is:
    *   `Time_leak = Total Capacity / |Eff_leak|`

**Common Problem Variations:**

*   **Finding Leak's Emptying Time:** Given inlet time and combined filling time (inlet + leak), find the time the leak takes to empty the full tank alone. (See Example [[10 - Pipes and Cisterns/01.E02 - One Filling, One Emptying Pipe Example.md]], which is structurally identical).
*   **Finding Filling Time with Leak:** Given inlet time and leak's emptying time, find the time to fill the tank when both are active.
*   **Effect of Leak on Partially Filled Tank:** Calculating how long a leak takes to empty a tank that is already partially full, or how long an inlet takes to fill the rest of the tank with the leak active.

**Solving Strategy (LCM Method Recommended):**

1.  Identify all inlets and the leak (outlet).
2.  Note the times given (`T_inlet`, `T_leak`, `T_combined`).
3.  Calculate Total Capacity (LCM of known times).
4.  Calculate individual efficiencies (positive for inlets, find the leak's negative efficiency if necessary using the combined efficiency).
5.  Calculate the net efficiency based on which components are active.
6.  Calculate the required time using `Time = Work / Net Efficiency`. Remember 'Work' might be the full capacity or just a portion depending on the question.

**Example Scenario:**

An inlet fills in 6 hours. A leak empties in 10 hours. How long to fill the tank if both are active?
1.  LCM(6, 10) = 30 units (Capacity).
2.  Eff(Inlet) = 30/6 = +5 units/hr.
3.  Eff(Leak) = 30/10 = -3 units/hr (negative).
4.  Net Efficiency = (+5) + (-3) = +2 units/hr.
5.  Time to fill = Capacity / Net Efficiency = 30 / 2 = 15 hours.
*   **See Example:** [[10 - Pipes and Cisterns/03.E01 - Leak Affecting Filling Time Example.md]]

**Related Concepts:**

*   [[10 - Pipes and Cisterns/01 - Basic Concepts (Filling Emptying Rates, LCM Method).md]] (Foundation)
*   [[10 - Pipes and Cisterns/02 - Pipes Opened Closed Intermittently.md]] (Leaks might only be active for part of the time)

#quant #pipes_and_cisterns #leak_problems #negative_work #lcm_method #efficiency #outlet_pipe