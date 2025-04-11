# 05 - Units Digit

**Tags:** #quant #number_system #units_digit #cyclicity

Finding the units digit (or the last digit) of an arithmetic expression, especially involving large powers, is a common question type in quantitative aptitude tests. The key principle is that the units digit of the result depends *only* on the units digits of the operands.

---

## Basic Operations

*   **Addition:** The units digit of a sum is the units digit of the sum of the units digits of the numbers being added.
    *   *Example:* Units digit of (12**3** + 45**6** + 78**9**) = Units digit of (3 + 6 + 9) = Units digit of (18) = **8**.
*   **Multiplication:** The units digit of a product is the units digit of the product of the units digits of the numbers being multiplied.
    *   *Example:* Units digit of (1**2** * 3**4** * 5**6**) = Units digit of (2 * 4 * 6) = Units digit of (8 * 6) = Units digit of (48) = **8**.
*   *See Example:* [[05.E03 - Unit Digit of Sum Product Example]]

---

## Units Digit of Powers (a^b) - Cyclicity

The units digits of powers of a number often repeat in a cycle. Finding the units digit of `a^b` involves:
1.  Focusing only on the units digit of the base `a`. Let this be `u`.
2.  Finding the repeating cycle of units digits for powers of `u`.
3.  Using the exponent `b` to determine where in the cycle the result falls.

**Cyclicity Rules:**

| Units Digit of Base (u) | Cyclicity Pattern                       | Cycle Length |
| :---------------------- | :-------------------------------------- | :----------- |
| 0                       | 0                                       | 1            |
| 1                       | 1                                       | 1            |
| 2                       | 2, 4, 8, 6                              | 4            |
| 3                       | 3, 9, 7, 1                              | 4            |
| 4                       | 4, 6                                    | 2            |
| 5                       | 5                                       | 1            |
| 6                       | 6                                       | 1            |
| 7                       | 7, 9, 3, 1                              | 4            |
| 8                       | 8, 4, 2, 6                              | 4            |
| 9                       | 9, 1                                    | 2            |

**Shortcut Method:**

To find the units digit of `u^b`:

1.  Identify the cycle length `L` for the units digit `u` from the table above.
2.  Find the remainder when the exponent `b` is divided by the cycle length `L`: `Rem = Rem(b / L)`.
    *   This is essentially finding `b mod L`. See [[04 - Remainder Theorem]].
3.  **Determine the result:**
    *   If `Rem` is **not 0**, the units digit is the `Rem`-th digit in the cycle for `u`.
    *   If `Rem` is **0**, the units digit is the **last** digit in the cycle for `u` (equivalent to the `L`-th digit).

*   *Example (Units digit of 7¹⁰³):*
    *   Base units digit `u = 7`. Cycle = (7, 9, 3, 1). Length `L = 4`.
    *   Exponent `b = 103`. Find `Rem(103 / 4)`. 103 = 4 * 25 + 3. `Rem = 3`.
    *   Since `Rem = 3`, the units digit is the 3rd digit in the cycle (7, 9, **3**, 1), which is 3.
    *   Units digit of 7¹⁰³ is **3**.

*   *Example (Units digit of 8⁷²):*
    *   Base units digit `u = 8`. Cycle = (8, 4, 2, 6). Length `L = 4`.
    *   Exponent `b = 72`. Find `Rem(72 / 4)`. 72 = 4 * 18 + 0. `Rem = 0`.
    *   Since `Rem = 0`, the units digit is the last (4th) digit in the cycle (8, 4, 2, **6**), which is 6.
    *   Units digit of 8⁷² is **6**.

*   *See Examples:*
    *   [[05.E01 - Unit Digit of Large Power (Cycle 4) Example]]
    *   [[05.E02 - Unit Digit of Large Power (Cycle 2) Example]]

---

**Connection to Remainder Theorem:**
Finding the units digit is equivalent to finding the remainder when the number is divided by 10. The cyclicity method is a specialized application of remainder properties ([[04 - Remainder Theorem]]).

**Special Cases:**
*   Any positive integer power of a number ending in 0, 1, 5, or 6 will end in 0, 1, 5, or 6 respectively.
*   Powers of numbers ending in 4: Units digit is 4 if the exponent is odd, 6 if the exponent is even.
*   Powers of numbers ending in 9: Units digit is 9 if the exponent is odd, 1 if the exponent is even.

---

**Related Concepts:**
*   [[04 - Remainder Theorem]] (Modulo 10)
*   [[01 - Divisibility Rules]] (Rule for 10)