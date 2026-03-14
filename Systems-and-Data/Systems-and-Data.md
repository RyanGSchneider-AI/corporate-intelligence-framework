# Systems and Data

> The authoritative reference for every formal system the organization uses, the data those systems own, and the business intelligence each system and combination of systems can produce. This document serves three distinct lenses — governance, data definition, and intelligence — unified around a single organizing spine: the system.
>
> **Governance lens:** What systems exist, who owns them, who can access them, when contracts renew, and which system is authoritative when data conflicts arise.
>
> **Data definition lens:** What key entities mean — precisely — where they live, how they are calculated, and what they are called by different teams. The source of truth that prevents "active customer" meaning four different things across four departments.
>
> **Intelligence lens:** What business questions each system can answer, what it cannot answer alone, and what becomes possible when systems are combined. The map that tells analysts, product managers, and AI agents where to look.

---

## Document Control

| Field | Value |
|---|---|
| **Last Updated** | YYYY-MM-DD |
| **Updated By** | |
| **Review Cadence** | Systems Registry and Access: quarterly / Data Dictionary: when entities are added or redefined / Intelligence Map: semi-annually or when systems change |
| **Primary Owner** | [e.g., CTO / VP Engineering / IT Operations / Data lead] |

> **Connected artifacts:**
> - **Metrics-Framework** — every metric definition should reference the System of Record and entity definition from this document; conflicts between metric calculations and system data surface here
> - **Key-Operational-Processes** — process records reference systems by name; system changes here trigger process impact assessment there
> - **Organizational-Risk-and-Compliance** — compliance obligations attached to systems here (GDPR, HIPAA, SOC 2 scope) should align with the compliance obligations register there
> - **Product-Build-Record** — system dependencies in Section 9 reference systems catalogued here; new systems introduced by a build should be added here at launch
> - **Cost-and-Benefit-Framework** — infrastructure cost estimates reference system costs captured in Section 2
> - **Institutional-Knowledge** — significant system decisions, migrations, and data conflicts resolved should be captured there after being logged here


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 For Governance and IT Operations

The Systems Registry (Section 2) is the complete inventory of formal systems. Use it to:
- Onboard new team members — understand what systems exist and who owns each
- Manage contract renewals — all renewal dates and contract owners in one view
- Provision and review access — access tiers and provisioning owners in Section 6
- Evaluate the impact of a system change or replacement — see which processes and data domains depend on it
- Confirm compliance scope — which systems are in scope for SOC 2, GDPR, HIPAA, and other obligations

### 1.2 For Data Work and AI Agents

The Data Dictionary (Section 4) is the authoritative source for entity definitions. Use it to:
- Resolve ambiguity about what a term means — "customer," "revenue," "active user" have precise definitions here
- Understand where data lives and how it is calculated
- Identify known aliases — what one team calls a thing vs. what another team calls it
- Surface known data quality issues before building on a data source

The System of Record Map (Section 3) is the conflict resolution reference. When two systems disagree, this document says which one is authoritative and why.

### 1.3 For Strategic and Analytical Work

The Data Intelligence Map (Section 5) answers "what can we know, and from where?" Use it to:
- Identify which systems can answer a specific business question
- Understand what data enrichment or system combination is needed for questions no single system can answer
- Evaluate gaps — business questions the organization cannot currently answer and what would be needed to answer them

### 1.4 Keeping This Document Current

This document degrades faster than most in the framework — systems are added, contracts change, and data definitions drift. The minimum viable maintenance cadence:

| Section | Trigger for Update |
|---|---|
| Systems Registry | Any system added, retired, or significantly changed |
| System of Record Map | Any data conflict resolved; any system added or retired |
| Data Dictionary | Any entity added, renamed, redefined, or found to be inconsistent across systems |
| Data Intelligence Map | Any system added or retired; any new analytical capability confirmed or gap identified |
| Access and Security Register | Any access tier change; any new compliance obligation; any personnel change affecting system ownership |
| Conflict and Exception Log | Any data conflict surfaced — log immediately, resolve over time |

