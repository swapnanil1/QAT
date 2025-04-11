# Triangles (Properties, Congruence, Similarity)

Tags: #quant #geometry #triangles #properties #congruence #similarity #concept #formula #angle_sum #triangle_inequality #pythagoras

---

**Introduction:**

A triangle is a fundamental geometric shape, a polygon with three sides and three angles (vertices). Triangles are ubiquitous in geometry problems, and understanding their properties, classifications, and relationships (congruence and similarity) is essential for solving a wide range of quantitative aptitude questions.

**Classification of Triangles:**

**Based on Sides:**

1.  **Equilateral Triangle:** All three sides are equal in length. All three angles are equal (each 60°).
2.  **Isosceles Triangle:** At least two sides are equal in length. The angles opposite the equal sides are also equal.
3.  **Scalene Triangle:** All three sides have different lengths. All three angles have different measures.

**Based on Angles:**

1.  **Acute-angled Triangle:** All three angles are acute (less than 90°).
2.  **Right-angled Triangle:** One angle is exactly 90°. The side opposite the right angle is the hypotenuse (longest side). The other two sides are legs. The Pythagorean theorem applies: `(Hypotenuse)^2 = (Leg1)^2 + (Leg2)^2`.
3.  **Obtuse-angled Triangle:** One angle is obtuse (greater than 90°).

**Basic Properties:**

1.  **Angle Sum Property:** The sum of the three interior angles of any triangle is always 180°.
2.  **Exterior Angle Property:** An exterior angle of a triangle is equal to the sum of the two opposite interior angles.
3.  **Triangle Inequality Theorem:** The sum of the lengths of any two sides of a triangle must be greater than the length of the third side. (e.g., `a + b > c`, `a + c > b`, `b + c > a`). The difference between any two sides must be less than the third side.
4.  **Side-Angle Relationship:** The side opposite the largest angle is the longest side, and the side opposite the smallest angle is the shortest side. Conversely, the angle opposite the longest side is the largest angle.

**Congruence of Triangles:**

*   **Definition:** Two triangles are congruent if they have the exact same shape and size. All corresponding sides and corresponding angles are equal. Symbol: `≅`.
*   **Criteria for Congruence:** (Conditions to prove congruence without checking all 6 parts)
    *   **SSS (Side-Side-Side):** If three sides of one triangle are equal to the three corresponding sides of another triangle.
    *   **SAS (Side-Angle-Side):** If two sides and the included angle (the angle between those two sides) of one triangle are equal to the corresponding parts of another triangle.
    *   **ASA (Angle-Side-Angle):** If two angles and the included side (the side between those two angles) of one triangle are equal to the corresponding parts of another triangle.
    *   **AAS (Angle-Angle-Side):** If two angles and a non-included side of one triangle are equal to the corresponding parts of another triangle.
    *   **RHS (Right angle-Hypotenuse-Side):** For right-angled triangles only. If the hypotenuse and one leg of one right triangle are equal to the hypotenuse and corresponding leg of another right triangle.
*   **CPCTC:** Corresponding Parts of Congruent Triangles are Congruent (or Equal). Once congruence is proven, we can state that all other corresponding parts are equal.

**Similarity of Triangles:**

*   **Definition:** Two triangles are similar if they have the same shape but not necessarily the same size. Corresponding angles are equal, and corresponding sides are in proportion (have the same ratio). Symbol: `~`.
*   **Criteria for Similarity:**
    *   **AAA (Angle-Angle-Angle):** If all three angles of one triangle are equal to the three corresponding angles of another triangle. (Implies AA)
    *   **AA (Angle-Angle):** If two angles of one triangle are equal to the two corresponding angles of another triangle (the third angles must also be equal due to the 180° sum). This is the most commonly used criterion.
    *   **SAS (Side-Angle-Side Similarity):** If two sides of one triangle are proportional to two corresponding sides of another triangle, and the included angles are equal.
    *   **SSS (Side-Side-Side Similarity):** If all three sides of one triangle are proportional to the three corresponding sides of another triangle.
*   **Properties of Similar Triangles:** If two triangles are similar with a ratio of corresponding sides `k`:
    *   Ratio of Perimeters = `k`
    *   Ratio of Areas = `k^2`
    *   Ratio of corresponding altitudes, medians, angle bisectors = `k`

**General Approach:**

1.  **Identify Given Information:** Note side lengths, angle measures, parallel lines ([[13 - Geometry/01 - Lines and Angles.md]]), or relationships mentioned.
2.  **Apply Basic Properties:** Use angle sum, exterior angle, or triangle inequality properties.
3.  **Look for Special Triangles:** Check if it's equilateral, isosceles, or right-angled. Apply relevant properties (e.g., Pythagoras for right triangles).
4.  **Check for Congruence/Similarity:** Determine if congruence or similarity criteria can be applied to relate triangles or find missing information.
5.  **Deduce and Solve:** Combine properties and relationships to find unknown sides or angles, often involving [[12 - Algebra/02 - Linear Equations (One Two Variables).md|Algebraic equations]].

**Examples:**
*   [[13 - Geometry/02.E01 - Angle Sum Property Example.md]]
*   [[13 - Geometry/02.E02 - Pythagoras Theorem Example.md]]
*   [[13 - Geometry/02.E03 - Similar Triangles Properties Example.md]]

**Related Concepts:**
*   [[13 - Geometry/01 - Lines and Angles.md]] (Foundation for angle relationships within triangles)
*   [[14 - Mensuration (2D and 3D)/01 - 2D Shapes Area and Perimeter (Triangle, Square, Rectangle, Circle).md]] (Calculating area and perimeter)
*   [[13 - Geometry/03 - Quadrilaterals (Properties).md]] (Often broken down into triangles)
*   Trigonometry (Uses triangle ratios - Sine, Cosine, Tangent)