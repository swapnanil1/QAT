## Installments

#quant #simple_and_compound_interest #simple_interest #compound_interest #installments #emi #formula #concept

## Definition

Installments refer to a series of regular, usually equal, payments made over a specified period to repay a loan or pay for a purchased item. Each payment typically covers both the interest accrued on the outstanding balance and a portion of the principal amount.

Calculations differ depending on whether simple interest or compound interest rules are applied. Compound interest (leading to Equated Monthly Installments or EMIs in practice) is far more common for real-world loans.

## 1. Installments under Simple Interest (SI)

This scenario usually involves calculating the equal annual payment required to discharge a *debt due in the future*.

**Concept:** Imagine a debt `D` is due after `T` years. Instead of paying `D` at the end, the debtor agrees to pay `T` equal annual installments `X`, starting from the end of the first year. The sum of the values of these installments, calculated at the end of `T` years (i.e., each installment plus the simple interest it earns until the end of year T), must equal the debt `D`.

*   The first installment `X` paid after 1 year earns SI for `(T-1)` years. Its value at end of T years = `X * (1 + R*(T-1)/100)`
*   The second installment `X` paid after 2 years earns SI for `(T-2)` years. Its value at end of T years = `X * (1 + R*(T-2)/100)`
*   ...
*   The last installment `X` paid after T years earns SI for 0 years. Its value = `X`.

Summing these up equals D. A simplified formula exists:

**Formula (for debt D due in T years):**

The equal Annual Installment `X` required to clear a debt `D` due in `T` years at `R`% p.a. simple interest is:
`X = (100 * D) / [ 100*T + (R * T * (T-1)) / 2 ]`

**Important Note:** Calculating installments to repay a loan taken *now* under simple interest is less common and involves summing the present values of installments, which can be complex. The formula above is specifically for clearing a *future* debt.

## 2. Installments under Compound Interest (CI)

This is the standard method for loans (like EMIs - Equated Monthly Installments).

**Concept:** A loan `P` is taken out now. It's repaid in `T` equal installments `X` at the end of each period (e.g., year, month). The interest rate per period is `r`. The Present Value (PV) of all these future installments must equal the original loan amount `P`.

`P = PV(1st Installment) + PV(2nd Installment) + ... + PV(Tth Installment)`
`P = [ X / (1+r)^1 ] + [ X / (1+r)^2 ] + ... + [ X / (1+r)^T ]`

This is the sum of a Geometric Progression.

**Formula (for loan P taken now):**

The equal installment `X` required per period to repay a loan `P` over `T` periods at a rate `r` per period is given by:

`P = X * [ (1 - (1+r)^-T) / r ]`

Rearranging to find the installment `X`:

`X = P * [ r / (1 - (1+r)^-T) ]`

Or equivalently:

`X = P * [ (r * (1+r)^T) / ((1+r)^T - 1) ]`

**Key parameters:**
*   `P`: Principal loan amount (Present Value).
*   `X`: Amount of each equal installment.
*   `r`: Rate of interest *per installment period*. If the annual rate is R and installments are monthly, `r = (R/12)/100`. If annual rate R and installments are annual, `r = R/100`.
*   `T`: Total number of installments (periods).

## Important Considerations

*   **SI vs CI:** Understand which interest type applies. SI installment questions often relate to clearing a future debt, while CI installments relate to repaying a current loan.
*   **Matching Periods:** In CI calculations, ensure the interest rate `r` and the number of periods `T` correspond to the frequency of installments (e.g., for monthly installments over 5 years with a 12% annual rate, `r = (12/12)/100 = 0.01` and `T = 5 * 12 = 60`).
*   **Formula Sheet:** These formulas, especially the CI one, are essential to memorise or understand how to derive from the present value concept.

## Related Concepts

*   Builds upon [[04 - Simple and Compound Interest/01 - Simple Interest (SI) Formula and Concepts.md]]
*   Builds upon [[04 - Simple and Compound Interest/02 - Compound Interest (CI) Formula and Concepts.md]]
*   Involves concepts of Present Value and Annuities (especially the CI formula).
*   Geometric Progression sum is used in deriving the CI formula.

## Example Links

*   [[04 - Simple and Compound Interest/04.E01 - Equal Installment Calculation (SI) Example.md]]
*   [[04 - Simple and Compound Interest/04.E02 - Equal Installment Calculation (CI) Example.md]]