---

## 2. Systems Registry

> The master inventory of all formal systems the organization uses. One row per system. Full records in Section 2.2 for systems that warrant detailed documentation.
>
> A "formal system" is any platform, application, or data store that the organization has formally adopted, pays for, or has designated as authoritative for any data domain. Spreadsheets and manual processes that serve as de facto systems of record are not captured here — but if a spreadsheet is the only source of truth for a critical data domain, that gap should be flagged in Section 3 and Section 7.

### 2.1 Systems Inventory

| System ID | System Name | Category | Vendor | Primary Owner | Status | System of Record For | Contract Renewal | Annual Cost | Notes |
|---|---|---|---|---|---|---|---|---|---|
| SYS-001 | [e.g., Salesforce] | [CRM] | [Salesforce] | [Name / Role] | [Active / Sunset / Evaluating] | [e.g., Customer relationships, pipeline, contracts] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-002 | [e.g., Stripe] | [Billing and payments] | [Stripe] | [Name / Role] | [Active] | [e.g., Billing, invoices, payment status, subscription terms] | [Month-to-month] | [$X,000/yr] | |
| SYS-003 | [e.g., PostgreSQL — production] | [Database] | [Self-hosted / AWS RDS] | [Name / Role] | [Active] | [e.g., Product data, user accounts, application state] | [Infrastructure — see SYS-010] | [See SYS-010] | |
| SYS-004 | [e.g., NetSuite] | [ERP / Accounting] | [Oracle] | [Name / Role] | [Active] | [e.g., Financial records, chart of accounts, AR/AP] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-005 | [e.g., Workday] | [HRIS] | [Workday] | [Name / Role] | [Active] | [e.g., Employee records, compensation, org structure] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-006 | [e.g., Zendesk] | [Customer support] | [Zendesk] | [Name / Role] | [Active] | [e.g., Support tickets, customer health signals, SLA records] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-007 | [e.g., Mixpanel] | [Product analytics] | [Mixpanel] | [Name / Role] | [Active] | [e.g., Product usage events, feature adoption, user behavior] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-008 | [e.g., HubSpot] | [Marketing automation] | [HubSpot] | [Name / Role] | [Active] | [e.g., Marketing contacts, campaign performance, lead source] | [YYYY-MM-DD] | [$X,000/yr] | |
| SYS-009 | [e.g., Snowflake] | [Data warehouse] | [Snowflake] | [Name / Role] | [Active] | [e.g., Analytical layer — not System of Record; aggregates from above] | [YYYY-MM-DD] | [$X,000/yr] | [Downstream of operational systems — not authoritative] |
| SYS-010 | [e.g., AWS] | [Cloud infrastructure] | [Amazon] | [Name / Role] | [Active] | [e.g., Infrastructure — not a data System of Record] | [Monthly] | [$X,000/yr] | |

> **System categories:** CRM / Billing and payments / ERP and accounting / HRIS / Customer support / Product analytics / Marketing automation / Data warehouse / Business intelligence / Cloud infrastructure / Communication / Document management / Security / Other

### 2.2 System Records

> Full detail per significant system. Copy the template for each system that warrants documentation beyond the inventory row. Prioritize: Systems of Record for critical data domains, systems with compliance obligations, and systems with high operational dependency.

---

**System ID:** SYS-[XXX]
**System Name:** [Name]
**Category:** [From Section 2.1]
**Vendor:** [Vendor name]
**Last Updated:** YYYY-MM-DD

#### Purpose and Scope

**What this system does:**
[1–2 sentences. What business function does this system serve?]

**What it is the System of Record for:**
[List every data domain for which this system is authoritative. Be specific. e.g., "Customer contracts and contract terms — Salesforce Opportunities are the authoritative record of what a customer has agreed to pay and for what."]

**What it is NOT the System of Record for:**
[Equally important. e.g., "Customer billing status — Stripe is authoritative for whether an invoice has been paid. Salesforce may reflect this data but Stripe is the source of truth."]

