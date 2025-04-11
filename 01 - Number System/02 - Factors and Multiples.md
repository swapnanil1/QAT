# 02 - Factors and Multiples

**Tags:** #quant #number_system #factors #multiples

Understanding factors and multiples is fundamental in number theory and crucial for solving various quantitative aptitude problems, especially those involving HCF/LCM, divisibility, and number properties.

---

## Definitions

*   **Factor:** A factor of a number `N` is an integer that divides `N` exactly, leaving no remainder. Factors are always less than or equal to the number itself.
    *   *Example:* Factors of 12 are 1, 2, 3, 4, 6, and 12.
*   **Multiple:** A multiple of a number `N` is obtained by multiplying `N` by an integer. Multiples are always greater than or equal to the number itself (considering positive integers).
    *   *Example:* Multiples of 12 are 12, 24, 36, 48, ...

---

## Prime Factorization

The foundation for working with factors is **Prime Factorization**. It involves expressing a number as a product of its prime factors.

*   **Method:** Use repeated division by prime numbers (starting with 2, 3, 5, etc.) until you reach 1.
*   **Format:** Express the number `N` as `N = p1^a * p2^b * p3^c * ...` where `p1, p2, p3...` are distinct prime bases and `a, b, c...` are their respective positive integer powers (exponents).
*   *Example:* Prime Factorization of 72:
    *   72 / 2 = 36
    *   36 / 2 = 18
    *   18 / 2 = 9
    *   9 / 3 = 3
    *   3 / 3 = 1
    *   So, 72 = 2 * 2 * 2 * 3 * 3 = **2³ * 3²**

---

## Finding the Total Number of Factors

**Shortcut:** Once you have the prime factorization `N = p1^a * p2^b * p3^c * ...`:
1.  Add 1 to each exponent: `(a+1)`, `(b+1)`, `(c+1)`, ...
2.  Multiply these results together.

**Formula:** Total Number of Factors = `(a+1) * (b+1) * (c+1) * ...`

*   *Example (for N = 72 = 2³ * 3²):*
    *   Exponents are 3 and 2.
    *   Add 1 to each: (3+1) = 4, (2+1) = 3.
    *   Multiply: 4 * 3 = 12.
    *   Therefore, 72 has 12 factors. (They are 1, 2, 3, 4, 6, 8, 9, 12, 18, 24, 36, 72).
*   *See Detailed Example:* [[02.E01 - Finding Number of Factors Example]]

---

## Finding the Sum of All Factors

**Shortcut:** Using the prime factorization `N = p1^a * p2^b * p3^c * ...`:
1.  For each prime factor `pi` with exponent `x`, calculate the sum of its powers from 0 to `x`: `(pi^0 + pi^1 + ... + pi^x)`.
2.  This sum can be calculated quickly using the geometric progression formula: `(pi^(x+1) - 1) / (pi - 1)`.
3.  Multiply these sums together for all prime factors.

**Formula:** Sum of Factors = `[(p1^(a+1) - 1) / (p1 - 1)] * [(p2^(b+1) - 1) / (p2 - 1)] * [(p3^(c+1) - 1) / (p3 - 1)] * ...`

*   *Example (for N = 72 = 2³ * 3²):*
    *   For prime factor 2 (exponent 3): (2^(3+1) - 1) / (2 - 1) = (2⁴ - 1) / 1 = (16 - 1) / 1 = 15.
    *   For prime factor 3 (exponent 2): (3^(2+1) - 1) / (3 - 1) = (3³ - 1) / 2 = (27 - 1) / 2 = 26 / 2 = 13.
    *   Multiply the results: 15 * 13 = 195.
    *   Therefore, the sum of all factors of 72 is 195.
*   *See Detailed Example:* [[02.E02 - Finding Sum of Factors Example]]

---

## Other Factor Concepts (Briefly)

*   **Number of Odd Factors:** Use the prime factorization. Ignore the power of 2. Apply the "Total Number of Factors" formula only to the exponents of the *odd* prime factors.
    *   *Example (72 = 2³ * 3²):* Odd prime factor is 3 with exponent 2. Number of odd factors = (2+1) = 3. (Factors are 1, 3, 9).
*   **Number of Even Factors:** Total Factors - Number of Odd Factors.
    *   *Example (72):* 12 - 3 = 9.
*   **Sum of Odd/Even Factors:** Similar logic applied to the sum formula components.
*   **Number of Prime Factors:** Simply count the number of distinct prime bases in the factorization.
    *   *Example (72 = 2³ * 3²):* Distinct prime bases are 2 and 3. Number of prime factors = 2.
*   **Perfect Number:** A number for which the sum of its *proper* factors (all factors except the number itself) is equal to the number itself. Equivalently, the sum of *all* factors is equal to twice the number (Sum of Factors = 2N).
    *   *Example:* Factors of 6 are 1, 2, 3, 6. Sum = 1+2+3+6 = 12. Since 12 = 2 * 6, 6 is a perfect number.

---

**Related Concepts:**
*   [[01 - Divisibility Rules]]
*   [[03 - HCF and LCM]] (Heavily relies on prime factorization)