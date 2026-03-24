# True recording of work and thoughts.
## 0
**Contingent convertibles**, often called **CoCos**, are a type of debt instrument used primarily by banks.

Here is a simple explanation:

**CoCos are bonds that automatically turn into equity (shares) or get written down when the issuer’s financial health falls below a certain level.**

Key points:
- **Trigger:** They have a specific trigger (e.g., the bank’s capital ratio drops too low).
- **Purpose:** They are designed to help a bank absorb losses without going bankrupt or needing a government bailout.
- **Risk:** If the trigger is hit, investors can suffer heavy losses (either by being forced to become shareholders of a struggling bank or losing their principal entirely).

---
A **Poisson process** is a simple way to model events that happen randomly over time (or space), where:

- Events occur one at a time.
- The number of events in any time interval follows a **Poisson distribution**.
- The times between events are **exponential** and independent of each other.
- What happens in one interval does not affect what happens in another (independent increments).

In plain words: if you are counting random, rare events that happen at a constant average rate (like customers arriving at a shop or emails arriving in your inbox), a Poisson process is the standard mathematical model for that.

---
**Economic capital** is the amount of capital a bank *internally* estimates it needs to cover unexpected losses, based on its own risk models. It’s a risk-based, internal measure.

**Regulatory capital** is the *minimum* amount of capital required by regulators (e.g., under Basel rules). It’s a legal requirement, not necessarily aligned with the bank’s own risk view.

In short:
- **Economic capital** = what the bank thinks it needs.
- **Regulatory capital** = what the law says it must have.

Banks often hold more than the regulatory minimum, but the two serve different purposes: one for internal risk management, the other for compliance and financial stability.

---
The denominator for all four of these key capital ratios is the same: **Risk-Weighted Assets (RWA)**.

While the numerators differ (representing different definitions of a bank’s capital cushion), the denominator remains constant. Below is a detailed explanation of what RWA is, followed by how it applies to each ratio.

### The Denominator: Risk-Weighted Assets (RWA)

Risk-Weighted Assets are not the total assets (leverage ratio exposure) on a bank’s balance sheet. Instead, they represent the bank’s assets adjusted for risk. The logic is that a bank should not need to hold the same amount of capital against a low-risk government bond as it does against an unsecured corporate loan.

RWA is calculated as the sum of three primary risk components:

1.  **Credit Risk RWA:** The risk that a borrower or counterparty will default. Each asset is assigned a risk weight (0%, 20%, 50%, 100%, or higher) based on the credit rating of the counterparty, the type of collateral, and the maturity.
    - *Example:* Cash and government bonds often have a 0% risk weight. Residential mortgages often have a 35% or 50% risk weight. Unsecured corporate loans typically have a 100% risk weight.
2.  **Operational Risk RWA:** The risk of loss resulting from inadequate or failed internal processes, people, systems, or external events (e.g., fraud, cyber-attacks). This is usually calculated as a percentage of gross income or via standardized indicators, rather than being tied to specific balance sheet assets.
3.  **Market Risk RWA:** The risk of losses in trading book positions arising from changes in market prices (interest rates, foreign exchange rates, equity prices).

$$ \text{Total RWA} = \text{Credit Risk RWA} + \text{Operational Risk RWA} + \text{Market Risk RWA} $$

### The Four Ratios

Here is how the denominator (RWA) applies to each specific capital ratio.

#### 1. Total Capital Ratio (Capital Adequacy Ratio)
This is the broadest measure of solvency. It compares all forms of regulatory capital to RWA.

- **Numerator:** Total Capital (Tier 1 + Tier 2 capital).
    - *Tier 1:* Going concern capital (Common Equity Tier 1 + Additional Tier 1 instruments like perpetual bonds).
    - *Tier 2:* Gone concern capital (subordinated debt, loan loss reserves up to a limit).
- **Denominator:** RWA.
- **Formula:**
    $$ \frac{\text{Tier 1 Capital} + \text{Tier 2 Capital}}{\text{RWA}} $$
- **Regulatory Minimum (Basel III):** Typically **8%**.

#### 2. Tier 1 Capital Ratio
This ratio focuses on the bank’s highest-quality capital—the capital that is permanently available to absorb losses while the bank is a going concern.

- **Numerator:** Tier 1 Capital (Common Equity Tier 1 + Additional Tier 1 instruments).
- **Denominator:** RWA.
- **Formula:**
    $$ \frac{\text{Common Equity Tier 1 (CET1)} + \text{Additional Tier 1 (AT1)}}{\text{RWA}} $$
- **Regulatory Minimum (Basel III):** Typically **6%** (though this includes the mandatory Capital Conservation Buffer in practice).