**Connected systems:**

| Connected System | Direction | What Flows | Frequency | Method | Notes |
|---|---|---|---|---|---|
| [e.g., SYS-002 Stripe] | [Outbound / Inbound / Bi-directional] | [e.g., Contract terms → triggers billing setup] | [e.g., Per event] | [e.g., Zapier / Native integration / Manual] | |
| [e.g., SYS-009 Snowflake] | [Outbound] | [e.g., Opportunity and account data → analytical layer] | [e.g., Nightly sync] | [e.g., Fivetran] | [e.g., 24-hour lag — not real-time] |

#### Ownership and Access

| Role | Name | Responsibility |
|---|---|---|
| **System Owner** | [Name] | Accountable for the system — contract, configuration, and data quality |
| **Technical Admin** | [Name] | Day-to-day administration, user provisioning, integrations |
| **Business Admin** | [Name] | Process configuration, field management, report ownership |
| **Backup Admin** | [Name / "None identified"] | Can administer if primary is unavailable |

**Access tiers:** [See Section 6 for full access register]

#### Contract and Vendor

| Field | Value |
|---|---|
| **Contract type** | [Annual / Multi-year / Month-to-month / Seat-based / Usage-based] |
| **Contract term** | [Start date — End date] |
| **Renewal date** | YYYY-MM-DD |
| **Renewal notice required** | [e.g., 30 / 60 / 90 days prior] |
| **Auto-renews** | [Yes / No] |
| **Contract owner** | [Name] |
| **Annual cost** | [$X,000] |
| **Pricing model** | [e.g., Per seat / Usage-based / Flat] |
| **Vendor contact** | [Name / email] |
| **Contract location** | [Link to contract in document management system] |

#### Compliance and Security

**Compliance scope:** [e.g., In scope for SOC 2 / Processes PHI — in scope for HIPAA BAA / Stores EU personal data — GDPR obligations apply / Not in scope for any current certification]

**Data classification:** [e.g., Contains PII / Contains PHI / Contains financial records / Internal only / Public]

**Key security controls:**
- [e.g., SSO enforced via Okta]
- [e.g., MFA required for all users]
- [e.g., Role-based access — no user has admin and data export rights simultaneously]
- [e.g., Data encrypted at rest and in transit]

**Vendor security posture:** [e.g., SOC 2 Type II certified — report reviewed annually / ISO 27001 certified / Self-attested — security questionnaire on file]

#### Known Issues and Risks

| Issue | Type | Impact | Status | Owner |
|---|---|---|---|---|
| [e.g., Duplicate account records — estimated 3–5% of accounts have duplicates] | [Data quality] | [e.g., Inflates account count metrics; causes routing errors in automation] | [Known — remediation in backlog] | [Name] |
| [e.g., Nightly sync to Snowflake fails ~2% of runs] | [Integration reliability] | [e.g., Stale data in analytics layer for affected records] | [Monitoring in place — engineering ticket open] | [Name] |

---

> **Copy this template for each system that warrants a full record.**

---

## 3. System of Record Map

> For each data domain, this section declares which system is authoritative — the source of truth when two systems disagree. This is the conflict resolution reference.
>
> **The official state is what is declared here.** When the current reality is messy — two systems both claiming to own a domain, no clear answer, or known gaps — that should be documented honestly in the "Current State" column and the intended resolution captured in the "Intended State" column. A known gap acknowledged is a gap that can be addressed. A gap that is not acknowledged will produce data conflicts that nobody can resolve.

