# Basic Probability Terminology (Event, Sample Space, P(E))

Tags: #quant #probability #basic_concepts #event #sample_space #probability_formula #concept #terminology

---

**Introduction:**

Probability is the branch of mathematics concerning numerical descriptions of how likely an event is to occur. It quantifies uncertainty and is used extensively in various fields, including statistics, finance, science, and risk assessment. Understanding the basic terminology and the fundamental formula for calculating probability is the first step in solving probability-based quantitative aptitude questions.

**Basic Definitions:**

*   **Random Experiment:** An experiment or process for which the outcome cannot be predicted with certainty, but the set of all possible outcomes is known. Examples: Tossing a coin, rolling a die, drawing a card from a deck.
*   **Outcome:** A single possible result of a random experiment. Example: Getting 'Heads' when tossing a coin; rolling a '4' on a die.
*   **Sample Space (S):** The set of all possible outcomes of a random experiment. It is usually denoted by `S`.
    *   Example (Coin Toss): `S = {Head, Tail}`. The total number of outcomes, `n(S)`, is 2.
    *   Example (Die Roll): `S = {1, 2, 3, 4, 5, 6}`. `n(S) = 6`.
    *   Example (Two Coin Tosses): `S = {HH, HT, TH, TT}`. `n(S) = 4`.
*   **Event (E):** Any subset of the sample space `S`. It represents a specific outcome or a set of outcomes of interest.
    *   Example (Die Roll): Event 'Getting an even number', `E = {2, 4, 6}`. The number of outcomes favorable to the event, `n(E)`, is 3.
    *   Example (Two Coin Tosses): Event 'Getting at least one Head', `E = {HH, HT, TH}`. `n(E) = 3`.
*   **Impossible Event:** An event that cannot occur. It corresponds to the empty set (`{}`) and has a probability of 0. Example: Rolling a '7' on a standard six-sided die.
*   **Sure Event (Certain Event):** An event that is certain to occur. It corresponds to the entire sample space `S` and has a probability of 1. Example: Getting a number less than 7 when rolling a standard six-sided die.
*   **Equally Likely Outcomes:** Outcomes in a sample space that have the same chance of occurring. Example: Each face of a fair die has an equal probability (1/6) of appearing.

---

**Fundamental Probability Formula:**

If all outcomes in a sample space `S` are equally likely, then the probability of an event `E` occurring, denoted by `P(E)`, is calculated as:

`P(E) = (Number of outcomes favorable to E) / (Total number of possible outcomes in S)`

`P(E) = n(E) / n(S)`

**Key Properties:**

*   The probability of any event `E` is always between 0 and 1, inclusive: `0 <= P(E) <= 1`.
*   The probability of an impossible event is 0.
*   The probability of a sure event is 1.
*   **Complementary Event (Not E):** The event that `E` does not occur is denoted by `E'`, `Ē`, or `E^c`. Its probability is given by:
    `P(Not E) = P(E') = 1 - P(E)`
    Also, `P(E) + P(E') = 1`.

---

**General Approach & Strategy:**

1.  **Identify the Random Experiment:** Understand the process being described (e.g., rolling dice, drawing cards).
2.  **Determine the Sample Space (S):** List or count all possible outcomes. Ensure they are mutually exclusive and exhaustive. Counting techniques like [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md|combinations]] or [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md|permutations]] might be needed for complex sample spaces. `n(S)` is the total number of outcomes.
3.  **Identify the Event (E):** Clearly define the specific outcome(s) of interest.
4.  **Count Favorable Outcomes (n(E)):** List or count the outcomes within the sample space that satisfy the conditions of the event `E`. Again, combinatorics may be required.
5.  **Apply the Formula:** Calculate `P(E) = n(E) / n(S)`.
6.  **Simplify:** Express the probability as a fraction in its simplest form, or as a decimal or percentage if required.
7.  **Use Complement (if easier):** Sometimes, calculating the probability of the event *not* happening (`P(E')`) is easier. Then, find `P(E) = 1 - P(E')`. This is useful for "at least one" type problems.

---

**Examples:**

*   [[16 - Probability/01.E01 - Simple Probability (Coin Toss) Example.md]] (Illustrates calculating basic probability with a simple coin toss experiment)
*   [[16 - Probability/01.E02 - Simple Probability (Dice Roll) Example.md]] (Demonstrates calculating basic probability with a standard die roll)

---

**Related Concepts:**

*   [[15 - Permutations and Combinations/01 - Factorial Notation.md]], [[15 - Permutations and Combinations/02 - Permutation (Arrangement) Formula (nPr).md]], [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Combinatorics are essential tools for counting `n(S)` and `n(E)` in complex scenarios)
*   [[16 - Probability/02 - Probability Rules (Addition, Multiplication).md]] (Explains how to calculate probabilities for combined events, like 'A or B' or 'A and B')
*   [[16 - Probability/03 - Problems on Cards, Balls, etc.md]] (Applies these basic concepts to common probability problem types)
*   [[17 - Data Interpretation (DI)/01 - Tables Interpretation.md]], [[17 - Data Interpretation (DI)/02 - Bar Graphs Interpretation.md]], [[17 - Data Interpretation (DI)/03 - Line Graphs Interpretation.md]], [[17 - Data Interpretation (DI)/04 - Pie Charts Interpretation.md]] (DI often involves calculating probabilities based on the data presented)