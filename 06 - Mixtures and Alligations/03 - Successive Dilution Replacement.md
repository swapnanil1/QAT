# Successive Dilution / Replacement

#quant #mixtures_and_alligations #mixture_problems #successive_dilution #replacement #formula #percentage

## Concept

Successive dilution or replacement involves a process where a certain quantity of a mixture is removed and replaced with an equal quantity of another substance (often a diluent like water, or one of the original components). This operation is repeated multiple times (`n` times).

The key aspect is tracking how the quantity or concentration of one specific component (usually the original pure substance or a component of the initial mixture) changes over these repeated operations.

## Formula Derivation and Logic

Let's consider a vessel containing an initial quantity `Q` of a pure liquid (e.g., milk, wine) in a total volume `V`. (Often, initially `Q=V` if starting with a pure liquid).
Let `x` be the volume of the mixture removed in each step, which is then replaced by an equal volume of a diluent (e.g., water). The total volume `V` remains constant after each operation.

*   **Initial State:** Quantity of original liquid = `Q`. Total Volume = `V`.
*   **After 1st Operation:**
    *   Volume removed = `x`. Amount of original liquid removed = `Q * (x/V)`.
    *   Amount of original liquid remaining = `Q - Q * (x/V) = Q * (1 - x/V)`.
    *   `x` volume of diluent is added. Total volume remains `V`.
*   **After 2nd Operation:**
    *   Current amount of original liquid = `Q * (1 - x/V)`.
    *   Volume removed = `x`. Amount of original liquid removed in this step = `[Q * (1 - x/V)] * (x/V)`.
    *   Amount of original liquid remaining = `[Q * (1 - x/V)] - [Q * (1 - x/V)] * (x/V)`
    *   Factor out `Q * (1 - x/V)`: `Q * (1 - x/V) * [1 - x/V] = Q * (1 - x/V)^2`.
    *   `x` volume of diluent is added. Total volume remains `V`.
*   **After n Operations:**
    Following the pattern, the amount of the original liquid remaining after `n` such operations is given by:

## Formula

`Final Quantity = Initial Quantity * (1 - (Volume Removed / Total Volume))^n`

Where:
*   `Final Quantity` is the amount of the original liquid remaining after `n` operations.
*   `Initial Quantity` is the starting amount of the liquid being tracked.
*   `Volume Removed` (`x`) is the amount taken out *in each* operation.
*   `Total Volume` (`V`) is the total volume of the mixture in the container (usually constant).
*   `n` is the number of times the operation (removal and replacement) is performed.

**Alternative Form:** If the mixture initially contains `Q` amount of component A in Total Volume `V`, and `x` litres are removed and replaced `n` times:
`Final Amount of A = Initial Amount of A * ( (V - x) / V )^n`
This is the same formula, just written slightly differently: `(1 - x/V) = (V - x) / V`.

## Key Points

*   This formula calculates the quantity of the **original substance** remaining. If you need the quantity of the substance added (like water), subtract the final quantity of the original substance from the total volume.
*   Ensure `x` and `V` are in the same units.
*   This applies when the replacement liquid does *not* contain the substance being tracked (e.g., replacing wine with water when tracking the amount of wine).
*   The total volume `V` typically remains constant throughout the process.

## Related Concepts

*   [[06 - Mixtures and Alligations/02 - Mixture Problems (Adding Removing).md]] (Builds upon the removal concept)
*   [[02 - Percentages/03 - Successive Percentage Change.md]] (Similar concept of repeated reduction, but applied multiplicatively)
*   [[05 - Ratio and Proportion/01 - Ratio Concepts (Duplicate, Triplicate, etc).md]]
*   [[12 - Algebra/04 - Indices and Surds.md]] (Dealing with powers in the formula)