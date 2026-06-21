# Product Build Record

> The complete record of a discrete product effort at a specific validation stage — from problem definition through requirements, cost estimation, execution, and validation findings. Multiple Product Build Records may execute against a single Business Case, each one moving through a validation stage (Prototype → Pilot → Beta → A/B → GA) and passing its findings forward to the next.
>
> **This document is a unit of learning, not just a unit of delivery.** A prototype record that answers one question well and informs the next record has done its job — even if nothing was shipped to customers. The Validation Stage field in Document Control signals what this record is trying to learn or deliver, and determines which sections are load-bearing.
>
> **This document is elaborated just-in-time, not front-loaded.** Fill each section to the depth the current increment actually needs — no more. Requirements, design, and estimates are expected to emerge and sharpen as you build and learn, not to be resolved in full before work starts. A record is not a gate to clear before development; it is a living workspace that grows alongside the work. Section 12 (Agent Handoff) is populated at handoff; Sections 13–14 are populated during and after execution. Each section completed adds value independently — and a record carried through to actuals and retrospective becomes a reference class anchor for future initiatives.
>
> **This record serves the team's velocity; it does not tax it.** The durable team pulls prioritized work and owns how and when it is sequenced — the Business Case sets which directions earn investment, and the team owns delivery, keeping its autonomy and cadence. The record's only job is to capture and broadcast learnings, and it should do so by augmenting the team (pulling context from commits, PRs, execution events, and metrics via AI assistance) rather than asking them to stop and write reports.
>
> Human teams may use this document without Section 12. AI-assisted teams will get significantly better results with Section 12 populated — it is the primary mechanism for reducing ambiguity at handoff.

---

## Document Control

| Field | Value |
|---|---|
| **Initiative Name** | |
| **Record Type** | Maintenance / Incremental Improvement / Strategic Request / Growth Initiative |
| **Validation Stage** | Prototype / Pilot / Beta / A/B Test / General Availability |
| **Status** | Shaping / In Build / Validating / Complete / Paused / Cancelled |
| **Author** | |
| **Created** | YYYY-MM-DD |
| **Last Updated** | YYYY-MM-DD |
| **Target Release** | YYYY-MM-DD |
| **Actual Release** | YYYY-MM-DD |
| **Linked Business Case** | [Optional — links to overarching prioritization context only, never an approval gate. Often "Not applicable"] |
| **Prior Build Record(s)** | [Link to predecessor record(s) in this validation sequence, or "First in sequence"] |
| **Linked Strategy Goal** | [Reference to Strategy-and-Intent goal this effort serves] |

> **Record Type Definitions:**
> - **Maintenance**: Bug fixes, technical debt, minor enhancements — low complexity, contained scope
> - **Incremental Improvement**: Meaningful enhancements to existing functionality — measurable growth within existing markets
> - **Strategic Request**: Customer-driven feature work — validate broad applicability before committing
> - **Growth Initiative**: New products, new user segments, or new markets — expanding beyond current footprint

> **Validation Stage Definitions:**
> - **Prototype**: An early, limited build designed to test a concept or hypothesis — not for customer use; produced to generate learning, not delivery. Requirements are deliberately lightweight. Success is defined as a clear answer to a specific question, not a shippable product.
> - **Pilot**: A controlled release to a defined, consenting subset of customers or users. Scope is real but bounded. Success criteria gate progression to broader rollout. Findings are expected to refine requirements for the next record.
> - **Beta**: Broader early access — more users than a pilot, less control. Designed to surface edge cases, gather qualitative feedback, and begin building reference customers. A beta record may run in parallel with continued development.
> - **A/B Test**: A specific variation tested against a control in a live environment. Requires a hypothesis, a measurement plan, a minimum sample size, and a decision framework defined before launch. Results feed directly into the next record or confirm GA readiness.
> - **General Availability**: Full release to the intended audience. All prior validation stages have produced sufficient confidence to commit to broad rollout.
>
> **A Business Case sets overarching, feature-level prioritization; Product Build Records deliver against it incrementally and do not loop back to it for approval or sequencing.** Once a direction is prioritized, the incremental, end-to-end delivery of value runs on its own cadence — each record captures lightweight, human-readable context for why choices were made and what was learned, rather than returning to a business-case gate. Findings flow forward: a prototype refines the next record's direction; a pilot sharpens what GA should be. Where findings materially change the original economic picture, they are surfaced back to the Business Case as context — not as a re-approval. Each record is lightweight relative to its stage — a prototype record does not need a full non-functional requirements section. The validation stage field signals to every reader which sections are load-bearing for this record.

