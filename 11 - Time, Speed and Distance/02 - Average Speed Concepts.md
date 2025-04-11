# Average Speed Concepts

**Definition:**

Average speed is defined as the **Total Distance Covered** divided by the **Total Time Taken** for the entire journey.

`Average Speed = Total Distance / Total Time`

**Crucial Point:**

Average speed is **NOT** typically the simple arithmetic average (mean) of the different speeds involved in the journey, unless the time spent traveling at each speed is exactly the same.

**Calculating Average Speed:**

The method depends on whether the journey involves segments of equal distance or equal time.

1.  **General Case (Unequal Distances and Unequal Times):**
    *   Calculate the distance covered in each segment (`d1, d2, d3, ...`).
    *   Calculate the time taken for each segment (`t1, t2, t3, ...`) using `t = d / s`.
    *   Calculate Total Distance = `d1 + d2 + d3 + ...`
    *   Calculate Total Time = `t1 + t2 + t3 + ...`
    *   Average Speed = `(d1 + d2 + ...) / (t1 + t2 + ...)`
    *   Average Speed = `(d1 + d2 + ...) / (d1/s1 + d2/s2 + ...)`
    *   **See Example:** [[08 - Averages/03.E02 - Average Speed Calculation Example.md]] (which calculated average speed for unequal distances and speeds).

2.  **Case 1: Equal Distances Covered at Different Speeds:**
    *   If an object travels the same distance `d` at two different speeds `s1` and `s2`.
        *   `t1 = d / s1`
        *   `t2 = d / s2`
        *   Total Distance = `d + d = 2d`
        *   Total Time = `t1 + t2 = d/s1 + d/s2 = d * (s1+s2) / (s1*s2)`
        *   Average Speed = Total Distance / Total Time = `2d / [d * (s1+s2) / (s1*s2)]`
        *   Average Speed = `2d * (s1*s2) / [d * (s1+s2)]`
        *   Average Speed = `(2 * s1 * s2) / (s1 + s2)`
    *   This is the **Harmonic Mean** of the two speeds.
    *   For three equal distances covered at speeds `s1, s2, s3`, the average speed is `3 / (1/s1 + 1/s2 + 1/s3)`.
    *   **See Example:** [[11 - Time, Speed and Distance/02.E01 - Average Speed (Equal Distances) Example.md]]

3.  **Case 2: Different Distances Covered in Equal Time Intervals:**
    *   If an object travels at different speeds `s1, s2, s3, ...` for the *same* duration of time `t` in each segment.
        *   `d1 = s1 * t`
        *   `d2 = s2 * t`
        *   Total Distance = `d1 + d2 + ... = (s1 + s2 + ...) * t`
        *   Total Time = `t + t + ... = n*t` (where `n` is the number of segments)
        *   Average Speed = Total Distance / Total Time = `[(s1 + s2 + ...) * t] / (n * t)`
        *   Average Speed = `(s1 + s2 + s3 + ...) / n`
    *   This is the simple **Arithmetic Mean** of the speeds.
    *   **See Example:** [[11 - Time, Speed and Distance/02.E02 - Average Speed (Equal Times) Example.md]]

**Relationship to Weighted Average:**

Average speed can be seen as a weighted average of speeds, where the **weights are the time intervals** spent at each speed:
`Average Speed = (s1*t1 + s2*t2 + ...) / (t1 + t2 + ...)`
Notice this simplifies back to `(d1 + d2 + ...) / (t1 + t2 + ...)`, the basic definition. Understanding this helps avoid common pitfalls.

**Related Concepts:**

*   [[11 - Time, Speed and Distance/01 - Basic Formula (D=S T) and Unit Conversions.md]] (Foundation)
*   [[08 - Averages/03 - Weighted Average.md]] (Conceptual link)
*   Harmonic Mean (Specific case for equal distances)
*   Arithmetic Mean (Specific case for equal times)

#quant #time_speed_distance #average_speed #harmonic_mean #arithmetic_mean #formula #weighted_average