# Metrics Framework

> The authoritative reference for what the organization formally measures — what each metric means precisely, where it comes from, and who sees it. This document covers metrics that derive from formal systems. Locally calculated figures, informal scorecards, and ad hoc analyses are not captured here — if a metric matters enough to inform decisions, it belongs in a system and in this register.
>
> **This document works in conjunction with Systems-and-Data**, which defines the underlying entities and systems that metrics are built on. Metric definitions here reference entity definitions there — they do not duplicate them. When a metric and its source entity disagree, the Systems-and-Data entity definition and System of Record designation take precedence.
>
> **Everything in this document is a measure, not a target.** Targets live in Strategy-and-Intent, where OKRs and goals are defined. When an OKR references a metric from this register, that connection is made there — not here. Keeping targets out of this document prevents the same number from living in two places and drifting apart. Metric records here include a reference field pointing to any Strategy-and-Intent goal that uses them — one directional pointer, no duplication.

---

## Document Control

| Field | Value |
|---|---|
| **Last Updated** | YYYY-MM-DD |
| **Updated By** | |
| **Review Cadence** | Register: quarterly / Metric records: when definitions or sources change / Visibility matrix: when org structure changes |
| **Primary Owner** | [e.g., CFO / VP Finance / Head of Data / COO] |

> **Connected artifacts:**
> - **Systems-and-Data** — all metrics reference a source system and entity definition from that document; data conflicts that affect metric values should be logged in the Conflict and Exception Log there
> - **Strategy-and-Intent** — OKRs and goals that use a metric as a success measure reference the metric ID here; that connection is made there, not here; metric records include a one-way reference field to the relevant goal
> - **Cost-and-Benefit-Framework** — benefit estimates reference metrics here for baseline values and expected post-initiative movement
> - **Product-Build-Record** — success metrics in Section 2.3 should use metrics defined here; benefit realization in Section 14.3 measures actuals against those definitions
> - **Internal-Stakeholders** — metric ownership and visibility align to the org structure captured there; department-level metrics map to the functions defined there
> - **Funding-and-Business-Model** — unit economics and financial health metrics here should be consistent with the financial snapshot there


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 Finding a Metric

The Metrics Register (Section 3) is the single-view reference. It is organized by category — Financial, Customer, Product, Sales, People, Operations. Use the category sections to browse within a domain. Use the Visibility and Access Matrix (Section 5) to understand who sees which categories.

For precise definitions and calculation methodology, follow the record reference in the register to the full Metric Record in Section 4.

### 1.2 Adding a Metric

A metric belongs in this register when:
- It derives from a formal system catalogued in Systems-and-Data
- It is used in regular reporting, dashboards, or business reviews
- It is referenced in a Business Case, Product Build Record, or OKR
- Its definition is disputed or ambiguous enough that a shared definition would prevent disagreement

A metric does not belong here if it is calculated locally by an individual, pulled ad hoc without a defined methodology, or not reproducible from a named system.

**When adding a metric:** confirm the source system is in the Systems-and-Data registry, confirm the entity definition exists or add it there, then add the metric to the register and create a full record if warranted.

### 1.3 Metric Levels

Metrics are assigned a level that reflects the organizational scope at which they are primarily used. Levels align to the org structure in Internal-Stakeholders.

| Level | Description | Examples |
|---|---|---|
| **Company** | Metrics reported at the organizational level — used in board reporting, investor updates, and company-wide reviews | ARR, headcount, NPS |
| **Executive** | Metrics used by the executive team for cross-functional decision-making — may not be broadly distributed | Gross margin, burn rate, runway |
| **Department** | Metrics owned and primarily used within a specific function | Sales pipeline coverage, feature adoption rate, support SLA compliance |
| **Team** | Metrics used within a sub-team or squad for operational management | Sprint velocity, individual quota attainment, ticket resolution time by agent |

A metric can appear at multiple levels — ARR is a Company metric that is also an Executive metric. When it does, visibility is determined by the most restrictive level it appears at.

### 1.4 Visibility

Visibility defines who is permitted to see a metric. It may be narrower than the level suggests — an Executive-level metric may be visible only to the Executive team even if the Finance department has adjacent interest. Visibility is governed by the matrix in Section 5 and should be enforced in dashboards and reporting tools.

