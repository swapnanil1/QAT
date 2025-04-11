# 04 - Remainder Theorem

**Tags:** #quant #number_system #remainders #modulo_arithmetic

The Remainder Theorem and related concepts deal with finding the remainder when an integer (or expression) is divided by another integer. This is a fundamental part of number theory with wide applications in competitive exams, often involving large numbers or powers where direct calculation is impossible.

---

## Basic Concepts

**Division Algorithm:**
For any integers `a` (dividend) and `d` (divisor) where `d > 0`, there exist unique integers `q` (quotient) and `r` (remainder) such that:
`a = d * q + r`
where `0 ≤ r < d`.

*   The remainder `r` is always non-negative and strictly less than the divisor `d`.
*   If `r = 0`, then `a` is perfectly divisible by `d` (See [[01 - Divisibility Rules]]).

*See Example:* [[04.E01 - Basic Remainder Calculation Example]]

**Modulo Notation:**
The expression `a ≡ r (mod d)` means that `a` and `r` have the same remainder when divided by `d`. It reads "`a` is congruent to `r` modulo `d`".

---

## Properties of Remainders (Modulo Arithmetic)

These properties are key to solving complex remainder problems quickly:

Let `Rem(x / d)` denote the remainder when `x` is divided by `d`.

1.  **Remainder of a Sum/Difference:**
    `Rem((a + b) / d) = Rem( Rem(a / d) + Rem(b / d) / d )`
    `Rem((a - b) / d) = Rem( Rem(a / d) - Rem(b / d) / d )`
    *   *Shortcut:* Find individual remainders, add/subtract them, and then find the remainder of the result when divided by `d`.

2.  **Remainder of a Product:**
    `Rem((a * b) / d) = Rem( Rem(a / d) * Rem(b / d) / d )`
    *   *Shortcut:* Find individual remainders, multiply them, and then find the remainder of the product when divided by `d`. This is extremely useful for large products.

3.  **Remainder of a Power:**
    `Rem(a^k / d) = Rem( [Rem(a / d)]^k / d )`
    *   *Shortcut:* Find the remainder of the base first, then raise this smaller remainder to the power `k`, and finally find the remainder of that result when divided by `d`. This often leads to finding patterns (cyclicity).

---

## Negative Remainders (Calculation Tool)

Sometimes, using a negative remainder (conceptually) simplifies intermediate calculations.
If `a = d * q + r`, then we can also write `a = d * (q+1) + (r-d)`.
The value `(r-d)` is the *negative remainder*. It's useful because its absolute value is sometimes smaller than `r`.

*   **Rule:** `Positive Remainder = Negative Remainder + Divisor`
*   **How to use:** Perform calculations (especially multiplication) using either the positive or negative remainder (whichever is smaller in magnitude). If the final result is negative, add the divisor once to get the standard positive remainder.

*See Example:* [[04.E02 - Negative Remainder Example]]

---

## Remainder Cyclicity

When finding the remainder of large powers `a^k / d`, the remainders often repeat in a cycle.

1.  Calculate the remainders for the first few powers: `Rem(a^1/d)`, `Rem(a^2/d)`, `Rem(a^3/d)`, ...
2.  Identify the pattern (cycle) of remainders. Let the cycle length be `L`. The cycle often starts after the first few terms, or immediately. A remainder of 1 often ends a cycle, as `1^n = 1`.
3.  Find the remainder of the exponent `k` when divided by the cycle length `L`: `Rem(k / L) = m`.
4.  The required remainder `Rem(a^k / d)` will be the same as the `m`-th remainder in the cycle (or the last one if `m=0`).

*   This concept is very similar to finding the [[05 - Units Digit]] of large powers.
*   *See Example:* [[04.E03 - Remainder Cyclicity Example]]

---

## Specific Remainder Theorems (Shortcuts for Primes/Co-primes)

1.  **Fermat's Little Theorem (FLT):**
    *   **Statement:** If `p` is a prime number, then for any integer `a` not divisible by `p`, we have:
        `a^(p-1) ≡ 1 (mod p)`
        (i.e., `Rem(a^(p-1) / p) = 1`)
    *   **Use Case:** Very powerful for simplifying large powers when the divisor is a prime number. You can reduce the exponent modulo `(p-1)`.
    *   *See Example:* [[04.E04 - Applying Fermat's Little Theorem Example]]

2.  **Euler's Totient Theorem (Generalization of FLT):**
    *   **Statement:** If `a` and `n` are co-prime integers (i.e., HCF(a, n) = 1, see [[03 - HCF and LCM]]), then:
        `a^φ(n) ≡ 1 (mod n)`
        where `φ(n)` (Euler's Totient Function) counts the positive integers less than or equal to `n` that are co-prime to `n`.
    *   **Calculating φ(n):** If prime factorization of `n = p1^a * p2^b * ...`, then `φ(n) = n * (1 - 1/p1) * (1 - 1/p2) * ...`
    *   **Use Case:** Works when the divisor `n` is not prime, as long as the base `a` is co-prime to `n`. Reduces the exponent modulo `φ(n)`.

3.  **Wilson's Theorem:** (Less common in basic quant, more number theory)
    *   **Statement:** For a prime number `p`, `(p-1)! ≡ -1 (mod p)`.

4.  **Chinese Remainder Theorem (CRT):** (Advanced)
    *   Used to solve systems of simultaneous congruences with co-prime moduli. E.g., Find a number `x` such that `x ≡ r1 (mod d1)`, `x ≡ r2 (mod d2)`, etc., where `d1, d2...` are pairwise co-prime.

---

**Related Concepts:**
*   [[01 - Divisibility Rules]] (Remainder is 0)
*   [[05 - Units Digit]] (Remainder when dividing by 10; uses cyclicity)
*   [[03 - HCF and LCM]] (Euler's Totient theorem requires co-prime condition)
*   [[03 - Quadratic Equations]] (Polynomial Remainder Theorem: Remainder when polynomial P(x) is divided by (x-a) is P(a))