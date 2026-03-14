# Company Cadences

> The structural rhythms that shape how the organization's year runs — fiscal boundaries, release philosophy, planning cycles, sales and marketing patterns, and the recurring pressures that affect team capacity. This document is evergreen: it captures how the organization operates year over year, not what is happening in any specific year.
>
> **Consult this document when** evaluating whether an initiative fits the organization's natural rhythm, understanding the structural constraints on timing, or creating a new Calendar-YYYY for an upcoming fiscal year. The cadences here are the template that each annual calendar is built from.
>
> Specific confirmed dates, this year's events, and the annual at-a-glance view live in **Calendar-[YYYY].md** — one file per fiscal year, created from this document at the start of each year.

---

## Document Control

| Field | Value |
|---|---|
| **Last Updated** | YYYY-MM-DD |
| **Updated By** | |
| **Review Cadence** | When organizational rhythms change — fiscal year structure, release model, planning cycle, or board cadence; not on an annual schedule |
| **Primary Owner** | [e.g., COO / Chief of Staff / Operations] |

> **Connected artifacts:**
> - **Calendar-[YYYY]** — the annual instance built from these cadences; one file per fiscal year in the Rhythm-and-Calendar folder
> - **Business-Case** — initiative timing should be evaluated against the capacity pressure patterns here and confirmed dates in the relevant Calendar-YYYY
> - **Product-Build-Record** — launch windows and freeze periods here inform the Dependencies and Constraints section
> - **Organizational-Risk-and-Compliance** — compliance filing windows and audit cadences here should be consistent with the obligations register there
> - **People-and-Talent-Strategy** — hiring cycles and performance review windows here affect capacity planning there
> - **Strategy-and-Intent** — planning cycle cadence here should align with the goal review rhythm there


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 For Initiative Timing

This document answers structural timing questions — the ones that are true every year regardless of specific dates:

| Question | Where to Look |
|---|---|
| When does the organization's fiscal year start and end, and how does that affect budget availability? | Section 2.1 |
| When does the product team freeze releases, and how often do major releases happen? | Section 3.1 and 3.2 |
| When is the sales team at capacity and unavailable for internal asks? | Section 5.1 |
| When do enterprise customers typically renew, and how does that affect CS capacity? | Section 4.2 |
| When is leadership at reduced operational capacity due to planning or board cycles? | Sections 2.3 and 6.1 |
| What is the typical pattern of organizational pressure across the fiscal year? | Section 7 |

For specific confirmed dates in the current or upcoming year, see Calendar-[YYYY].md.

### 1.2 For Creating a New Annual Calendar

At the start of each fiscal year, use this document as the template for Calendar-[YYYY].md:
- Carry forward the fiscal structure from Section 2.1
- Populate confirmed event dates from Section 4.1 (industry events) and Section 5.2 (marketing campaigns) as they are known
- Use the capacity pressure patterns from Section 7 as the starting point for the annual capacity summary
- Add year-specific events, releases, and dates as they are confirmed

---

## 2. Fiscal and Financial Cadences

> The financial boundaries and internal reporting rhythms that govern how the organization plans, allocates resources, and measures performance. These are structural — they change only when the organization deliberately changes its fiscal or governance structure.

### 2.1 Fiscal Year Structure

| Field | Value |
|---|---|
| **Fiscal year start** | [e.g., November 1] |
| **Fiscal year end** | [e.g., October 31] |
| **Fiscal quarters** | [e.g., Q1: Nov–Jan / Q2: Feb–Apr / Q3: May–Jul / Q4: Aug–Oct] |
| **Budget cycle** | [e.g., Budget planning begins 8 weeks before fiscal year end; approved by board at final board meeting of the fiscal year] |
| **Financial close** | [e.g., Monthly close by the 10th of the following month; annual close within 30 days of fiscal year end] |

**Why this matters for initiative timing:**
[e.g., Initiatives requiring budget approval above $X must be included in the annual budget cycle or require a mid-year budget amendment — which requires board approval and adds 4–6 weeks to the timeline. Initiatives approved in Q4 frequently slip to Q1 due to budget transition and team reset.]

### 2.2 Financial Close Windows

> Periods when Finance team capacity is significantly reduced. Avoid scheduling major initiative reviews or launches that require Finance involvement during these windows.

