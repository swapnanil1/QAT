# 06 - Base Conversions

**Tags:** #quant #number_system #base_conversion #binary #octal #hexadecimal #decimal

Base conversion deals with representing the same numerical value using different number systems (bases). While the standard system is decimal (base-10), other bases like binary (base-2), octal (base-8), and hexadecimal (base-16) are crucial in computer science and occasionally appear in quantitative reasoning problems.

---

## Understanding Number Bases & Place Value

Any number's value is determined by the digits it contains and their positions (place values). In a base-`b` system:
*   There are `b` unique digits (usually 0 to `b-1`).
*   The place values (from right to left) are powers of the base: `b⁰`, `b¹`, `b²`, `b³`, ...

*   **Decimal (Base-10):** Digits 0-9. Place values: 10⁰=1, 10¹=10, 10²=100, ...
    *   Example: 253₁₀ = (2 * 10²) + (5 * 10¹) + (3 * 10⁰) = 200 + 50 + 3 = 253.
*   **Binary (Base-2):** Digits 0, 1. Place values: 2⁰=1, 2¹=2, 2²=4, 2³=8, ...
*   **Octal (Base-8):** Digits 0-7. Place values: 8⁰=1, 8¹=8, 8²=64, ...
*   **Hexadecimal (Base-16):** Digits 0-9 and A(10), B(11), C(12), D(13), E(14), F(15). Place values: 16⁰=1, 16¹=16, 16²=256, ...

*(Notation: A number's base is often indicated by a subscript, e.g., 1101₂)*

---

## Conversion Methods

**1. Decimal (Base-10) to Any Base `b`:**

*   **Method: Repeated Division**
    1.  Divide the decimal number by the target base `b`.
    2.  Record the **remainder**.
    3.  Replace the number with the **quotient**.
    4.  Repeat steps 1-3 until the quotient becomes 0.
    5.  The sequence of remainders, read in **reverse order** (bottom-up), forms the number in base `b`.
*   *See Examples:*
    *   [[06.E01 - Decimal to Binary Example]]
    *   [[06.E03 - Decimal to Octal Example]]

**2. Any Base `b` to Decimal (Base-10):**

*   **Method: Sum of Place Value Products**
    1.  Identify the digits of the number in base `b`.
    2.  Identify the place value (powers of `b`: `b⁰`, `b¹`, `b²`, ... starting from the rightmost digit).
    3.  Multiply each digit by its corresponding place value.
    4.  Sum up all these products. The result is the decimal equivalent.
*   *See Example:* [[06.E02 - Binary to Decimal Example]]

**3. Binary (Base-2) <-> Octal (Base-8) Shortcut:**

*   **Concept:** Since 8 = 2³, each octal digit corresponds to exactly **3** binary digits (bits).
*   **Binary to Octal:**
    1.  Group the binary digits into sets of 3, starting from the **right**. Add leading zeros if needed to complete the leftmost group.
    2.  Convert each 3-bit group into its corresponding octal digit (0-7).
    *   *(Lookup: 000=0, 001=1, 010=2, 011=3, 100=4, 101=5, 110=6, 111=7)*
*   **Octal to Binary:**
    1.  Convert each octal digit into its 3-bit binary equivalent.
    2.  Concatenate the binary groups.

**4. Binary (Base-2) <-> Hexadecimal (Base-16) Shortcut:**

*   **Concept:** Since 16 = 2⁴, each hexadecimal digit corresponds to exactly **4** binary digits (bits).
*   **Binary to Hexadecimal:**
    1.  Group the binary digits into sets of 4, starting from the **right**. Add leading zeros if needed.
    2.  Convert each 4-bit group into its corresponding hexadecimal digit (0-9, A-F).
    *   *(Lookup: 0000=0...1001=9, 1010=A, 1011=B, 1100=C, 1101=D, 1110=E, 1111=F)*
*   **Hexadecimal to Binary:**
    1.  Convert each hexadecimal digit into its 4-bit binary equivalent.
    2.  Concatenate the binary groups.
*   *See Example:* [[06.E04 - Binary to Hexadecimal Example]]

**5. Conversions Between Other Bases (e.g., Octal to Hexadecimal):**
*   The easiest way is usually to convert the source base to Decimal first, then convert the decimal result to the target base.
*   Alternatively, convert the source base to Binary (using shortcuts if applicable), then convert the binary result to the target base (using shortcuts if applicable).

---

**Table of Common Values (0-15):**

| Decimal | Binary | Octal | Hexadecimal |
| :------ | :----- | :---- | :---------- |
| 0       | 0000   | 0     | 0           |
| 1       | 0001   | 1     | 1           |
| 2       | 0010   | 2     | 2           |
| 3       | 0011   | 3     | 3           |
| 4       | 0100   | 4     | 4           |
| 5       | 0101   | 5     | 5           |
| 6       | 0110   | 6     | 6           |
| 7       | 0111   | 7     | 7           |
| 8       | 1000   | 10    | 8           |
| 9       | 1001   | 11    | 9           |
| 10      | 1010   | 12    | A           |
| 11      | 1011   | 13    | B           |
| 12      | 1100   | 14    | C           |
| 13      | 1101   | 15    | D           |
| 14      | 1110   | 16    | E           |
| 15      | 1111   | 17    | F           |

---

**Related Concepts:**
*   Understanding place value is fundamental to [[01 - Number System]] basics.