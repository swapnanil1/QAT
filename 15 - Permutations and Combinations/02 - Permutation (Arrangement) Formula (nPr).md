# Permutation (Arrangement) Formula (nPr)

Tags: #quant #permutations_and_combinations #permutation #arrangement #npr #formula #concept #factorial

---

**Introduction:**

A permutation refers to an arrangement of objects in a specific order. When we select `r` objects from a set of `n` distinct objects and arrange them, the number of possible arrangements is called the number of permutations of `n` objects taken `r` at a time. Order matters in permutations (e.g., 'ABC' is a different permutation from 'BCA'). Permutations use [[15 - Permutations and Combinations/01 - Factorial Notation.md|factorial notation]] heavily in their calculations.

**Definition and Formula:**

The number of permutations of `n` distinct objects taken `r` at a time, denoted as `nPr`, `P(n, r)`, or similar notations, is given by the formula:

`nPr = n! / (n - r)!`

Where:
*   `n` is the total number of distinct objects available.
*   `r` is the number of objects being selected and arranged.
*   `n >= r >= 0`.

**Key Concepts:**

*   **Order Matters:** The defining characteristic of permutation is that the sequence or order of the chosen objects is important.
*   **Distinct Objects:** The basic `nPr` formula assumes all `n` objects are distinct. Formulas for permutations with repetitions exist but are less common in basic aptitude.
*   **Arrangement of all Objects:** If we arrange all `n` objects (`r = n`), the formula becomes:
    `nPn = n! / (n - n)! = n! / 0! = n! / 1 = n!`
    So, the number of ways to arrange `n` distinct objects is `n!`.

**Example Calculation:**

Find the number of ways to arrange 3 letters from the set {A, B, C, D} (n=4, r=3).
`4P3 = 4! / (4 - 3)!`
`4P3 = 4! / 1!`
`4P3 = (4 * 3 * 2 * 1) / 1`
`4P3 = 24`
The arrangements are: ABC, ACB, BAC, BCA, CAB, CBA, ABD, ADB, BAD, BDA, DAB, DBA, ACD, ADC, CAD, CDA, DAC, DCA, BCD, BDC, CBD, CDB, DBC, DCB. (Total 24)

---

**Permutations with Repetitions (Non-Distinct Objects):**

If there are `n` objects in total, where there are `n1` identical objects of type 1, `n2` identical objects of type 2, ..., `nk` identical objects of type k such that `n1 + n2 + ... + nk = n`, then the number of distinct permutations of these `n` objects is:

`n! / (n1! * n2! * ... * nk!)`

Example: How many distinct ways can the letters of the word "MISSISSIPPI" be arranged?
Total letters `n = 11`.
M = 1 (`n1=1`)
I = 4 (`n2=4`)
S = 4 (`n3=4`)
P = 2 (`n4=2`)
Number of arrangements = `11! / (1! * 4! * 4! * 2!)` = 39916800 / (1 * 24 * 24 * 2) = 39916800 / 1152 = 34650.

---

**General Approach & Strategy:**

1.  **Identify n and r:** Determine the total number of objects (`n`) and the number of objects being arranged (`r`).
2.  **Check for Order:** Confirm that the problem involves arrangement where order matters. If order doesn't matter, it's a [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md|combination]] problem.
3.  **Check for Distinctness:** Determine if all objects are distinct or if there are repetitions. Apply the appropriate formula (`nPr` or the formula for non-distinct objects).
4.  **Apply Formula:** Substitute `n` and `r` (and `n1, n2,...` if applicable) into the chosen formula.
5.  **Simplify:** Use factorial properties (especially cancellation, as shown in [[15 - Permutations and Combinations/01.E01 - Calculating Factorials Example.md|this example]]) to simplify the expression.

---

**Examples:**

*   [[15 - Permutations and Combinations/02.E01 - Arranging Letters Example.md]] (Illustrates arranging distinct letters, possibly with restrictions)
*   [[15 - Permutations and Combinations/02.E02 - Arranging People in Seats Example.md]] (Demonstrates arranging distinct items (people) in distinct positions (seats))

---

**Related Concepts:**

*   [[15 - Permutations and Combinations/01 - Factorial Notation.md]] (Foundation for calculating permutations)
*   [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Contrasting concept where order does *not* matter)
*   [[15 - Permutations and Combinations/04 - Circular Permutations.md]] (A special type of permutation for arranging items in a circle)
*   [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md]] (Permutations are used to count outcomes for probability calculations)