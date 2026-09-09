---
course: Operations_Management_I
type: case-notes
title: "Tastee Snax Cookie Company (A) — Notes"
source: https://hbsp.harvard.edu/tu/cea2e128
product_id: UV5918 — Darden
tags: [case-notes, operations_management_i, project-management, cpm, critical-path, scheduling]
---

# Tastee Snax Cookie Company (A) — Notes

📄 Case PDF: [[Tastee_Snax_Cookie_Company_A.pdf]]

## Quick Read
> Darden case. **Kevin Lindeman**, VP Marketing of **Tastee Snax** (a regional southeastern US baked-goods snack maker), must get a **no-fat cookie** to market fast — the company's share has fallen sharply after negative fat-consumption press and heavy no-fat advertising by national rivals, and the traditional 24-month new-product cycle would leave Tastee Snax "irretrievably behind." **Bill Hamilton**, a business-school grad, recommends **Critical Path Methodology (CPM)** for its cross-department coordination and per-department project coordinators. Lindeman puts **Katy Motte** on it; she collects task times and predecessors across R&D/Manufacturing, Marketing, and Advertising & Promotion, builds three sub-networks, consolidates them, and runs forward/backward passes to get start/finish times and slack (**Exhibit 1**). The class task: build the CPM network, find the critical path and project duration, and decide how to schedule (and possibly compress) the launch.

## Case Notes

### Setup
- Three components: **(A) R&D/Manufacturing**, **(B) Marketing**, **(C) Advertising & Promotion** — total 25 activities in Exhibit 1, each with a duration (weeks), immediate predecessors, and computed slack.
- CPM's stated benefits (Hamilton): forces departments to **agree on tasks, durations, dependencies and hand-offs at the planning stage**; each department names a **project coordinator** accountable for its tasks; the network then serves as a communication and progress-monitoring tool.

### Exhibit 1 — key activities (duration wks; predecessors)
- **A2** Complete product development (5; A1, B1) · **A4** Prepare manufacturing specifications (6; A3, B6) · **A5** Produce for test market (4; A4) · **A6** Order special equipment (1; A4, B11) · **A7** Receive & install special equipment (6; A6) · **A8** Produce product (6; A7)
- **B1** Perform focus group (3; none) · **B5** Perform taste test (4; A2, B4) · **B6** Review results & choose product (4; B5) · **B9** Run test market (8; A5, B3, B8) · **B11** Evaluate test-market results financially (5; B9)
- High-slack items: **B7** pricing/volume analysis (7; none) — **15 weeks slack**; B10 awareness study — 6; B12 national marketing plan — 5; most Advertising activities (C1–C5) — 3–8 weeks slack.

### Critical path (forward/backward pass on Exhibit 1)
**B1 → A2 → B5 → B6 → A4 → A5 → B9 → B11 → A6 → A7 → A8**
= 3 + 5 + 4 + 4 + 6 + 4 + 8 + 5 + 1 + 6 + 6 = **≈ 52 weeks (~12 months)**

- Front end (development → taste test → specs → test-market production): B1→A2→B5→B6→A4→A5 = 26 weeks.
- Back end (test market → serial equipment chain): B9 (8) → B11 (5) → A6 (1) → A7 (6) → A8 (6) = 26 weeks.
- **A5 "produce for test market" is critical** because B9 (run test market) needs it and it is driven by A4.
- vs. the traditional **24-month** cycle, CPM shows the launch is feasible in **~1 year** by running the R&D, marketing and advertising streams **in parallel** rather than sequentially — so Lindeman's fear is answerable: with disciplined project planning Tastee Snax can compete in the no-fat market.

### Central decision
- **Build the CPM network from Exhibit 1**, compute ES/EF, LS/LF and slack, identify the **critical path and ~52-week duration**, and use it to decide: (a) can Tastee Snax launch fast enough to compete; (b) where to concentrate management attention (critical-path activities, especially the long ones — B9 test market 8, A4/A7/A8 at 6 each, A2/B11 at 5); and (c) whether/how to **crash or overlap** activities to compress the schedule further — while using CPM to enforce cross-department coordination.

### Key takeaways
- **CPM mechanics:** activities + durations + immediate predecessors → network; **forward pass** for earliest start/finish (ES = max EF of predecessors); **backward pass** for latest start/finish (LF = min LS of successors); **slack = LS − ES = LF − EF**; the **critical path** is the longest path / the zero-slack chain and sets the minimum project duration.
- **Where the time is:** the critical path is dominated by the 8-week test market and the **serial post-test-market equipment chain** (financial evaluation → order → 6-week install → 6-week production). Non-critical work (pricing analysis with 15 weeks slack, awareness study, national plan, most advertising) can slip within its float without moving the finish.
- **Compression options (fast-tracking / crashing):**
  - **Order the special equipment (A6/A7) before the test-market financial evaluation (B11)**, accepting the risk the product might not proceed — removes ~7 weeks of the ~7-week equipment lead from the end of the project.
  - **Shorten or run a smaller/faster test market (B9)** — directly shortens the critical path.
  - Legal approval (B3) already overlaps packaging development (non-critical) — verify it stays off the path.
  - Crashing adds cost and risk (committing to equipment/tooling pre-results); trade that against the value of earlier entry into a fast-growing category.
- **Watch near-critical paths:** the B2→B3 packaging/legal chain has only 3 weeks of slack — if it slips, the critical path shifts.
- **Estimation caveat:** durations are single-point estimates — **PERT / three-point estimates** would capture uncertainty and give a probability distribution for the completion date.
- **Reconcile the data:** the prose description and Exhibit 1 in the case are deliberately not fully consistent — check each activity's predecessors and duration against the worksheet before trusting the network.
- **Organizational value:** CPM's main payoff here is forcing R&D, Marketing and Advertising to negotiate a single integrated plan up front, with named coordinators accountable for on-time delivery.
