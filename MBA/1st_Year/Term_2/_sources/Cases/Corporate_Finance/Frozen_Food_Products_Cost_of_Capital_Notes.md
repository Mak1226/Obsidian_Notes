---
course: Corporate_Finance
type: case-notes
title: "Frozen Food Products: Cost of Capital — Notes"
source: https://hbsp.harvard.edu/tu/6b489f62
product_id: W12324 (9B12N028) — Ivey
companion_reading: "Leveraged Betas and the Cost of Equity (https://hbsp.harvard.edu/tu/ddb34620)"
tags: [case-notes, corporate_finance]
---

# Frozen Food Products: Cost of Capital — Notes

📄 Case PDF: [[Frozen_Food_Products_Cost_of_Capital.pdf]]

## Quick Read
> Ivey case (S.K. Mitra, IIM Raipur). **Maria D'souza** runs a private Indian tropical-fruit pulp/puree/concentrate company (founded by her father, ~1980) and wants to add a **frozen-foods line using IQF (individual quick-freezing)** technology — an expansion meant to roughly double the business. She has five-year projected financials (Exhibits 1–2) and a 5% perpetual growth assumption thereafter, but no discount rate: the firm is unlisted, so it has no observable beta. The task is the **pure-play / comparable-company method**: unlever the equity betas of eight listed food-processing firms, average to an asset beta, relever at the project's target capital structure (D:E = 1:3), build the cost of equity via CAPM and then the WACC, and finally value the project.

## Case Notes

### Key facts
- **Project financing:** target **debt:equity = 1:3** (initial: total assets 8,000('000) = equity 6,000 + debt 2,000, Exhibit 2). Parent has negligible debt; project kept on separate books.
- **Projected income statement (Exhibit 1, '000):** Revenue 4,400 → 6,400 over Yr1–5; EBITDA 2,000 → 2,800; depreciation @15%; interest @8%; PBT 935 → 1,554; tax @30%; **PAT 655 → 1,088**.
- **Projected balance sheet (Exhibit 2, '000):** Equity 6,000 → 7,734; Debt 2,000 → 2,578; Net fixed assets 6,000 → 7,113 (gross FA 6,000 → 12,000); Working capital 2,000 → 3,200.
- **Terminal value:** 5% perpetual growth in cash flows beyond Year 5.
- **CAPM inputs given:** risk-free rate **8%** (India 10-yr G-Sec 1998–2012 average; ≈ RBI benchmark); **market risk premium 8%** (Fernandez et al. 2012 survey — vs 5.4% Canada, 5.5% US); uniform **tax 30%**; **cost of debt 8%**, debt treated as risk-free for all firms.
- **Comparables (Exhibit 3, S&P CNX 500 "Food & Food Processing"):** Advanta India (β 0.547), Britannia (0.264), GSK Consumer Healthcare (0.096, no debt), Jubilant Foodworks (0.986, no debt), Kwality Dairy (0.636), Rei Agro (0.539, very high debt), Venky's (0.669), Zydus Wellness (0.537, no debt). Table gives book value, market cap (E), book debt (D) and net income for each; betas estimated on 1 year of daily returns vs. BSE Sensex-30.

### Central decision
- **What discount rate should D'souza use to compute the project NPV**, and is the frozen-foods expansion value-creating? Concretely: (1) unlever each comparable's β, (2) pick a representative asset β, (3) relever at D/E = 1/3, (4) compute Ke = 8% + β·8%, (5) compute WACC = 0.75·Ke + 0.25·8%·(1−0.30), (6) discount project free cash flows (5 explicit years + terminal value = FCF₆/(WACC − 5%)), (7) compare NPV with the ~8,000('000) initial outlay.

### Key takeaways
- **Pure-play method:** for a private firm or a stand-alone project, borrow risk from listed peers in the same business — same customers/operations/assets ⇒ similar business risk ⇒ similar unlevered (asset) beta.
- **Unlever → average → relever (Hamada):** βU = βL / [1 + (1−t)(D/E)]; average the βU across comparables (using judgment on outliers — Rei Agro's extreme leverage, GSK's implausibly low beta, Jubilant's high beta); then βL,project = βU · [1 + (1−0.30)(1/3)].
- **Only financial-leverage risk is stripped out;** the residual business risk should be roughly comparable across the peer set. Use **market value** for equity but **book value** for debt (as the case does).
- **Indicative result:** peer equity betas average ≈ 0.5; unlevered ≈ 0.4–0.45; relevered ≈ 0.5–0.6 ⇒ Ke ≈ 12–13%; **WACC ≈ 10–12%**. Comfortably above the 5% terminal growth rate, so the NPV is positive on the base-case projections → accept the expansion.
- **Sensitivities that matter:** choice of comparables and estimation window for beta; the unusually high Indian risk-free rate (8%) and MRP (8%); and the (WACC − g) spread, since the terminal value dominates project value.
