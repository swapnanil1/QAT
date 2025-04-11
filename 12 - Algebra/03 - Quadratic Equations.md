# Quadratic Equations

Tags: #quant #algebra #quadratic_equations #formula #concept #roots #discriminant #factorization

---

**Introduction:**

A quadratic equation is a polynomial equation of the second degree, meaning it contains at least one term that is squared. The standard form is `ax^2 + bx + c = 0`, where `x` represents the variable, and `a`, `b`, and `c` are constants (coefficients), with the crucial condition that `a ≠ 0`. Graphically, a quadratic equation represents a parabola. Solving a quadratic equation means finding the values of `x` (called roots or solutions) for which the equation holds true; these roots correspond to the x-intercepts of the parabola.

**Number of Roots:**

A quadratic equation always has two roots. These roots can be:
*   Two distinct real numbers.
*   Two equal real numbers (one distinct real root).
*   Two complex conjugate numbers (often referred to as "no real roots" in introductory contexts).

**Methods for Solving Quadratic Equations:**

1.  **Factoring:**
    *   This method involves rewriting the quadratic expression `ax^2 + bx + c` as a product of two linear factors `(px + q)(rx + s)`.
    *   Set the factored expression equal to zero: `(px + q)(rx + s) = 0`.
    *   Apply the zero-product property: If the product of two factors is zero, then at least one of the factors must be zero. So, either `px + q = 0` or `rx + s = 0`.
    *   Solve these two linear equations to find the two roots.
    *   This method is usually the quickest *if* the quadratic expression is easily factorable. It often relies on finding two numbers that multiply to `ac` and add up to `b`.
    *   Connection to identities: [[12 - Algebra/01 - Basic Algebraic Identities.md|Identities]] like `a^2 - b^2` can sometimes lead to factorable quadratic forms.

2.  **Quadratic Formula:**
    *   This formula provides the roots for *any* quadratic equation, regardless of whether it's easily factorable.
    *   Formula: `x = [-b ± sqrt(b^2 - 4ac)] / (2a)`
    *   The `±` sign indicates that there are two roots: one using the plus sign and one using the minus sign.

3.  **Completing the Square:**
    *   This method involves manipulating the equation `ax^2 + bx + c = 0` into the form `(x + k)^2 = h`, from which `x` can be easily solved by taking the square root.
    *   It's the method used to derive the quadratic formula itself but is less commonly used for direct solving in timed tests compared to factoring or the formula.

**The Discriminant (Δ):**

The expression inside the square root in the quadratic formula, `Δ = b^2 - 4ac`, is called the discriminant. It determines the nature of the roots without actually solving for them:

*   **If `Δ > 0`:** (`b^2 - 4ac > 0`) The equation has two distinct real roots.
*   **If `Δ = 0`:** (`b^2 - 4ac = 0`) The equation has exactly one real root (or two equal real roots). The quadratic expression is a perfect square trinomial.
*   **If `Δ < 0`:** (`b^2 - 4ac < 0`) The equation has two complex conjugate roots (no real roots).

**Relationship Between Roots and Coefficients (Vieta's Formulas):**

If `α` and `β` are the roots of the quadratic equation `ax^2 + bx + c = 0`, then:

*   **Sum of the roots:** `α + β = -b/a`
*   **Product of the roots:** `α * β = c/a`
    These relationships are useful for forming a quadratic equation if the roots are known, or for finding the sum/product of roots without solving the equation.

**General Approach:**

1.  **Standard Form:** Ensure the equation is written as `ax^2 + bx + c = 0`.
2.  **Attempt Factoring:** Try to factor the quadratic expression first, as it's often the fastest method.
3.  **Use Quadratic Formula:** If factoring is difficult or not obvious, apply the quadratic formula `x = [-b ± sqrt(b^2 - 4ac)] / (2a)`.
4.  **Check Discriminant (Optional):** If only the nature of the roots is needed, calculate the discriminant `Δ = b^2 - 4ac`.
5.  **Simplify:** Simplify the roots obtained.

**Examples:**
*   [[12 - Algebra/03.E01 - Solving Quadratic Equation by Factoring Example.md]]
*   [[12 - Algebra/03.E02 - Quadratic Formula Example.md]]
*   [[12 - Algebra/03.E03 - Nature of Roots Example.md]]

**Related Concepts:**
*   [[12 - Algebra/01 - Basic Algebraic Identities.md]] (Useful for factoring and recognizing patterns)
*   [[12 - Algebra/02 - Linear Equations (One Two Variables).md]] (Solving linear equations is a sub-step in factoring)
*   [[12 - Algebra/04 - Indices and Surds.md]] (Handling the square root in the quadratic formula)