# Logarithms

Tags: #quant #miscellaneous_optional #logarithms #formula #algebra

---

**Introduction:**
Logarithms are the inverse operation to exponentiation. Just as division undoes multiplication, logarithms undo exponentiation. They are used to solve equations where the unknown is in the exponent, and they are crucial in simplifying calculations involving very large or very small numbers, especially in fields like finance, science, and engineering. In aptitude tests, logarithm problems often test the understanding and application of logarithm properties (laws).

**Basic Definitions:**
*   **Logarithm:** If `b^y = x`, then the logarithm of `x` to the base `b` is `y`. This is written as `log_b(x) = y`.
    *   `b` is the **base** (must be positive and not equal to 1).
    *   `x` is the **argument** or **number** (must be positive).
    *   `y` is the **logarithm** or **exponent**.
*   **Common Logarithm:** A logarithm with base 10. Written as `log(x)` or `log_10(x)`.
*   **Natural Logarithm:** A logarithm with base `e` (Euler's number, approximately 2.71828). Written as `ln(x)` or `log_e(x)`.
*   **Antilogarithm:** The inverse of the logarithm. If `log_b(x) = y`, then `x` is the antilogarithm of `y` to the base `b`. Finding the antilogarithm is equivalent to exponentiation: `x = b^y`.

---

**Key Formulas/Properties/Methods:**
Understanding these properties is essential for solving logarithm problems:

1.  **Basic Logarithmic Identities:**
    *   `log_b(1) = 0` (Since `b^0 = 1`)
    *   `log_b(b) = 1` (Since `b^1 = b`)
    *   `log_b(b^y) = y` (Logarithm undoes the exponentiation with the same base)
    *   `b^(log_b(x)) = x` (Exponentiation undoes the logarithm with the same base)

2.  **Product Rule:**
    *   `log_b(m * n) = log_b(m) + log_b(n)`
    *   The logarithm of a product is the sum of the logarithms of the factors. (Note: Arguments `m` and `n` must be positive).

3.  **Quotient Rule:**
    *   `log_b(m / n) = log_b(m) - log_b(n)`
    *   The logarithm of a quotient is the difference between the logarithm of the numerator and the logarithm of the denominator. (Note: Arguments `m` and `n` must be positive).

4.  **Power Rule:**
    *   `log_b(m^p) = p * log_b(m)`
    *   The logarithm of a number raised to a power is the power times the logarithm of the number.

5.  **Change of Base Formula:**
    *   `log_b(x) = log_c(x) / log_c(b)`
    *   This allows converting a logarithm from one base (`b`) to another base (`c`). Often used to convert to base 10 or base `e` for easier calculation or use of tables/calculators.
    *   A common specific case: `log_b(x) = 1 / log_x(b)`

---

**General Approach & Strategy:**

1.  **Identify the Goal:** Determine if you need to solve for an unknown variable, simplify an expression, or evaluate a logarithmic value.
2.  **Check Bases:** Ensure all logarithms in an equation or expression are to the same base. If not, use the Change of Base formula to convert them to a common base (often base 10 or `e`, or a base present elsewhere in the problem).
3.  **Apply Logarithm Laws:** Use the Product, Quotient, and Power rules strategically to expand or condense logarithmic expressions.
    *   To solve equations, often condense multiple log terms into a single log term.
    *   To simplify, expand or condense as needed.
4.  **Convert to Exponential Form:** If you have an equation like `log_b(x) = y`, converting it to its equivalent exponential form `b^y = x` can often help solve for the unknown.
5.  **Solve the Resulting Equation:** After applying log rules and/or converting form, you might be left with an algebraic equation (linear, quadratic, exponential). Solve this using appropriate algebraic techniques.
6.  **Check Validity:** Remember the argument of a logarithm must always be positive (`x > 0`) and the base must be positive and not equal to 1 (`b > 0, b != 1`). Discard any potential solutions that violate these conditions.

---

**Examples:**
*(No specific examples for this concept have been defined in the vault structure yet)*

---

**Related Concepts:**

*   [[12 - Algebra/04 - Indices and Surds.md]] (Provides the foundational rules of exponents, which logarithms are the inverse of; understanding exponent rules is crucial for logarithms)
*   [[12 - Algebra/01 - Basic Algebraic Identities.md]] (May be needed to solve equations that arise after applying logarithm rules)
*   [[01 - Number System/08 - Simplification and Approximation.md]] (General simplification techniques may be applicable alongside logarithm rules)