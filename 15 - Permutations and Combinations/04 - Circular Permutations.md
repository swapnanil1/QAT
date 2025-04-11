# Circular Permutations

Tags: #quant #permutations_and_combinations #permutation #circular_permutation #arrangement #concept #formula #factorial

---

**Introduction:**

Circular permutations deal with arranging objects around a fixed circle (like people around a table or beads on a necklace). Unlike linear permutations [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md|which arrange items in a row]], circular arrangements have no fixed starting or ending point. Rotating the entire arrangement doesn't create a new distinct permutation. This difference requires a modified formula derived from linear permutations.

**Definition and Formula:**

**Case 1: Distinct Objects around a Circle (Clockwise/Anticlockwise are different)**

The number of ways to arrange `n` distinct objects around a fixed circle is given by:

`(n - 1)!`

**Reasoning:**
In a linear arrangement, there are `n!` ways. However, in a circle, arrangements like ABCD, BCDA, CDAB, DABC are considered the same because they can be obtained by rotating the circle. For every distinct circular arrangement, there are `n` corresponding linear arrangements. Therefore, we divide the total linear permutations (`n!`) by `n` to account for these rotations:
`n! / n = (n * (n-1)!) / n = (n - 1)!`

**Case 2: Objects like Beads/Keys on a String/Ring (Clockwise/Anticlockwise are the same)**

When the arrangement can be flipped over (like a necklace or keychain) without changing the arrangement, the clockwise and anticlockwise arrangements are considered identical. In this case, we divide the result from Case 1 by 2.

The number of ways to arrange `n` distinct objects in a circular manner where clockwise and anticlockwise arrangements are considered the same is:

`(n - 1)! / 2` (for `n > 2`)

**Note:** This second case is less common in typical aptitude tests compared to the first (people around a table). Always assume Case 1 unless the problem explicitly mentions flipping or symmetrical equivalence (like beads on a necklace).

---

**Key Concepts:**

*   **Relative Position:** What matters in circular permutations is the relative position of objects to each other, not their absolute position (as there's no start/end).
*   **Fixing One Position:** The `(n-1)!` formula can be understood by fixing the position of one object. Once one object is fixed, the problem reduces to arranging the remaining `(n-1)` objects in the remaining `(n-1)` linear spots relative to the fixed object, which can be done in `(n-1)!` ways.
*   **Distinction from Linear:** Always differentiate between arranging items in a line (`n!`) and arranging them in a circle (`(n-1)!`).

---

**General Approach & Strategy:**

1.  **Identify Circular Arrangement:** Confirm the problem involves arranging items in a circle.
2.  **Check for Distinct Objects:** The basic formulas assume distinct objects. (Constraints might apply, similar to linear permutations).
3.  **Determine if Clockwise/Anticlockwise Matter:**
    *   People around a table, seating arrangements: Clockwise is usually distinct from anticlockwise. Use `(n - 1)!`.
    *   Beads on a necklace, keys on a ring: Clockwise/Anticlockwise might be considered the same. Use `(n - 1)! / 2`. (Read the problem carefully).
4.  **Apply Formula:** Substitute the number of distinct objects (`n`) into the appropriate formula.
5.  **Handle Constraints:** If there are constraints (e.g., certain people must sit together, or no two people sit together), adapt the strategies used for linear permutations (grouping, gap method) but apply them to the circular arrangement logic. For example, if 2 people must sit together, treat them as one block, arrange `(n-1)` units circularly in `(n-1-1)! = (n-2)!` ways, and then arrange the 2 people within the block in `2!` ways. Total = `(n-2)! * 2!`.

---

**Examples:**

*   [[15 - Permutations and Combinations/04.E01 - Arranging People around Table Example.md]] (Illustrates the basic circular permutation formula and arrangements with constraints)

---

**Related Concepts:**

*   [[15 - Permutations and Combinations/01 - Factorial Notation.md]] (Foundation for calculating the results)
*   [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md]] (Highlights the difference between linear and circular arrangements)
*   [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Selection concepts might be combined, e.g., selecting a group *then* arranging them circularly)