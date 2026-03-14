# Organizational Risk and Compliance

> A living record of the organization's known risks and external compliance obligations. Risk is the organization's exposure to bad outcomes — financial, operational, reputational, strategic, or security-related. Compliance is the organization's obligations to external parties — regulators, certifying bodies, customers, and lenders. They overlap but are managed differently and owned by different people. This document serves both.
>
> **This document is most valuable when it is maintained continuously, not consulted only after something goes wrong.** A risk register that is accurate is a decision-making tool. A risk register that is stale is a false sense of security.

---

## Document Control

| Field | Value |
|---|---|
| **Last Updated** | YYYY-MM-DD |
| **Updated By** | |
| **Review Cadence** | Risk inventory: quarterly / Compliance register: at each obligation renewal / Full document: annually |
| **Primary Owner** | [e.g., COO / General Counsel / CFO / CEO] |

> **Connected artifacts:**
> - **Cost-and-Benefit-Framework** — risk reduction benefit claims should reference risk records here for probability and impact inputs
> - **Key-Operational-Processes** — process failure modes here feed the risk inventory; compliance obligations often manifest as process requirements there
> - **Funding-and-Business-Model** — funding structure and ownership model create compliance obligations reflected in Section 4
> - **External-Stakeholders** — regulators, certifying bodies, and key vendors with compliance obligations are catalogued there; referenced here
> - **Institutional-Knowledge** — significant risk events, near-misses, and compliance findings belong there after being logged here
> - **Strategy-and-Intent** — strategic risks here should be visible in the Strategic Assumptions and Risks section there
> - **Company-Calendar** — compliance renewal dates, audit schedules, and regulatory filing deadlines should appear there


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 For Risk Management

The Risk Inventory (Section 2) provides a single view of known organizational risks. Use it to:
- Understand what risks the organization has acknowledged and what mitigation is in place
- Identify risks that are unmitigated or inadequately controlled
- Source probability and impact inputs for Cost-and-Benefit-Framework risk reduction benefit claims
- Evaluate whether a proposed strategic or product initiative introduces new risks or changes existing ones

When a new initiative is being evaluated — in a Business Case or Product Build Record — ask: does this initiative create a new risk, increase the probability or impact of an existing risk, or reduce risk? Update this document when the answer is yes.

### 1.2 For Compliance Management

The Compliance Obligations Register (Section 4) and Certifications and Audits log (Section 5) provide a complete view of the organization's external obligations. Use them to:
- Ensure no renewal, filing, or audit deadline is missed
- Onboard new team members responsible for compliance functions
- Provide a complete compliance picture to investors, board members, auditors, or acquirers
- Identify compliance obligations that would be affected by a proposed change in product, market, or structure

### 1.3 Risk Categories

> Used consistently throughout this document and in Cost-and-Benefit-Framework risk reduction estimates.

| Category | Description | Examples |
|---|---|---|
| **Compliance and regulatory** | Risk of violation, fine, sanction, or enforcement action by a regulatory body | Data privacy breach, missed filing, operating without required license |
| **Operational** | Risk of disruption to core business operations | System outage, key person departure, process failure, supply chain disruption |
| **Reputational** | Risk of damage to brand, customer trust, or market position | Public incident, product failure at scale, negative press or social media event |
| **Financial** | Risk of direct financial loss not captured by other categories | Fraud, uncollectible receivables, unexpected liability, contract dispute |
| **Strategic** | Risk of a market, competitive, or structural shift that erodes organizational position | Competitor capability leap, market contraction, technology displacement, loss of key channel |
| **Security** | Risk of unauthorized access, data loss, or system compromise | Data breach, ransomware, insider threat, third-party vendor compromise |
| **Legal and contractual** | Risk of legal action, contract breach, or intellectual property dispute | Customer lawsuit, vendor default, IP infringement claim |
| **People** | Risk associated with talent — availability, capability, or conduct | Key person departure, hiring failure in a critical role, misconduct |

---

## 2. Risk Inventory

> A single-view register of all known organizational risks. One row per risk. Full records in Section 3 for risks that warrant detailed documentation.
>
> **Expected value = Probability × Impact.** This is the number that enables comparison across risks and feeds Cost-and-Benefit-Framework benefit claims.

