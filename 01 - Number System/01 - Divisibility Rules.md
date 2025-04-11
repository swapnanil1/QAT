# 01 - Divisibility Rules

**Tags:** #quant #number_system #divisibility

Divisibility rules are shortcuts to determine if a number is exactly divisible by another number without performing the full division. They are extremely useful in competitive exams for:
*   Quickly checking factors.
*   Simplifying fractions.
*   Solving problems related to HCF/LCM and number properties.
*   Eliminating options in Multiple Choice Questions (MCQs).

---

## Core Divisibility Rules

Here are the most common and useful divisibility rules:

*   **Divisibility by 2:**
    *   **Rule:** The last digit of the number must be even (0, 2, 4, 6, 8).
    *   *Example:* 50**8** is divisible by 2. 13**5** is not.

*   **Divisibility by 3:**
    *   **Rule:** The sum of the digits of the number must be divisible by 3.
    *   *Example:* 513 -> 5+1+3 = 9. Since 9 is divisible by 3, 513 is divisible by 3.
    *   *See Example:* [[01.E01 - Divisibility by 3 Example]]

*   **Divisibility by 4:**
    *   **Rule:** The number formed by the last two digits must be divisible by 4, OR the last two digits must be 00.
    *   *Example:* 73**24** -> 24 is divisible by 4, so 7324 is divisible by 4. 15**00** is divisible by 4. 81**10** -> 10 is not divisible by 4, so 8110 is not.

*   **Divisibility by 5:**
    *   **Rule:** The last digit of the number must be 0 or 5.
    *   *Example:* 19**5** and 23**0** are divisible by 5. 45**6** is not.

*   **Divisibility by 6:**
    *   **Rule:** The number must be divisible by BOTH 2 AND 3. (Apply both rules).
    *   *Example:* 132 -> Last digit is 2 (divisible by 2). Sum of digits is 1+3+2=6 (divisible by 3). So, 132 is divisible by 6.

*   **Divisibility by 7:** (Less common shortcut, often slower than dividing)
    *   **Rule:** Double the last digit and subtract it from the rest of the number. If the result is 0 or divisible by 7, the original number is divisible by 7. Repeat the process if needed.
    *   *Example:* 343 -> 34 - (2 * 3) = 34 - 6 = 28. Since 28 is divisible by 7, 343 is divisible by 7.

*   **Divisibility by 8:**
    *   **Rule:** The number formed by the last three digits must be divisible by 8, OR the last three digits must be 000.
    *   *Example:* 57**128** -> 128 is divisible by 8 (128 / 8 = 16), so 57128 is divisible by 8. 4**000** is divisible by 8.
    *   *See Example:* [[01.E02 - Divisibility by 8 Example]]

*   **Divisibility by 9:**
    *   **Rule:** The sum of the digits of the number must be divisible by 9. (Similar to rule for 3).
    *   *Example:* 729 -> 7+2+9 = 18. Since 18 is divisible by 9, 729 is divisible by 9.

*   **Divisibility by 10:**
    *   **Rule:** The last digit of the number must be 0.
    *   *Example:* 12**0** is divisible by 10. 54**1** is not.

*   **Divisibility by 11:**
    *   **Rule:** Find the difference between the sum of digits at odd places (from right) and the sum of digits at even places (from right). If the difference is 0 or divisible by 11, the number is divisible by 11.
    *   *Example:* 13574 -> (4+5+1) - (7+3) = 10 - 10 = 0. So, 13574 is divisible by 11.
    *   *Example:* 987 -> (7+9) - 8 = 16 - 8 = 8. Not divisible by 11.
    *   *See Example:* [[01.E03 - Divisibility by 11 Example]]

---

## Divisibility by Composite Numbers

To check if a number is divisible by a composite number (like 6, 12, 15, 72, etc.):
1.  Break the composite number into two or more **co-prime** factors (factors that have no common divisor other than 1).
2.  Check if the original number is divisible by **each** of these co-prime factors using their respective rules.
3.  If the number is divisible by ALL the co-prime factors, it is divisible by the composite number.

*   *Example:* To check divisibility by **72**:
    *   Co-prime factors of 72 are 8 and 9 (since HCF(8, 9) = 1).
    *   Check if the number is divisible by 8 AND divisible by 9.
    *   *See Example:* [[01.E04 - Divisibility by 72 (Composite) Example]]

*   *Example:* To check divisibility by **12**:
    *   Co-prime factors of 12 are 3 and 4.
    *   Check if the number is divisible by 3 AND divisible by 4.

---

**Related Concepts:**
*   [[02 - Factors and Multiples]]
*   [[03 - HCF and LCM]]
*   [[07 - Digital Root (Casting Out Nines)]] (Related to divisibility by 9)