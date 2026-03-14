# Key Operational Processes

> A living inventory of the recurring processes the organization depends on to function — and a reference for evaluating how any change in product, strategy, or structure will interact with those processes.
>
> **The purpose of this document is not to document processes for their own sake.** It is to make visible what the organization actually does repeatedly, who owns it, how mature it is, and what breaks if it is disrupted. A business that does not know what its recurring processes are cannot reliably evaluate the impact of its own decisions.
>
> **Consult this document when:** a new product feature is being scoped, a strategic initiative is being evaluated, a new sales channel is being added, a key person is leaving, or any operational change is being considered. Processes that are not acknowledged cannot be protected.

---

## Document Control

| Field | Value |
|---|---|
| **Last Updated** | YYYY-MM-DD |
| **Updated By** | |
| **Review Cadence** | Annually, or when a significant product, structural, or strategic change occurs |
| **Primary Owner** | [e.g., COO / Head of Operations / CEO] |

> **Connected artifacts:**
> - **Product-Build-Record** — requirements and retrospectives should reference affected processes from this document
> - **Business-Case** — benefit claims involving process efficiency should reference the relevant process record here
> - **Cost-and-Benefit-Framework** — labor cost estimates for process-dependent work should reference process ownership and step counts here
> - **People-and-Talent-Strategy** — key person risk is amplified when critical processes are undocumented or single-owned
> - **Organizational-Risk-and-Compliance** — process failure modes here feed the risk inventory there
> - **Institutional-Knowledge** — significant process decisions and their reasoning belong there


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 For Ongoing Operations

This document tells anyone in the organization — including new hires and AI agents — what recurring work exists, who owns it, and how it is executed. It is the answer to: *"What does this organization actually do, repeatedly, that keeps it running?"*

Process records here are not procedure manuals. They capture enough detail to:
- Understand what the process does and why it exists
- Know who owns it and who else is involved
- Identify what systems it depends on
- Recognize what failure looks like and what causes it
- Assess what a proposed change would disrupt

For step-by-step procedure documentation, link to the relevant runbook, SOP, or system documentation from within the process record.

### 1.2 For Evaluating Change

Before any of the following decisions is finalized, the relevant process records should be reviewed:

| Decision Type | Processes Most Likely Affected |
|---|---|
| New product feature or capability | Customer onboarding, customer support, billing, any process that touches the affected data or workflow |
| New pricing model or tier | Billing and collections, sales channel compensation, customer onboarding, financial reporting |
| New sales channel | Channel onboarding, channel compensation, order management, customer onboarding |
| Geographic or market expansion | Compliance processes, financial reporting, customer onboarding, supply chain |
| Key person departure | Any process where that person is listed as Primary Owner or sole executor |
| System replacement or upgrade | Every process that lists the affected system as a dependency |
| Merger, acquisition, or restructure | All processes — ownership and execution may change across the board |

> **The question to ask for each affected process:** Does this change alter the trigger, inputs, steps, outputs, owner, or systems this process depends on? If yes, the process record should be updated and the change evaluated for disruption risk before the initiative launches.

### 1.3 Maturity Levels

> Every process is assigned a maturity level in the Process Inventory. Maturity affects how much risk a change to that area carries and how urgently documentation should be improved.

| Level | Label | Description |
|---|---|---|
| 4 | **Documented and stable** | Process is fully documented, consistently executed, understood by multiple people, and reviewed periodically |
| 3 | **Documented and in progress** | Process is documented but execution is inconsistent, or documentation is outdated relative to current practice |
| 2 | **Undocumented but consistent** | Process is executed reliably but lives primarily in people's heads — departure of the owner creates significant risk |
| 1 | **Ad hoc** | Process exists but is executed inconsistently, with no clear owner or documentation — outcomes are variable |
| 0 | **Known gap** | A process is known to be needed but has not yet been established — currently handled by workaround or exception |

---

## 2. Process Inventory

> A single-view register of all recurring processes the organization has identified. One row per process. Full detail in Section 3.
>
> **Add a row here first, then create a full record in Section 3.** The inventory is the map; the records are the territory.

