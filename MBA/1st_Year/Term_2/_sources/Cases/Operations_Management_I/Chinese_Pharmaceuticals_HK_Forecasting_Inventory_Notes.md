---
course: Operations_Management_I
type: case-notes
title: "Chinese Pharmaceuticals (HK) Limited: Effective Forecasting for Optimal Inventory Management — Notes"
source: https://hbsp.harvard.edu/tu/b92801dd
product_id: ST5 (UST005/1808) — HKUST
supplement: Spreadsheet for Students ST5S-XLS-ENG (https://hbsp.harvard.edu/tu/b2e2adf9)
tags: [case-notes, operations_management_i, forecasting, exponential-smoothing, seasonality, inventory, safety-stock]
---

# Chinese Pharmaceuticals (HK) Limited: Effective Forecasting for Optimal Inventory Management — Notes

📄 Case PDF: [[Chinese_Pharmaceuticals_HK_Forecasting_Inventory.pdf]]

## Quick Read
> HKUST case (Lau & Fernandez). **Jason Kwok**, GM of Chinese Pharmaceuticals (HK), supplies Chinese herbal medicines to Hong Kong. Its best-seller **Noto37** (a Notoginseng-based cholesterol/blood-pressure remedy, ~40% category share, up to **80% of sales in peak winter**) has **gone out of stock again** at its biggest customer, **Mannings** (300 stores) — risking loss of precious shelf space. The supply chain has a **90–100 day total lead time** (Yunnan raw material 4–6 weeks + testing 7–9 days + HK contract manufacturing 8 weeks) and demand is strongly seasonal (winter/CNY peak ~+50%, spring trough ~−50%) with a rising trend. Inventory is managed "by circumstance" (reorder at ~1.5 months' supply, cap ~3 months = warehouse capacity). An MBA intern applied **simple exponential smoothing (α = 0.4)** to 3 years of monthly sales. Jason must judge whether that method is right and design better forecasting and inventory practices.

## Case Notes

### Key facts
- **Supply chain (Exhibit 1), lead times:** Yunnan supplier delivers "super fine" Notoginseng powder in **4–6 weeks**; independent-lab testing (metals/toxins/water) **7–9 days**; HK contract manufacturer takes up to **2 months (8 weeks)** to produce Noto37 → **total ≥ 90–100 days** from placing the Yunnan order to sellable product. Cash-flow limits stop the company buying cheap raw material in spring/winter — it buys regular quantities year-round.
- **Distribution:** local transport delivers Noto37 once or twice a week to Mannings (300), Watson's (180+), and 500+ neighbourhood pharmacies (~1,000 outlets).
- **Seasonality:** winter to Chinese New Year = peak, sales up to **50% above average**; spring **50% below average**; summer/autumn near the annual mean.
- **Inventory practice:** no owned warehouse — leases space, adds space before the peak; targets **≤ 3 months' supply** (= leased finished-goods capacity); **reorders at ~1.5 months' supply**. Actual stock swings with variable deliveries to ~1,000 outlets, manufacturer delays, Yunnan drought, and weekly promotions. Inventory position driven more by available warehouse space than by any analysis.
- **The intern's model:** **simple exponential smoothing** — F₍t+1₎ = α·Sₜ + (1−α)·F₍t+1₎... i.e. F₍t+1₎ = Fₜ + α·(Sₜ − Fₜ); **α = 0.4**, initial F₂ = S₁ = 3,303 units. Exhibit 2 = 36 months (Jul-09 to Jun-12) of actuals and forecasts; Exhibit 3 plots them.
- **Data pattern (Exhibit 2/3):** sales rise from ~3,300 (Jul-09) to ~9,700 (Dec-11) — a clear **upward trend** — with a pronounced **winter peak** every year (~7,300 in 2010, ~9,700 in 2011) and a spring trough. The simple-ES forecast **visibly trails the actuals and undershoots every winter peak** — exactly when the stockout occurs — and overshoots every spring.
- **Near-term firefighting:** Jason got the Yunnan supplier to add workers for an extra batch, testing halved, and pushed the manufacturer to queue-jump for a small delivery in 2 weeks + a larger one in 30 days.

### Central decision
- **Is simple exponential smoothing (α = 0.4) an appropriate forecasting method for Noto37**, given the trend-plus-seasonality demand? If not, which method should replace it, how should forecast accuracy and bias be measured, and how should the chosen forecast (and its error) be translated into an inventory policy — safety stock and reorder point for a target service level — that fits the 90–100 day lead time and the 3-month warehouse cap?

### Key takeaways
- **Simple ES is the wrong tool here:** it assumes a roughly level series with no trend or seasonality, so it **systematically lags** — the Exhibit 3 forecast is below actuals every winter (missing the peak, causing the Mannings stockout) and above them every spring (overstock). Raising α reduces lag but adds noise and still can't model seasonality.
- **Use a trend + seasonal model:** (a) **Holt-Winters / Winters' method** (level + trend + seasonal — the natural fit); or (b) **trend-adjusted (double) ES + multiplicative monthly seasonal indices** computed from the 3 years; or (c) **regression with a time trend + 11 monthly seasonal dummies**, or classical decomposition (centered moving average → seasonal indices → deseasonalize → trend → reseasonalize).
- **Measure error and bias:** compute **MAD, MSE/RMSE, MAPE** on a holdout for each candidate; run a **tracking signal** (cumulative error ÷ MAD) to catch persistent bias — simple ES on this data would flag a running winter under-forecast. Choose on out-of-sample accuracy, not in-sample fit.
- **Forecast → inventory:** with a credible seasonal forecast, set a **season-specific reorder policy**. Reorder point = expected demand over the **protection interval (~90–100 day total lead time)** + **safety stock = z·σ_L** (σ_L = SD of forecast error over the lead time; z from the service level, which should be high given the cost of losing Mannings shelf space). Because the lead time spans a full quarter and demand is seasonal, planning must be **time-phased** — order for winter in late summer — not a static "1.5 months' supply."
- **Design around the constraints:** pre-book peak-season warehouse space and raw-material supply from the seasonal forecast; hold some safety stock as **super-fine powder** (shorter remaining lead time, less obsolescence) as well as finished goods; qualify a second Notoginseng source / manufacturing slot to cushion Yunnan drought and queue delays; and feed the Holt-Winters forecast into an MRP/time-phased plan.
- **Firefighting ≠ a system:** the extra Yunnan batch, halved testing and queue-jumping buy time now; the permanent fix is a trend-and-seasonal forecast driving a seasonally time-phased inventory plan with explicit safety stock for a chosen service level.
