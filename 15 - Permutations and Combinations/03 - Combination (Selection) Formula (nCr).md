# Combination (Selection) Formula (nCr)

Tags: #quant #permutations_and_combinations #combination #selection #ncr #formula #concept #factorial

---

**Introduction:**

A combination refers to the selection of objects where the order of selection does not matter. Unlike [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md|permutations, where order is crucial]], combinations focus solely on choosing a group or subset of items from a larger set. For example, selecting a committee of 3 people {A, B, C} is the same combination regardless of whether they were chosen in the order A then B then C, or B then C then A. Combinations are fundamental in probability and counting problems and rely heavily on [[15 - Permutations and Combinations/01 - Factorial Notation.md|factorial notation]].

**Definition and Formula:**

The number of combinations of `n` distinct objects taken `r` at a time, denoted as `nCr`, `C(n, r)`, or $\binom{n}{r}$ (read as "n choose r"), is given by the formula:

`nCr = n! / (r! * (n - r)!)`

Where:
*   `n` is the total number of distinct objects available.
*   `r` is the number of objects being selected.
*   `n >= r >= 0`.

**Key Concepts:**

*   **Order Does Not Matter:** This is the defining characteristic. Selecting {Apple, Banana} is the same as selecting {Banana, Apple}.
*   **Selection/Choosing:** The focus is purely on which items are included in the group, not their arrangement within the group.
*   **Distinct Objects:** The basic `nCr` formula assumes all `n` objects are distinct.

---

**Properties:**

*   **Symmetry Property:** `nCr = nC(n-r)`
    *   Selecting `r` objects to include is mathematically equivalent to selecting `n-r` objects to exclude.
    *   Example: Choosing 2 items from 5 (`5C2`) is the same as choosing 3 items from 5 to leave behind (`5C3`). Both equal `5! / (2! * 3!) = 10`.
*   **Edge Cases:**
    *   `nC0 = n! / (0! * n!) = 1` (There's one way to choose zero items: choose nothing).
    *   `nC1 = n! / (1! * (n-1)!) = n * (n-1)! / (1 * (n-1)!) = n` (There are `n` ways to choose one item from `n`).
    *   `nCn = n! / (n! * 0!) = 1` (There's one way to choose all `n` items).
*   **Pascal's Identity (Less Common in Basic Aptitude):** `nCr + nC(r-1) = (n+1)Cr`. This identity relates combinations and forms the basis of Pascal's Triangle.

---

**Relationship with Permutation:**

Permutation involves both selection and arrangement. Combination is only selection. The relationship is:

`nPr = nCr * r!`

This means the number of ways to arrange `r` items from `n` (`nPr`) is equal to the number of ways to first *select* `r` items (`nCr`) and then *arrange* those chosen `r` items (`r!`). Rearranging gives `nCr = nPr / r!`, which also leads back to the main `nCr` formula.

---

**Example Calculation:**

Find the number of ways to choose 3 letters from the set {A, B, C, D} (n=4, r=3).
`4C3 = 4! / (3! * (4 - 3)!)`
`4C3 = 4! / (3! * 1!)`
`4C3 = (4 * 3!) / (3! * 1)`
`4C3 = 4 / 1 = 4`
The combinations (groups) are: {A, B, C}, {A, B, D}, {A, C, D}, {B, C, D}. (Total 4). Contrast this with `4P3 = 24` calculated in the permutation concept note, where the order within each group mattered.

---

**General Approach & Strategy:**

1.  **Identify n and r:** Determine the total number of distinct items (`n`) and the number being selected (`r`).
2.  **Check for Order:** Confirm that the problem requires only selection where order does *not* matter. If order matters, use permutations.
3.  **Apply Formula:** Substitute `n` and `r` into the `nCr = n! / (r! * (n - r)!)` formula.
4.  **Simplify:** Use factorial properties, especially cancellation (as shown in [[15 - Permutations and Combinations/01.E01 - Calculating Factorials Example.md|this factorial simplification example]]), to evaluate the expression. Utilize the symmetry `nCr = nC(n-r)` if `r` is large (e.g., calculate `10C8` as `10C2`).

---

**Examples:**

*   [[15 - Permutations and Combinations/03.E01 - Selecting a Committee Example.md]] (Illustrates a classic combination scenario of forming a group where order is irrelevant)
*   [[15 - Permutations and Combinations/03.E02 - Selecting Items Example.md]] (Demonstrates selecting items, possibly with constraints involving specific inclusions/exclusions)

---

**Related Concepts:**

*   [[15 - Permutations and Combinations/01 - Factorial Notation.md]] (Provides the factorial mechanism needed for calculation)
*   [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md]] (Highlights the key difference: order matters in permutations, not combinations)
*   [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md]] (Combinations are crucial for calculating the number of favorable outcomes and total outcomes in probability problems)
*   [[18 - Miscellaneous (Optional)/02 - Series and Progressions (AP, GP).md]] (Binomial Theorem, which uses combinations (`nCr`) as coefficients, might be relevant in advanced contexts but usually not basic aptitude)