| Process ID | Process Name | Category | Owner | Frequency | Maturity | Systems Involved | Key Person Risk | Record Status | Notes |
|---|---|---|---|---|---|---|---|---|---|
| OP-001 | [e.g., New customer onboarding] | [Customer-facing] | [Name / Role] | [Per new customer] | [4] | [e.g., CRM, billing platform, product] | [Low / Medium / High] | [Full record / Summary only / Inventory only] | |
| OP-002 | [e.g., Feature expansion for existing customer] | [Customer-facing] | [Name / Role] | [Per request] | [3] | [e.g., CRM, product, support platform] | [Medium] | [Full record] | |
| OP-003 | [e.g., Sales channel onboarding] | [Sales and distribution] | [Name / Role] | [Per new channel] | [2] | [e.g., CRM, contract management, billing] | [High] | [Summary only] | |
| OP-004 | [e.g., Sales channel compensation] | [Financial] | [Name / Role] | [Monthly] | [3] | [e.g., Billing platform, payroll, CRM] | [Medium] | [Full record] | |
| OP-005 | [e.g., Customer billing and collections] | [Financial] | [Name / Role] | [Monthly / Per event] | [4] | [e.g., Billing platform, ERP, bank] | [Low] | [Full record] | |
| OP-006 | [e.g., Month-end financial close] | [Financial] | [Name / Role] | [Monthly] | [3] | [e.g., ERP, billing platform, payroll] | [High] | [Full record] | |
| OP-007 | [e.g., Supply chain engagement] | [Operations] | [Name / Role] | [Per production cycle] | [2] | [e.g., Procurement system, ERP] | [High] | [Summary only] | |
| OP-008 | [e.g., Recurring build / manufacturing run] | [Operations] | [Name / Role] | [Per production cycle] | [3] | [e.g., MES, ERP, QA system] | [Medium] | [Full record] | |
| OP-009 | [e.g., Regulatory compliance reporting] | [Compliance] | [Name / Role] | [Quarterly / Annual] | [3] | [e.g., ERP, compliance platform] | [Medium] | [Full record] | |
| OP-010 | [e.g., Customer support escalation handling] | [Customer-facing] | [Name / Role] | [Ongoing] | [2] | [e.g., Support platform, CRM, product] | [Medium] | [Summary only] | |

> Add rows as processes are identified. Processes do not need a full record to appear in the inventory — an inventory-only entry is still valuable as an acknowledgment that the process exists.

---

## 3. Process Records

> One record per significant process. Copy the template below and complete for each process in the inventory that warrants full documentation. Processes with maturity level 1 or 2 are highest priority for documentation.
>
> Not every process needs a full record immediately. An inventory entry with a summary is better than no record. A full record is the goal over time.

---

### Process Record Template

---

**Process ID:** OP-[XXX]
**Process Name:** [Name]
**Category:** [Customer-facing / Financial / Sales and distribution / Operations / Compliance / People / Technology / Other]
**Last Updated:** YYYY-MM-DD
**Maturity Level:** [0–4]

#### Overview

**What this process does:**
[1–2 sentences. What recurring work does this process accomplish, and why does it exist?]

**Why it matters:**
[What breaks or degrades if this process fails or is disrupted? Frame in terms of customer, financial, or operational impact.]

**Trigger:**
[What starts this process? e.g., A new customer signs a contract / The first of the month arrives / A purchase order is received / A customer submits a support request]

**Frequency:**
[e.g., Per event / Daily / Weekly / Monthly / Quarterly / Annually / Per production cycle]

---

#### Ownership

| Role | Name | Responsibility |
|---|---|---|
| **Primary Owner** | [Name] | Accountable for the process end-to-end — escalation point if it breaks |
| **Executor(s)** | [Name(s)] | Responsible for running the process day-to-day |
| **Reviewer / Approver** | [Name] | Signs off on output or exceptions (if applicable) |
| **Backup** | [Name / "None identified"] | Can execute if primary is unavailable |

**Key person risk:** [Low / Medium / High]
**Risk note:** [e.g., Only one person knows how to run this process. Departure would require significant knowledge transfer or reconstruction.]

---

#### Inputs and Dependencies

**Inputs required to begin:**

| Input | Source | Owner | Notes |
|---|---|---|---|
| [e.g., Signed customer contract] | [e.g., Sales / CRM] | [Name] | [e.g., Must be countersigned before process begins] |
| [e.g., Customer configuration form] | [e.g., Customer] | [Name] | [e.g., Required fields: X, Y, Z] |
| [e.g., Prior month billing data] | [e.g., Billing platform export] | [Name] | [e.g., Available by the 3rd of each month] |

**System dependencies:**

| System | Role in Process | System of Record for | Notes |
|---|---|---|---|
| [e.g., CRM] | [e.g., Source of customer data and contract terms] | [e.g., Customer relationship data] | [e.g., Must be updated before process begins] |
| [e.g., Billing platform] | [e.g., Generates invoices and tracks payment status] | [e.g., Billing and collections data] | |
| [e.g., ERP] | [e.g., Receives posted transactions for financial reporting] | [e.g., Financial records] | |