| Data Domain | System of Record | System ID | Current State | Intended State | Confidence | Last Reviewed | Notes |
|---|---|---|---|---|---|---|---|
| **Customer identity and profile** | [e.g., Salesforce] | [SYS-001] | [e.g., Clean — Salesforce is unambiguously the master] | [Same] | [High] | YYYY-MM-DD | |
| **Customer contract terms** | [e.g., Salesforce] | [SYS-001] | [e.g., Clean — Opportunity record is authoritative] | [Same] | [High] | YYYY-MM-DD | |
| **Billing and payment status** | [e.g., Stripe] | [SYS-002] | [e.g., Clean — Stripe is authoritative; Salesforce reflects but does not own] | [Same] | [High] | YYYY-MM-DD | |
| **Revenue — recognized** | [e.g., NetSuite] | [SYS-004] | [e.g., Messy — NetSuite is intended SoR but Stripe revenue figures are used in reporting because NetSuite sync is delayed] | [NetSuite as sole authoritative source — requires sync improvement] | [Low] | YYYY-MM-DD | [See EVT-003 in Section 7] |
| **Product usage and feature adoption** | [e.g., Mixpanel] | [SYS-007] | [e.g., Clean — Mixpanel events are the source; warehouse is downstream] | [Same] | [High] | YYYY-MM-DD | |
| **Employee records and org structure** | [e.g., Workday] | [SYS-005] | [e.g., Clean] | [Same] | [High] | YYYY-MM-DD | |
| **Support tickets and SLA records** | [e.g., Zendesk] | [SYS-006] | [e.g., Clean] | [Same] | [High] | YYYY-MM-DD | |
| **Marketing contacts and lead source** | [e.g., HubSpot] | [SYS-008] | [e.g., Partial — lead source is in HubSpot but syncs to Salesforce inconsistently; both are queried] | [HubSpot as authoritative for pre-opportunity data; Salesforce for post-opportunity] | [Medium] | YYYY-MM-DD | |
| **Analytical and reporting data** | [e.g., Snowflake] | [SYS-009] | [e.g., Downstream aggregate — not a System of Record; authoritative systems above are the sources] | [Same] | [High] | YYYY-MM-DD | [Reports that contradict operational systems should be investigated — Snowflake is not authoritative] |

> **Confidence levels:**
> - **High** — system ownership is clear, enforced, and understood by all teams that touch this domain
> - **Medium** — system ownership is declared but not fully enforced; multiple systems are queried in practice
> - **Low** — system ownership is contested, unclear, or the declared owner is not the system teams actually use
>
> Low confidence entries are the highest priority for resolution. They are the source of the data conflicts that produce disagreements in business reviews, incorrect metrics, and AI agent errors.

---

## 4. Data Dictionary

> Authoritative definitions of the key data entities and terms the organization uses. Organized by domain. Each entry anchors to its System of Record from Section 3.
>
> **The goal is shared understanding, not exhaustive documentation.** Not every database field needs an entry. Entries belong here when: (a) a term means different things to different teams, (b) a metric or report depends on a precise definition, (c) an AI agent or new team member would make a wrong assumption without it, or (d) a data quality issue exists that users need to know about.

### 4.1 Data Dictionary — Entry Template

> Copy for each entity that warrants definition.

---

**Entity:** [Name — e.g., "Active Customer"]
**Domain:** [e.g., Customer / Revenue / Product / People]
**System of Record:** [System name + ID from Section 3]
**Last Updated:** YYYY-MM-DD
**Owner:** [Name / Role — who is responsible for maintaining this definition]

**Definition:**
[Precise definition. e.g., "A customer account with at least one paid subscription in a non-cancelled, non-paused state as of the measurement date. Trial accounts are not Active Customers. Accounts with a past-due balance that have not been formally cancelled are Active Customers until cancellation is recorded in Stripe."]

**How it is determined:**
[Where does this value come from? Calculated, assigned, or recorded? e.g., "Derived from Stripe subscription status field. Status = 'active' or 'past_due' qualifies. Status = 'cancelled', 'trialing', or 'paused' does not."]

**Known aliases:**
| Team / Context | What They Call It | Notes |
|---|---|---|
| [e.g., Sales] | [e.g., "Live customer" or "paying customer"] | [e.g., Sales uses this interchangeably — they mean the same thing but the term is not standardized] |
| [e.g., Finance] | [e.g., "Revenue-generating account"] | [e.g., Finance may include paused accounts in this count — confirm before using Finance figures] |
| [e.g., Product] | [e.g., "Active account"] | [e.g., Product may use product login activity as the qualifier, not billing status — different definition] |