| Risk ID | Risk Name | Category | Probability (Annual) | Impact if Occurs | Expected Value (Annual) | Mitigation Status | Owner | Residual Risk | Last Reviewed | Record |
|---|---|---|---|---|---|---|---|---|---|---|
| RSK-001 | [e.g., Key person departure — critical process owner] | People | [e.g., 20%] | [e.g., $150K] | [e.g., $30K] | [Mitigated / Partial / Unmitigated] | [Name] | [Low / Med / High] | YYYY-MM-DD | [Full / Summary / Inventory only] |
| RSK-002 | [e.g., Data breach — customer PII exposure] | Security | [e.g., 8%] | [e.g., $800K] | [e.g., $64K] | [Partial] | [Name] | [Med] | YYYY-MM-DD | [Full] |
| RSK-003 | [e.g., Regulatory filing missed — annual license renewal] | Compliance | [e.g., 5%] | [e.g., $200K] | [e.g., $10K] | [Mitigated] | [Name] | [Low] | YYYY-MM-DD | [Summary] |
| RSK-004 | [e.g., Primary vendor failure or exit] | Operational | [e.g., 10%] | [e.g., $500K] | [e.g., $50K] | [Partial] | [Name] | [Med] | YYYY-MM-DD | [Full] |
| RSK-005 | [e.g., Market contraction in primary segment] | Strategic | [e.g., 15%] | [e.g., $1.2M] | [e.g., $180K] | [Unmitigated] | [Name] | [High] | YYYY-MM-DD | [Full] |

> **Mitigation status definitions:**
> - **Mitigated** — controls are in place and assessed as adequate; residual risk is acceptable
> - **Partial** — controls exist but are incomplete, untested, or reduce but do not adequately address the risk
> - **Unmitigated** — no meaningful control is in place; risk is accepted, deferred, or not yet addressed
>
> **Residual risk** is the risk that remains after mitigation controls are applied. A mitigated risk can still carry medium or high residual risk if the controls only partially reduce probability or impact.

---

## 3. Risk Records

> Full detail per significant risk. Copy the template for each risk that warrants documentation beyond an inventory entry. Prioritize: unmitigated risks, high expected value risks, and risks with high residual exposure after mitigation.

---

### Risk Record Template

---

**Risk ID:** RSK-[XXX]
**Risk Name:** [Name]
**Category:** [From Section 1.3]
**Last Updated:** YYYY-MM-DD
**Owner:** [Name / Role]

#### Description

**What is the risk:**
[1–2 sentences describing the risk event — what could happen, under what conditions.]

**Why it exists:**
[What organizational, market, or structural condition creates this exposure? e.g., We have a single vendor for a critical infrastructure component with no contractual continuity obligation and no qualified alternative identified.]

**Who or what is affected if it occurs:**
[Customers / Revenue / Operations / Reputation / Regulatory standing / Specific systems or processes]

---

#### Probability Assessment

| Field | Value |
|---|---|
| **Annual probability estimate** | [e.g., 10%] |
| **Probability basis** | [Historical data / Industry benchmark / Expert judgment / Analogous situation / Assumption] |
| **Basis detail** | [e.g., Industry benchmark — Gartner 2023 report on SaaS vendor concentration risk places single-vendor dependency in this category at 8–12% annual disruption probability] |
| **Confidence in estimate** | [High / Medium / Low] |
| **Last validated** | YYYY-MM-DD |

> Probability estimates without a stated basis are assumptions. Label them as such. See Cost-and-Benefit-Framework Section 3.3 for probability estimation standards.

---

#### Impact Assessment

| Field | Value |
|---|---|
| **Estimated impact if occurs** | [$XXX,000] |
| **Impact components** | [e.g., $200K operational recovery cost / $150K revenue at risk during disruption / $150K reputational — estimated customer churn] |
| **Impact basis** | [e.g., Estimated from prior vendor disruption in 2021 — actual cost was $180K; adjusted upward for current scale] |
| **Impact type** | [Direct financial / Operational disruption / Regulatory / Reputational / Combined] |
| **Time to recover** | [e.g., 2–4 weeks to restore full operational capacity] |

**Expected value (annual):** [Probability × Impact = $XXX,000/year]

---

#### Current Controls and Mitigation

> What is the organization currently doing to reduce the probability or impact of this risk?

| Control | Type | Mechanism | Effectiveness | Owner | Last Tested |
|---|---|---|---|---|---|
| [e.g., Vendor contract — 90-day termination notice required] | Probability reduction | [e.g., Contractual obligation gives 90 days to find alternative] | [Partial — reduces surprise, does not eliminate disruption] | [Legal] | YYYY-MM-DD |
| [e.g., Vendor alternatives shortlist maintained] | Impact reduction | [e.g., Two qualified alternatives identified and pre-vetted] | [Partial — not contracted; transition would still take 4–6 weeks] | [Operations] | YYYY-MM-DD |
| [e.g., Data export and portability tested quarterly] | Impact reduction | [e.g., Ensures data can be migrated without vendor cooperation] | [Effective] | [Engineering] | YYYY-MM-DD |

**Mitigation status:** [Mitigated / Partial / Unmitigated]

**Residual risk after controls:**