#### 3. Core Tier 1 Capital Ratio
*Note: This term is largely historical. Prior to Basel 2.5 and Basel III, regulators used "Core Tier 1" to refer to what is now defined as Common Equity Tier 1 (CET1). In modern regulatory reporting, this ratio is functionally identical to the CET1 ratio.*

If you encounter this term in older financial statements or specific jurisdictions (such as the UK pre-2013), it refers to the highest quality capital, excluding innovative hybrid instruments that were previously allowed in Tier 1.

- **Numerator:** Core Tier 1 Capital (essentially common equity + retained earnings + disclosed reserves, minus regulatory deductions).
- **Denominator:** RWA.

#### 4. Common Equity Tier 1 (CET1) Ratio
This is the strictest and most important capital ratio in the Basel III framework. It measures the highest quality capital—only common shares and retained earnings—against risk.

- **Numerator:** Common Equity Tier 1 Capital.
    - *Includes:* Common shares (paid-up capital), stock surplus, retained earnings, accumulated other comprehensive income (AOCI), and disclosed reserves.
    - *Excludes (Deductions):* Goodwill, deferred tax assets (that rely on future profitability), intangible assets, and significant investments in financial institutions’ capital instruments.
- **Denominator:** RWA.
- **Formula:**
    $$ \frac{\text{Common Equity Tier 1 Capital}}{\text{RWA}} $$
- **Regulatory Minimum (Basel III):** **4.5%** (plus Capital Conservation Buffer of 2.5%, effectively requiring 7.0% to avoid restrictions).

### Summary Table

| Ratio | Numerator (Capital Type) | Denominator | Purpose |
| :--- | :--- | :--- | :--- |
| **Common Equity Tier 1 (CET1)** | Common shares, retained earnings (highest quality) | RWA | Measures core loss-absorbing capacity; the strictest metric. |
| **Core Tier 1** | (Historical term) Common equity + disclosed reserves | RWA | Predecessor to CET1; rarely used in modern Basel III reporting. |
| **Tier 1** | CET1 + Additional Tier 1 (e.g., perpetual bonds) | RWA | Measures going-concern capital, including hybrid instruments. |
| **Total Capital** | Tier 1 + Tier 2 (e.g., subordinated debt) | RWA | Measures total solvency, including gone-concern capital. |

### Critical Distinction: RWA vs. Leverage Ratio Denominator
It is important to note that while RWA is the denominator for these four capital ratios, the **Leverage Ratio** uses a different denominator: **Total Exposure Measure** (which is essentially the non-risk-weighted balance sheet plus off-balance-sheet exposures).

If a bank wants to improve its CET1 ratio (Capital/RWA), it can either increase capital (numerator) or decrease RWA (denominator) by selling high-risk-weighted assets or switching to lower-risk-weighted assets. This creates an incentive structure where banks might favor government bonds (0% risk weight) over corporate loans (100% risk weight), which is why regulators use the leverage ratio (non-risk-weighted) as a backstop to ensure banks do not over-leverage simply by chasing low-risk-weight assets.

---
Trying to understand this work in fisrt reading. You'll get there!

---

**Key Credit Risk Parameters under Basel II IRB**

- **PD (Probability of Default)**  
  The long‑run average percentage of borrowers in a given rating grade that are expected to default within a one‑year horizon. It is a *through‑the‑cycle* measure, reflecting average credit quality rather than current economic conditions.

- **EAD (Exposure at Default)**  
  The estimated total amount outstanding (drawn balance plus any additional drawdowns before default) at the moment the borrower defaults. For fixed loans it is the principal; for revolving facilities it incorporates a *credit conversion factor* to reflect potential usage before default.

- **LGD (Loss Given Default)**  
  The proportion of the exposure (EAD) that is not recovered after default, i.e., \( \text{LGD} = 1 - \text{recovery rate} \). It depends on collateral, seniority, and the workout process.

These three parameters are multiplied to obtain the **Expected Loss (EL)** for a credit facility:

$$
\text{EL} = \text{PD} \times \text{EAD} \times \text{LGD}
$$

In the IRB framework, regulatory capital is designed to cover *unexpected losses* (UL), which is the difference between a high percentile of the loss distribution (e.g., 99.9%) and the expected loss.

---
$$
UL=\sum^{N}_{i=1}\sigma_i\rho_i
$$

**Your understanding:**

> $σ_i$ is the risk that this facility has on its own, unrelated to other instruments (stand‑alone),  
> $ρ_i$ adjusts the stand‑alone risk in the context of overall risk through the idea that “higher correlation leads to stronger risk transmission at default”, thereby obtaining the true UL.

**A more precise explanation:**

