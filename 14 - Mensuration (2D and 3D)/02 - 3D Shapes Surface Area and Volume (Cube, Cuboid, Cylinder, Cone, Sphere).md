# 3D Shapes Surface Area and Volume (Cube, Cuboid, Cylinder, Cone, Sphere)

Tags: #quant #mensuration_2d_and_3d #3d_shapes_surface_area_volume #formula #cube #cuboid #cylinder #cone #sphere #concept

---

**Introduction:**

This section extends mensuration concepts from 2D shapes to 3D objects (solids). For 3D shapes, the key measurements are Surface Area (the total area of all surfaces) and Volume (the amount of space the object occupies). Understanding these formulas is crucial for solving various quantitative problems involving solid geometry.

**Basic Definitions:**

*   **Surface Area (SA):** The total area of the outer surface of a 3D object. It's measured in square units (e.g., cm², m²).
    *   **Lateral Surface Area (LSA) / Curved Surface Area (CSA):** The area of the surfaces excluding the top and bottom bases (applicable to shapes like cylinders, cones).
    *   **Total Surface Area (TSA):** The area of all surfaces, including bases.
*   **Volume (V):** The measure of the three-dimensional space enclosed by the boundary of a 3D object. It's measured in cubic units (e.g., cm³, m³).

---

**Formulas & Properties by Shape:**

**1. Cube**

*   A solid with six equal square faces. All edges (side length `a`) are equal.
*   **(Imagine a standard dice shape)**
*   **Lateral Surface Area (LSA):** Area of 4 side faces. `LSA = 4 * a^2`
*   **Total Surface Area (TSA):** Area of all 6 faces. `TSA = 6 * a^2`
*   **Volume (V):** `V = a^3`
*   **Length of Diagonal (Space Diagonal):** Connects opposite vertices through the interior. `Diagonal = a * sqrt(3)`

**2. Cuboid (Rectangular Parallelepiped)**

*   A solid with six rectangular faces. Opposite faces are equal. Edges are length (`l`), breadth (`b`), height (`h`).
*   **(Imagine a rectangular box, like a brick)**
*   **Lateral Surface Area (LSA):** Area of 4 side faces (walls). `LSA = 2 * (l + b) * h`
*   **Total Surface Area (TSA):** Area of all 6 faces. `TSA = 2 * (lb + bh + lh)`
*   **Volume (V):** `V = l * b * h`
*   **Length of Diagonal (Space Diagonal):** `Diagonal = sqrt(l^2 + b^2 + h^2)` (derived using [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md|Pythagoras theorem twice]]).

**3. Cylinder (Right Circular Cylinder)**

*   A solid with two parallel circular bases connected by a curved surface. Radius (`r`), height (`h`).
*   **(Imagine a standard can)**
*   **Curved Surface Area (CSA) / Lateral Surface Area (LSA):** Area of the curved surface. `CSA = 2 * pi * r * h`
*   **Total Surface Area (TSA):** CSA + Area of two circular bases (`pi * r^2` each). `TSA = 2 * pi * r * h + 2 * pi * r^2` or `TSA = 2 * pi * r * (h + r)`
*   **Volume (V):** Area of base * height. `V = pi * r^2 * h`

**4. Cone (Right Circular Cone)**

*   A solid with a circular base and a vertex, connected by a curved surface. Radius (`r`), height (`h`), slant height (`l`).
*   **(Imagine an ice cream cone)**
*   **Slant Height (l):** The distance from the vertex to any point on the circumference of the base. `l = sqrt(r^2 + h^2)` (derived using [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md|Pythagoras theorem]]).
*   **Curved Surface Area (CSA) / Lateral Surface Area (LSA):** Area of the curved surface. `CSA = pi * r * l`
*   **Total Surface Area (TSA):** CSA + Area of the circular base (`pi * r^2`). `TSA = pi * r * l + pi * r^2` or `TSA = pi * r * (l + r)`
*   **Volume (V):** One-third the volume of a cylinder with the same base and height. `V = (1/3) * pi * r^2 * h`

**5. Sphere**

*   A perfectly round geometric object in 3D space; set of points equidistant (radius `r`) from a center.
*   **(Imagine a ball)**
*   **Surface Area (SA) (Total):** `SA = 4 * pi * r^2` (There's no distinction between lateral and total for a sphere).
*   **Volume (V):** `V = (4/3) * pi * r^3`
*   **Hemisphere (Half-sphere):**
    *   Curved Surface Area (CSA): `CSA = 2 * pi * r^2`
    *   Total Surface Area (TSA): CSA + Area of circular base. `TSA = 2 * pi * r^2 + pi * r^2 = 3 * pi * r^2`
    *   Volume (V): `V = (2/3) * pi * r^3`

---

**Key Considerations & Tips:**

*   **Units:** Be extremely careful with units. If dimensions are in cm, SA/LSA/CSA will be in cm², and Volume will be in cm³. Mismatched units require conversion (e.g., using principles from [[11 - Time, Speed and Distance/01 - Basic Formula (D=S T) and Unit Conversions.md|unit conversion concepts]]). Pay attention to volume unit conversions (e.g., liters to cm³ or m³: 1 liter = 1000 cm³; 1 m³ = 1000 liters).
*   **Formula Memorization:** Accurate recall of these formulas is essential. Use flashcards or practice writing them.
*   **Distinguish LSA/CSA vs TSA:** Read the question carefully to determine if the bases are included in the required area.
*   **Slant Height (Cone):** Remember that the cone formulas often use slant height (`l`), which might need to be calculated first using `l = sqrt(r^2 + h^2)` if `r` and `h` are given.
*   **Combined/Modified Solids:** Problems may involve objects made by combining shapes (e.g., cone on a cylinder) or removing parts (e.g., drilling a conical hole in a cube). Calculate volumes/areas of individual parts and add/subtract as needed.
*   **Melting/Recasting:** When one solid shape is melted and recast into another shape (or multiple smaller shapes), the **Volume remains constant**. Equate the volume formulas.
*   **Visualization:** Try to visualize the 3D shape described in the problem. Sketching can help identify the relevant dimensions and surfaces.

---

**Examples:**

*   [[14 - Mensuration (2D and 3D)/02.E01 - Volume of Cuboid Example.md]] (Illustrates calculating cuboid volume and related quantities)
*   [[14 - Mensuration (2D and 3D)/02.E02 - Surface Area of Cylinder Example.md]] (Demonstrates calculating cylinder surface area)
*   [[14 - Mensuration (2D and 3D)/02.E03 - Volume of Cone Example.md]] (Shows calculation involving cone volume and slant height)
*   [[14 - Mensuration (2D and 3D)/02.E04 - Surface Area Volume of Sphere Example.md]] (Covers calculations for sphere surface area and volume)

---

**Related Concepts:**

*   [[14 - Mensuration (2D and 3D)/01 - 2D Shapes Area and Perimeter (Triangle, Square, Rectangle, Circle).md]] (Foundation for understanding faces and bases of 3D shapes)
*   [[13 - Geometry/02 - Triangles (Properties, Congruence, Similarity).md]] (Pythagoras theorem is crucial for diagonals and slant height)
*   [[12 - Algebra/01 - Basic Algebraic Identities.md]] & [[12 - Algebra/02 - Linear Equations (One Two Variables).md]] (Often needed to solve for unknown dimensions)
*   [[02 - Percentages/02 - Percentage Increase and Decrease.md]] (Problems might involve percentage changes in dimensions affecting volume/SA)
*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]] (Ratios of dimensions, areas, and volumes)