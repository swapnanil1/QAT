# Problems on Cards, Balls, Dice, and Coins

Tags: #quant #probability #probability_rules #cards #balls_urn #dice #coins #combinatorics #concept #application

---

**Introduction:**

Many quantitative aptitude probability questions revolve around standard scenarios involving drawing cards from a deck, selecting balls from bags/urns, rolling dice, or tossing coins. While the fundamental principles remain the same (using definitions from [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md|basic probability]] and rules from [[16 - Probability/02 - Probability Rules (Addition, Multiplication).md|probability rules]]), mastering the specific nuances and counting techniques for each scenario is key to solving problems efficiently.

---

**Common Scenarios and Approaches:**

**1. Problems on Playing Cards**

*   **Standard Deck:** Assumed unless otherwise stated: 52 cards, 4 suits (Hearts ♥, Diamonds ♦, Clubs ♣, Spades ♠), 13 ranks (A, 2-10, J, Q, K). Hearts/Diamonds are Red, Clubs/Spades are Black (26 each). 12 Face cards (J, Q, K of each suit). 4 Aces.
*   **Calculating n(S):** Often involves selecting `r` cards from 52. Use combinations ([[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md|nCr formula]]) as order of drawing usually doesn't matter for the final hand. Example: Drawing 2 cards from 52, `n(S) = 52C2`.
*   **Calculating n(E):** Define the event (e.g., getting 2 Kings). Count favorable outcomes using combinations based on the available cards matching the criteria. Example: Getting 2 Kings from 4 available Kings, `n(E) = 4C2`.
*   **'Without Replacement':** Most card problems imply drawing without replacement, making subsequent draws dependent events. The multiplication rule for dependent events (`P(A and B) = P(A) * P(B|A)`) is often applicable if considering sequential draws. For selecting a *hand* simultaneously, using combinations (`nCr`) is usually more direct.

**2. Problems on Balls in Bags/Urns**

*   **Setup:** Typically involves a bag containing balls of different colors. Balls of the same color are usually considered identical for selection purposes but distinct when calculating probabilities (imagine tiny numbers on them).
*   **Calculating n(S):** Similar to cards, selecting `r` balls from a total of `N` balls involves combinations: `n(S) = NC`r.
*   **Calculating n(E):** Use combinations based on the constraints. Example: Bag has 5 Red, 3 Blue balls. Event: Draw 2 Red balls when drawing 2 total. `n(E) = 5C2` (ways to choose 2 Red from 5). `n(S) = 8C2` (ways to choose any 2 from 8). `P(E) = 5C2 / 8C2`.
*   **'AND'/'OR' Constraints:** Combine combinations using the multiplication principle (for 'AND') or addition (for 'OR'). Example: Draw 1 Red AND 2 Blue. `n(E) = (Ways to choose 1 Red) * (Ways to choose 2 Blue) = 5C1 * 3C2`.

**3. Problems on Dice**

*   **Single Die:** Sample Space `S = {1, 2, 3, 4, 5, 6}`. `n(S)=6`. (Covered in [[16 - Probability/01.E02 - Simple Probability (Dice Roll) Example.md|single die example]])
*   **Two Dice:** Sample Space consists of pairs `(x, y)` where `x` is the result of the first die, `y` of the second. `S = {(1,1), (1,2), ..., (6,6)}`. `n(S) = 6 * 6 = 36`.
*   **Calculating n(E):** Often involves the sum, difference, or specific combination of outcomes on the dice. List the favorable pairs systematically. Example: Event 'Sum is 8'. `E = {(2,6), (3,5), (4,4), (5,3), (6,2)}`. `n(E)=5`. `P(E) = 5/36`.
*   **Three or More Dice:** `n(S) = 6^k` where `k` is the number of dice. Listing outcomes becomes tedious; combinatorics or pattern recognition is needed.

**4. Problems on Coins**

*   **Single Coin:** `S = {H, T}`, `n(S)=2`.
*   **Multiple Coins:** For `k` coins tossed simultaneously (or one coin tossed `k` times), `n(S) = 2^k`. Outcomes are sequences like HTH, TTT etc. (Covered in [[16 - Probability/01.E01 - Simple Probability (Coin Toss) Example.md|two coin example]])
*   **Calculating n(E):** Often involves counting outcomes with a specific number of Heads/Tails. Use combinations. Example: Toss 5 coins. Event 'Exactly 3 Heads'. This is equivalent to choosing *which* 3 tosses out of 5 will be Heads. `n(E) = 5C3 = 10`. `n(S) = 2^5 = 32`. `P(E) = 10/32 = 5/16`.

---

**General Strategy Revisited:**

1.  **Understand the Setup:** Know the composition (deck of cards, number/color of balls, faces of dice, fair coins).
2.  **Determine n(S):** Calculate the total number of possible outcomes, often using `n^k` (for dice/coins) or `NCr` (for cards/balls).
3.  **Define the Event E:** Translate the worded requirement into a specific condition on the outcomes.
4.  **Determine n(E):** Calculate the number of outcomes satisfying the event condition, typically using combinations (`nCr`) and multiplication/addition principles for complex events.
5.  **Calculate Probability:** `P(E) = n(E) / n(S)`.
6.  **Consider Rules:** Apply addition/multiplication rules if the event involves 'OR' / 'AND' conditions. Remember independence vs. dependence.

---

**Examples:**

*   [[16 - Probability/03.E01 - Drawing Cards Probability Example.md]] (Illustrates selecting multiple cards from a deck with specific conditions)
*   [[16 - Probability/03.E02 - Drawing Balls from Bag Example.md]] (Demonstrates selecting balls of specific colors from a bag)

---

**Related Concepts:**

*   [[16 - Probability/01 - Basic Terminology (Event, Sample Space, P(E)).md]] (Provides the foundational P(E)=n(E)/n(S) formula)
*   [[16 - Probability/02 - Probability Rules (Addition, Multiplication).md]] (Rules are frequently applied in these problems, especially for combined conditions)
*   [[15 - Permutations and Combinations/03 - Combination (Selection) Formula (nCr).md]] (Essential for calculating n(S) and n(E) when selecting groups of items like cards or balls)
*   [[15 - Permutations and Combinations/01 - Factorial Notation.md]] (Needed for combination calculations)