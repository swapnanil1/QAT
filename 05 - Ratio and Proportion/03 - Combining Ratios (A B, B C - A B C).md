# Combining Ratios (A B, B C -> A B C)

#quant #ratio_and_proportion #ratio_concepts #combining_ratios

## Concept

Often, we are given ratios relating different pairs of quantities, and we need to find the relationship or ratio connecting all of them, or specifically the ratio between the first and the last quantity. For example, if we know the ratio of A to B (`A : B`) and the ratio of B to C (`B : C`), we can find the combined ratio `A : B : C`.

## Method for Combining Two Ratios (A:B and B:C)

Suppose we have:
`A : B = a : b`
`B : C = c : d`

**Goal:** Find the ratio `A : B : C`.

**Steps:**

1.  **Identify the Common Term:** The common term is B.
2.  **Make the Common Term Equal:** The value corresponding to B is `b` in the first ratio and `c` in the second ratio. We need to make these values equal.
    *   Find the Least Common Multiple (LCM) of `b` and `c`. Let `LCM(b, c) = L`.
    *   Multiply the first ratio (`a : b`) by `L/b`. The new ratio is `(a * L/b) : (b * L/b) = (a * L/b) : L`.
    *   Multiply the second ratio (`c : d`) by `L/c`. The new ratio is `(c * L/c) : (d * L/c) = L : (d * L/c)`.
3.  **Combine:** Now that the value for B is `L` in both adjusted ratios, we can write the combined ratio:
    `A : B : C = (a * L/b) : L : (d * L/c)`

**Simpler Method (Equivalent):**

1.  Multiply the first ratio (`a : b`) by `c` (the 'B' value from the second ratio).
    `A : B = (a * c) : (b * c)`
2.  Multiply the second ratio (`c : d`) by `b` (the 'B' value from the first ratio).
    `B : C = (c * b) : (d * b)`
3.  Combine: Since the 'B' term is now `b*c` in both,
    `A : B : C = (a * c) : (b * c) : (b * d)`

**Example:**
If `A : B = 2 : 3` and `B : C = 4 : 5`.
Common term is B. Values are 3 and 4. `LCM(3, 4) = 12`.
Multiply `(2 : 3)` by `12/3 = 4` -> `8 : 12`.
Multiply `(4 : 5)` by `12/4 = 3` -> `12 : 15`.
Combined ratio `A : B : C = 8 : 12 : 15`.

Using simpler method:
Multiply `(2 : 3)` by 4 -> `8 : 12`.
Multiply `(4 : 5)` by 3 -> `12 : 15`.
Combined ratio `A : B : C = 8 : 12 : 15`.

## Method for Combining More Than Two Ratios (A:B, B:C, C:D)

Suppose:
`A : B = a : b`
`B : C = c : d`
`C : D = e : f`

**Goal:** Find `A : B : C : D`.

**Method 1: Step-by-step**
1. Combine `A:B` and `B:C` to get `A:B:C` (as shown above). Let this be `p : q : r`.
2. Now combine `A:B:C = p : q : r` with `C:D = e : f`.
3. The common term is C. Values are `r` and `e`. Find `LCM(r, e)`.
4. Adjust both ratios (`p:q:r` and `e:f`) to make the C term equal to `LCM(r, e)`.
5. Write the final combined ratio `A : B : C : D`.

**Method 2: Shortcut / Visual Method**
Write the ratios like this:
`A : B = a : b`
`B : C =     c : d`
`C : D =         e : f`

Then calculate:
*   `A = a * c * e` (Multiply first terms of all ratios)
*   `B = b * c * e` (Start with B's value in first ratio, multiply by subsequent first terms)
*   `C = b * d * e` (Start with B's value, use C's value from second, then D's value from third) - *Correction: C = b * d * e*
*   `D = b * d * f` (Multiply last terms of all ratios) - *Correction: D = b * d * f*

Let's re-evaluate the visual method logic:
`A : B = a : b`
`B : C =   c : d`
`C : D =     e : f`
-----------------------
`A = a * c * e` (Path down the left)
`B = b * c * e` (Path starts at b, goes down left)
`C = b * d * e` (Path starts at b, goes to d, goes down left)
`D = b * d * f` (Path starts at b, goes to d, goes to f)

**Example:**
`A:B = 1:2`, `B:C = 3:4`, `C:D = 5:6`
`A = 1 * 3 * 5 = 15`
`B = 2 * 3 * 5 = 30`
`C = 2 * 4 * 5 = 40`
`D = 2 * 4 * 6 = 48`
Combined ratio `A : B : C : D = 15 : 30 : 40 : 48`.
(This combined ratio can be simplified by dividing all terms by their GCD, if any. In this case, GCD is 1).

## Key Points

*   Always ensure the common term is correctly identified and aligned.
*   Using the LCM is generally efficient, especially if the values are large.
*   The shortcut method for multiple ratios is fast but requires careful application of the multiplication pattern.
*   Simplify the final combined ratio if possible.

## Related Concepts

*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]]
*   [[05 - Ratio and Proportion/02 - Proportion Concepts (Fourth, Third, Mean).md]]
*   [[05 - Ratio and Proportion/04 - Applications (Division, Coins).md]] (Combined ratios are essential for solving division problems)
*   [[07 - Partnership/01 - Basic Concepts (Investment, Time, Profit Ratio).md]] (Often need to combine investment or time ratios)