1. **$σ_i$ (stand‑alone standard deviation)**  
   It does measure the volatility of credit losses for the $i^{th}$ facility on its own, **but** this volatility itself does not assume independence from other assets. In fact, σ_i already incorporates the facility’s own PD, EAD, LGD, and its own return uncertainty.  
   However, it **does not reflect** the co‑movement between this facility’s losses and the losses of other facilities in the portfolio.

2. **$ρ_i$ (correlation with the overall portfolio)**  
   It is not the pairwise correlation between this facility and another single facility; rather, it is the correlation between this facility’s credit losses and **the total portfolio loss**.  
   Therefore, ρ_i directly measures:  
   - When the overall portfolio performs poorly, how likely is this facility to also suffer a loss?  
   - If ρ_i is high, this facility’s losses are highly correlated with the overall portfolio and are not easily diversified away.

3. **What $UL = \sum \sigma_i \rho_i$ means**  
   This formula is used in the **risk contribution** framework to decompose the portfolio’s unexpected loss (UL) into contributions from each facility.  
   - $σ_i$ is the facility’s own risk “magnitude”  
   - $ρ_i$ is the facility’s risk “direction / correlation”  
   - Their product is the facility’s **marginal contribution** to the total UL  

   Thus, **ρ_i does not simply “adjust” σ_i**; rather, it converts σ_i from “stand‑alone risk” into “contribution to portfolio risk”.

**A simple analogy:**

- $σ_i$ is like the volatility of an individual stock  
- $ρ_i$ is like the correlation of that stock with the overall market (portfolio)  
- $σ_i × ρ_i$ is the stock’s **contribution to total market risk** (portfolio volatility), not its own standalone volatility

**Summary:**

Your intuition — “higher correlation leads to stronger risk transmission and thus a larger role in overall risk” — is correct.  
More precisely:  
> $UL = \sum \sigma_i \rho_i$ is not “adjusting $σ_i$ by $ρ_i$ to obtain total UL”; instead, it **decomposes total UL into each facility’s risk contribution**, where $ρ_i$ determines how much of the facility’s standalone risk translates into portfolio risk.

---
### Why does this work?

**1. What is the problem?**

The first sentence of the original text says:

> Part of the difficulty in assessing banks’ RWA calculations is distinguishing between differences that arise from portfolio risk and asset quality and those that arise from differences in models.

When regulators look at two banks’ risk‑weighted assets (RWA), they often find different results.  
The question is: **where does this difference come from?**

There are two possibilities:

- **Source A: The portfolios themselves are different**  
  For example, Bank A’s loan portfolio contains many high‑risk industries, while Bank B’s portfolio consists mainly of low‑risk retail mortgages. Even if both banks use exactly the same model, their RWA will differ.

- **Source B: The models are different**  
  Both banks face the same loan portfolio, but because their internal models (PD, LGD, correlation assumptions, etc.) differ, the calculated RWA also differ.

In reality, both sources are present and intertwined. Regulators cannot directly tell whether the observed difference comes from different portfolio risks or from different models.

**2. How is this solved?**

The following sentences explain:

> To identify differences between banks’ internal models, regulators have undertaken a number of exercises in which banks applied internal models to estimate key risk parameters for a **hypothetical portfolio assets**. This ensured that differences in calculated risk weights are down to differences in banks’ modelling approaches, rather than differences in the risk of portfolios being assessed.

Regulators design a **hypothetical portfolio** and ask each bank to apply its own internal model to calculate the RWA for that **same** portfolio.

**3. Why does this allow the distinction?**

Because now:

- **The portfolio is fixed and identical across banks**  
  All banks are calculating RWA for the same set of hypothetical loans (same industries, same sizes, same PD/LGD input assumptions, etc.).
- **Portfolio risk differences are eliminated** (all banks face the same portfolio).
- Therefore, if the calculated RWA still differ across banks, **the only remaining source is differences in their models** (methodologies, assumptions, parameter estimation techniques, etc.).

This allows regulators to **compare the models themselves** without interference from differences in actual portfolios.

**4. An analogy**

Suppose you want to compare the cooking skills of two chefs:

- If you let each chef cook a dish of their own choice – one makes braised pork, the other steamed fish – and the tastes differ, you cannot be sure whether the difference comes from the different dishes or from the chefs’ skills.
- If you give them **exactly the same ingredients and the same recipe** for the same dish, and the results still taste different, then the difference must be due to the chefs’ skills.

In this analogy:
- Banks = chefs  
- Hypothetical portfolio = same ingredients and recipe  
- RWA = the final taste of the dish

**5. Summary**

**The exercise works because:**

- Using the same hypothetical portfolio **eliminates “differences in portfolio risk” as a variable**.
- Any remaining differences in calculated RWA can only be attributed to **differences in banks’ internal modelling approaches**.
- This is a common **benchmarking** technique used by regulators to assess the comparability of internal models, rather than comparing the absolute RWA of banks’ real portfolios.

---
