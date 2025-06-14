# EPE & PFE Simulation for Interest Rate Swap using Monte Carlo

This project simulates the **Expected Positive Exposure (EPE)** and **Potential Future Exposure (PFE)** of a vanilla fixed-for-floating **Interest Rate Swap (IRS)** using a **Monte Carlo simulation** of future interest rates modeled under the **Hull-White one-factor model**.

---

## Purpose

To model counterparty credit risk exposure profiles for an IRS, estimating:

- **EPE:** Average positive exposure over simulated future paths.
- **PFE:** Tail risk exposure (e.g., 95th percentile) at future time points.

This is useful for CVA, regulatory capital, and risk management applications.

---

## Model Details

- **Swap Type:** Payer IRS (fixed pays fixed rate, floating receives LIBOR-like rate)
- **Tenor:** 1 year, semi-annual payments
- **Notional:** $100 million
- **Interest Rate Model:** Hull-White 1-factor model
- **Simulation:** 10,000 Monte Carlo paths, monthly steps
