# Pipes Opened Closed Intermittently

**Concept:**

These problems are a variation where pipes (inlets or outlets) are not all operating continuously for the entire duration. They might be opened or closed after specific time intervals, opened sequentially, or operate in a pattern similar to [[09 - Time and Work/03 - Alternate Days Work.md]].

**Key Approach:**

The fundamental approach is to track the amount of the tank filled or emptied during each specific time interval when a particular combination of pipes is active. The LCM method remains the most effective tool.

**Steps for Solving (LCM Method):**

1.  **Assume Total Capacity:** Calculate the LCM of the individual times taken by each pipe to fill or empty the tank alone. This is the Total Capacity in units.
2.  **Calculate Individual Efficiencies:** Determine the filling rate (positive efficiency) or emptying rate (negative efficiency) for each pipe: `Efficiency = Total Capacity / Time`.
3.  **Track Work Over Intervals:** Break the problem down into time intervals based on when pipes are opened or closed.
    *   For each interval, determine which pipes are active.
    *   Calculate the **net efficiency** for that specific interval by summing the efficiencies of the active pipes.
    *   Calculate the amount of work (volume filled/emptied) during that interval: `Work Done = Net Efficiency * Duration of Interval`.
4.  **Monitor Cumulative Work:** Keep track of the total volume filled in the tank after each interval.
5.  **Determine Remaining Work/Time:**
    *   If the problem asks for the total time to fill the tank, continue calculating interval by interval until the cumulative work equals the Total Capacity. The final interval might not be fully utilized; calculate the time needed for the remaining work using the net efficiency active during that final phase: `Time for Remainder = Remaining Work / Net Efficiency`.
    *   If the problem asks for the state of the tank after a certain time, calculate the cumulative work done up to that time.

**Common Scenarios:**

*   **Sequential Opening:** Pipe A is opened first, then Pipe B is opened after some time, then Pipe C, etc. Calculate work done by A alone, then A+B together, then A+B+C together.
*   **Closing After Some Time:** All pipes start together, but one or more are closed after a certain period. Calculate work done by all pipes, then recalculate the net efficiency for the remaining pipes and find the time needed to complete the rest of the work.
*   **Alternating Pipes:** Similar to alternate days work. Pipe A works for one hour, then Pipe B for the next hour. Calculate work done per cycle and proceed as in [[09 - Time and Work/03 - Alternate Days Work.md]].

**Example Outline (Pipe closed after some time):**

Pipes A (fills in 10h) and B (fills in 15h) are opened together. After 3 hours, Pipe B is closed. How much more time will Pipe A take to fill the remaining tank?
1.  LCM(10, 15) = 30 units (Capacity).
2.  Eff(A) = +3 units/hr, Eff(B) = +2 units/hr.
3.  **Interval 1 (0-3 hours):** A and B are open.
    *   Net Efficiency = Eff(A) + Eff(B) = 3 + 2 = 5 units/hr.
    *   Work Done in 3 hours = 5 units/hr * 3 hr = 15 units.
    *   Tank filled = 15 units.
4.  **Remaining Work:** Total Capacity - Work Done = 30 - 15 = 15 units.
5.  **Interval 2 (After 3 hours):** Only Pipe A is open.
    *   Net Efficiency = Eff(A) = 3 units/hr.
    *   Time needed for remaining work = Remaining Work / Net Efficiency = 15 units / 3 units/hr = 5 hours.
6.  Answer: Pipe A will take 5 more hours.
*   **See Example:** [[10 - Pipes and Cisterns/02.E01 - Pipe Closed After Some Time Example.md]]

**Key Considerations:**

*   Carefully map the timeline and which pipes are active during each phase.
*   Always use the correct net efficiency for the specific combination of pipes working in an interval.
*   Remember to handle negative efficiencies for outlet pipes.

#quant #pipes_and_cisterns #intermittent_operation #lcm_method #efficiency #work_rate #time_intervals