---

## 2. Metric Taxonomy

> The organization's classification of metrics by category and the department ownership that determines who governs each. Align department names to the org structure in Internal-Stakeholders.

| Category | Description | Primary Owner (Department) | Key Consumers |
|---|---|---|---|
| **Financial** | Revenue, cost, margin, cash, and unit economics | Finance | Executive, Board, Product, Sales |
| **Customer** | Acquisition, retention, satisfaction, and lifetime value | Customer Success / Sales | Executive, Sales, Marketing, Product |
| **Product** | Usage, adoption, activation, retention, and feature engagement | Product | Product, Engineering, Executive |
| **Sales** | Pipeline, conversion, velocity, and quota attainment | Sales | Executive, Sales, Finance |
| **People** | Headcount, hiring, attrition, and capacity | HR / People | Executive, Department heads |
| **Operations** | Process performance, system reliability, and operational efficiency | Operations / Engineering | Executive, Operations, Engineering |

---

## 3. Metrics Register

> One row per metric. Organized by category. Full records in Section 4 for metrics that warrant detailed documentation.
>
> **The entries below are illustrative examples.** They demonstrate the structure and the kinds of metrics organizations commonly track — they are not a prescribed set. Replace them entirely with the metrics your organization actually measures. The register is only valuable when it reflects what the organization genuinely uses, not a generic list of industry-standard metrics.

### 3.1 Financial Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-F001 | MRR (Monthly Recurring Revenue) | Company | Executive, Finance, Sales leadership | | [e.g., Stripe — SYS-002] | [MRR — S&D 4.2] | Sum of normalized monthly value of all active subscriptions as of measurement date | Finance | Full |
| MET-F002 | ARR (Annual Recurring Revenue) | Company | Executive, Finance, Sales leadership | | [e.g., Stripe — SYS-002] | [ARR — S&D 4.2] | MRR × 12 | Finance | Full |
| MET-F003 | Net Revenue Retention (NRR) | Company | Executive, Finance | | [e.g., Stripe — SYS-002] | [NRR — S&D 4.2] | (Starting MRR + expansion − contraction − churn) ÷ Starting MRR × 100 | Finance | Full |
| MET-F004 | Gross Revenue Retention (GRR) | Company | Executive, Finance | | [e.g., Stripe — SYS-002] | [Active Customer — S&D 4.2] | (Starting MRR − contraction − churn) ÷ Starting MRR × 100 | Finance | Full |
| MET-F005 | Gross Margin | Executive | Executive only | | [e.g., NetSuite — SYS-004] | [Revenue, COGS — S&D 4.2] | (Revenue − COGS) ÷ Revenue × 100 | Finance | Full |
| MET-F006 | Burn Rate | Executive | Executive only | | [e.g., NetSuite — SYS-004] | | Net cash consumed per month | Finance | Summary |
| MET-F007 | Runway | Executive | Executive only | | [e.g., NetSuite — SYS-004] | | Cash on hand ÷ Monthly burn rate | Finance | Summary |
| MET-F008 | CAC (Customer Acquisition Cost) | Executive | Executive, Finance, Sales leadership | | [e.g., NetSuite + HubSpot] | [Customer — S&D 4.2] | Total sales and marketing spend ÷ New customers acquired in period | Finance / Sales | Full |
| MET-F009 | LTV (Customer Lifetime Value) | Executive | Executive, Finance, Sales leadership | | [e.g., Stripe + NetSuite] | [Active Customer, MRR — S&D 4.2] | Average MRR per customer ÷ Monthly churn rate × Gross margin % | Finance | Full |
| MET-F010 | LTV:CAC Ratio | Executive | Executive, Finance | | Derived | [MET-F009, MET-F008] | LTV ÷ CAC | Finance | Summary |

