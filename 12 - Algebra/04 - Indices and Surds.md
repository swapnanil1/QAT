# Indices and Surds

Tags: #quant #algebra #indices #exponents #surds #roots #concept #formula #simplification #rationalization

---

**Introduction:**

Indices (or exponents/powers) and surds (roots) are fundamental concepts in algebra dealing with powers and roots of numbers or variables. Mastery of their laws and manipulation techniques is crucial for simplifying complex expressions encountered in various quantitative aptitude topics, particularly in algebra and [[01 - Number System/08 - Simplification and Approximation.md|Simplification]].

**Indices (Exponents):**

An index indicates how many times a base number is multiplied by itself. In the expression `a^m`, `a` is the base, and `m` is the index/exponent/power.

**Laws of Indices:**

Assuming `a`, `b` are real numbers and `m`, `n` are rational numbers:

1.  **Product Rule:** `a^m * a^n = a^(m+n)` (When multiplying powers with the same base, add the indices).
2.  **Quotient Rule:** `a^m / a^n = a^(m-n)` (When dividing powers with the same base, subtract the indices).
3.  **Power of a Power Rule:** `(a^m)^n = a^(m*n)` (When raising a power to another power, multiply the indices).
4.  **Power of a Product Rule:** `(a * b)^m = a^m * b^m`
5.  **Power of a Quotient Rule:** `(a / b)^m = a^m / b^m` (where `b ≠ 0`)
6.  **Zero Index:** `a^0 = 1` (Any non-zero number raised to the power of zero is 1).
7.  **Negative Index:** `a^(-m) = 1 / a^m` (A negative index indicates the reciprocal of the base raised to the positive index).
8.  **Fractional Index (Roots):** `a^(1/n) = nth_root(a)` (The nth root of `a`). More generally, `a^(m/n) = (nth_root(a))^m = nth_root(a^m)`.

**Surds (Roots):**

A surd is an irrational root of a rational number. It's a root that cannot be simplified to a whole number or a terminating/repeating decimal (e.g., `sqrt(2)`, `cuberoot(5)`). An expression like `sqrt(4)` is not a surd because it simplifies to 2 (a rational number).

*   **Order of a Surd:** The index of the root (e.g., `sqrt(a)` is order 2, `cuberoot(a)` is order 3).
*   **Simplest Form:** A surd is in its simplest form when the number under the root sign (radicand) has no factors that are perfect nth powers (where n is the order of the surd). Example: `sqrt(12) = sqrt(4*3) = sqrt(4)*sqrt(3) = 2*sqrt(3)`.
*   **Like Surds:** Surds having the same order and the same radicand (e.g., `2*sqrt(3)` and `5*sqrt(3)`). Only like surds can be added or subtracted directly.
*   **Comparison of Surds:** To compare surds, convert them to the same order. Example: Compare `sqrt(3)` and `cuberoot(5)`. LCM of orders 2 and 3 is 6. `sqrt(3) = 3^(1/2) = 3^(3/6) = 6th_root(3^3) = 6th_root(27)`. `cuberoot(5) = 5^(1/3) = 5^(2/6) = 6th_root(5^2) = 6th_root(25)`. Since `27 > 25`, `sqrt(3) > cuberoot(5)`.

**Operations with Surds:**

*   **Addition/Subtraction:** Only possible for like surds. `p*sqrt(a) + q*sqrt(a) = (p+q)*sqrt(a)`.
*   **Multiplication:** `nth_root(a) * nth_root(b) = nth_root(a*b)` (Surds must be of the same order).
*   **Division:** `nth_root(a) / nth_root(b) = nth_root(a/b)` (Surds must be of the same order).
*   **Rationalization:** The process of eliminating a surd from the denominator of a fraction.
    *   If the denominator is `sqrt(a)`, multiply numerator and denominator by `sqrt(a)`.
    *   If the denominator is `a + sqrt(b)`, multiply numerator and denominator by its conjugate `a - sqrt(b)`.
    *   If the denominator is `sqrt(a) + sqrt(b)`, multiply numerator and denominator by its conjugate `sqrt(a) - sqrt(b)`. This uses the identity `(p+q)(p-q) = p^2 - q^2` (from [[12 - Algebra/01 - Basic Algebraic Identities.md]]).

**General Approach:**

1.  **Apply Laws:** Use the laws of indices to simplify expressions involving powers.
2.  **Simplify Surds:** Reduce surds to their simplest form.
3.  **Convert Orders (if needed):** For multiplication, division, or comparison, ensure surds have the same order.
4.  **Combine Like Terms:** Add or subtract like surds.
5.  **Rationalize:** If required, eliminate surds from the denominator.

**Examples:**
*   [[12 - Algebra/04.E01 - Laws of Indices Application Example.md]] (Illustrates simplifying expressions using index laws)
*   [[12 - Algebra/04.E02 - Simplifying Surds Example.md]] (Illustrates simplifying, operating, and rationalizing surds)

**Related Concepts:**
*   [[01 - Number System/01 - Divisibility Rules.md]] (Understanding factors helps simplify surds)
*   [[12 - Algebra/01 - Basic Algebraic Identities.md]] (Crucial for rationalizing denominators with binomial surds)
*   [[12 - Algebra/03 - Quadratic Equations.md]] (Roots from the quadratic formula often involve surds)
*   [[01 - Number System/08 - Simplification and Approximation.md]] (Indices and surds feature heavily)