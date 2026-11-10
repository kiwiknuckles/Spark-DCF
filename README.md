# Spark New Zealand (NZX: SPK) — DCF Valuation & Stock Pitch

A self-directed equity valuation of Spark New Zealand: a fully linked three-statement model, an unlevered DCF, and a two-page buy recommendation.

**Call: BUY — fair value $2.80 per share, implying 39% upside to $2.01 (October 2026), 12-month view.**

## Files

| File | What it is |
|---|---|
| `Investment_Memo.pdf` | Two-page stock pitch: thesis, business snapshot, catalysts, valuation, risks, and what would change my mind |
| `DCF_SPK.xlsx` | The model — 11 tabs, FY21–FY26 actuals and FY27–FY30 forecasts |

## The thesis in brief

At $2.01, Spark trades at 5.5x FY26 adjusted EBITDAI. My DCF only matches that price if cash flow grows ~0.5% a year forever, or if the discount rate is 7.9%, so the market is pricing in a slow decline. Spark has guided FY27 free cash flow of $300–350m (flat to up on FY26's $308m) alongside stable EBITDAI. If the FY27 results confirm that guidance, near-zero growth becomes hard to justify. I'm not arguing Spark deserves Telstra/TPG's 8.4x, only that the gap to the 6.9x my valuation implies is too wide.

## Model structure

- **Income Statement / Balance Sheet / Cash Flow** — fully linked; the balance sheet balances in every year
- **Assumptions IS / BS / CF** — all drivers in one place; historical columns calculate actual ratios, forecast columns hold inputs
- **FCFF** — unlevered free cash flow build, with a NOPAT bridge check and a reconciliation to Spark's own FCF definition
- **WACC** — CAPM with a peer-based beta (Telstra, TPG), market-value weights, cross-checked against Spark's impairment-test discount rate
- **DCF Valuation** — Gordon Growth (base case) and exit-multiple (cross-check) terminal values; EV → equity → per-share bridge
- **Sensitivity** — WACC × terminal growth and WACC × exit multiple grids, with check cells

Colour coding: blue = input, black = formula, green = link to another sheet. Sources and judgement calls are noted in red in column O.

## Key assumptions

| Input | Value | Basis |
|---|---|---|
| FY27 EBITDAI | $1,045m | Midpoint of Spark's $1,010–1,080m guidance |
| Capex | 11% of revenue from FY28 | Within Spark's 10–12% target range |
| Lease additions | ~$150m a year | FY26 cash paid on leases $141m, guided to rise |
| WACC | 6.6% | Cost of equity 7.7% (incl. a 2.0% judgement premium), after-tax cost of debt 4.3% |
| Terminal growth | 2.0% | RBNZ inflation-target midpoint |

## What I learned

- **Reconcile cash, not just earnings.** My first version calibrated EBITDAI to guidance but produced FY27 FCF of $473m against Spark's $300–350m guidance. The gap was lease costs: EBITDAI is struck before them under NZ IFRS 16. Adding them cut my fair value from $4.77 to $2.80 and brought FCF to $323m, inside guidance.
- **Know whether a debt figure is net or gross.** Spark's $1,781m net debt (including leases) is already net of cash; subtracting cash again overstated equity value.
- **Silent errors are the real risk.** The biggest bugs (a tax sign error, a SUM range gap, a paired formula updated in only one cell) produced no error messages, only wrong numbers. Check cells caught them.
- **Don't average your way to a target.** The 8.4x peer multiple implies 2.8% perpetual growth, so I show it as a re-rating scenario rather than averaging it into fair value.

## Sources

Spark New Zealand FY21–FY25 annual reports and FY26 results (Results Presentation and Detailed Financials, August 2026), available at [investors.sparknz.co.nz](https://investors.sparknz.co.nz). Peer multiples and betas from Yahoo Finance.

## Disclaimer

Student project for learning and portfolio purposes. Not investment advice. Prices and figures are as at October 2026.

— Francis Kayembe, Bachelor of Business (Finance and Accounting), AUT
