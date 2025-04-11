# Series and Progressions (AP, GP)

Tags: #quant #miscellaneous_optional #series_and_progressions #arithmetic_progression #geometric_progression #formula #algebra

---

**Introduction:**
A sequence is a set of numbers arranged in a definite order according to some rule. A series is the sum of the terms of a sequence. A progression is a sequence where the terms follow a specific pattern, often involving a constant difference or a constant ratio between consecutive terms. The most common types encountered in quantitative aptitude are Arithmetic Progression (AP) and Geometric Progression (GP). Understanding their properties and formulas is key to solving related problems efficiently.

**Basic Definitions:**
*   **Sequence:** An ordered list of numbers, called terms (e.g., 2, 4, 6, 8,...).
*   **Term:** Each number in a sequence (e.g., in 2, 4, 6, 8, the first term is 2, the second is 4, etc.). The nth term is often denoted by `a_n` or `T_n`.
*   **Series:** The sum of the terms of a sequence (e.g., 2 + 4 + 6 + 8 + ...).
*   **Arithmetic Progression (AP):** A sequence where the difference between any term and its preceding term is constant. This constant difference is called the **common difference (d)**.
*   **Geometric Progression (GP):** A sequence where the ratio of any term to its preceding term is constant. This constant ratio is called the **common ratio (r)**. (Terms must be non-zero).
*   **Harmonic Progression (HP):** A sequence where the reciprocals of the terms form an Arithmetic Progression. (Terms must be non-zero).

---

**Key Formulas/Properties/Methods:**

**1. Arithmetic Progression (AP):**
*   **General Form:** `a, a+d, a+2d, a+3d, ...` where `a` is the first term and `d` is the common difference.
*   **Common Difference:** `d = a_n - a_(n-1)`
*   **nth Term (a_n):** `a_n = a + (n-1)d` (Calculates the value of the term at the nth position)
*   **Sum of First n Terms (S_n):**
    *   `S_n = n/2 * [2a + (n-1)d]` (Use when first term `a`, common difference `d`, and number of terms `n` are known)
    *   `S_n = n/2 * (a + l)` (Use when first term `a`, last term `l` (which is `a_n`), and number of terms `n` are known)
*   **Arithmetic Mean (AM):** The AM of two numbers `x` and `y` is `(x+y)/2`. If `x, A, y` are in AP, then `A = (x+y)/2`.

**2. Geometric Progression (GP):**
*   **General Form:** `a, ar, ar^2, ar^3, ...` where `a` is the first term and `r` is the common ratio.
*   **Common Ratio:** `r = a_n / a_(n-1)`
*   **nth Term (a_n):** `a_n = a * r^(n-1)` (Calculates the value of the term at the nth position)
*   **Sum of First n Terms (S_n):**
    *   `S_n = a * (r^n - 1) / (r - 1)` (Commonly used when `|r| > 1` or when `r` is positive and greater than 1)
    *   `S_n = a * (1 - r^n) / (1 - r)` (Commonly used when `|r| < 1`)
    *   Note: These two forms are equivalent. Choose based on convenience to avoid negative denominators. Formula requires `r != 1`.
    *   If `r = 1`, the sequence is `a, a, a, ...` and `S_n = n * a`.
*   **Sum of an Infinite GP (S_infinity):**
    *   `S_infinity = a / (1 - r)`
    *   This formula is valid **only if** the absolute value of the common ratio is less than 1 (`|r| < 1`). Otherwise, the sum diverges (tends to infinity or doesn't settle).
*   **Geometric Mean (GM):** The GM of two positive numbers `x` and `y` is `sqrt(x*y)`. If `x, G, y` are in GP, then `G = sqrt(x*y)`.

**3. Harmonic Progression (HP):**
*   A sequence `h_1, h_2, h_3, ...` is in HP if `1/h_1, 1/h_2, 1/h_3, ...` is in AP.
*   To find the nth term of an HP, find the nth term of the corresponding AP (using `a = 1/h_1` and `d = 1/h_2 - 1/h_1`, etc.) and take its reciprocal.
*   There is no simple standard formula for the sum of n terms of an HP.

---

**General Approach & Strategy:**

1.  **Identify Progression Type:** Determine if the sequence has a common difference (AP), common ratio (GP), or if its reciprocals have a common difference (HP).
2.  **Extract Knowns:** Identify the given information: first term (`a`), common difference (`d`)/ratio (`r`), number of terms (`n`), a specific term's value (`a_n`), or the sum (`S_n`).
3.  **Determine the Goal:** Understand what needs to be calculated: a specific term, the sum of terms, the number of terms, `a`, `d`, or `r`.
4.  **Select Formula:** Choose the appropriate formula based on the progression type and the goal.
5.  **Substitute and Solve:** Plug the known values into the formula and solve the resulting equation, which might involve techniques from [[12 - Algebra/02 - Linear Equations (One Two Variables).md|linear equations]] or [[12 - Algebra/03 - Quadratic Equations.md|quadratic equations]].
6.  **Check Conditions:** Verify any conditions required by the formulas used (e.g., `r != 1` for finite GP sum, `|r| < 1` for infinite GP sum).

---

**Examples:**
*(No specific examples for this concept have been defined in the vault structure yet)*

---

**Related Concepts:**

*   [[12 - Algebra/04 - Indices and Surds.md]] (Crucial for handling the powers `r^n` in GP formulas)
*   [[12 - Algebra/02 - Linear Equations (One Two Variables).md]] (Often needed to solve for `n`, `a`, or `d` after substituting values into AP/GP formulas)
*   [[12 - Algebra/03 - Quadratic Equations.md]] (May arise when solving problems involving sums or terms in progressions)
*   [[08 - Averages/01 - Basic Average Formula.md]] (The concept of Arithmetic Mean is directly related to AP)
*   [[01 - Number System/01 - Divisibility Rules.md]] (Can be useful in identifying patterns or properties of terms in a sequence)