**Where it appears:**
[Which reports, dashboards, metrics, or documents reference this entity? e.g., "MRR calculation, customer count KPI, churn rate denominator, CS account assignments."]

**Known data quality issues:**
[e.g., "~3% of accounts have duplicate records in Salesforce. When Stripe subscription count and Salesforce account count disagree, Stripe is authoritative per Section 3. See EVT-001 in Section 7."]

**What this entity is NOT:**
[Negative definition — what common misconceptions exist? e.g., "A customer with an active trial is not an Active Customer. A customer whose subscription is paused is not an Active Customer even though they may still have product access."]

---

### 4.2 Data Dictionary — Entries by Domain

> Add an entry block (using the template above) for each entity in each domain. Sample entries below — replace with the organization's actual entities.

#### Customer Domain

**Entity: Customer**
**Domain:** Customer
**System of Record:** [e.g., Salesforce — SYS-001]

[Complete using template above]

---

**Entity: Active Customer**
**Domain:** Customer
**System of Record:** [e.g., Stripe — SYS-002 for status; Salesforce — SYS-001 for profile]

[Complete using template above]

---

**Entity: Churned Customer**
**Domain:** Customer
**System of Record:** [e.g., Stripe — SYS-002]

[Complete using template above — be precise about when churn is recorded vs. when it is effective]

---

#### Revenue Domain

**Entity: MRR (Monthly Recurring Revenue)**
**Domain:** Revenue
**System of Record:** [e.g., Stripe — SYS-002]

[Complete using template above — include whether MRR is contracted or billed, how annual contracts are normalized, whether discounts are included or excluded]

---

**Entity: ARR (Annual Recurring Revenue)**
**Domain:** Revenue
**System of Record:** [e.g., Stripe — SYS-002 / NetSuite — SYS-004]

[Complete using template above — note any difference between how Finance calculates ARR and how the product/sales team does]

---

**Entity: Net Revenue Retention (NRR)**
**Domain:** Revenue
**System of Record:** [e.g., Stripe — SYS-002]

[Complete using template above — define the measurement window, what counts as expansion vs. contraction, and whether churned customers are included in the denominator]

---

#### Product Domain

**Entity: Active User**
**Domain:** Product
**System of Record:** [e.g., Mixpanel — SYS-007]

[Complete using template above — define the activity threshold: any login? A qualifying action? In what time window?]

---

**Entity: Feature Adoption**
**Domain:** Product
**System of Record:** [e.g., Mixpanel — SYS-007]

[Complete using template above — define adoption: first use? Regular use? What threshold distinguishes "adopted" from "tried"?]

---

#### People Domain

**Entity: Employee**
**Domain:** People
**System of Record:** [e.g., Workday — SYS-005]

[Complete using template above — note whether contractors are included or excluded and how to distinguish in the system]

---

**Entity: Headcount**
**Domain:** People
**System of Record:** [e.g., Workday — SYS-005]

[Complete using template above — define whether headcount is filled seats, budgeted seats, or FTE-equivalent; whether contractors count; and as-of what date]

---

> Add domains and entities as needed. The entries above are illustrative starting points — the organization should define the entities that actually cause confusion or disagreement in practice.

---

## 5. Data Intelligence Map

> What business questions each system can answer, what it cannot answer alone, and what becomes possible when systems are combined. This section is for analysts, product managers, and AI agents who need to know where to look — not just what exists, but what it can tell you.
>
> **The most valuable entries here are the combinations** — the business questions that require crossing system boundaries and the enrichment that makes them possible.

### 5.1 Per-System Intelligence Summary