| Close Type | Typical Window | Capacity Impact | Notes |
|---|---|---|---|
| [e.g., Monthly close] | [e.g., First 10 days of each month] | [e.g., Finance at reduced capacity for ad hoc requests] | [e.g., Invoices must be submitted by the 5th] |
| [e.g., Annual close] | [e.g., First 30 days after fiscal year end] | [e.g., Finance fully committed — no bandwidth for new initiatives] | |
| [e.g., Annual audit] | [e.g., Q4 — typically 2 weeks] | [e.g., Finance and Legal unavailable — no infrastructure changes] | [e.g., See Organizational-Risk-and-Compliance for audit schedule] |
| [e.g., Budget planning] | [e.g., Q4 — 8 weeks before fiscal year end] | [e.g., Leadership bandwidth significantly reduced] | [e.g., Department heads preparing submissions] |

### 2.3 Board and Investor Reporting Cadence

| Meeting / Report | Frequency | Typical Timing | Owner | Capacity Impact | Notes |
|---|---|---|---|---|---|
| [e.g., Board meeting] | [Quarterly] | [e.g., Third week of the month following quarter end] | [CEO / CFO] | [e.g., Leadership bandwidth consumed for 1 week prior — avoid major approvals] | |
| [e.g., Investor update] | [Monthly] | [e.g., First week of each month] | [CEO / CFO] | [Low] | [e.g., Requires metrics package from Finance] |
| [e.g., Annual investor meeting] | [Annual] | [e.g., Early in new fiscal year — typically November] | [CEO] | [High — full preparation week] | |

---

## 3. Product and Release Cadences

> The product team's release philosophy and the structural freeze periods that apply every year. Specific release dates and this year's planned features live in Calendar-[YYYY].md.

### 3.1 Release Philosophy

**Release model:** [e.g., Continuous delivery with monthly milestone releases / Quarterly major releases / Event-driven releases tied to market moments]

**Release cadence:** [e.g., Minor releases: bi-weekly / Major releases: quarterly / Hotfixes: as needed with expedited review]

**Typical release window:** [e.g., Releases deploy Tuesday–Thursday; no Friday or weekend deploys except for critical hotfixes]

**Why this matters for initiative timing:**
[e.g., A feature that misses the Q2 major release window will not ship until Q3 unless it qualifies for a minor release. Plan initiative timelines to account for release windows — not just build completion.]

### 3.2 Structural Freeze Periods

> Recurring periods when code deployments are restricted or prohibited. Specific dates for each year are confirmed in Calendar-[YYYY].md.

| Freeze Type | Typical Timing | Scope | Reason | Exceptions |
|---|---|---|---|---|
| [e.g., Holiday freeze] | [e.g., ~2 weeks spanning late December and early January] | [e.g., No production deploys] | [e.g., Reduced on-call capacity; high customer usage period] | [e.g., Critical security patches only — requires VP Engineering approval] |
| [e.g., Conference freeze] | [e.g., 1 week prior to and during major industry conference] | [e.g., No major feature releases] | [e.g., Stability during high-visibility period; go-to-market team focused on event] | [e.g., Hotfixes only] |
| [e.g., Audit freeze] | [e.g., Annual audit window — typically Q4] | [e.g., No infrastructure changes] | [e.g., Auditors require stable environment for evidence collection] | [e.g., None — no exceptions during audit] |

### 3.3 Infrastructure Maintenance Windows

| Maintenance Type | Typical Timing | Impact | Owner | Notes |
|---|---|---|---|---|
| [e.g., Cloud provider maintenance] | [e.g., First Sunday of each month, 2–4am] | [e.g., Potential 30-min service interruption] | [Engineering] | [e.g., Customers notified 72 hours in advance] |
| [e.g., Planned migrations] | [e.g., Scheduled as needed — announced 4 weeks prior] | [e.g., Read-only or downtime window] | [Engineering] | [e.g., Requires release freeze for 2 weeks surrounding migration] |

---

## 4. Industry and Market Cadences

> Recurring external events and customer patterns that shape the market environment. The organization does not control these — but they create predictable windows of opportunity and pressure that product, sales, and marketing activities should be planned around.

### 4.1 Recurring Industry Events

> The events the organization participates in year over year. Specific dates for each year are confirmed in Calendar-[YYYY].md.

