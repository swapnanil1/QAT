# 2D Shapes Area and Perimeter (Triangle, Square, Rectangle, Circle)

Tags: #quant #mensuration_2d_and_3d #2d_shapes_area_perimeter #formula #triangle #square #rectangle #circle #concept

---

**Introduction:**

Mensuration is the branch of geometry dealing with the measurement of lengths, areas, and volumes of geometric figures. This section focuses on 2D (planar) shapes, specifically calculating their Perimeter (the distance around the boundary) and Area (the space enclosed within the boundary). We will cover the fundamental formulas for common shapes like triangles, squares, rectangles, and circles, which form the basis for many quantitative aptitude problems.

**Basic Definitions:**

*   **Perimeter:** The total length of the boundary of a closed 2D figure. It's measured in linear units (e.g., meters, cm).
*   **Area:** The measure of the surface enclosed by the boundary of a closed 2D figure. It's measured in square units (e.g., square meters (m²), cm²).

---

**Formulas & Properties by Shape:**

**1. Triangle**

*   A polygon with three sides and three angles. (See [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md|basic triangle geometric properties here]]).
*   **Perimeter (P):** Sum of the lengths of the three sides (`a`, `b`, `c`).
    `P = a + b + c`
*   **Area (A):**
    *   General Formula (Base `b`, Height `h`): `A = 1/2 * b * h` (Height must be perpendicular to the base).
    *   Heron's Formula (Sides `a`, `b`, `c` known): Calculate semi-perimeter `s = (a + b + c) / 2`, then `A = sqrt(s * (s - a) * (s - b) * (s - c))`.
    *   Equilateral Triangle (Side `a`): `A = (sqrt(3) / 4) * a^2`

**2. Square**

*   A quadrilateral with four equal sides (`s`) and four right angles. (See [[13 - Geometry/03 - Quadrilaterals (Properties).md|basic quadrilateral geometric properties here]]).
*   **Perimeter (P):** `P = 4 * s`
*   **Area (A):** `A = s^2`
*   **Diagonal (d):** `d = s * sqrt(2)`. Also, `A = d^2 / 2`.

**3. Rectangle**

*   A quadrilateral with opposite sides equal (length `l`, breadth `b`) and four right angles. (See [[13 - Geometry/03 - Quadrilaterals (Properties).md|basic quadrilateral geometric properties here]]).
*   **Perimeter (P):** `P = 2 * (l + b)`
*   **Area (A):** `A = l * b`
*   **Diagonal (d):** `d = sqrt(l^2 + b^2)` (Derived using [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md|Pythagoras theorem learned for triangles]]).

**4. Circle**

*   Set of points equidistant (radius `r`) from a center. (See [[13 - Geometry/04 - Circles (Properties, Tangents, Chords).md|basic circle geometric properties here]]).
*   Diameter `d = 2 * r`. Pi (`pi`) ≈ 22/7 or 3.14.
*   **Circumference (C) (Perimeter):** `C = 2 * pi * r` or `C = pi * d`
*   **Area (A):** `A = pi * r^2`

---

**Key Considerations & Tips:**

*   **Units Consistency:** Always ensure lengths are in the same unit *before* calculation. Area units will be the square of the length unit (e.g., cm vs cm²). Be mindful of conversions, similar to those detailed in [[11 - Time, Speed and Distance/01 - Basic Formula (D=S T) and Unit Conversions.md|unit conversions for speed/distance problems]].
*   **Formula Choice:** Select the correct triangle area formula based on given info (sides vs base/height).
*   **Visualization:** Sketching the shape helps identify dimensions and relationships.
*   **Combined Figures:** Problems might combine shapes (e.g., rectangle with semicircles). Break down into standard components, calculate separately, then add/subtract areas/perimeters as required.
*   **Relationships:** Be ready for problems linking perimeter and area (e.g., find area given perimeter, or find the side length difference given area and perimeter).

---

**Examples:**

*   [[14 - Mensuration (2D and 3D)/01.E01 - Area of Triangle Example.md]] (Illustrates applying Heron's formula for triangle area)
*   [[14 - Mensuration (2D and 3D)/01.E02 - Area Circumference of Circle Example.md]] (Demonstrates calculating circle area and circumference)
*   [[14 - Mensuration (2D and 3D)/01.E03 - Area of Rectangle Example.md]] (Shows calculation of rectangle area and related parameters)

---

**Related Concepts:**

*   [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md]] (Provides foundational geometric properties of triangles used in area calculations, like height and Pythagoras)
*   [[13 - Geometry/03 - Quadrilaterals (Properties).md]] (Details properties of squares and rectangles relevant for perimeter/area formulas)
*   [[13 - Geometry/04 - Circles (Properties, Tangents, Chords).md]] (Explains fundamental geometric properties of circles relevant for area/circumference)
*   [[11 - Time, Speed and Distance/01 - Basic Formula (D=S T) and Unit Conversions.md]] (Explains unit conversion principles applicable here, e.g., cm to m)
*   [[14 - Mensuration (2D and 3D)/02 - 3D Shapes Surface Area and Volume (Cube, Cuboid, Cylinder, Cone, Sphere).md]] (The next logical step, extending mensuration concepts to 3D objects)