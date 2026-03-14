# Strategy and Intent
> Part of the Corporate Intelligence Framework — Organizational Intelligence
> A living document that captures organizational goals, the reasoning and assumptions
> behind them, and how they connect to the initiatives, teams, and artifacts that
> execute against them.
>
> This artifact is framework-agnostic — it can express goals as OKRs, strategic pillars,
> themed initiatives, or simple goal statements. Use whatever structure reflects how
> your organization actually thinks and communicates strategy.
>
> **This document is always live.** It does not reset at the end of a cycle.
> Goals are added, updated, and retired as strategy evolves — not replaced wholesale.
> Historical goals are retained for institutional continuity.

---

## Document Control

| Field | Value |
|---|---|
| **Organization / Company** | |
| **Maintainer** | |
| **Status** | Active |
| **Last Updated** | YYYY-MM-DD |

> Like Institutional Knowledge, this document has a **Maintainer** rather than an Author.
> Strategy is collectively owned. The Maintainer ensures goals are captured consistently
> and that the document reflects current organizational direction.

> **Connected artifacts:**
> - **Metrics-Framework** — Key Results in goal entries reference metric IDs from that document; targets are defined here and measures are defined there; when a goal uses a metric as a success indicator, the metric record there carries a one-way pointer back to this goal
> - **Business-Case** — initiatives funded by a Business Case should reference the goal they serve here
> - **Product-Build-Record** — build efforts reference the linked strategy goal in Document Control
> - **Organizational-Risk-and-Compliance** — strategic risks here are distinct from operational risks there; both should be reviewed together when strategy shifts
> - **Funding-and-Business-Model** — organizational drivers and horizon there should be consistent with long-term goals here
> - **People-and-Talent-Strategy** — capability needs there should be traceable to goals here


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

> Strategic Context is the northstar artifact in the Corporate Intelligence Framework.
> Every other artifact should be readable in light of what is here.

| Audience | Primary Use |
|---|---|
| **Executive Leadership** | Communicate and align organizational direction |
| **Product / Engineering** | Connect initiative and Product Build Record work to company goals |
| **Sales / Marketing** | Frame go-to-market efforts against strategic priorities |
| **Finance** | Evaluate investment and budget decisions against stated goals |
| **New Team Members** | Understand where the organization is going and why |
| **AI Agents** | Orient execution against organizational intent before acting |

---

## 2. Organizational Mission & Vision

> The foundational context that all goals serve.
> These should change rarely — if ever. If they change, capture why in Institutional Knowledge.

**Mission**: [What does this organization exist to do? One or two sentences.]

**Vision**: [What does success look like at scale? Where is the organization going?]

**Core Values**: [The principles that govern how the organization operates and makes decisions.]
- [Value 1]
- [Value 2]
- [Value 3]

---

## 3. Strategic Goals

> Goals are organized by time horizon — Long-Term, Near-Term, and Current.
> Each goal includes the reasoning behind it, not just the goal itself.
> Connect goals to initiatives and artifacts where they exist.
>
> **On metrics and targets:** Key Results that reference a formal metric should use the metric ID from Metrics-Framework (e.g., MET-F003 — NRR). This creates a clean connection between the target set here and the measure defined there — without duplicating the definition in both places.
>
> When setting a metric as a target, consider whether optimizing that metric could produce behavior that serves the number but not the underlying goal. The most useful check is to ask: what would a team do to hit this number without actually achieving what we want? If the answer is obvious, pair the target metric with a counterbalancing measure. Targets that are easy to game without detection tend to get gamed.

---

### 3.1 Long-Term Goals
> 3–5 year horizon. These are directional — they shape decisions today even if outcomes are years away.

---

**Goal ID**: SG-001
**Goal**: [e.g., Become the category leader in our primary market segment]
**Owner**: [Name / Role]
**Last Updated**: YYYY-MM-DD

**Why This Goal**:
[The real reasoning. What market opportunity, organizational capability, or strategic insight
makes this the right direction? Include what was considered and not chosen.]

**Key Results / Success Indicators**:
- [e.g., X% market share in our primary segment by YYYY]
- [e.g., Net revenue retention above X% — MET-F003]
- [e.g., Recognized in [industry analyst report] as a leading solution in our category]

> Where a Key Result references a formal metric, include the metric ID from Metrics-Framework. The measure's definition lives there — only the target value lives here.

**Connected Initiatives**:
- [Initiative name — link to Product-Build-Record or Business-Case]

