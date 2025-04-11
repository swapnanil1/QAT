# 08 - Averages/02 - Properties of Averages

# Properties of Averages

Understanding the properties of averages (arithmetic mean) can significantly simplify calculations and problem-solving.

**Key Properties:**

1.  **Effect of Adding/Subtracting a Constant:**
    *   If each observation in a dataset is increased by a constant value `k`, the average of the new dataset also increases by `k`.
    *   If each observation in a dataset is decreased by a constant value `k`, the average of the new dataset also decreases by `k`.
    *   **Example:** If the average score of 10 students is 75, and each student gets 5 bonus marks, the new average will be 75 + 5 = 80.
    *   **See Example:** [[08 - Averages/02.E02 - Effect of Multiplying Dividing Each Value Example.md]] (although named for multiplication/division, the concept is related and will be illustrated there too)

2.  **Effect of Multiplying/Dividing by a Constant:**
    *   If each observation in a dataset is multiplied by a non-zero constant `k`, the average of the new dataset is also multiplied by `k`.
    *   If each observation in a dataset is divided by a non-zero constant `k`, the average of the new dataset is also divided by `k`.
    *   **Example:** If the average monthly saving of 5 employees is Rs. 2000, and everyone's saving doubles next month, the new average saving will be 2000 * 2 = Rs. 4000.
    *   **See Example:** [[08 - Averages/02.E02 - Effect of Multiplying Dividing Each Value Example.md]]

3.  **Sum of Deviations:**
    *   The sum of the deviations of each observation from the average is always zero.
    *   Let `A` be the average of observations `x1, x2, ..., xn`. Then `(x1 - A) + (x2 - A) + ... + (xn - A) = 0`.
    *   This property is useful in checking calculations and understanding the balancing nature of the mean.

4.  **Average Lies Between Minimum and Maximum:**
    *   The average of a dataset always lies between the smallest (minimum) and the largest (maximum) observation in the dataset.
    *   `Minimum Value <= Average <= Maximum Value`.
    *   The average can be equal to the minimum or maximum only if all observations are identical.

5.  **Effect of Adding/Removing Observations:**
    *   If a new observation added to the group has a value **greater** than the original average, the new average will **increase**.
    *   If a new observation added has a value **less** than the original average, the new average will **decrease**.
    *   If a new observation added has a value **equal** to the original average, the new average will **remain unchanged**.
    *   The reverse applies when removing observations. Removing a value greater than the average decreases the new average, and removing a value less than the average increases the new average.
    *   **See Example:** [[08 - Averages/02.E01 - Effect of Adding Removing Value Example.md]]

6.  **Average of Combined Groups:**
    *   If two groups have averages `A1` and `A2` and counts `n1` and `n2` respectively, the combined average is *not* simply `(A1 + A2) / 2` unless `n1 = n2`.
    *   The combined average is calculated using the [[08 - Averages/03 - Weighted Average.md]] concept:
        `Combined Average = (n1*A1 + n2*A2) / (n1 + n2)`

**Related Concepts:**

*   [[08 - Averages/01 - Basic Average Formula.md]]
*   [[08 - Averages/03 - Weighted Average.md]]
*   [[08 - Averages/04 - Problems on Ages, Runs, etc.md]] (Many age/run problems involve adding/removing members/innings)

#quant #averages #properties_of_average #arithmetic_mean #mean #shortcut