### 3.2 Customer Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-C001 | Active Customer Count | Company | Company-wide | | [e.g., Stripe — SYS-002] | [Active Customer — S&D 4.2] | Count of accounts with active or past-due subscription status as of measurement date | CS / Finance | Full |
| MET-C002 | Customer Churn Rate (Logo) | Company | Executive, CS, Finance | | [e.g., Stripe — SYS-002] | [Churned Customer — S&D 4.2] | Customers lost in period ÷ Customers at start of period × 100 | CS / Finance | Full |
| MET-C003 | MRR Churn Rate | Company | Executive, Finance | | [e.g., Stripe — SYS-002] | [MRR — S&D 4.2] | MRR lost to churn in period ÷ MRR at start of period × 100 | Finance | Full |
| MET-C004 | NPS (Net Promoter Score) | Company | Company-wide | | [e.g., Survey platform — SYS-XXX] | | (% Promoters − % Detractors) | CS | Full |
| MET-C005 | CSAT (Customer Satisfaction) | Department — CS | CS, Product, Executive | [e.g., Zendesk — SYS-006] | | Average satisfaction score on closed tickets in period | CS | Summary |
| MET-C006 | Time to First Value | Department — CS / Product | CS, Product | [e.g., Product DB — SYS-003 + Stripe] | [Active Customer — S&D 4.2] | Days from subscription start to first qualifying product action | CS / Product | Full |
| MET-C007 | Expansion MRR | Company | Executive, Finance, CS | | [e.g., Stripe — SYS-002] | [MRR — S&D 4.2] | MRR added from existing customers (upsell, cross-sell, seat expansion) in period | CS / Sales | Summary |

### 3.3 Product Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-P001 | Monthly Active Users (MAU) | Company | Company-wide | | [e.g., Mixpanel — SYS-007] | [Active User — S&D 4.2] | Count of unique users performing a qualifying action in the calendar month | Product | Full |
| MET-P002 | Daily Active Users (DAU) | Department — Product | Product, Engineering | [e.g., Mixpanel — SYS-007] | [Active User — S&D 4.2] | Count of unique users performing a qualifying action on a given day | Product | Summary |
| MET-P003 | DAU/MAU Ratio (Stickiness) | Department — Product | Product, Executive | Derived | [MET-P002, MET-P001] | DAU ÷ MAU × 100 | Product | Summary |
| MET-P004 | Feature Adoption Rate | Department — Product | Product, CS | [e.g., Mixpanel — SYS-007] | [Feature Adoption — S&D 4.2] | Users who have adopted feature ÷ Eligible users × 100 | Product | Full |
| MET-P005 | Activation Rate | Department — Product | Product, CS, Executive | [e.g., Mixpanel + Stripe] | [Active User, Active Customer — S&D 4.2] | New customers completing activation milestone within defined window ÷ New customers in period × 100 | Product | Full |
| MET-P006 | User Retention (D30 / D90) | Department — Product | Product, Executive | [e.g., Mixpanel — SYS-007] | [Active User — S&D 4.2] | Users active on Day 30/90 after first use ÷ Users who completed first use × 100 | Product | Full |
| MET-P007 | Core Workflow Completion Rate | Department — Product | Product, CS | [e.g., Mixpanel — SYS-007] | | Users completing defined workflow ÷ Users who initiated it × 100 | Product | Summary |

### 3.4 Sales Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-S001 | Pipeline Value | Department — Sales | Sales, Executive, Finance | [e.g., Salesforce — SYS-001] | | Sum of weighted opportunity value across all open stages | Sales | Full |
| MET-S002 | Pipeline Coverage Ratio | Department — Sales | Sales, Executive | [e.g., Salesforce — SYS-001] | | Pipeline value ÷ Revenue target for period | Sales | Summary |
| MET-S003 | Win Rate | Department — Sales | Sales, Executive, Product | [e.g., Salesforce — SYS-001] | | Opportunities won ÷ Opportunities closed (won + lost) × 100 | Sales | Full |
| MET-S004 | Average Contract Value (ACV) | Company | Executive, Sales, Finance | | [e.g., Salesforce — SYS-001] | | Total ARR from new bookings ÷ Number of new customers in period | Sales / Finance | Full |
| MET-S005 | Sales Cycle Length | Department — Sales | Sales, Executive | [e.g., Salesforce — SYS-001] | | Average days from opportunity creation to close (won) | Sales | Summary |
| MET-S006 | Quota Attainment | Department — Sales | Sales leadership, Executive | [e.g., Salesforce — SYS-001] | | Closed ARR ÷ Quota × 100 — by rep and team | Sales | Summary |
| MET-S007 | Lead Conversion Rate | Department — Sales / Marketing | Sales, Marketing | [e.g., HubSpot + Salesforce] | | Leads converted to opportunities ÷ Total leads in period × 100 | Sales / Marketing | Summary |