---

#### Process Steps

> Capture the key steps — enough to understand the flow and identify where failure typically occurs. For detailed procedure documentation, link to the relevant runbook or SOP.

| Step | Description | Owner | System Used | Typical Duration | Notes |
|---|---|---|---|---|---|
| 1 | [e.g., Verify all required inputs are received and complete] | [Role] | [e.g., CRM, email] | [e.g., 30 min] | [e.g., Process does not begin until all inputs are confirmed] |
| 2 | [e.g., Create customer account in product and billing system] | [Role] | [e.g., Product admin, billing platform] | [e.g., 1 hr] | |
| 3 | [e.g., Configure product to customer's contracted specifications] | [Role] | [e.g., Product admin] | [e.g., 2–4 hrs] | [e.g., Configuration checklist required] |
| 4 | [e.g., Send welcome communication and access credentials] | [Role] | [e.g., Email, CRM] | [e.g., 30 min] | |
| 5 | [e.g., Schedule kickoff call and assign CSM] | [Role] | [e.g., CRM, calendar] | [e.g., 15 min] | |
| 6 | [e.g., Confirm go-live and update CRM status] | [Role] | [e.g., CRM] | [e.g., 15 min] | |

**Runbook / SOP link:** [Link or "Not yet documented"]
**Estimated total process time:** [e.g., 4–6 hours elapsed / 1–2 business days]

---

#### Outputs

| Output | Recipient | Format | Notes |
|---|---|---|---|
| [e.g., Active customer account] | [e.g., Customer / CSM] | [e.g., Product access + welcome email] | |
| [e.g., CRM record updated to Active] | [e.g., Sales / Finance] | [e.g., CRM status field] | [e.g., Triggers billing setup] |
| [e.g., Kickoff call scheduled] | [e.g., Customer / CSM] | [e.g., Calendar invite] | |

---

#### Known Failure Modes

> Where does this process most commonly break, slow down, or produce incorrect output? Honest documentation of failure modes is more valuable than an idealized description of how the process is supposed to work.

| Failure Mode | Cause | Frequency | Impact | Current Mitigation |
|---|---|---|---|---|
| [e.g., Process stalls waiting for customer configuration form] | [e.g., Customer is slow to respond or submits incomplete information] | [e.g., ~30% of onboardings] | [e.g., Delays go-live by 3–7 days] | [e.g., Follow-up reminder at 48 hours] |
| [e.g., Billing setup created with wrong contract terms] | [e.g., CRM contract data not updated before billing setup begins] | [e.g., Occasional] | [e.g., Incorrect invoicing — requires manual correction] | [e.g., Checklist step to verify CRM before billing setup] |
| [e.g., CSM not assigned before go-live] | [e.g., Assignment step missed under volume pressure] | [e.g., Rare] | [e.g., Customer has no point of contact at go-live] | [e.g., None — known gap] |

---

#### Downstream Process Dependencies

> Which other processes depend on the output of this one, or are triggered by its completion?

| Dependent Process | Process ID | Dependency | Notes |
|---|---|---|---|
| [e.g., Customer billing and collections] | [OP-005] | [e.g., Requires active customer account and confirmed contract terms] | [e.g., Billing setup must be completed as part of onboarding] |
| [e.g., Month-end financial close] | [OP-006] | [e.g., New customers activated mid-month require pro-rated billing entry] | |

---

#### Change Impact Notes

> Notes on how changes to product, pricing, systems, or structure have affected or would affect this process. Updated when a change is evaluated or after it lands.

| Date | Change | Impact on This Process | Status |
|---|---|---|---|
| YYYY-MM-DD | [e.g., New pricing tier added] | [e.g., Onboarding configuration step now requires tier selection — checklist updated] | [e.g., Process updated] |
| YYYY-MM-DD | [e.g., CRM migration from X to Y] | [e.g., All CRM steps in this process will need to reference new system — full retrain required] | [e.g., In progress] |

---

#### Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Should CSM assignment happen at contract signing or at go-live?] | [Name] | YYYY-MM-DD | |

---

> **Copy this template for each process that warrants a full record. Add the Process ID and name to the inventory in Section 2.**

---

## 4. Process Categories

> The organization defines its own process categories here. Categories determine how processes are grouped in the inventory and make it easier to assess impact when a change touches a particular area of the business.
>
> Suggested starting categories — edit to reflect the organization's actual structure:

| Category | Description | Examples |
|---|---|---|
| **Customer-facing** | Processes that directly involve the customer — from first contact through ongoing relationship management | New customer onboarding, feature expansion, customer support escalation, renewal management |
| **Financial** | Processes that generate, record, or manage financial transactions and reporting | Billing and collections, sales channel compensation, month-end close, accounts payable, payroll |
| **Sales and distribution** | Processes that bring the product or service to market through any channel | Sales channel onboarding, channel compensation, order management, deal desk |
| **Operations** | Processes that keep the business running — supply chain, production, logistics, facilities | Supply chain engagement, manufacturing runs, inventory management, vendor management |
| **Compliance** | Processes required by regulatory, legal, or contractual obligations | Regulatory reporting, license renewals, audit preparation, data privacy compliance |
| **People** | Processes related to the employment lifecycle | Hiring, onboarding, performance review, offboarding, benefits administration |
| **Technology** | Processes related to maintaining and evolving the technology stack | Release management, incident response, access provisioning, backup and recovery |
| **Other** | Processes that do not fit the categories above | [Define as needed] |

---

## 5. Change Impact Guide

> A structured prompt for evaluating how a proposed change interacts with existing processes. Use this alongside a Business Case or Product Build Record when a significant change is being scoped.
>
> The goal is not to block change — it is to ensure that process disruption is visible, planned for, and reflected in the cost and timeline estimates for the initiative.

### 5.1 Change Impact Assessment

**Initiative or change being evaluated:** [Name / link to Business Case or Product Build Record]

**Step 1 — Identify affected processes:**

Review the Process Inventory (Section 2) and identify every process that the proposed change could affect. A process is affected if the change alters any of the following for that process:

| Element | Question to Ask |
|---|---|
| Trigger | Does this change alter what starts the process? |
| Inputs | Does this change add, remove, or modify what the process needs to begin? |
| Steps | Does this change require new steps, eliminate existing steps, or change how steps are executed? |
| Outputs | Does this change alter what the process produces or who receives it? |
| Owner | Does this change shift who is responsible for any part of the process? |
| Systems | Does this change add, remove, or modify a system this process depends on? |
| Frequency | Does this change alter how often this process runs or what triggers it? |

**Affected processes:**

| Process ID | Process Name | Element(s) Affected | Impact Assessment | Action Required |
|---|---|---|---|---|
| [OP-XXX] | [Name] | [Trigger / Inputs / Steps / Outputs / Owner / Systems / Frequency] | [No change / Minor adjustment / Significant update required / Process redesign required] | [e.g., Update step 3, retrain executor, update runbook] |

**Step 2 — Assess disruption risk:**

For each affected process, consider:
- **Maturity:** A change to a maturity level 1 or 2 process carries more risk than the same change to a level 4 process — the lower the maturity, the less resilience the process has
- **Key person risk:** If the affected process has high key person risk, a change that disrupts it without adequate knowledge transfer is a compounded risk
- **Downstream dependencies:** A change that disrupts a process with multiple downstream dependencies can cascade across the operation

**Step 3 — Reflect in the initiative estimate:**

Process update work is a cost. If this change requires:
- Runbook or SOP updates — estimate the time
- Executor retraining — estimate the time and who delivers it
- System reconfiguration — estimate the effort and flag as a dependency
- Process redesign — consider whether this warrants its own initiative

Add these costs to the Business Case or Product Build Record cost estimate. Process disruption that is not estimated is a hidden cost.

---

## 6. Process Health Register

> A consolidated view of process health across the organization — updated at each annual review or when a significant change is made. Surfaces which processes are most at risk and where documentation investment is most urgent.

| Process ID | Process Name | Maturity | Key Person Risk | Last Reviewed | Documentation Status | Priority for Improvement | Notes |
|---|---|---|---|---|---|---|---|
| [OP-001] | [Name] | [0–4] | [Low / Med / High] | YYYY-MM-DD | [Full record / Summary / Inventory only / None] | [High / Medium / Low / None] | |

**Health register guidance:**

Prioritize documentation improvement for processes that meet any of the following criteria:
- Maturity level 0 or 1 — execution is inconsistent or nonexistent
- Maturity level 2 with High key person risk — one departure away from failure
- Any process in the Financial or Compliance category with maturity below 3
- Any process that appears frequently in the Change Impact Notes as disrupted by product or strategic changes — repeated disruption signals that the process is fragile or poorly understood

---

## 7. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there recurring processes we are aware of but have not yet added to the inventory?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., Which maturity level 1 or 2 processes carry the most operational risk and should be prioritized for documentation?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Who owns the annual process health review, and is it on the Company Calendar?] | [Name] | YYYY-MM-DD | |
