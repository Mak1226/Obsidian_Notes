---
course: Operations_Management_I
type: case-notes
title: "ABC Shipyard: The Facility Layout — Notes"
source: https://hbsp.harvard.edu/tu/d18b16de
product_id: W16803 (9B16D023) — Ivey
supplement: Student Spreadsheet W16802-XLS-ENG (https://hbsp.harvard.edu/tu/0bf44bc2)
tags: [case-notes, operations_management_i, facility-layout, theory-of-constraints, cellular-manufacturing, wip]
---

# ABC Shipyard: The Facility Layout — Notes

📄 Case PDF: [[ABC_Shipyard_The_Facility_Layout.pdf]]

## Quick Read
> Ivey case (Dixit, Raj, Sharma). October 2, 2014. **Rayul Pitambar**, COO of **ABC Shipyard** (Big City, eastern India; 70 hectares; ~4 ships/year, 50,000 t/yr steel capacity), has an order from a marine-logistics company for **five Handymax 55,000 DWT bulk carriers, US$140 million, to be delivered in two years** — attractive in a booming shipbuilding market, but the current layout and throughput may not support it. The block-erection area is jammed with **~100 semi-finished blocks** because the steel shop maximizes its own KPI (tonnes cut per day) by running large same-thickness batches and delivers the wrong mix of plates. Pitambar, the steel-shop manager (Sudesh) and the block-erection manager (Bidesh) debate fixes: subordinate steel scheduling to block erection (Theory of Constraints), reorganize the steel shop into product-focused cells (physical later, **virtual now**), and re-lay-out the process shops for linear material flow — and how to **scientifically justify** the layout investment to top management.

## Case Notes

### Key facts
- **Product / process:** ships built as **"blocks"** (Exhibit 1: flat midship blocks, curved aft/fore blocks) → keel → midship → aft → fore → join → complete ship. Process flow (Exhibit 3): steel cutting → sub-assembly → panel fabrication → outfitting prep → painting → pre-outfitting → **block erection** → block assembly → launching → final outfitting → commissioning.
- **Layout (Exhibit 2):** a **hybrid** — **process-focused** shops (steel shop + stockyard, pipe shop, paint shop, general purpose shop, sub-assembly, panel fabrication) feeding a **fixed-position** back end (block erection area → 600-tonne Goliath crane → dock → quay). Cranes scale up along the flow: 10T (steel), 25T (sub-assembly), 50T (panel fab), 600T Goliath (super blocks 200–300 t).
- **Steel shop:** processes **34,000 t/yr** for two section types — **flat** (midship blocks, ~70% of steel processed) and **curved** (aft/fore, ~25%, needs thermal/cold bending). Biggest set-up cost is switching between flat and curved plates.
- **Outfitting shop:** only ~4 t of steel/day but **~50% of all labour hours** — the single greatest chunk of manual labour.
- **The WIP crisis:** block erection is full for ~18 months with ~100 semi-finished blocks. Cause: the steel shop runs **large batches of one thickness/profile** to maximize its "tonnes cut per day" KPI → other thicknesses unavailable → block erection halts blocks half-done and starts new ones for which plates exist → yard fills with semi-finished blocks → runs out of space → consumption rate of available plates falls → **WIP rises further (vicious cycle)**. A local-KPI failure, not a capacity shortage.
- **The constraint (Theory of Constraints):** early stages (steel prep, cutting, sub-assembly) are repetitive across ship types → economies of scale possible. But the **block erection area and the dock are fixed-position and expensive to expand** — they **limit shipyard throughput**. Per ToC: fully utilize the constraint and subordinate every other decision to it → the steel shop's output should be governed by block erection's input requirements.
- **Product-focused cells:** group dedicated steel-shop machines into a **flat-block line** and a **curved-block line** → linear material flow, minimal movement, fewer set-ups — a product layout *inside* the process-focused steel shop. Physical reconfiguration would stall production (two ships underway), so adopt **virtual cells** now (logical grouping, no machine moves) and physically reconfigure during planned shut-downs later.
- **Re-lay-out the process shops:** current material movement is "unnecessarily convoluted." High-flow pairs sit far apart (steel shop → paint shop; pipe shop → sub-assembly; warehouse should be near general purpose/outfitting, not the design office). Need a **scientific method** to measure how far the layout deviates from the ideal **linear flow toward block erection** — but relocation needs considerable investment and top-management approval.

### Central decision
- **Should ABC accept the 5-carrier order (2-year delivery), and how should it raise throughput to deliver?** Specifically: (a) fix the WIP crisis by subordinating steel-shop scheduling to block-erection requirements (Theory of Constraints / Drum-Buffer-Rope); (b) reorganize the steel shop into **product-focused flat/curved cells** (virtual now, physical later); (c) re-lay-out the process shops for shortest-path, near-linear material flow toward the constraint; and **what quantitative method** (from-to / load-distance, relationship chart, Muther's Systematic Layout Planning, plus throughput and WIP analysis) can justify the investment?

### Key takeaways
- **Hybrid layout, friction at the handoff:** process layout fits the high-variety early steel work; fixed position is unavoidable once blocks are too big to move. The problem is coordination between the two, not either layout by itself.
- **Local optimization destroys global throughput:** the steel shop's tonnes-per-day KPI produces the wrong plate mix; the fix is to schedule the steel shop to the block-erection **pull signal** and finish each block completely before starting the next.
- **Theory of Constraints / Drum-Buffer-Rope:** identify the constraint (block erection + dock), exploit it (keep it fully utilized), subordinate upstream to it (release plates only as the constraint consumes), and only then consider elevating it (costly capacity expansion).
- **Mutual benefit for the steel shop:** flat-block and curved-block **cells** cut the biggest set-up (flat↔curved switch), so the shop can serve varying block-erection demand *without* losing throughput — group technology / cellular manufacturing, staged as virtual → physical.
- **Layout method (Muther's SLP):** build a **from-to / relationship chart** of inter-shop flows (Exhibit 3), compute a **load × distance score** for the current layout, generate alternatives placing high-flow pairs adjacent, recompute, and pick the one closest to linear flow.
- **Justify the investment with operational metrics → NPV/payback:** quantify current vs. proposed on (1) load-distance / material-handling cost, (2) set-up hours saved by cells, (3) WIP reduction and freed block-erection space, (4) throughput (ships/year) and cycle-time gain, (5) incremental order capacity and revenue from the booming market — versus the relocation capex.
- **Sequencing under two live ships:** do the zero-capex fixes first (ToC scheduling, virtual cells, Sudesh–Bidesh information sharing), capture the throughput gain, then phase physical cells and shop relocations into planned shut-downs.