### 3.5 People Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-HR001 | Total Headcount | Company | Company-wide | | [e.g., Workday — SYS-005] | [Headcount — S&D 4.2] | Count of active employees as of measurement date | HR / Finance | Full |
| MET-HR002 | Headcount by Department | Department | Department heads, Executive, Finance | | [e.g., Workday — SYS-005] | [Headcount, Employee — S&D 4.2] | Count of active employees per department | HR | Summary |
| MET-HR003 | Voluntary Attrition Rate | Executive | Executive, HR | | [e.g., Workday — SYS-005] | [Employee — S&D 4.2] | Voluntary departures in period ÷ Average headcount × 100 | HR | Full |
| MET-HR004 | Time to Fill (Open Roles) | Department — HR | HR, Department heads | [e.g., ATS — SYS-XXX] | | Average days from role opening to accepted offer | HR | Summary |
| MET-HR005 | Offer Acceptance Rate | Department — HR | HR, Executive | [e.g., ATS — SYS-XXX] | | Offers accepted ÷ Offers extended × 100 | HR | Summary |
| MET-HR006 | Revenue per Employee | Executive | Executive, Finance | | Derived | [MET-F002, MET-HR001] | ARR ÷ Total headcount | Finance / HR | Summary |

### 3.6 Operations Metrics

| Metric ID | Metric Name | Level | Visibility | Source System | Entity Reference | Calculation Summary | Owner | Record |
|---|---|---|---|---|---|---|---|---|
| MET-O001 | System Uptime / Availability | Company | Company-wide | | [e.g., Monitoring platform — SYS-XXX] | | (Total time − Downtime) ÷ Total time × 100 | Engineering | Full |
| MET-O002 | Incident Response Time (P1) | Department — Engineering | Engineering, Executive | [e.g., Incident management — SYS-XXX] | | Average time from P1 incident detection to acknowledgment | Engineering | Summary |
| MET-O003 | Support SLA Compliance | Department — CS | CS, Engineering, Executive | [e.g., Zendesk — SYS-006] | | Tickets responded to within SLA ÷ Total tickets in period × 100 | CS | Summary |
| MET-O004 | Deployment Frequency | Department — Engineering | Engineering, Product | [e.g., CI/CD platform — SYS-XXX] | | Count of production deployments per period | Engineering | Summary |
| MET-O005 | Change Failure Rate | Department — Engineering | Engineering, Product | [e.g., CI/CD + Incident management] | | Deployments causing incident or rollback ÷ Total deployments × 100 | Engineering | Summary |
| MET-O006 | Mean Time to Recovery (MTTR) | Department — Engineering | Engineering, Executive | [e.g., Incident management — SYS-XXX] | | Average time from incident detection to resolution | Engineering | Full |

---

## 4. Metric Records

> Full detail for metrics that warrant documentation beyond the register entry. Prioritize: metrics used in Board or investor reporting, metrics that are targets in OKRs, metrics with known calculation disputes or data quality issues, and metrics that require cross-system joins.

### 4.1 Metric Record Template

---

**Metric ID:** MET-[XXX]
**Metric Name:** [Name]
**Category:** [Financial / Customer / Product / Sales / People / Operations]
**Last Updated:** YYYY-MM-DD
**Owner:** [Name / Role]

#### Definition

**What this metric measures:**
[1–2 sentences. What business reality does this metric reflect? Why does it matter?]

**Precise definition:**
[The exact definition — specific enough that two analysts calculating it independently would get the same number. Reference the Systems-and-Data entity definition rather than duplicating it. e.g., "Derived from the Active Customer entity defined in Systems-and-Data Section 4.2. A customer is counted as churned in the month their Stripe subscription status transitions to 'cancelled' — not the month they gave notice or the month their access was revoked."]

**Calculation:**
```
[Formula or step-by-step calculation. e.g.,
  Numerator: MRR lost to churn in period
    = Sum of MRR from subscriptions cancelled in period
  Denominator: MRR at start of period
    = Sum of MRR from all active subscriptions on first day of period
  MRR Churn Rate = (Numerator ÷ Denominator) × 100
]
```