**Notes**:
[Anything that shapes how this goal should be interpreted or pursued.]

---

> Add long-term goals following the pattern above.

---

### 3.2 Near-Term Goals
> 6–18 month horizon. More specific than long-term goals — these should be measurable.

---

**Goal ID**: SG-010
**Goal**: [e.g., Launch next-generation capability for existing enterprise customers]
**Owner**: [Name / Role]
**Last Updated**: YYYY-MM-DD

**Why This Goal**:
[Why now? What customer pressure, competitive signal, or internal capability makes
this the right priority at this moment?]

**Key Results / Success Indicators**:
- [e.g., X enterprise customers live on new capability by YYYY-MM-DD — MET-C001]
- [e.g., Customer satisfaction score above X — MET-C004]
- [e.g., Zero critical incidents in first 90 days post-launch — MET-O001]

> Where a Key Result references a formal metric, include the metric ID from Metrics-Framework. The measure's definition lives there — only the target value lives here.

**Connected Initiatives**:
- [Initiative name — link to Product-Build-Record or Business-Case]

**Notes**:

---

> Add near-term goals following the pattern above.

---

### 3.3 Current Focus
> 30–90 day horizon. Specific, time-boxed, and directly actionable.
> These are the goals the organization is executing against right now.

---

**Goal ID**: SG-020
**Goal**: [e.g., Complete RTP certification with [processor] and begin beta with two pilot customers]
**Owner**: [Name / Role]
**Due**: YYYY-MM-DD
**Last Updated**: YYYY-MM-DD

**Why This Goal**:
[What unblocks, what it proves, or what commitment it fulfills.]

**Success Conditions**:
- [e.g., Certification completed and documented]
- [e.g., Two pilot customers onboarded and transacting — MET-C001]
- [e.g., Post-pilot review scheduled]

> Where a success condition references a formal metric, include the metric ID from Metrics-Framework.

**Connected Initiatives**:
- [Initiative name — link to Product-Build-Record or Business-Case]

**Notes**:

---

> Add current focus goals following the pattern above.

---

## 4. Strategic Assumptions and Risks
> Strategy is built on beliefs about the world — about the market, the customer,
> the competitive landscape, and the organization's own capabilities. Those beliefs
> are rarely written down, which means when they turn out to be wrong, nobody notices
> the connection between the failed assumption and the failing strategy.
>
> This section makes those beliefs explicit. Capturing assumptions doesn't mean
> they're correct — it means they're visible, which is the first step to testing
> and updating them.

### 4.1 Strategic Assumptions
> What does the organization believe to be true that underpins its current strategy?
> If any of these assumptions changed significantly, the strategy should be revisited.
> Add entries in order of strategic importance — most foundational first.

---

**Assumption ID**: SA-001
**Assumption**: [What the organization believes to be true.]
**Category**: Market / Customer / Competitive / Regulatory / Organizational
**Basis**: [Why we believe this — data, experience, expert input, or reasoned judgment.]
**Confidence**: High / Medium / Low
**How We'd Know If It's Wrong**: [What signal or evidence would indicate this assumption has changed or failed?]
**Last Reviewed**: YYYY-MM-DD

---

> Add assumption entries above this line, most foundational first.

### 4.2 Strategic Risks
> What could make the strategy wrong — not execution failures, but directional risks?
> These are distinct from operational risks (see Organizational-Risk-and-Compliance.md).
> Strategic risks are threats to the direction itself: a market shift, a competitive
> move, a regulatory change, or an assumption that proves false.

---

**Risk ID**: SR-001
**Risk**: [What could undermine the strategy.]
**Category**: Market / Competitive / Regulatory / Technological / Organizational
**Likelihood**: High / Medium / Low
**Impact if realized**: [What changes about the strategy or organization if this risk materializes.]
**Connected Assumption**: [SA-ID if this risk is tied to a specific assumption above.]
**Early Warning Signals**: [What would we see before this risk fully materializes?]
**Response**: [How would the organization respond if this risk materialized?]
**Last Reviewed**: YYYY-MM-DD

---

> Add risk entries above this line.

---

## 5. Goal History

> Goals that have been achieved, paused, or retired are recorded here.
> Retain for institutional continuity — understanding past goals provides context
> for current direction and prevents revisiting decisions already made.

| Goal ID | Goal | Outcome | Date Closed | Notes |
|---|---|---|---|---|
| [SG-00X] | [Goal statement] | [What was accomplished or why it was retired] | YYYY-MM-DD | |

---

## 6. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | | | | |
