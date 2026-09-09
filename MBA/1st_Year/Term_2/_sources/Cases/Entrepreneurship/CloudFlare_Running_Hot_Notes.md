---
course: Entrepreneurship
type: case-notes
title: "CloudFlare, Inc.: Running Hot — Notes"
source: https://hbsp.harvard.edu/tu/21799197
product_id: 9-813-145 (HBS)
tags: [case-notes, entrepreneurship, scaling, org-design]
---

# CloudFlare, Inc.: Running Hot — Notes

📄 Case PDF: [[CloudFlare_Running_Hot.pdf]]

## Quick Read
> HBS case (Eisenmann & Godden). July 2012. CloudFlare (founded 2009; SF; protects and speeds up websites via a global CDN + security network) is growing explosively — 2B+ page views/day (~1% of the internet), ~500k customer sites — with just **35 employees, 26 of them engineers**, no sales team, no HR function, no titles, and a deliberately flat, self-directed culture. But a **fifth employee in three months has just resigned**. Co-founders **Matthew Prince (CEO)**, **Michelle Zatlyn**, and **Lee Holloway** must decide whether this is normal attrition for a hot startup or a signal that the culture, structure and management practices that built the team now need to change as CloudFlare scales — and how Prince's own always-on style fits.

## Case Notes

### Key facts
- **Scale vs. headcount:** ~500k websites, 550M unique monthly visitors, 2B+ daily page views, servers in 17 data centers — run by **35 people (26 engineers)**. Site loads ~2x faster and uses ~60% less bandwidth with CloudFlare.
- **Business model:** ~95% of revenue from subscriptions (Free / Pro $20 / Business $200 / Enterprise $3,000+ per month), rest from ads on CAPTCHA "challenge" pages. **~4% of customers pay.** Revenue run-rate ~$4.8M; estimated costs ~$7.85M (infra ~$2.6M + ~$150k/employee) → **~$3M annual loss** at current scale. Rumored $1B valuation (spring 2012); next raise expected within a year, no urgent cash need.
- **Funding history:** won HBS Business Plan Contest 2009 → $2.05M Series A (Venrock, Pelion, Nov 2009) → launched at TechCrunch Disrupt Oct 2010 → $20M Series B (NEA, Venrock, Pelion, Nov 2010).
- **Strategy / tech philosophy:** target the "long tail" of SMB sites priced out of Akamai/Limelight/Barracuda; grow via word-of-mouth + ~hundreds of hosting-company resale deals (GoDaddy, HostMonster ≈ 25% of customers). Prince deliberately **"runs near capacity limits"** so crises force proprietary software fixes rather than "throwing money at problems" — filing a patent roughly every 3 weeks (Railgun, etc.).
- **Org design:** no titles, no reporting lines, no roadmap; priorities set on Post-it notes, reset at a whole-company meeting **every Friday at 5 p.m.** Just hired product engineer **Dane Knecht** ("not a manager — I want engineers assisted, not managed"). No HR: ad hoc raises, unstructured hiring ("we're terrible at follow-up"), no onboarding. Distinguishes **need-based** vs. **opportunity-based** hires.
- **The five resignations (patterns, not just anecdotes):**
  1. **Dale Kiefling** (tech ops): pager every ~8 min, 24/7; a 2-person team; impossible hiring bar; new baby; quit just short of 1-year option vesting — "not sustainable."
  2. **David Conrad** (opportunity hire; ex-CTO Nominum; ICANN/ARIN/APNIC/ISC): no defined role; wanted structure, process, redundancy that founders resisted; felt underutilized; quit just before vesting.
  3. **David Zakur** (36, two kids, family on East Coast, long commute): hired for ad monetization that "never took off"; couldn't get buy-in; the Friday 5 p.m. ritual "brutal" for family life.
  4. A **burned-out jack-of-all-trades engineer**: work kept piling on; Prince offered a 2-month sabbatical; still contributing, expected to return.
  5. An **engineer** who wanted a bigger team and management responsibility he wouldn't get; disagreed with Prince on strategy/staffing.

### Central decision
- **Is the loss of five people natural attrition or a warning sign?** What, if anything, should change in CloudFlare's culture, organizational structure, and management processes as it scales — and can those changes be made **without undermining** the brilliant, self-directed, mission-driven engineering culture? Is CloudFlare hiring the wrong kinds of people? And how should Prince's own management style adapt, and how should he communicate whatever he decides?

### Key takeaways
- **The exits rhyme:** chronic understaffing of 24/7 ops ("running hot"), opportunity hires with no real mandate, senior people wanting process the founders won't grant, a strategy ("poke the giant, don't monetize yet") that frustrates people hired to build now, and rigid rituals that penalize anyone not young, single and local. Near-vest departures are a loud workload/satisfaction signal.
- **Flat works at 15, frays at 35→70:** likely needs a thin "middle layer" *across* functions (not just in engineering), light-touch HR (handbook, review cadence, onboarding), and basic office IT — introduced bottom-up so it doesn't calcify into bureaucracy.
- **"Run hot" is a real innovation strategy** (forces automation, generates defensible IP) but has a human cost; separate *productive constraint* from *unsustainable understaffing* and staff critical ops (a proper NOC, Asia coverage) before people break.
- **Founder-CEO self-awareness:** Prince's no-vacation, always-on example sets the norm that pushes others out; he is "the last to know when something's wrong" and needs deliberate feedback channels (Michelle, Dane as go-between) and to visibly model sustainable behavior.
- **Hiring discipline:** keep opportunity hires (they bring ideas like lazy-loading images) but give each a concrete problem to own; be candid in interviews that a role "may be premature"; fix follow-up and onboarding.
