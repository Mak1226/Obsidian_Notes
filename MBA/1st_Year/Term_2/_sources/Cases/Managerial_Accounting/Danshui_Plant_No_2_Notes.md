---
course: Managerial_Accounting
type: case-notes
title: "Danshui Plant No. 2 — Notes"
source: https://hbsp.harvard.edu/tu/e90fb059
product_id: 4148 (9-913-525) — HBS Brief Case
tags: [case-notes, managerial_accounting, flexible-budget, variance-analysis, cvp]
---

# Danshui Plant No. 2 — Notes

📄 Case PDF: [[Danshui_Plant_No_2.pdf]]

## Quick Read
> HBS Brief Case (fictitious). August 2010. **Wentao Chen** manages **Danshui Plant No. 2** (southern China), a contract-manufacturing profit center in month 3 of a **12-month contract to assemble 2.4 million Apple iPhone 4 units** (**200,000/month budget**). Production is stuck at **180,000/month** because the plant cannot hire enough qualified labor even after raising wages ~30%. The August report compares actual results at 180,000 units to the **static master budget at 200,000 units**, showing a $672,000 loss vs. a $100,000 budgeted profit and a $772,000 adverse net-income variance — an apples-to-oranges comparison. Controller Bingqian Li wants a **flexible budget at 180,000 units** so performance is judged against what *should* have been spent at actual volume. The class task: rebuild the report as a flexible budget, decompose the variances (materials price/usage, labor rate/efficiency, overhead spending), and recommend what Chen should do over the remaining nine months.

## Case Notes

### Key facts
- **Standard variable cost per unit (Exhibit 1):** purchased chips $125.35 (flash memory $27.00, app processor $10.75, phone-call chip $14.05, gyroscope $2.60, 8 other chips $70.95) + variable supplies & tools $62.54 = $187.89; + assembly & packaging labor $13.11 + shipping $1.06 → **total standard variable cost = $202.06/unit**.
- **Budgeted fixed overhead (Exhibit 2):** factory rent $400,000 + machine depreciation $150,000 + utilities & local taxes $52,000 + supervision $127,000 = **$729,000/month**.
- **Transfer (revenue) price:** $41,240,000 / 200,000 = **$206.20/unit** ⇒ standard **contribution margin ≈ $4.14/unit**.
- **August report (Exhibit 3, $000):** static budget (200k units) net income **+$100**; actual (180k units) net income **−$672**; net-income variance **$772 U**. Revenue $37,476 actual vs. $41,240 budget; total cost $38,148 actual vs. $41,140 budget.
- **Operational issues cited:** cannot hire enough labor despite a ~30% wage rise since July (Foxconn Shenzhen raised starting pay ~35% since March and is building plants where unemployment is high); **1,000 Samsung flash memories damaged by heat during installation** in August and replaced; Samsung raised the flash-memory price **$2/unit** mid-June and Apple raised revenue recovery by an equal $2 (net neutral); the standard was not updated for either.

### Numbers to work

**Break-even (Q1):** $729,000 fixed ÷ $4.14 CM/unit ≈ **176,100 units**. So at 180,000 the plant should have made a small profit; budgeted profit at 200,000 = 200,000 × 4.14 − 729,000 ≈ **$99k**.

**Expected vs. actual unit cost (Q2):** at 200,000 units, total cost/unit = $41,140,000 / 200,000 = **$205.71** (variable $202.06 + fixed $3.65). Actual at 180,000 = $38,148,000 / 180,000 = **$211.93/unit** — higher mainly from spreading fixed cost over 20,000 fewer units plus the labor overrun.

**Flexible budget at 180,000 units (Q3):**
- Variable: 180,000 × $202.06 = **$36,370,800**; fixed **$729,000**; total cost **$37,099,800**.
- Revenue: 180,000 × $206.20 = **$37,116,000** → **flexible-budget net income ≈ +$16,000**.
- **Volume/sales-shortfall effect:** 20,000 units × $4.14 CM = **~$83,000 less contribution** (explains most of the drop from the $100k budget to the ~$16k flexible-budget profit).
- **Cost-overrun (flexible-budget) variances at 180,000 units:** the ~$688,000 gap between the flexible-budget +$16k and the actual −$672k is almost entirely the **assembly & packaging labor variance ≈ $732,000 U** (actual $3,092k vs. flexible budget $2,359.8k). Other lines are small: flash memory ~$389k U, 8-other-chips ~$128k F, supplies ~$48k U, fixed supervision $7k U.

**Component variances (Q4):**
- **Flash memory:** actual $5,249k; std $27 × 180,000 good units = $4,860k. Units used ≈ **181,000** (180,000 + 1,000 scrapped). Usage/efficiency variance = 1,000 × $27 = **$27k U** (the damaged units); price variance = $5,249k − 181,000 × $27 = **$362k U** — but essentially all of that is the **un-updated standard** (Samsung +$2/unit since mid-June); at a $29 standard the price variance ≈ $0, offset by Apple's matching $2 revenue increase.
- **Assembly & packaging labor:** total variance ≈ **$732k U**. Driven by the **~30% wage hike** to attract scarce workers ⇒ a large unfavorable **rate variance** (~$700k: $13.11 × 30% ≈ $3.93/unit × 180,000), with a smaller unfavorable **efficiency variance** (~$24k) from training/rework of new hires.
- **Overhead spending variance:** fixed overhead actual $736k vs. budget $729k → **$7k U**, all in supervision; rent, depreciation, utilities/taxes exactly on budget (committed). If fixed overhead is applied per unit, there is also a **volume variance ≈ $73k U** ($3.65 × 20,000 unabsorbed).

### Central decision
- Rebuild the August report as a **flexible budget at 180,000 units**, split the $772,000 adverse net-income variance into the **volume shortfall (~$83k)** and **genuine cost overruns at 180,000 units (~$688k, overwhelmingly labor rate)**, and decide what Chen should do for the remaining nine months — given a contract contribution margin of only **~$4.14/unit** that leaves almost no room for input-cost inflation.

### Key takeaways
- **Fix the report first:** the static-budget comparison mixes the (uncontrollable) volume shortfall with real cost performance; a flexible budget shows Danshui's *cost* problem is one line — assembly labor — not a broad failure, and materials usage is actually good.
- **The structural problem is the contract economics:** ~$4.14 CM/unit and a ~176,000-unit break-even mean any wage inflation (or the inability to reach 200,000) tips the contract into loss regardless of effort. Input-cost pass-through works for chips (Samsung +$2 ↔ Apple +$2) but **not for local wages**.
- **Labor supply is the binding constraint:** raising wages to hit 200,000 units enlarges the rate variance faster than volume adds contribution — model the trade-off explicitly.
- **Realistic options:** (1) renegotiate the transfer price / add a wage-index escalator with Apple, or cut the committed annual quantity to ~2.16M; (2) invest in training and targeted automation for the labor-intensive, damage-prone steps (esp. flash-memory installation) to cut scrap and efficiency loss; (3) add or relocate capacity where labor is available, or subcontract overflow; (4) update the standards for the $2 flash-memory change and the new wage rates so future variances are meaningful.
- Whatever Chen does, the contract is **structurally loss-making at prevailing wages** without a price renegotiation or a real productivity gain — at 180,000 *or* 200,000 units.
