# 03 - HCF and LCM

**Tags:** #quant #number_system #hcf #lcm #gcd

Highest Common Factor (HCF), also known as Greatest Common Divisor (GCD), and Least Common Multiple (LCM) are fundamental concepts derived from factors and multiples. They are essential tools for simplifying fractions, solving problems involving distribution, time & work scenarios, and various number theory questions.

---

## Definitions

*   **HCF (Highest Common Factor) / GCD (Greatest Common Divisor):**
    *   The largest positive integer that divides two or more given integers without leaving a remainder.
    *   *Example:* Factors of 12 are {1, 2, 3, 4, 6, 12}. Factors of 18 are {1, 2, 3, 6, 9, 18}. The common factors are {1, 2, 3, 6}. The highest common factor (HCF) is 6.

*   **LCM (Least Common Multiple):**
    *   The smallest positive integer that is a multiple of two or more given integers.
    *   *Example:* Multiples of 12 are {12, 24, 36, 48, 60, 72, ...}. Multiples of 18 are {18, 36, 54, 72, ...}. The common multiples are {36, 72, ...}. The least common multiple (LCM) is 36.

---

## Methods for Finding HCF/GCD

1.  **Prime Factorization Method (Most Reliable):**
    *   Find the prime factorization of each number (See [[02 - Factors and Multiples]]).
    *   Identify the common prime factors.
    *   Multiply these common prime factors, taking the **lowest power** of each common prime factor present in the factorizations.
    *   *Example (HCF of 72 and 90):*
        *   72 = 2³ * 3²
        *   90 = 2¹ * 3² * 5¹
        *   Common primes are 2 and 3.
        *   Lowest power of 2 is 2¹. Lowest power of 3 is 3².
        *   HCF = 2¹ * 3² = 2 * 9 = 18.

2.  **Euclidean Algorithm (Division Method) (Very Efficient):**
    *   Divide the larger number by the smaller number and find the remainder.
    *   If the remainder is 0, the smaller number is the HCF.
    *   If the remainder is not 0, replace the larger number with the smaller number and the smaller number with the remainder.
    *   Repeat the division process until the remainder is 0. The last non-zero divisor is the HCF.
    *   *See Example:* [[03.E02 - HCF using Euclidean Algorithm Example]]

3.  **Subtraction Factor Method (Conceptual, Can be Slow):**
    *   Repeatedly subtract the smaller number from the larger number until both numbers become equal. This equal number is the HCF.
    *   *See Example:* [[03.E01 - HCF using Subtraction Factor Method Example]]

---

## Methods for Finding LCM

1.  **Prime Factorization Method (Most Reliable):**
    *   Find the prime factorization of each number.
    *   Identify **all** prime factors that appear in *any* of the factorizations.
    *   Multiply these prime factors together, taking the **highest power** of each prime factor present.
    *   *Example (LCM of 72 and 90):*
        *   72 = 2³ * 3²
        *   90 = 2¹ * 3² * 5¹
        *   All primes involved are 2, 3, and 5.
        *   Highest power of 2 is 2³. Highest power of 3 is 3². Highest power of 5 is 5¹.
        *   LCM = 2³ * 3² * 5¹ = 8 * 9 * 5 = 72 * 5 = 360.
    *   *See Example:* [[03.E03 - LCM using Prime Factorization Example]]

2.  **Common Division Method (Good for Multiple Numbers):**
    *   Arrange the numbers in a row.
    *   Divide the numbers by a common prime factor that divides at least two of them. Write the quotients below and carry down any numbers not divisible.
    *   Repeat the process until no two numbers share a common prime factor.
    *   The LCM is the product of all the prime divisors used and the remaining undivided numbers in the last row.
    *   *See Example:* [[03.E04 - LCM using Common Division Method Example]]

---

## Fundamental Relationship between HCF and LCM

For any two positive integers `a` and `b`:
**HCF(a, b) * LCM(a, b) = a * b**

*   **Use Case:** If you know any three of these values (HCF, LCM, a, b), you can find the fourth. This is a very common shortcut in MCQs.
*   **Caution:** This relationship **does not** directly apply to three or more numbers (i.e., HCF(a,b,c) * LCM(a,b,c) ≠ a*b*c).
*   *See Example:* [[03.E05 - LCM HCF Relation Example]]

---

## Applications & Related Concepts

*   [[01 - Number System/01 - Divisibility Rules.md]] (Essential for speeding up prime factorization and division methods)
*   [[01 - Number System/02 - Factors and Multiples.md]] (The core concepts upon which HCF and LCM are built)
*   [[01 - Number System/04 - Remainder Theorem.md]] (Some advanced HCF/LCM problems involve remainders)
*   [[09 - Time and Work/01 - Basic Concepts (Work Rate, LCM Method).md]] (LCM is used extensively to find a common work unit)
*   [[10 - Pipes and Cisterns/01 - Basic Concepts (Filling Emptying Rates, LCM Method).md]] (LCM is used to find a common capacity unit)