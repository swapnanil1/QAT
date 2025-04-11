# Factorial Notation

Tags: #quant #permutations_and_combinations #factorial #concept #formula

---

**Introduction:**

Factorial notation is a fundamental concept primarily used in permutations (arrangements) and combinations (selections), as well as in probability calculations. It represents the product of all positive integers less than or equal to a given non-negative integer. Understanding factorials is the first step towards solving problems involving arrangements and selections.

**Definition and Formula:**

For a non-negative integer `n`, the factorial of `n`, denoted by `n!` (read as "n factorial"), is defined as:

`n! = n * (n-1) * (n-2) * ... * 3 * 2 * 1`

**Special Cases:**

*   **Zero Factorial:** By definition, `0! = 1`. This is a convention necessary for many combinatorial formulas, like the combination formula `nCr = n! / (r! * (n-r)!)` when `r=0` or `r=n`.
*   **One Factorial:** `1! = 1`

**Examples:**

*   `2! = 2 * 1 = 2`
*   `3! = 3 * 2 * 1 = 6`
*   `4! = 4 * 3 * 2 * 1 = 24`
*   `5! = 5 * 4 * 3 * 2 * 1 = 120`
*   `6! = 6 * 5 * 4 * 3 * 2 * 1 = 720`

---

**Properties and Rules:**

*   **Recursive Property:** `n! = n * (n-1)!`
    *   Example: `5! = 5 * 4! = 5 * 24 = 120`
*   **Not Distributive:** Factorial does not distribute over addition or subtraction. `(a + b)! != a! + b!` and `(a - b)! != a! - b!`.
*   **Division/Cancellation:** Factorials are often simplified by cancellation in fractions.
    *   Example: `8! / 5! = (8 * 7 * 6 * 5!) / 5! = 8 * 7 * 6 = 336`
    *   Example: `10! / (7! * 3!) = (10 * 9 * 8 * 7!) / (7! * (3 * 2 * 1)) = (10 * 9 * 8) / 6 = 10 * 3 * 4 = 120`

---

**General Approach & Tips:**

*   **Calculation:** For small values of `n`, calculate factorials directly. Memorizing values up to 6! or 7! can be helpful.
*   **Simplification:** When dealing with ratios of factorials, always expand the larger factorial until it matches the smaller one to allow for cancellation. Avoid calculating the full large factorial value.
    *   Example: To calculate `12! / 10!`, write it as `(12 * 11 * 10!) / 10!` and cancel `10!`.
*   **Applications:** Factorial notation is the building block for [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md|permutations (nPr)]] and [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md|combinations (nCr)]].

---

**Examples:**

*   [[15 - Permutations and Combinations/01.E01 - Calculating Factorials Example.md]] (Illustrates direct calculation and simplification of factorial expressions)

---

**Related Concepts:**

*   [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md]] (Uses factorials in its definition)
*   [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Uses factorials extensively in its definition)
*   [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md]] (Combinatorics, using factorials, helps determine the number of outcomes in sample spaces)