| Event | Type | Typical Timing | Organizational Role | Strategic Importance | Notes |
|---|---|---|---|---|---|
| [e.g., Primary industry conference] | [Conference / Trade show] | [e.g., Annually — February] | [e.g., Exhibiting — booth / Speaking / Attending] | [e.g., Highest lead generation event of year — product releases should be stable 3 weeks prior] | |
| [e.g., Regional conference] | [Conference] | [e.g., Annually — May] | [e.g., Sponsoring] | [e.g., Strong presence in key customer segment] | |
| [e.g., Partner summit] | [Partner event] | [e.g., Annually — September] | [e.g., Attending] | [e.g., Medium — relationship maintenance] | |
| [e.g., Customer advisory board] | [Customer event] | [e.g., Annually — Q3] | [e.g., Hosting] | [e.g., High — product roadmap input and reference customer engagement] | |
| [e.g., Analyst briefing cycle] | [Analyst] | [e.g., Semi-annual — typically March and September] | [e.g., Briefing and inquiry sessions] | [e.g., Critical for enterprise sales cycle — evaluation timing affects deals] | |

### 4.2 Customer Renewal Patterns

> When customers tend to renew — by segment. Renewal clusters create predictable CS and Sales pressure that affects capacity for other work.

| Segment | Renewal Pattern | Peak Renewal Window | Capacity Impact | Notes |
|---|---|---|---|---|
| [e.g., Enterprise] | [e.g., Annual — aligned to customer fiscal year] | [e.g., January and July] | [e.g., CS team at 80%+ capacity during peak renewal months] | [e.g., Majority of enterprise contracts close in Q1 and Q3 of our fiscal year] |
| [e.g., Mid-market] | [e.g., Annual — contract anniversary] | [e.g., Spread throughout year — slight Q2 concentration] | [e.g., Moderate — no single peak] | |
| [e.g., SMB] | [e.g., Monthly] | [e.g., Ongoing] | [e.g., Low per-renewal; largely automated] | |

---

## 5. Sales and Marketing Cadences

> Recurring sales and marketing cycles. These affect team capacity and create windows where new initiatives land well or poorly.

### 5.1 Sales Rhythms

| Rhythm | Frequency | Typical Timing | Capacity Impact | Notes |
|---|---|---|---|---|
| [e.g., Sales kickoff] | [Annual] | [e.g., First week of fiscal year] | [High — sales team fully committed 3–5 days] | [e.g., No external meetings scheduled during SKO] |
| [e.g., Quarterly business review] | [Quarterly] | [e.g., First two weeks of each quarter] | [Medium — sales leadership bandwidth consumed] | [e.g., Pipeline review and forecast] |
| [e.g., End of quarter push] | [Quarterly] | [e.g., Final 2 weeks of each quarter] | [High — sales team fully focused on closing] | [e.g., Avoid new internal asks during this window] |
| [e.g., Pipeline review] | [Weekly] | [e.g., Mondays] | [Low] | |

### 5.2 Marketing Campaign Rhythms

> Recurring campaign types and their typical position in the year. Specific campaigns and dates for each year are confirmed in Calendar-[YYYY].md.

| Campaign Type | Typical Frequency | Typical Window | Teams Involved | Notes |
|---|---|---|---|---|
| [e.g., Annual product launch campaign] | [Annual] | [e.g., Aligned to major Q2 release] | [Marketing, Product] | [e.g., Requires product stable in production 3 weeks prior] |
| [e.g., Conference lead nurture] | [Annual] | [e.g., 6 weeks post-primary conference] | [Marketing, Sales] | [e.g., Highest-ROI demand generation window of year] |
| [e.g., End-of-year promotion] | [Annual] | [e.g., November–December] | [Marketing, Sales] | [e.g., Targets prospects with budget to spend before calendar year end] |
| [e.g., Customer case study program] | [Quarterly] | [e.g., One published per quarter] | [Marketing, CS] | [e.g., Requires reference customer coordination — see Reference-Customers-and-Champions] |

### 5.3 Partner and Channel Cadences

| Activity | Frequency | Typical Window | Owner | Notes |
|---|---|---|---|---|
| [e.g., Partner program review] | [Annual] | [e.g., Q4] | [Partnerships] | [e.g., Annual review of partner tier, compensation, and co-marketing commitments] |
| [e.g., Partner enablement training] | [Semi-annual] | [e.g., Q1 and Q3] | [Partnerships / Sales] | [e.g., New product features and updated sales materials] |

---

## 6. Organizational Cadences

