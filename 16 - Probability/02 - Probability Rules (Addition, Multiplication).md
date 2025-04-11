# Probability Rules (Addition, Multiplication)

Tags: #quant #probability #probability_rules #addition_rule #multiplication_rule #mutually_exclusive #independent_events #conditional_probability #concept #formula

---

**Introduction:**

While the basic formula `P(E) = n(E) / n(S)` (from [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md|basic probability concepts]]) works for single events, we often need to calculate the probability of combinations of events, such as the probability of event A *or* event B occurring, or the probability of event A *and* event B occurring. The Addition and Multiplication rules provide the framework for these calculations.

---

**1. Addition Rule (Probability of 'A or B')**

The Addition Rule is used to find the probability that either event A *or* event B (or both) occurs. The specific formula depends on whether the events are mutually exclusive.

*   **Mutually Exclusive Events:** Two events are mutually exclusive if they cannot occur at the same time (i.e., they have no outcomes in common; their intersection is empty).
    *   Example: Rolling a '1' and rolling a '6' on a single die roll.
    *   **Formula:** `P(A or B) = P(A U B) = P(A) + P(B)`

*   **Non-Mutually Exclusive Events (Inclusive Events):** Events that can occur at the same time (i.e., they have one or more outcomes in common; their intersection is not empty).
    *   Example: Drawing a 'King' and drawing a 'Heart' from a deck of cards (the King of Hearts is common).
    *   **General Formula:** `P(A or B) = P(A U B) = P(A) + P(B) - P(A and B)`
        *   `P(A and B)` or `P(A ∩ B)` is the probability that *both* A and B occur. Subtracting it prevents double-counting the common outcomes.
        *   Note: This general formula also works for mutually exclusive events because if A and B are mutually exclusive, `P(A and B) = 0`, and the formula reduces to `P(A) + P(B)`.

---

**2. Multiplication Rule (Probability of 'A and B')**

The Multiplication Rule is used to find the probability that both event A *and* event B occur. The specific formula depends on whether the events are independent.

*   **Independent Events:** Two events are independent if the occurrence of one event does not affect the probability of the other event occurring.
    *   Example: Tossing a coin twice; the outcome of the first toss does not influence the outcome of the second toss. Rolling a die and tossing a coin.
    *   **Formula:** `P(A and B) = P(A ∩ B) = P(A) * P(B)`

*   **Dependent Events:** Two events are dependent if the occurrence of one event *does* affect the probability of the other event occurring.
    *   Example: Drawing two cards from a deck *without replacement*; the outcome of the first draw changes the probabilities for the second draw.
    *   **General Formula:** `P(A and B) = P(A ∩ B) = P(A) * P(B|A)`
        *   `P(B|A)` is the **conditional probability** of event B occurring *given that* event A has already occurred.

---

**3. Conditional Probability (Probability of 'B given A')**

Conditional probability `P(B|A)` is the probability of event B happening, knowing that event A has already happened.

*   **Formula:** `P(B|A) = P(A and B) / P(A)` (provided `P(A) > 0`)

This formula can be rearranged to give the general multiplication rule: `P(A and B) = P(A) * P(B|A)`.

*   **For Independent Events:** If A and B are independent, then `P(B|A) = P(B)` (knowing A happened doesn't change B's probability). Substituting this into the conditional probability formula yields `P(A and B) / P(A) = P(B)`, which rearranges to `P(A and B) = P(A) * P(B)`, the multiplication rule for independent events.

---

**General Approach & Strategy:**

1.  **Identify Events:** Clearly define the events A and B involved in the problem.
2.  **Determine the Conjunction:** Are you looking for `P(A or B)` or `P(A and B)`?
3.  **Check Exclusivity/Independence:**
    *   If 'OR': Are A and B mutually exclusive? (Can they happen together?) Use the appropriate Addition Rule.
    *   If 'AND': Are A and B independent? (Does one affect the other?) Use the appropriate Multiplication Rule. Consider if conditional probability is needed.
4.  **Calculate Individual Probabilities:** Determine `P(A)`, `P(B)`, and potentially `P(A and B)` or `P(B|A)` based on the problem context, often using concepts from [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md|basic probability]].
5.  **Apply the Correct Rule:** Substitute the calculated probabilities into the chosen rule formula.
6.  **Calculate Result:** Compute the final probability.

---

**Examples:**

*   [[16 - Probability/02.E01 - Probability of 'A or B' (Mutually Exclusive) Example.md]] (Illustrates the Addition Rule for events that cannot happen together)
*   [[16 - Probability/02.E02 - Probability of 'A or B' (Not Mutually Exclusive) Example.md]] (Demonstrates the general Addition Rule when events overlap)
*   [[16 - Probability/02.E03 - Probability of 'A and B' (Independent) Example.md]] (Shows the Multiplication Rule for independent events)
*   *(Dependent event examples often fall under specific problem types, e.g., drawing cards without replacement, covered in [[16 - Probability/03 - Problems on Cards, Balls, etc.md]])*

---

**Related Concepts:**

*   [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md]] (Provides the foundation for calculating individual probabilities P(A) and P(B))
*   [[16 - Probability/03 - Problems on Cards, Balls, etc.md]] (Applies these rules frequently in standard probability scenarios)
*   [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Often needed to calculate `n(E)` and `n(S)` for determining individual probabilities before applying rules)
*   [[17 - Data Interpretation (DI)/01 - Tables Interpretation.md]] etc. (DI problems may require applying these rules to data, e.g., probability of selecting someone who meets condition A or condition B)