| Field | Value |
|---|---|
| **Post-mitigation probability** | [e.g., 10% — controls do not reduce likelihood, only impact] |
| **Post-mitigation impact** | [e.g., $250K — reduced from $500K by pre-vetted alternatives and data portability] |
| **Post-mitigation expected value** | [e.g., $25K/year] |
| **Residual risk level** | [Low / Medium / High] |
| **Residual risk rationale** | [e.g., Medium — probability unchanged, impact meaningfully reduced, but 4–6 week transition period still carries significant operational and revenue risk] |

---

#### Early Warning Signals

> What observable signals would indicate this risk is becoming more likely or that controls are degrading? Early warning signals allow the organization to act before the risk event occurs.

| Signal | How to Monitor | Monitoring Owner | Escalation Trigger |
|---|---|---|---|
| [e.g., Vendor financial distress indicators] | [e.g., Quarterly review of vendor public filings and credit rating] | [Name] | [e.g., Credit downgrade or missed earnings by 2+ quarters] |
| [e.g., Vendor personnel changes — key contacts departing] | [e.g., LinkedIn monitoring, relationship check-ins] | [Name] | [e.g., CTO or CEO departure at vendor] |
| [e.g., Vendor support response time degrading] | [e.g., Track in support log — flag if P1 response time exceeds SLA 2+ times in a quarter] | [Name] | [e.g., Two SLA misses in a rolling 90 days] |

---

#### Response Plan

> What will the organization do if this risk event occurs? A response plan does not need to be a detailed playbook — it needs to be enough to ensure the first 48 hours are not spent figuring out who does what.

**Immediate response (first 48 hours):**
[e.g., Activate vendor alternatives shortlist. Notify executive team. Assess current data export completeness. Communicate holding message to affected customers.]

**Owner of response:** [Name / Role]
**Escalation path:** [e.g., Operations lead → COO → CEO → Board if revenue impact exceeds $X]

**Recovery target:** [e.g., Full operational restoration within 4–6 weeks]

**Response plan last reviewed:** YYYY-MM-DD

---

#### Risk History

> Prior occurrences or near-misses. Each event logged here should also appear in Section 6 (Risk and Compliance Event Log).

| Date | Event | Actual Impact | Response | Lesson |
|---|---|---|---|---|
| YYYY-MM-DD | [e.g., Vendor experienced 36-hour outage] | [e.g., $45K operational impact — below estimate] | [e.g., Activated backup process; customer communication sent within 2 hours] | [e.g., Backup process worked but took longer than expected to activate — pre-staging would reduce recovery time] |

---

> **Copy this template for each risk that warrants a full record.**

---

## 4. Compliance Obligations Register

> Every external obligation the organization is subject to — regulatory, standards-based, contractual, or lender-imposed. A compliance obligation missed is often a risk event. The two registers are intentionally separate: risk is probabilistic; compliance is a fixed obligation with a known deadline.

| Obligation ID | Obligation Name | Type | Governing Body / Party | Scope | Renewal / Filing Date | Owner | Current Status | Consequence of Non-Compliance | Notes |
|---|---|---|---|---|---|---|---|---|---|
| CMP-001 | [e.g., State business license — [State]] | Regulatory | [e.g., State Secretary of State] | [e.g., Right to operate in [State]] | [e.g., Annual — MM/DD] | [Name] | [Current / Due soon / Overdue / Under review] | [e.g., Cease and desist, fines up to $X] | |
| CMP-002 | [e.g., SOC 2 Type II certification] | Standards | [e.g., AICPA / Audit firm] | [e.g., Security, availability, confidentiality of customer data] | [e.g., Annual audit — Q3] | [Name] | [Current — expires YYYY-MM-DD] | [e.g., Customer contract termination rights, loss of enterprise sales] | |
| CMP-003 | [e.g., GDPR — EU data subject rights compliance] | Regulatory | [e.g., EU Data Protection Authorities] | [e.g., Any processing of EU resident personal data] | [e.g., Ongoing — no fixed renewal] | [Name] | [Compliant — last assessed YYYY-MM-DD] | [e.g., Fines up to 4% of global annual revenue] | |
| CMP-004 | [e.g., Customer contract — data residency requirement] | Contractual | [e.g., Customer name] | [e.g., All customer data must remain in US-based infrastructure] | [e.g., Contract term — through YYYY-MM-DD] | [Name] | [Compliant] | [e.g., Material breach — termination right, potential damages] | |
| CMP-005 | [e.g., Debt covenant — minimum cash balance] | Lender | [e.g., Lender name] | [e.g., Minimum $X cash balance at all times] | [e.g., Quarterly reporting] | [Name / CFO] | [Compliant] | [e.g., Loan acceleration, default] | |
| CMP-006 | [e.g., Employment law — [State] wage and hour compliance] | Regulatory | [e.g., State labor board] | [e.g., All employees in [State]] | [e.g., Ongoing] | [Name / HR] | [Compliant] | [e.g., Class action exposure, fines] | |