> Internal recurring rhythms that shape team capacity — planning cycles, company events, and people processes.

### 6.1 Planning Cycles

| Planning Event | Frequency | Typical Window | Capacity Impact | Notes |
|---|---|---|---|---|
| [e.g., Annual strategic planning] | [Annual] | [e.g., Q4 — 6 weeks before fiscal year end] | [High — leadership at significantly reduced operational capacity] | [e.g., Defer major approvals during this window] |
| [e.g., Quarterly OKR / goal review] | [Quarterly] | [e.g., Final week of each quarter] | [Medium — leadership bandwidth] | |
| [e.g., Product roadmap planning] | [Semi-annual] | [e.g., Q2 and Q4] | [Medium — product and cross-functional input] | [e.g., Roadmap inputs due from all departments 2 weeks prior] |
| [e.g., Annual budget planning] | [Annual] | [e.g., Q4 — runs concurrently with strategic planning] | [High — all department heads involved] | |

### 6.2 Company Events

| Event | Frequency | Typical Timing | Capacity Impact | Notes |
|---|---|---|---|---|
| [e.g., All-hands meeting] | [Monthly] | [e.g., Last Thursday of each month] | [Low — 1–2 hours] | [e.g., No competing meetings scheduled] |
| [e.g., Annual company offsite] | [Annual] | [e.g., Q3 — July or August] | [High — full company 3 days] | [e.g., Engineering sprint planning deferred by 1 week] |
| [e.g., Department offsites] | [Annual per department] | [e.g., Staggered Q2 and Q3] | [Medium per department] | |

### 6.3 People and HR Cadences

| Event | Frequency | Typical Window | Capacity Impact | Notes |
|---|---|---|---|---|
| [e.g., Performance review cycle] | [Annual] | [e.g., Q4 — ahead of fiscal year] | [High — manager bandwidth significantly reduced] | [e.g., Avoid major project asks during review period] |
| [e.g., Compensation review] | [Annual] | [e.g., Tied to performance review] | [Medium — HR and Finance] | |
| [e.g., Benefits open enrollment] | [Annual] | [e.g., Q4 — typically October] | [Low] | |
| [e.g., Summer hiring slowdown] | [Annual — if applicable] | [e.g., July–August] | [Medium — reduced recruiting capacity] | [e.g., Plan critical hires for Q2 or Q4 if possible] |

---

## 7. Capacity Pressure Patterns

> A structural summary of when organizational capacity is most constrained — year over year, regardless of specific dates. Use this as the starting point for the capacity pressure summary in each Calendar-[YYYY].md.
>
> These patterns are based on the cadences above. When a year has an unusual concentration of events, the annual calendar may show higher pressure than the typical pattern suggests.

| Period | Teams Typically Affected | Typical Pressure | Driver | Notes |
|---|---|---|---|---|
| [e.g., First week of fiscal year] | [Sales] | [High] | [Sales kickoff] | [e.g., Sales team fully committed — no external meetings or internal asks] |
| [e.g., Primary conference week + 1 week prior] | [Sales, CS, Marketing, Executive] | [High] | [Industry conference] | [e.g., Entire go-to-market team at conference; no capacity for launches or major reviews] |
| [e.g., Enterprise renewal peaks — Jan and Jul] | [CS] | [High] | [Customer renewals] | [e.g., CS at capacity — avoid CS-dependent launches] |
| [e.g., End of each quarter — final 2 weeks] | [Sales] | [Medium–High] | [Quarter-end push] | [e.g., Sales fully focused on closing; avoid new internal asks] |
| [e.g., Q4 — strategic planning + budget + audit] | [Leadership, Finance, Legal] | [High] | [Concurrent year-end processes] | [e.g., Leadership bandwidth at annual low — major decisions should come earlier in the year] |
| [e.g., Q3 — company offsite + summer PTO] | [All] | [Medium] | [Offsite + vacation] | [e.g., Plan around offsite dates confirmed in Calendar-YYYY] |
| [e.g., Monthly close — first 10 days of month] | [Finance] | [Medium] | [Financial close] | [e.g., Finance unavailable for ad hoc requests] |

---

## 8. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there recurring cadences not captured here that affect team capacity in predictable ways?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., Are the capacity pressure patterns in Section 7 accurate relative to how the year actually feels? Has the team validated them?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Are there partner or channel cadences not captured in Section 5.3?] | [Name] | YYYY-MM-DD | |