> **How much depth each section warrants — by record type and validation stage.**
> A guide for *right-sizing* a record, not a checklist of deliverables. Nothing here is a gate; it points to where the signal is for the work in front of you, and every section is still elaborated just-in-time.
>
> | Section | Maintenance | Incremental | Strategic / Growth — Prototype | Strategic / Growth — Pilot / Beta | Strategic / Growth — A/B | Strategic / Growth — GA |
> |---|---|---|---|---|---|---|
> | 1. Problem Statement | 1.2 only | All | All | All | 1.2 + hypothesis | All |
> | 2. Goals & Metrics | Goals + 1 KPI | All | Learning goals only | All | Hypothesis + success metric | All |
> | 3. Personas | Optional | Optional | Lightweight | Recommended | Recommended | Recommended |
> | 4. Cost Estimate | Optional — relative value by default | Optional — relative value by default | ROM if a figure is needed | Optional | ROM if a figure is needed | Three-point if a financial commitment needs it |
> | 5. Functional Requirements (regulated overlay) | Skip unless regulated | Skip unless regulated | Skip unless regulated | Skip unless regulated | Skip unless regulated | Skip unless regulated |
> | 6. User Stories (requirements home) | Recommended | Recommended | Lightweight — core concept only | Full | Variation defined only | Full |
> | 7. Non-Functional Requirements | Affected only | Affected only | Skip | Key areas only | Skip | All |
> | 8. Design & UX | Optional | Recommended | Wireframes / mockups | Recommended | Recommended | Recommended |
> | 9. Dependencies & Constraints | Recommended | Recommended | Key blockers only | Recommended | Recommended | Recommended |
> | 10. Open Questions | Recommended | Recommended | Recommended — questions drive the prototype | Recommended | Recommended | Recommended |
> | 11. Test & Validation | Recommended | Recommended | Concept validation methods | Pilot-appropriate methods | A/B test plan | Full QA + sign-off |
> | 12. Agent Handoff | Optional | Optional | Optional | Optional | Optional | Optional |
> | 13. Execution Log | Recommended | Recommended | Recommended | Recommended | Recommended | Recommended |
> | 14. Actuals & Retrospective | Recommended | Recommended | Recommended — findings feed next record | Recommended | Recommended — decision logged | Recommended |
>
> "Full" and the per-cell depths describe how far a section should eventually go for that stage — not what must exist before build starts. Elaborate each just-in-time. The learning-capture sections (Execution Log, Actuals & Retrospective) are the framework's strong default — populate them as a byproduct of the work, ideally automated, never as a gate.


> **Significant Change Log**
> A record of meaningful changes to this document after initial creation — entries made when the scope, intent, assumptions, or decisions captured here shift in a way that would affect how a reader interprets this effort. Routine progress updates, status changes, and date confirmations do not require a log entry. A log entry is warranted when: the scope or success criteria change materially, a key assumption underlying this effort is revised, a decision is reversed or significantly modified, or new information emerges mid-effort that would have changed the original document if known at the start.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context for anyone reviewing this record after the fact.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The event, decision, or discovery that prompted it — e.g., Board review raised new constraint / Mid-pilot finding invalidated original hypothesis / Scope reduced due to resource reallocation] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. Problem Statement

### 1.1 Context
> What environment is this solution going into? Describe the existing system, workflow, or market context.
> Keep to 2–3 paragraphs. Link to supporting research, data, or prior documents.

[Describe the market, customer, or operational context that makes this problem worth solving.]

### 1.2 Problem Definition

**The problem is:** [One clear sentence.]

**We know this is a problem because:** [Evidence — data, customer feedback, support tickets, research.]

**If we don't solve this:** [Consequence of inaction — lost revenue, churn, compliance risk, etc.]

### 1.3 Opportunity
> What is the size and shape of the opportunity if we solve this well?

[Quantify where possible: affected users, revenue potential, cost savings, risk reduction.]

---

## 2. Goals and Success Metrics

### 2.1 Business Goals

- [ ] Goal 1: [e.g., Reduce customer onboarding time by X%]
- [ ] Goal 2: [e.g., Increase feature adoption among existing accounts by X%]
- [ ] Goal 3: [e.g., Achieve SOC2 / HIPAA / ISO compliance requirement]

### 2.2 User Goals

- [ ] User Goal 1: [e.g., Complete the core workflow in under 3 minutes]
- [ ] User Goal 2: [e.g., Understand current status without contacting support]

### 2.3 Success Metrics (KPIs)

| Metric | Baseline | Target | Measurement Method | Lookback Date |
|---|---|---|---|---|
| [e.g., Onboarding completion rate] | X% | Y% | [e.g., Funnel report] | [e.g., 90 days post-launch] |
| [e.g., Support ticket volume] | X/week | Y/week | [e.g., Helpdesk report] | [e.g., 60 days post-launch] |
| [e.g., Time to complete core flow] | Xs | Ys | [e.g., Session recording] | [e.g., 30 days post-launch] |