> **Obligation types:**
> - **Regulatory** — required by a government body; non-compliance risks fines, sanctions, or loss of license to operate
> - **Standards** — required by an industry standards body or certification program; typically voluntary but often required by customers
> - **Contractual** — required by a customer, partner, or vendor agreement; non-compliance risks contract breach
> - **Lender** — required by a debt or credit agreement; non-compliance risks loan acceleration or default
> - **Internal policy** — self-imposed; included here when the organization has made a public or board-level commitment

---

## 5. Certifications and Audits

> Active certifications and their audit history. Certifications are a subset of compliance obligations — they are included separately because they have a distinct lifecycle: scope definition, audit preparation, audit execution, finding remediation, and certification renewal.

### 5.1 Active Certifications

| Certification | Governing Body | Scope | Current Status | Expiry / Renewal Date | Audit Firm | Owner | Notes |
|---|---|---|---|---|---|---|---|
| [e.g., SOC 2 Type II] | [e.g., AICPA] | [e.g., Security, availability, confidentiality — production environment] | [e.g., Certified — report dated YYYY-MM-DD] | [e.g., Annual — next audit Q3 YYYY] | [e.g., Audit firm name] | [Name] | [e.g., Customer-facing report available on request] |
| [e.g., ISO 27001] | [e.g., ISO / Certifying body] | [e.g., Information security management system] | [e.g., Certified] | [e.g., 3-year cycle — surveillance audit annual] | [e.g., Certifying body name] | [Name] | |
| [e.g., HIPAA attestation] | [e.g., HHS / Self-attested] | [e.g., Handling of PHI for healthcare customers] | [e.g., Attested — BAA template current] | [e.g., Reviewed annually] | [e.g., External counsel] | [Name] | |

### 5.2 Audit History

| Certification | Audit Date | Period Covered | Outcome | Findings | Remediation Status | Notes |
|---|---|---|---|---|---|---|
| [e.g., SOC 2 Type II] | YYYY-MM-DD | [e.g., YYYY-MM-DD to YYYY-MM-DD] | [Clean / Qualified / Adverse] | [e.g., 2 exceptions noted — access review process and backup testing cadence] | [e.g., Both remediated — YYYY-MM-DD] | |
| | | | | | | |

### 5.3 Upcoming Audit Preparation

| Certification | Next Audit Date | Preparation Owner | Preparation Start Date | Key Preparation Tasks | Status |
|---|---|---|---|---|---|
| [e.g., SOC 2 Type II] | YYYY-MM-DD | [Name] | YYYY-MM-DD | [e.g., Evidence collection, control testing, vendor review] | [Not started / In progress / Ready] |

---

## 6. Risk and Compliance Event Log

> A running record of risk events that occurred, near-misses, compliance findings, and remediation actions. This is the organization's ground truth for risk history — the source of historical data that makes future probability estimates defensible and the record that demonstrates good faith effort to regulators and auditors.
>
> Log entries do not need to be long. A brief, accurate entry made promptly is more valuable than a detailed entry reconstructed from memory weeks later. Significant entries should also be captured in Institutional-Knowledge.md.

| Date | Event ID | Type | Description | Risk / Obligation Affected | Actual Impact | Response Taken | Remediation Status | Owner | Logged to Institutional Knowledge |
|---|---|---|---|---|---|---|---|---|---|
| YYYY-MM-DD | EVT-001 | [Risk event / Near-miss / Compliance finding / Audit finding / Policy breach] | [Brief description of what occurred] | [RSK-XXX or CMP-XXX] | [Actual financial, operational, or regulatory impact] | [What was done in response] | [Remediated / In progress / Accepted / Deferred] | [Name] | [Yes — link / No] |
| | | | | | | | | | |

**Event type definitions:**
- **Risk event** — a risk from the inventory materialized in whole or in part
- **Near-miss** — a risk event that almost occurred but was averted — as valuable as an actual event for improving controls
- **Compliance finding** — an obligation was not met, or a gap was identified before a formal audit
- **Audit finding** — a finding raised by an external auditor or regulator
- **Policy breach** — an internal policy was violated, whether or not it resulted in external consequence

---

## 7. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there compliance obligations the organization is subject to that have not yet been added to the register?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., Which unmitigated risks in the inventory require a formal mitigation decision — accept, transfer, or remediate?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Are all compliance renewal dates reflected in the Company Calendar?] | [Name] | YYYY-MM-DD | |
| 4 | [e.g., Which risk records are overdue for a probability reassessment based on new market or operational information?] | [Name] | YYYY-MM-DD | |