| System | Can Answer | Cannot Answer Alone | Requires Combination With | Key Limitations |
|---|---|---|---|---|
| [e.g., Salesforce SYS-001] | [e.g., Pipeline by stage, win/loss by rep, deal velocity, account health by relationship] | [e.g., Whether a won deal is actually paying, product usage by account, support ticket volume by account] | [e.g., Stripe for payment status, Mixpanel for usage, Zendesk for support] | [e.g., Data quality degrades without consistent rep hygiene; duplicate accounts affect counts] |
| [e.g., Stripe SYS-002] | [e.g., MRR, ARR, churn rate, payment status, subscription changes, revenue by plan] | [e.g., Who the account contact is, what features they use, whether they're satisfied] | [e.g., Salesforce for account context, Mixpanel for usage, Zendesk for health] | [e.g., Revenue figures lag NetSuite by up to 24 hours; annual contracts require normalization for MRR] |
| [e.g., Mixpanel SYS-007] | [e.g., Feature adoption, user activation, retention curves, funnel completion, session frequency] | [e.g., Whether the user is on a paid plan, their contract value, their support history] | [e.g., Stripe for plan/revenue context, Zendesk for support correlation] | [e.g., Requires user ID consistency across systems for joins; anonymous users inflate some counts] |
| [e.g., Zendesk SYS-006] | [e.g., Ticket volume by account, SLA compliance, resolution time, issue categories, CSAT] | [e.g., Whether the account is at risk of churn, their product usage, their contract value] | [e.g., Salesforce for account context, Stripe for revenue context] | [e.g., Ticket categorization is inconsistent — taxonomy discipline affects analytical value] |
| [e.g., Snowflake SYS-009] | [e.g., Cross-system questions — joins across all of the above] | [e.g., Nothing on its own — downstream aggregate only] | [e.g., All operational systems above — Snowflake is the combination layer] | [e.g., Nightly sync — 24-hour lag; not real-time; authoritative systems override on conflict] |

### 5.2 Business Question Map

> The inverse of 5.1 — organized by business question rather than by system. Start here when you have a question and need to know where to find the answer.

| Business Question | Can Be Answered By | Systems Required | Data Entities Involved | Notes |
|---|---|---|---|---|
| [e.g., What is our current MRR?] | [Single system] | [Stripe — SYS-002] | [MRR — see Section 4.2] | [e.g., Use Stripe directly for current state; Snowflake for trended view] |
| [e.g., Which accounts are at risk of churn?] | [Multi-system] | [Zendesk + Mixpanel + Stripe] | [Active Customer, Feature Adoption, Support ticket volume] | [e.g., No single system answers this — requires combining support volume, usage decline, and billing status] |
| [e.g., What is our net revenue retention?] | [Single system + definition] | [Stripe — SYS-002] | [NRR — see Section 4.2] | [e.g., Calculation is in Stripe; confirm definition alignment with Finance before reporting] |
| [e.g., Which product features correlate with retention?] | [Multi-system] | [Mixpanel + Stripe] | [Feature Adoption, Active Customer, Churned Customer] | [e.g., Requires user ID join between Mixpanel and Stripe; user ID consistency must be verified] |
| [e.g., What is our pipeline coverage for next quarter?] | [Single system] | [Salesforce — SYS-001] | [Pipeline, deal stage, close date] | [e.g., Quality depends on rep hygiene — verify stage definitions are being applied consistently] |
| [e.g., What is our CAC by channel?] | [Multi-system] | [HubSpot + Salesforce + NetSuite] | [Lead source, won opportunity, acquisition cost] | [e.g., Requires clean lead source attribution in HubSpot and consistent cost categorization in NetSuite] |
| [e.g., What is our fully-loaded cost per employee?] | [Multi-system] | [Workday + NetSuite] | [Headcount, compensation, benefits, overhead allocation] | [e.g., Overhead allocation methodology should be defined in Cost-and-Benefit-Framework] |

### 5.3 Known Intelligence Gaps

> Business questions the organization cannot currently answer well — and what would be needed to answer them. This is the analytical roadmap input.

| Business Question | Why It Cannot Be Answered | What Would Enable It | Priority | Owner |
|---|---|---|---|---|
| [e.g., Customer health score] | [e.g., No single view combining usage, support, billing, and relationship data — requires multi-system join that does not currently exist in a maintained form] | [e.g., A maintained customer health model in Snowflake joining Mixpanel + Zendesk + Stripe + Salesforce] | [High] | [Name] |
| [e.g., True CAC by channel at the account level] | [e.g., Lead source attribution degrades after the first touch; multi-touch attribution model not implemented] | [e.g., Multi-touch attribution configuration in HubSpot or a dedicated attribution tool] | [Medium] | [Name] |
| [e.g., Product usage by contract value segment] | [e.g., User ID in Mixpanel is not consistently matched to account ID in Stripe — join fails for ~20% of accounts] | [e.g., Engineering effort to standardize user/account ID across product and billing systems] | [High] | [Name] |

---

## 6. Access and Security Register

> Who can access each system, at what level, and under what conditions. This section serves IT governance, compliance audits, and onboarding. It is the reference for confirming that access is appropriate and that no individual has more access than their role requires.

### 6.1 Access Tier Definitions

> Define the organization's access tiers once here — applied consistently across all systems below.

| Tier | Label | Description | Provisioning Authority |
|---|---|---|---|
| 1 | **Admin** | Full system access including configuration, user management, data export, and integration management | [e.g., System Owner + CTO approval] |
| 2 | **Power User** | Full data access and reporting; cannot modify system configuration or manage users | [e.g., System Owner approval] |
| 3 | **Standard User** | Access to data and functionality within their role scope; cannot export bulk data or modify shared configuration | [e.g., Manager approval + System Admin provisioning] |
| 4 | **Read Only** | Can view but not modify; cannot export bulk data | [e.g., Manager approval] |
| 5 | **No Access** | Not provisioned — access requires a formal request | [e.g., N/A] |

### 6.2 Access Register by System

| System | System ID | Admin(s) | Power Users | Standard Users | Read Only | Access Review Cadence | Last Reviewed | Notes |
|---|---|---|---|---|---|---|---|---|
| [e.g., Salesforce] | [SYS-001] | [Name(s)] | [Name(s) or "See roster"] | [e.g., All sales team + CS team] | [e.g., Finance, Executive] | [Quarterly] | YYYY-MM-DD | [e.g., Admin access limited to 2 individuals; export rights require Admin tier] |
| [e.g., Stripe] | [SYS-002] | [Name(s)] | [Name(s)] | [e.g., Finance team] | [e.g., Executive] | [Quarterly] | YYYY-MM-DD | [e.g., API key access is a separate register — see engineering credentials vault] |
| [e.g., NetSuite] | [SYS-004] | [Name(s)] | [e.g., Finance team] | [e.g., Department heads — expense approval only] | [e.g., Executive, Legal] | [Quarterly] | YYYY-MM-DD | |
| [e.g., Workday] | [SYS-005] | [Name(s)] | [e.g., HR team] | [e.g., All employees — self-service only] | [e.g., Finance — headcount reporting] | [Quarterly] | YYYY-MM-DD | [e.g., Manager access to direct reports only — skip-level requires HR approval] |

### 6.3 Sensitive Data and Compliance Obligations by System

| System | System ID | Data Classification | Compliance Scope | Key Obligations | Owner |
|---|---|---|---|---|---|
| [e.g., Salesforce] | [SYS-001] | [PII — customer contact data] | [GDPR, CCPA] | [e.g., Data subject request process; retention policy; cross-border transfer restrictions] | [Name / Legal] |
| [e.g., Stripe] | [SYS-002] | [PII + financial data] | [PCI-DSS (handled by Stripe), GDPR] | [e.g., No raw card data stored in org systems; Stripe is PCI-compliant on our behalf] | [Name / Finance] |
| [e.g., Workday] | [SYS-005] | [PII + HR sensitive data] | [GDPR, CCPA, applicable employment law] | [e.g., Access to compensation data restricted to HR and Finance; right to access requests routed through HR] | [Name / HR / Legal] |
| [e.g., Zendesk] | [SYS-006] | [PII — customer communications] | [GDPR, CCPA] | [e.g., Support ticket retention policy; data subject deletion requests must be actioned within 30 days] | [Name / Legal] |

> Cross-reference with Organizational-Risk-and-Compliance for full compliance obligations register. System-level obligations here should be consistent with what is captured there.

### 6.4 Access Provisioning and Offboarding

**New access provisioning process:**
[e.g., Manager submits access request via [ticketing system] → System Admin reviews against role and need → provisioned within 2 business days → logged in access register → quarterly access review will include new provisioning]

**Offboarding — system access revocation:**
[e.g., HR notifies IT on or before last day → IT deactivates all system access within 4 hours of notification → access register updated → any admin access held by departing individual transferred before last day — not after]

**Quarterly access review:**
[e.g., System Admins review their access registers and confirm each user's access tier is still appropriate to their role. Any access that cannot be justified is revoked. Changes logged here.]

---

## 7. Conflict and Exception Log

> A running record of data conflicts — when two systems disagreed, how the conflict was resolved, and whether the System of Record designation in Section 3 was updated as a result. This is the feedback loop that keeps the System of Record Map honest over time.
>
> Log entries should be made as soon as a conflict is discovered — even before it is resolved. A logged unresolved conflict is more useful than an unlogged one. Significant conflicts and their resolutions should also be captured in Institutional-Knowledge.md.

| Event ID | Date Discovered | Systems in Conflict | Data Domain | Description of Conflict | Resolution | SoR Map Updated | Logged to Institutional Knowledge | Owner |
|---|---|---|---|---|---|---|---|---|
| EVT-001 | YYYY-MM-DD | [e.g., Salesforce vs. Stripe] | [e.g., Active Customer count] | [e.g., Salesforce showed 312 active accounts; Stripe showed 298 active subscriptions. Discrepancy of 14 accounts. Investigation found 11 cancelled accounts not updated in Salesforce and 3 trial accounts incorrectly marked as customers in Salesforce.] | [e.g., Stripe count confirmed as authoritative per Section 3. Salesforce records corrected. Process updated to require CRM update within 48 hours of cancellation in Stripe.] | [Yes / No / Pending] | [Yes — link / No] | [Name] |
| EVT-002 | YYYY-MM-DD | [e.g., Snowflake vs. Stripe] | [e.g., MRR] | [e.g., Monthly finance report from Snowflake showed MRR $4K lower than Stripe dashboard. Caused by failed nightly sync on the 3rd — 6 new subscriptions missed.] | [e.g., Snowflake backfilled. Monitoring alert added for sync failures. Finance report now includes sync health check before distribution.] | [No — SoR was already correct] | [No — below threshold] | [Name] |
| EVT-003 | YYYY-MM-DD | [e.g., Stripe vs. NetSuite] | [e.g., Recognized revenue] | [e.g., Stripe revenue figures used in reporting differ from NetSuite recognized revenue by ~8% due to NetSuite sync delay and different treatment of annual contract revenue recognition.] | [e.g., Unresolved — NetSuite is the intended SoR for recognized revenue but Stripe is used in practice due to sync delay. Resolution requires NetSuite sync improvement and alignment on revenue recognition methodology. See Section 3 — confidence level Low.] | [No — marked Low confidence in Section 3 pending resolution] | [Yes — link] | [Name / CFO] |

---

## 8. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there systems in use by individual teams or departments that have not been added to the registry?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., Which Low-confidence System of Record entries in Section 3 have a resolution plan and timeline?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Are all systems with PII or sensitive data reflected in Organizational-Risk-and-Compliance?] | [Name] | YYYY-MM-DD | |
| 4 | [e.g., Which Data Dictionary entries are missing that cause the most confusion or disagreement in practice?] | [Name] | YYYY-MM-DD | |
| 5 | [e.g., Is the quarterly access review on the Company Calendar for each system owner?] | [Name] | YYYY-MM-DD | |
