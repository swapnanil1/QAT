# 08 - Averages/03 - Weighted Average

# Weighted Average

**Definition:**

A weighted average (or weighted mean) is an average where some data points contribute more significantly ("weigh" more) than others towards the final average. Unlike a simple average [[08 - Averages/01 - Basic Average Formula.md]] where all observations have equal importance, in a weighted average, each observation is assigned a weight reflecting its relative importance or frequency.

**Formula:**

Let the observations (values) be `x1, x2, x3, ..., xn`.
Let their corresponding weights be `w1, w2, w3, ..., wn`.

The weighted average `Aw` is calculated as:
`Aw = (w1*x1 + w2*x2 + w3*x3 + ... + wn*xn) / (w1 + w2 + w3 + ... + wn)`

Or, using summation notation:
`Aw = (Σ(wi * xi)) / (Σwi)`

Where:
*   `xi` is the value of the i-th observation.
*   `wi` is the weight assigned to the i-th observation.
*   `Σ(wi * xi)` is the sum of the products of each observation and its weight.
*   `Σwi` is the sum of all the weights.

**Key Concepts:**

*   **Weights:** Represent the importance, frequency, or contribution of each observation. Weights must be non-negative, but they don't necessarily have to sum to 1 (though they can be normalized to do so). Higher weights give more influence to the corresponding observation.
*   **Simple Average as a Special Case:** If all weights are equal (e.g., `w1 = w2 = ... = wn = 1`), the weighted average formula reduces to the simple average formula.

**Applications:**

Weighted averages are used in various scenarios:

1.  **Academic Grades:** Calculating GPA where subjects have different credit hours (weights).
2.  **Financial Portfolios:** Calculating the average return of a portfolio where different assets have different investment amounts (weights).
3.  **Statistics:** Calculating the mean of a frequency distribution where values occur multiple times (frequencies act as weights).
4.  **Mixtures:** Finding the average price or property (e.g., concentration) of a mixture formed by combining items with different prices/properties and quantities (weights). See [[06 - Mixtures and Alligations/01 - Alligation Rule Concept.md]].
5.  **Average Speed:** Calculating average speed when different distances are covered at different speeds. The time taken for each part acts as the weight, or if distances are given, a harmonic mean approach (related to weighted average) might be needed. See [[11 - Time, Speed and Distance/02 - Average Speed Concepts.md]] and [[08 - Averages/03.E02 - Average Speed Calculation Example.md]].
6.  **Combined Groups:** Calculating the average of combined groups with different sizes (group sizes act as weights), as mentioned in [[08 - Averages/02 - Properties of Averages.md]].

**Related Concepts:**

*   [[08 - Averages/01 - Basic Average Formula.md]] (Simple Average)
*   [[06 - Mixtures and Alligations/01 - Alligation Rule Concept.md]] (Visual method often related to weighted averages)
*   [[11 - Time, Speed and Distance/02 - Average Speed Concepts.md]]

#quant #averages #weighted_average #formula #mean #statistics