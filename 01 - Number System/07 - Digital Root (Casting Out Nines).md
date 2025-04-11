# 07 - Digital Root (Casting Out Nines)

**Tags:** #quant #number_system #digital_root #casting_out_nines #calculation_check

The **Digital Root** of a non-negative integer is the single-digit value obtained by an iterative process of summing digits, on each step using the result of the previous step as input to the digit summation. The process continues until a single-digit number is reached.

This concept is closely related to **Casting Out Nines**, a shortcut technique used primarily to check the validity of arithmetic calculations (addition, subtraction, multiplication).

---

## Calculating the Digital Root

There are a few ways to find the digital root:

**Method 1: Iterative Summation**
1.  Sum the digits of the number.
2.  If the sum is a single digit, that's the digital root.
3.  If the sum has more than one digit, repeat step 1 with the sum.
*   *See Example:* [[07.E01 - Calculating Digital Root Example]]

**Method 2: Modulo 9 Property (The Core Connection)**
The digital root of a number `N` is equivalent to its remainder when divided by 9, with one exception:
*   `Digital Root = Rem(N / 9)` if `Rem(N / 9)` is not 0.
*   `Digital Root = 9` if `Rem(N / 9)` is 0.
*   Essentially: `Digital Root = (N - 1) mod 9 + 1`

*   This directly connects to the [[01 - Divisibility Rules]] for 9: A number is divisible by 9 if and only if its digital root is 9.

**Method 3: "Casting Out Nines" Shortcut**
While summing the digits (using Method 1), you can ignore (cast out) any digit that is 9, or any group of digits that sum to 9 or a multiple of 9. This often simplifies the summation significantly.
*   *Example:* Digital Root of 918273
    *   Sum: 9 + 1 + 8 + 2 + 7 + 3
    *   Cast out 9: (1 + 8) + (2 + 7) + 3
    *   Cast out (1+8)=9 and (2+7)=9: Remaining is 3.
    *   Digital Root = 3.
*   *See Example:* [[07.E01 - Calculating Digital Root Example]]

---

## Checking Arithmetic using Digital Roots ("Casting Out Nines")

The principle is that the digital root of the result of an arithmetic operation should be the same as the digital root obtained by performing the same operation on the digital roots of the operands.

**Steps:**
1.  Consider an equation (e.g., A + B = C or A * B = C).
2.  Calculate the digital root of each operand (DR(A), DR(B)).
3.  Perform the same operation on these digital roots (e.g., DR(A) + DR(B) or DR(A) * DR(B)).
4.  Calculate the digital root of the result from step 3 (let's call it DR_Check).
5.  Calculate the digital root of the claimed result of the original operation (DR(C)).
6.  **Verification:** If `DR_Check == DR(C)`, the calculation is *likely* correct. If `DR_Check != DR(C)`, the calculation is **definitely incorrect**.

*   *See Example:* [[07.E02 - Checking Arithmetic using Digital Root Example]]

**Use Case in Exams (MCQs):**
If you perform a calculation and need to choose the correct answer from options, you can:
1.  Find the digital root of your calculated answer.
2.  Quickly find the digital roots of the MCQ options.
3.  Eliminate options whose digital roots do not match your answer's digital root.
4.  Alternatively, apply the casting out nines check to the proposed equation formed by the question and each option.

**Important Limitations:**
*   Casting out nines does **not** catch all errors. For example, it cannot detect transposition errors (e.g., writing 27 instead of 72) because they often have the same digital root.
*   It doesn't catch errors involving adding or removing 9s, or decimal point errors.
*   It's primarily a quick *check* or *elimination* tool, not a foolproof validation method. Use with caution for division.

---

**Related Concepts:**
*   [[01 - Divisibility Rules]] (Rule for 9 is directly based on this)
*   [[04 - Remainder Theorem]] (Digital root is essentially remainder modulo 9)