> **Note:** Lookback Date is when this metric will be evaluated in Section 14 (Actuals and Retrospective). Set it now, not after launch.

### 2.4 Non-Goals

- [e.g., Multi-language support — English only for v1]
- [e.g., Mobile app — web only for v1]
- [e.g., Bulk import — single-record workflow only in this phase]

---

## 3. Users and Personas
> Reference Roles-and-Personas.md for full persona detail. Summarize here — only the role types relevant to this initiative.
>
> For most initiatives, the primary user is the most important persona to capture. For initiatives with significant go-to-market, pricing, or compliance implications, buyer, gatekeeper, and affected party personas may also be relevant. Do not force role types that are not meaningfully present — capture what shapes this initiative.

### 3.1 Primary User

**Persona**: [Name / Role — link to full persona in Roles-and-Personas if defined]
**Key Need**: [What they are trying to accomplish]
**Pain Point**: [What currently frustrates or blocks them]

### 3.2 Other Relevant Roles

> Include only the role types that meaningfully affect this initiative's design, delivery, or adoption.

| Role Type | Persona | Relevance to This Initiative |
|---|---|---|
| [e.g., Buyer] | [e.g., VP Operations — link to Roles-and-Personas] | [e.g., Approval authority for this feature's pricing tier — ROI framing required] |
| [e.g., Gatekeeper] | [e.g., IT Security Reviewer] | [e.g., Security review required before launch — SOC 2 documentation needed] |
| [e.g., Internal Affected Party] | [e.g., Finance Team] | [e.g., Data flow change affects month-end reconciliation process] |
| [e.g., External Affected Party] | [e.g., End Consumer] | [e.g., Consumer-facing communication generated by this feature — accessibility required] |

### 3.3 Out-of-Scope

- [e.g., End consumers interacting directly with the product — B2B only for this initiative]
- [e.g., External partners — internal users only in this phase]

---

## 4. Cost Estimate

> Estimate to the depth the decision in front of you needs — a rough forecast to size a bet, not a gate to clear before work can start. **When sequencing the development work itself, order it by relative business value — the agile default — rather than absolute cost.** ROM and Three-Point (see Cost-and-Benefit-Framework) are *available tools* for putting a money figure behind a financial commitment, not required steps — reach for them only when stakes or uncertainty justify it. Actuals are recorded in Section 14, and the estimate-vs-actual gap is where the learning is — that loop matters more than up-front precision.
> All estimates reference the Cost-and-Benefit-Framework for methods and labor rates.

### 4.1 Cost Summary

> Lightweight by default. Capture a rough cost only if a financial decision needs one — otherwise note that delivery is sequenced by relative business value and move on.

| Item | Rough Estimate | Basis / Provenance | Confidence | One-Time / Annual |
|---|---|---|---|---|
| [e.g., Build effort] | [e.g., ~6–8 weeks, 2 eng] | [e.g., Expert judgment — analogous to Initiative X] | [Low / Med / High] | One-time |
| [e.g., External / vendor] | [e.g., $X/yr] | [e.g., Current pricing tier] | [Med] | Annual |
| [e.g., Ongoing maintenance] | [e.g., ~X hrs/mo] | [e.g., Similar feature] | [Low] | Annual |

**Opportunity cost:** [What this displaces, or "not identified."]
**Provenance:** [Historical analogy / Structured decomposition / Expert judgment / Assumption — one line on what the figure rests on. Don't present a number without saying what it's based on.]

> **When a higher-stakes financial commitment needs a decomposed, defensible estimate** — a budget envelope, an investment decision, a Business Case — use ROM or Three-Point per the Cost-and-Benefit-Framework (Part 2) and link or attach it here. Those are tools for the financial decision, not a required step for delivery.

---

## 5. Functional Requirements — Optional (Regulated / Compliance Overlay)

> **Most records skip this section.** Requirements live as user stories with acceptance criteria in Section 6 — a story plus its acceptance criteria *is* the requirement. Maintaining a separate numbered specification on top of stories is a traceability overlay, not a default.
>
> **Use this register only when an audit trail is genuinely needed** — regulated, compliance-bound, or large multi-team builds where requirement → story → test traceability must be demonstrable. When you do use it, give each requirement a `REQ-` ID and link it from the relevant story (Section 6) and test case (Section 11.6).
> **Priority**: P0 = Must have (launch blocker) | P1 = Should have | P2 = Nice to have

| ID | Requirement | Priority | Linked Story | Notes |
|---|---|---|---|---|
| REQ-001 | [e.g., User must be able to log in with email and password] | P0 | Story 1 | |
| REQ-002 | [e.g., System must lock account after 5 failed attempts] | P0 | Story 1 | Security requirement |
| REQ-010 | [e.g., Reports must generate within 5 seconds for 12 months of data] | P0 | Story 2 | Performance SLA |

> If you are not in a regulated or audit context, leave this section empty and work entirely from Section 6.

---

## 6. User Stories

> **This is the primary home for requirements.** A story with its acceptance criteria *is* the requirement — for most work you need nothing more. The numbered register in Section 5 is an optional overlay used only in regulated or audit contexts.
>
> Format: **As a** [persona], **I want to** [action], **so that** [outcome].

---

### Story 1: [Short descriptive title]

**As a** [persona],
**I want to** [action],
**so that** [outcome].

**Acceptance Criteria:**
- [ ] AC-001: Given [context], when [action], then [expected result]
- [ ] AC-002: Given [context], when [action], then [expected result]
- [ ] AC-003: Given [context], when [action], then [expected result]

**Linked Requirements (only if using the §5 overlay):** REQ-001, REQ-002
**Priority:** P0

---

### Story 2: [Short descriptive title]

**As a** [persona],
**I want to** [action],
**so that** [outcome].

**Acceptance Criteria:**
- [ ] AC-004: Given [context], when [action], then [expected result]
- [ ] AC-005: Given [context], when [action], then [expected result]

**Linked Requirements (only if using the §5 overlay):** REQ-010, REQ-011
**Priority:** P0

---

> Add stories as needed.

---

## 7. Non-Functional Requirements

> Capture the non-functional requirements the current increment actually touches — the performance, security, accessibility, and reliability bars relevant now. Don't pre-specify the full set up front; add to this section as increments reach surfaces that need it.
> Maintenance and Incremental: complete only sections affected by this change.

### 7.1 Performance
- [ ] [e.g., Page load time must not exceed 2 seconds on a standard broadband connection]
- [ ] [e.g., API must respond within 500ms at P99 under normal load]
- [ ] [e.g., System must support X concurrent users without degradation]

### 7.2 Security and Compliance
- [ ] [e.g., All sensitive data must be encrypted at rest and in transit]
- [ ] [e.g., Feature must comply with applicable requirements — SOC2 / HIPAA / GDPR / ISO 27001]
- [ ] [e.g., User data handling must comply with applicable privacy regulations]

### 7.3 Accessibility
- [ ] [e.g., All interactive elements must meet WCAG 2.1 AA standards]
- [ ] [e.g., Screen reader compatibility required for all user-facing flows]

### 7.4 Reliability and Uptime
- [ ] [e.g., Target uptime: 99.9%]
- [ ] [e.g., Graceful degradation required if a downstream dependency is unavailable]

---

## 8. Design and UX

### 8.1 Design Assets

| Asset | Link | Status |
|---|---|---|
| Wireframes | [Figma link] | Draft |
| Final Designs | [Figma link] | Pending |
| Design System Reference | [Link] | |

### 8.2 UX Principles for This Feature

- [e.g., Minimize steps — target no more than 3 screens to complete core flow]
- [e.g., Error messages must be plain language, never raw error codes]
- [e.g., All destructive actions require a confirmation step]

---

## 9. Dependencies and Constraints

### 9.1 Dependencies

| Dependency | Type | Owner | Status | Risk if Delayed |
|---|---|---|---|---|
| [e.g., Third-party data provider API] | External vendor | [Name] | Confirmed | High |
| [e.g., Auth service upgrade] | Internal team | [Team] | In progress | Medium |
| [e.g., Legal review] | Internal | Legal | Not started | High |

### 9.2 Constraints

- **Timeline**: [e.g., Must ship before Q3 regulatory deadline]
- **Budget**: [e.g., No new vendor contracts — must use existing stack]
- **Technical**: [e.g., Must integrate with legacy system via existing API — no schema changes]
- **Regulatory**: [e.g., Data must remain within specified geographic boundaries]

---

## 10. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Does this feature apply to all account tiers or only paid plans?] | [Name] | YYYY-MM-DD | |
| 2 | [e.g., What is the fallback behavior if the upstream service is unavailable?] | [Name] | YYYY-MM-DD | |
| 3 | [e.g., Are there regional variations in the workflow that need to be accommodated?] | [Name] | YYYY-MM-DD | |

---

## 11. Test and Validation

> Validation means different things at different stages. Internal QA confirms that what was built works correctly. User and market validation confirms that what was built is the right thing. Both matter — but they belong at different points in the lifecycle and require different methods.
>
> Complete the subsections that correspond to this record's Validation Stage. A prototype record needs concept validation, not a full QA suite. A GA record needs full QA, not just a concept question. Complete what is appropriate; leave the rest clearly marked as not applicable for this stage.

### 11.1 Validation Strategy

> Define upfront what this build needs to validate and how. The questions being answered here should drive which methods are used.

**The primary question this build is designed to answer:**
[One sentence. e.g., "Do users understand the new navigation pattern without instruction?" / "Does the pilot segment experience the projected time savings?" / "Does variant B produce a higher completion rate than variant A?"]

**Validation method(s) for this stage:** [Select all that apply]
- [ ] Internal QA — requirement and acceptance criteria verification
- [ ] Concept / usability testing — structured sessions with representative users
- [ ] Prototype review — stakeholder or user feedback on early build or mockup
- [ ] Pilot — controlled release to defined customer subset
- [ ] Beta — broader early access with instrumented feedback collection
- [ ] A/B test — live comparison of variant against control
- [ ] Post-launch measurement — metric lookback at defined intervals

**Who provides validation input:**
[e.g., Internal QA team / 5 representative customers recruited from Reference-Customers-and-Champions / Pilot cohort of 10 accounts / All users — 50/50 split]

**What a successful validation looks like for this stage:**
[Define clearly before testing begins — not after results come in. e.g., "80% of usability test participants complete the core task without assistance" / "Pilot accounts report 30%+ time savings within 30 days" / "Variant B completion rate exceeds variant A by ≥5% with p<0.05"]

**What finding would cause this build to be revised or abandoned:**
[The honest answer to "what would change our minds?" e.g., "If fewer than 50% of pilot accounts activate the feature within 60 days, we will treat adoption friction as unresolved and create a new record before GA commitment."]

---

### 11.2 Concept and Usability Validation
> *Applicable stages: Prototype, Pilot, Beta. Skip for Maintenance, Incremental, and A/B.*

**Method:** [e.g., Moderated usability sessions / Unmoderated remote testing / Stakeholder walkthrough / Customer interview]
**Participants:** [Number, recruitment source, how representative of target persona]
**Session structure:** [Brief description — what participants were asked to do or evaluate]

| Session # | Participant | Role / Segment | Task Completion | Key Observations | Follow-on Questions Surfaced |
|---|---|---|---|---|---|
| 1 | [Name / Anonymous] | [e.g., Operations Manager — mid-market] | [Complete / Partial / Failed] | [What they did, said, or struggled with] | |
| 2 | | | | | |

**Synthesis:**
[What patterns emerged across sessions? What worked, what didn't, and what was surprising? 3–5 sentences.]

**Findings that change the requirements:**
[List any requirement that should be added, removed, or modified based on these findings. These become inputs to the next Product Build Record if this is a prototype or pilot stage.]

- [e.g., REQ-003 — users expected inline validation, not a modal error. Requirement should be revised.]
- [e.g., New requirement needed — users looked for a "save draft" option that does not exist in current scope.]

---

### 11.3 Pilot Validation
> *Applicable stages: Pilot. Skip for all others.*

**Pilot design:**

| Field | Value |
|---|---|
| **Pilot cohort** | [How many accounts / users, how selected, from what segment] |
| **Pilot duration** | [Start date — end date] |
| **Instrumentation** | [How is usage and outcome data being collected?] |
| **Success criteria** | [From Section 11.1 — repeated here for clarity] |
| **Gate decision** | [What happens at pilot end — proceed to beta / GA / revise / stop?] |

**Pilot participants:**

| Organization | Contact | Segment | Activation Date | Engaged | Notes |
|---|---|---|---|---|---|
| [Name] | [Name] | [e.g., Mid-market / Healthcare] | YYYY-MM-DD | [Yes / No / Partial] | |

**Pilot results:**

| Metric | Target | Actual | Notes |
|---|---|---|---|
| [e.g., Feature activation rate] | [e.g., >70% within 30 days] | | |
| [e.g., Reported time savings] | [e.g., ≥30%] | | |
| [e.g., Support tickets generated] | [e.g., <2 per account] | | |

**Qualitative feedback summary:**
[What did pilot participants say — in their own words where possible. What did they value, what frustrated them, what surprised them.]

**Gate decision:**
- [ ] Proceed to Beta / GA — success criteria met; requirements confirmed
- [ ] Revise and re-pilot — findings require material requirement changes; new record to be created
- [ ] Stop — findings indicate the approach does not solve the problem as hypothesized

**Gate decision rationale:**
[Brief explanation of the decision and what evidence drove it.]

**Findings that feed the next record:**
[Requirements added, removed, or revised based on pilot. Benefit estimate adjustments for the Business Case. Persona or Product Chronicle updates triggered.]

---

### 11.4 Beta Validation
> *Applicable stages: Beta. Skip for all others.*

**Beta design:**

| Field | Value |
|---|---|
| **Beta cohort** | [Size, selection method, segment coverage] |
| **Beta duration** | [Start — end] |
| **Access model** | [e.g., Opt-in / Invited / Feature flag — % of traffic] |
| **Feedback collection** | [e.g., In-app survey / NPS pulse / CS check-in / Support ticket monitoring] |
| **Success criteria** | [From Section 11.1] |

**Quantitative results:**

| Metric | Baseline | Target | Actual | Notes |
|---|---|---|---|---|
| [e.g., Adoption rate — beta cohort] | | | | |
| [e.g., Error rate] | | | | |
| [e.g., NPS — beta users] | | | | |

**Qualitative feedback themes:**
[What were the most common themes in feedback? What was praised, what was criticized, what was requested?]

**Edge cases surfaced:**
[Unexpected behaviors, failure modes, or use cases discovered during beta that were not anticipated in requirements.]

**GA readiness assessment:**
- [ ] Ready for GA — no material issues; proceed
- [ ] Ready with known limitations — proceed with documented exceptions and a plan to address
- [ ] Not ready — material issues require a new record before GA

---

### 11.5 A/B Test Plan and Results
> *Applicable stages: A/B Test. Skip for all others.*

**Hypothesis:**
[Formal hypothesis statement: "We believe that [variant] will produce [outcome] for [audience] because [reasoning]. We will know this is true when [measurable result]."]

**Test design:**

| Field | Value |
|---|---|
| **Control (A)** | [Description of current / baseline experience] |
| **Variant (B)** | [Description of what is being changed] |
| **Audience** | [Who is in the test — segment, % of traffic, inclusion/exclusion criteria] |
| **Split** | [e.g., 50/50 / 80/20] |
| **Primary metric** | [The one metric that determines the winner] |
| **Secondary metrics** | [Metrics monitored for unintended effects] |
| **Minimum sample size** | [Calculated before launch — not after] |
| **Minimum run duration** | [e.g., 2 weeks minimum regardless of sample size — accounts for day-of-week effects] |
| **Decision framework** | [e.g., Adopt B if primary metric improves ≥5% with p<0.05 and no secondary metric degrades >10%] |

**Results:**

| Metric | Control (A) | Variant (B) | Difference | Statistical Significance | Notes |
|---|---|---|---|---|---|
| [Primary metric] | | | | [p = X / Not significant] | |
| [Secondary metric] | | | | | |

**Decision:**
- [ ] Adopt variant B — hypothesis confirmed; proceed to GA
- [ ] Retain control A — hypothesis not confirmed; variant did not outperform
- [ ] Inconclusive — insufficient sample or significance; extend test or redesign
- [ ] Stop — variant B caused meaningful degradation in secondary metrics

**Decision rationale and next record implications:**
[What the results mean for the next step. If adopting B, what GA requirements change? If retaining A, what was learned about the hypothesis that informs a revised approach?]

---

### 11.6 Internal QA — Test Cases
> *Applicable stages: Pilot, Beta, GA. Lightweight for Prototype. Skip for A/B (no new build).*

> Maps tests to what they verify. By default, link each test to a story / acceptance criterion in Section 6 — the "Linked Requirement" column is only needed when you are using the Section 5 regulated overlay. Populate the Results column during QA.

| Test ID | Linked Requirement | Linked Story / AC | Test Description | Expected Result | Actual Result | Pass / Fail | Tested By | Date |
|---|---|---|---|---|---|---|---|---|
| TC-001 | REQ-001 | AC-001 | [e.g., Log in with valid credentials] | [e.g., User reaches dashboard] | | | | |
| TC-002 | REQ-002 | AC-002 | [e.g., Enter wrong password 5 times] | [e.g., Account locked, notification sent] | | | | |
| TC-003 | REQ-010 | AC-004 | [e.g., Generate report for 6-month range] | [e.g., Report renders within 5 seconds] | | | | |
| TC-004 | REQ-011 | AC-005 | [e.g., Generate report under concurrent load] | [e.g., Response within SLA at P99] | | | | |

### 11.7 Edge Cases and Negative Tests

| Test ID | Scenario | Expected Behavior | Actual Result | Pass / Fail |
|---|---|---|---|---|
| TC-E001 | [e.g., Submit form with missing required fields] | [e.g., Inline validation shown, submission blocked] | | |
| TC-E002 | [e.g., Submit the same form twice rapidly] | [e.g., Duplicate submission prevented] | | |
| TC-E003 | [e.g., Network drops mid-submission] | [e.g., Graceful failure, no partial record created] | | |

### 11.8 Validation Confirmation

> The team confirms the work is validated and ready — owned by the people who built it, not a gate cleared by outside approvers. One line is enough: what was validated, by whom, and that it meets the bar for this stage.

**Validated and ready:** [Yes / Not yet — what's outstanding]
**Confirmed by (team):** [Name(s) / role(s)] **Date:** YYYY-MM-DD
**Notes:** [Anything a reader should know — known limitations carried forward, deferred edge cases, etc.]

> **Formal multi-role sign-off (optional — GA and regulated contexts only):** where a release genuinely requires documented approval (compliance, contractual, or safety-critical), record it here.
>
> | Role | Name | Approval | Date |
> |---|---|---|---|
> | Product | | | |
> | Engineering Lead | | | |
> | QA Lead | | | |
> | Compliance / Legal (if applicable) | | | |

---

## 12. Agent Handoff Instructions

> Written for AI-assisted development teams or autonomous agents.
> Human teams may skip this section — all requirements are fully stated above.

### 12.1 Objective

In plain language, the goal of this build is: [One sentence — what are we building and what should it do?]

### 12.2 Inputs

- [ ] This Product Build Record (requirements and acceptance criteria)
- [ ] Design assets: [Link]
- [ ] API documentation: [Link]
- [ ] Existing codebase context: [Repo / branch / folder]
- [ ] Test data / sandbox credentials: [Link or location]

### 12.3 Explicit Constraints

- **Do not** modify shared services — integrate via API only
- **Do not** deploy to production — deliver to staging environment only
- **Do not** introduce new external dependencies without approval
- **Do not** store sensitive data outside approved, compliant storage
- [Add constraints specific to this initiative]

### 12.4 Ambiguity Protocol

1. Check the Open Questions log (Section 10) first
2. Default to the most conservative interpretation that satisfies the requirement
3. Flag the ambiguity as a comment in the PR — do not silently choose
4. Do not block on minor unknowns — implement with a clearly marked `TODO`
5. Log any new questions discovered during development in Section 10

### 12.5 Definition of Done

- [ ] The increment is working, validated, and delivers the value this record set out to deliver
- [ ] Acceptance criteria for the agreed scope are passing (the P0 stories in Section 6; plus the Section 5 register where the regulated overlay is in use)
- [ ] All test cases in Section 11 pass
- [ ] No regressions in [existing feature / test suite]
- [ ] Code is documented and follows [style guide / conventions link]
- [ ] Test results are filled into Section 11
- [ ] Any deviations from the agreed scope are documented with rationale
- [ ] PR submitted to [branch] with staging deployment link confirmed

---

## 13. Execution Log

> A running record of anything that happens during the build that affects scope, cost, timeline, or outcome. Updated in real time — not reconstructed after the fact.
>
> **Why this exists:** Mid-build decisions are where estimates diverge from actuals. Without a record of what changed and why, the retrospective cannot produce useful learning, and future estimates cannot account for the patterns that actually drive variance. Brief entries are better than no entries.

| Date | Type | Description | Impact | Decision / Resolution | Owner |
|---|---|---|---|---|---|
| YYYY-MM-DD | [Scope change / Blocker / Decision / Discovery / Team change / External dependency] | [What happened] | [Cost / Timeline / Quality — brief impact statement] | [What was decided and by whom] | [Name] |
| | | | | | |
| | | | | | |

**Execution log entry types:**
- **Scope change** — requirements added, removed, or modified after approval
- **Blocker** — something that stopped or significantly slowed progress
- **Decision** — a meaningful choice made during build that wasn't covered by the requirements
- **Discovery** — something learned during build that was not known at estimate time
- **Team change** — a change in who is working on the initiative
- **External dependency** — a delay or change caused by something outside the team's control

---

## 14. Actuals and Retrospective

> Completed after launch and at defined lookback intervals. This section closes the loop between estimate and reality — and generates the reference class data that improves future estimates.
>
> Complete as much of this section as the initiative allows. A full retrospective produces the most value — but even partial actuals (just cost and timeline) are worth capturing. An organization that captures actuals without a full retrospective is still learning. One that captures nothing learns nothing.
>
> The more consistently this section is completed, the faster the organization's estimates improve. Treat it as an investment in the next initiative, not an obligation on this one.

### 14.1 Cost Actuals

| Cost Item | Estimated (Weighted) | Actual | Variance | Variance % | Notes |
|---|---|---|---|---|---|
| Internal labor — build | | | | | |
| Internal labor — maintenance (first year) | | | | | |
| External / vendor | | | | | |
| Infrastructure | | | | | |
| **Total** | | | | | |

**Timeline actuals:**

| | Estimated | Actual | Variance |
|---|---|---|---|
| Build start date | | | |
| Launch date | | | |
| Total elapsed calendar time | | | |

---

### 14.2 Variance Analysis

> Required when any cost or timeline variance exceeds 20%. Brief is fine — the goal is a usable signal for future estimates, not a post-mortem report.

**Primary driver of cost variance:**
[What was the single biggest reason actual cost differed from estimate? e.g., Discovery during build revealed an undocumented dependency in the legacy auth system — added 40 hours of unplanned engineering work.]

**Primary driver of timeline variance:**
[e.g., External vendor API documentation was incomplete — 2-week delay waiting for clarification and updated specs.]

**Was the estimate provenance appropriate for this initiative?**
[e.g., Structured decomposition was appropriate. The variance was not a method problem — it was a discovery problem. The estimate would have been more accurate with a spike to investigate the legacy system before committing.]

**What would have improved this estimate?**
[e.g., A 1–2 day technical discovery sprint before three-point estimation. The unknowns in the legacy system were knowable — we chose not to investigate before estimating.]

---

### 14.3 Benefit Realization

> Measured at the lookback dates defined in Section 2.3. Copy the metrics table from Section 2.3 and fill in actuals.
>
> For Prototype and Pilot stages, benefit realization is measured against the learning goals defined in Section 11.1 — not against the full Business Case targets, which are validated progressively across the sequence of records.

**Lookback date:** YYYY-MM-DD  **Days post-launch:** [X]

| Metric | Baseline | Target | Actual | vs. Target | Notes |
|---|---|---|---|---|---|
| [From Section 2.3] | | | | [On track / Below / Exceeded] | |
| | | | | | |

**Benefit realization summary:**
[2–3 sentences on whether the initiative delivered its intended benefits at this stage. Honest assessment. e.g., Pilot accounts reported an average 34% reduction in manual processing time against a 30% target — hypothesis confirmed. Adoption rate within the pilot cohort was 65%, below the 80% target — onboarding friction is unresolved and should be addressed before GA commitment.]

**Business Case implications:**
[Does this record's findings change the benefit estimates in the linked Business Case? If so, describe the revision. e.g., Pilot results support the cost reduction benefit estimate. Revenue growth estimate should be revised downward — adoption friction will likely delay benefit realization by one quarter relative to the original model. Business Case owner notified: [Name], YYYY-MM-DD.]

**Will this initiative continue to the next validation stage or require a new record?**
- [ ] Continue to next stage — [Pilot / Beta / A/B / GA] — findings support progression; new record to be created
- [ ] Revise and repeat this stage — findings require material changes; new record at same stage
- [ ] Proceed to GA from here — no further staged validation needed
- [ ] Stop — findings indicate the approach does not solve the problem as hypothesized
- [ ] Complete — this was a GA record; no further validation stages

**Next record implications:**
[What should the next Product Build Record do differently based on what was learned here? What requirements should change? What hypotheses remain open? What should be carried forward and what should be abandoned? This is the primary handoff from one record to the next.]

- [e.g., Onboarding step 3 needs to be redesigned before GA — users consistently stall here]
- [e.g., The mobile experience was not tested in the pilot — it should be a specific test case in the beta record]
- [e.g., Requirement REQ-008 was never triggered in pilot — confirm it is still needed before carrying forward]

---

### 14.4 Reference Class Record

> This section is the initiative's contribution to the organization's cost history. Future initiatives will reference it via reference-class forecasting (see Cost-and-Benefit-Framework, Reference Class and Cost History) when estimating comparable work.

**Initiative summary for reference class use:**

| Field | Value |
|---|---|
| **Initiative type** | [e.g., New integration — third-party API / UI feature — new surface / Backend refactor / Compliance work] |
| **Team composition** | [e.g., 1 senior eng, 1 mid eng, 0.5 PM, 0.25 designer] |
| **Total actual effort (hours)** | |
| **Total actual cost** | |
| **Calendar duration** | |
| **Estimate provenance used** | [Historical analogy / Structured decomposition / Expert judgment / Assumption] |
| **Estimate accuracy** | [e.g., Came in at 112% of weighted estimate — 12% over] |
| **Primary variance driver** | [One sentence — the most useful thing to know for a future similar estimate] |
| **Comparable to** | [Describe in plain language what future initiative would be similar enough to use this as a reference: e.g., Any initiative involving integration with a third-party API where the vendor's documentation cannot be validated before estimation] |

---

### 14.5 Retrospective Notes

> Anything worth preserving for the organization or for future teams working in this area. Feed significant learnings into Institutional-Knowledge.md.

**What worked well:**
- [e.g., Breaking the build into two phases with a checkpoint allowed us to course-correct after the legacy system discovery]
- [e.g., The three-point estimate surfaced the pessimistic case early — leadership was not surprised by the overrun]

**What didn't work:**
- [e.g., Open questions were not resolved before build began — two of them caused scope changes mid-build]
- [e.g., The execution log was not maintained in real time — reconstructed from memory, which reduced its accuracy]

**What to do differently next time:**
- [e.g., Require a technical discovery spike for any initiative touching systems with undocumented legacy behavior]
- [e.g., Assign explicit execution log ownership at kickoff — not a shared responsibility]

**Logged to Institutional-Knowledge.md:** [ ] Yes — [link or reference] [ ] Not yet

---

*Product Build Record — [Initiative Name] — Status: [Current Status]*
