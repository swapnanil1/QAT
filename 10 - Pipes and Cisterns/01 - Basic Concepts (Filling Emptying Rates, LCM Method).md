# Basic Concepts (Filling/Emptying Rates, LCM Method)

**Introduction:**

Pipes and Cisterns problems are a specific application of the concepts learned in [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]]. Instead of workers doing a job, these problems involve pipes filling or emptying a tank (cistern).

**Core Concepts:**

1.  **Cistern/Tank:** Represents the total 'work' to be done (filling the tank completely). Usually considered as 1 unit or assigned a capacity based on LCM.
2.  **Inlet Pipe:** A pipe that fills the tank. The work done by an inlet pipe is considered **positive (+)**.
3.  **Outlet Pipe/Leak:** A pipe or leak that empties the tank. The work done by an outlet pipe is considered **negative (-)**.
4.  **Rate of Filling/Emptying:** This is analogous to the 'Rate of Work' or 'Efficiency' in Time and Work. It's the fraction of the tank filled or emptied per unit of time (e.g., per hour, per minute).
    *   If an inlet pipe can fill a tank in `x` hours, its filling rate = `1/x` of the tank per hour.
    *   If an outlet pipe can empty a full tank in `y` hours, its emptying rate = `1/y` of the tank per hour (often treated as `-1/y` in combined calculations).

5.  **Combined Rate:** When multiple pipes (inlets and outlets) operate simultaneously, their rates are combined algebraically (adding filling rates, subtracting emptying rates).
    *   Net Rate = (Sum of rates of all inlets) - (Sum of rates of all outlets).
    *   If the Net Rate is positive, the tank is filling.
    *   If the Net Rate is negative, the tank is emptying.
    *   If the Net Rate is zero, the tank level remains constant (filling rate equals emptying rate).

6.  **Time to Fill/Empty:**
    *   Time to fill = `Total Capacity (Work) / Net Filling Rate`
    *   Time to empty = `Total Capacity (Work) / Net Emptying Rate`

**Methods for Solving:**

1.  **Fraction Method:**
    *   Uses the rates `1/x` (inlet) and `1/y` (outlet).
    *   Combined rate = `(Sum of 1/x) - (Sum of 1/y)`.
    *   Time = `1 / |Combined Rate|`. (Absolute value because time is positive).
    *   Can become complex with multiple pipes.

2.  **LCM Method (Capacity Method):**
    *   This is generally preferred, similar to the LCM method in Time and Work.
    *   **Step 1:** Assume the Total Capacity of the tank is the LCM of the individual times taken by each pipe to fill or empty it.
    *   **Step 2:** Calculate the 'efficiency' (volume filled/emptied per unit time) for each pipe relative to this capacity.
        *   Inlet Efficiency = `Total Capacity (LCM) / Time to Fill` (Positive value).
        *   Outlet Efficiency = `Total Capacity (LCM) / Time to Empty` (Represented as a Negative value).
    *   **Step 3:** Calculate the net combined efficiency by algebraically summing the individual efficiencies.
    *   **Step 4:** Calculate the time taken: Time = `Total Capacity (LCM) / |Net Combined Efficiency|`.
    *   **Example:** Inlet A fills in 10 hrs, Outlet B empties in 15 hrs.
        *   LCM(10, 15) = 30 units (Tank Capacity).
        *   A's efficiency = 30 / 10 = +3 units/hr.
        *   B's efficiency = 30 / 15 = -2 units/hr (negative because it empties).
        *   Combined efficiency = (+3) + (-2) = +1 unit/hr (net filling).
        *   Time to fill the tank = Total Capacity / Combined Efficiency = 30 / 1 = 30 hours.
    *   **See Examples:** [[10 - Pipes and Cisterns/01.E01 - Two Pipes Filling Tank Example.md]], [[10 - Pipes and Cisterns/01.E02 - One Filling, One Emptying Pipe Example.md]]

**Key Difference from Time and Work:**

The main difference is the concept of **negative work** (emptying). In Time and Work, usually, everyone contributes positively towards completing the job. In Pipes and Cisterns, outlets work against the inlets.

#quant #pipes_and_cisterns #basic_concepts #lcm_method #efficiency #work_rate #negative_work #formula #time_and_work_analogy