**Measurement period:** [e.g., Monthly / Quarterly / As of date / Trailing 12 months]
**Measurement date convention:** [e.g., Calculated on the last day of each calendar month / As of 11:59pm on the measurement date in the company's reporting timezone]

---

#### Source and Provenance

| Field | Value |
|---|---|
| **Source system(s)** | [System name + ID from Systems-and-Data] |
| **Entity definition(s)** | [Reference to Systems-and-Data Section 4.2 entry] |
| **Query / report location** | [Link to dashboard, saved report, or data warehouse query] |
| **Calculated by** | [System / Data warehouse / Manual — Finance / Automated pipeline] |
| **Refresh cadence** | [e.g., Real-time / Daily / Weekly / Monthly close] |
| **Lag** | [e.g., No lag — live / 24-hour lag — nightly sync / Monthly — available by the 5th of the following month] |

**Cross-system dependencies:**
[Does this metric require a join across systems? If so, describe the join and flag any known reliability issues. e.g., "Time to First Value requires joining Stripe subscription start date (SYS-002) with the first qualifying product event in Mixpanel (SYS-007) via user ID. User ID consistency is ~80% — see Systems-and-Data Intelligence Gaps Section 5.3."]

---

#### Level and Visibility

| Field | Value |
|---|---|
| **Level** | [Company / Executive / Department — [name] / Team — [name]] |
| **Visible to** | [List roles and teams] |
| **Restricted from** | [List roles or teams explicitly excluded, if any] |
| **Where it appears** | [e.g., Board deck, monthly investor update, CS dashboard, product weekly] |

---

#### Strategy-and-Intent Reference

**Referenced in Strategy-and-Intent as:** [Goal or OKR ID and name, or "Not currently referenced as a target" — e.g., "G-004: Reduce MRR churn rate to below 1.2% monthly (FY2026 Q2)"]

**Baseline:** [Current value as of last measurement date — YYYY-MM-DD]

> Targets are defined and owned in Strategy-and-Intent. This field is a one-way pointer — updated when a goal referencing this metric is added or changed there. Do not duplicate the target value or goal description here.

---

#### Known Issues and Data Quality

| Issue | Impact | Status | Owner |
|---|---|---|---|
| [e.g., Cancelled accounts not updated in Salesforce within 48 hours] | [e.g., Logo churn rate may understate actual churn by 1–3% at any point in time] | [e.g., Process control in place — compliance monitored monthly] | [Name] |
| [e.g., Annual contracts normalized to monthly using contract value ÷ 12] | [e.g., Mid-year expansions on annual contracts may not be reflected until renewal] | [e.g., Known limitation — documented in Board deck footnote] | [Name] |

**Conflicts with other metrics or reports:**
[Is there a known case where this metric and another metric or report tell different stories? Reference the relevant entry in Systems-and-Data Conflict and Exception Log if applicable.]

---

#### Metric History

> Significant changes to this metric's definition, calculation, or source over time. Essential for longitudinal comparisons — a metric that changed definition mid-year cannot be trended without this record.

| Date | Change | Reason | Impact on Historical Data |
|---|---|---|---|
| YYYY-MM-DD | [e.g., Definition updated — paused subscriptions now excluded from Active Customer count] | [e.g., Paused accounts were distorting churn rate calculation] | [e.g., Historical active customer counts prior to this date include paused accounts — not comparable without restatement] |

---

> **Copy this template for each metric that warrants a full record.**

---

## 5. Visibility and Access Matrix

> Which roles and teams see which metric categories. Governs how dashboards, reports, and data access are configured. Aligns to the org structure in Internal-Stakeholders.
>
> This matrix defines the default visibility. Individual metrics may have more restrictive visibility — those exceptions are noted in the metric's record. No metric should be more broadly visible than its category default without explicit approval from the metric owner.

| Metric Category | Board | CEO / Executive Team | Finance | Sales Leadership | Sales (Individual) | Marketing | Product | Engineering | CS Leadership | CS (Individual) | HR | Department Heads | All Employees |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Financial — Company** | ✓ | ✓ | ✓ | Summary only | — | — | Summary only | — | — | — | — | Summary only | — |
| **Financial — Executive** | ✓ | ✓ | ✓ | — | — | — | — | — | — | — | — | — | — |
| **Financial — Unit Economics** | ✓ | ✓ | ✓ | Summary only | — | — | Summary only | — | — | — | — | — | — |
| **Customer — Retention / Churn** | ✓ | ✓ | ✓ | ✓ | — | — | ✓ | — | ✓ | — | — | Summary only | — |
| **Customer — Satisfaction** | — | ✓ | — | ✓ | — | — | ✓ | — | ✓ | ✓ | — | ✓ | Summary only |
| **Product — Usage / Adoption** | — | ✓ | — | Summary only | — | Summary only | ✓ | ✓ | ✓ | — | — | Summary only | — |
| **Sales — Pipeline / Conversion** | Summary only | ✓ | ✓ | ✓ | Own data only | — | Summary only | — | — | — | — | Summary only | — |
| **Sales — Quota Attainment** | Summary only | ✓ | ✓ | ✓ | Own data only | — | — | — | — | — | — | — | — |
| **People — Headcount** | ✓ | ✓ | ✓ | — | — | — | — | — | — | — | ✓ | ✓ | Summary only |
| **People — Attrition / Hiring** | Summary only | ✓ | Summary only | — | — | — | — | — | — | — | ✓ | Summary only | — |
| **Operations — Reliability** | — | ✓ | — | — | — | — | ✓ | ✓ | ✓ | — | — | Summary only | Summary only |
| **Operations — Engineering** | — | Summary only | — | — | — | — | ✓ | ✓ | — | — | — | — | — |

> **Key:** ✓ = Full visibility / Summary only = Aggregates and trends, not individual records / Own data only = Access to their own data, not peers / — = No access by default
>
> Update this matrix when: the org structure changes, a new metric category is added, or a visibility policy decision is made. Changes to this matrix should be reflected in dashboard and reporting tool access controls.

---

## 6. Metric Conflicts and Alignment Log

> When two metrics tell different stories, or when the same metric is calculated differently by different teams, this is where that gets surfaced and resolved. Mirrors the purpose of the Conflict and Exception Log in Systems-and-Data — which handles data conflicts at the entity level. This log handles conflicts at the metric level.
>
> Log entries should be made as soon as a conflict is discovered. Significant resolutions should also be captured in Institutional-Knowledge.md.

| Event ID | Date | Metrics in Conflict | Description | Root Cause | Resolution | Metric Records Updated | Logged to Institutional Knowledge | Owner |
|---|---|---|---|---|---|---|---|---|
| MCF-001 | YYYY-MM-DD | [e.g., MET-F001 (Finance MRR) vs. Sales-reported MRR] | [e.g., Finance reported MRR of $412K; Sales reported $427K in the same board deck. Discrepancy of $15K.] | [e.g., Sales was including LOIs and verbal commitments not yet in Stripe. Finance uses Stripe as the sole source per Systems-and-Data SoR map.] | [e.g., Definition clarified — MRR is Stripe-only. Sales pipeline value is a separate metric (MET-S001). Board deck template updated to use Finance figure with Sales pipeline as separate line.] | [e.g., MET-F001 record updated with known conflict note] | [Yes — link / No] | [Name] |
| MCF-002 | YYYY-MM-DD | [e.g., MET-C001 (Active Customer Count) — CS vs. Finance figures] | [e.g., CS reported 298 active customers; Finance reported 312. CS was using Stripe; Finance was using Salesforce.] | [e.g., Salesforce not updated for 14 cancelled accounts. System of Record is Stripe per Systems-and-Data Section 3.] | [e.g., Stripe count confirmed authoritative. Salesforce records corrected. See also EVT-001 in Systems-and-Data Conflict Log.] | [e.g., MET-C001 record updated] | [Yes] | [Name] |

---

## 7. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there metrics currently used in board or investor reporting that are not in this register?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., Which metric records are missing for metrics referenced in Strategy-and-Intent OKRs?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Does the visibility matrix reflect current dashboard and reporting tool access controls, or does it need to be enforced?] | [Name] | YYYY-MM-DD | |
| 4 | [e.g., Which metrics currently have definition disagreements between teams that should be resolved and logged in Section 6?] | [Name] | YYYY-MM-DD | |
