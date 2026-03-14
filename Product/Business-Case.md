# Business Case: [Initiative Name]
> Part of the Corporate Intelligence Framework — Product
>
> The Business Case answers one question: *Should we pursue this?*
> It is the argument for committing organizational resources — time, money, and attention —
> to a specific initiative. It is written before a Product Build Record and informs whether one
> should exist at all.
>
> **A Business Case is recommended but not required.** Not every initiative needs a
> formal Business Case — a small maintenance update or a quick fix may need nothing
> more than a Product Build Record. But most decisions that consume meaningful organizational resources
> benefit from at least a brief, honest answer to: what are we doing, why does it matter,
> and is it worth it? Even a few paragraphs of clear reasoning is a Business Case in spirit.
> This template scales from that brief rationale to a formal executive or investor document.
>
> **A Business Case is not a Product Build Record.** It does not define requirements or solutions in detail.
> It defines the problem, the opportunity, and the argument for acting — or not acting.
> A Product Build Record follows if the Business Case is approved.
>
> **Rejected Business Cases have value.** A "no" decision recorded here becomes
> institutional memory. It prevents the same initiative from being relitigated without
> the context of why it was previously declined. File rejected cases in
> Institutional-Knowledge.md with a summary and link.

---

## Document Control

| Field | Value |
|---|---|
| **Initiative Name** | |
| **Author** | |
| **Sponsor** | |
| **Date** | YYYY-MM-DD |
| **Status** | Draft / Under Review / Approved / Rejected / On Hold |
| **Decision Needed By** | YYYY-MM-DD |
| **Related Build Record(s)** | [Link to Product-Build-Record(s) if they exist — a build record may precede or follow this document] |


> **Significant Change Log**
> A record of meaningful changes to this document after initial creation — entries made when the scope, intent, assumptions, or decisions captured here shift in a way that would affect how a reader interprets this effort. Routine progress updates, status changes, and date confirmations do not require a log entry. A log entry is warranted when: the scope or success criteria change materially, a key assumption underlying this effort is revised, a decision is reversed or significantly modified, or new information emerges mid-effort that would have changed the original document if known at the start.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context for anyone reviewing this record after the fact.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The event, decision, or discovery that prompted it — e.g., Board review raised new constraint / Mid-pilot finding invalidated original hypothesis / Scope reduced due to resource reallocation] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. The One-Paragraph Summary
> Write this last. It should stand alone — a reader who only reads this section
> should understand what is being proposed, why it matters, and what it will take.
> If you can't summarize it clearly in one paragraph, the case isn't fully formed yet.

[What is being proposed, what problem it solves or opportunity it captures,
what it will cost in rough terms, and what the expected return or outcome is.]

---

## 2. Problem or Opportunity
> What is the situation that makes this initiative worth considering?
> Be specific. Vague problems produce vague solutions.
> Ground this in customer evidence, market data, or organizational reality where possible.

### 2.1 The Situation
[What is happening — in the market, with customers, or inside the organization —
that creates the need or opportunity this initiative addresses?]

### 2.2 Who Is Affected and How
[Which customers, segments, or internal teams are affected?
What is the cost of the current situation to them — in time, money, friction, or
missed opportunity? Reference Customer Personas or Reference Customers and Champions
where relevant.]

### 2.3 Why Now
[Why does this need to be addressed now rather than later?
What changes if we wait — competitive window, customer commitment, regulatory deadline,
internal capacity, market timing? If there is no urgency, say so honestly —
it may affect prioritization.]

---

## 3. Proposed Initiative
> A clear description of what is being proposed — not a requirements document.
> The goal is to communicate the shape and scope of the solution clearly enough
> to evaluate it. Save the details for the Product Build Record.

### 3.1 What We Are Proposing
[What is the initiative? Describe it in plain language — what it does, who it serves,
and what it changes about the current state.]

### 3.2 What This Is Not
[Explicitly scope out what this initiative does not include.
This is not the same as the Product Build Record's scope — it's a higher-level boundary that prevents
misaligned expectations before work begins.]

### 3.3 Strategic Alignment
[How does this initiative connect to organizational strategy?
Reference Strategic-Context.md goals directly where applicable.
If this initiative does not connect to a stated strategic goal, explain why it
should be pursued anyway — or reconsider whether it should be.]

---

## 4. Alternatives Considered
> A Business Case that only presents one option hasn't been fully stress-tested.
> Always include "do nothing" as an explicit alternative — it forces honest evaluation
> of the cost of inaction and grounds the recommendation in a real comparison.
>
> Note: "We are not building X" is a scoping decision that belongs in the Product Build Record,
> not here. This section evaluates whether to pursue the initiative at all,
> and through what approach.

| Alternative | Description | Why Not Recommended |
|---|---|---|
| Do nothing | Maintain current state | [What happens if we don't act — cost of inaction, competitive risk, customer impact, or why this is actually acceptable] |
| [Alternative A] | [Brief description of a different approach] | [Why considered and set aside] |
| [Alternative B] | [Brief description of a different approach] | [Why considered and set aside] |

---

## 5. Expected Benefits
> What does success look like — and how will we know we've achieved it?
> Benefits should be as specific as possible. Vague benefits ("improved customer experience")
> are hard to approve and impossible to measure.
> Reference Cost-and-Benefit-Framework.md for estimation methodology.
>
> Distinguish between quantifiable and strategic benefits — both are legitimate,
> but conflating them obscures the actual return.

### 5.1 Quantifiable Benefits
| Benefit | Estimate | Basis for Estimate | Timeframe |
|---|---|---|---|
| [e.g., Reduced support volume] | [e.g., ~30% reduction] | [e.g., Based on similar feature rollout] | [e.g., Within 6 months of launch] |
| [e.g., New revenue from segment X] | [e.g., $X–$Y ARR] | [e.g., X prospects in pipeline blocked by this gap] | [e.g., Within 12 months] |

### 5.2 Strategic and Qualitative Benefits
- [e.g., Closes a known competitive gap]
- [e.g., Strengthens relationship with a key Reference Customer who has requested this]
- [e.g., Positions the product for expansion into a new segment]
- [e.g., Reduces organizational dependency on a manual workaround]

---

## 6. Estimated Cost and Effort
> What will this initiative require — in time, money, and organizational attention?
> Estimates do not need to be precise to be useful. A rough, honestly characterized
> estimate is more valuable than false precision.
> Reference Cost-and-Benefit-Framework.md for estimation methodology.
> Flag assumptions clearly — the estimate is only as good as what it's built on.

### 6.1 Resource Estimate
| Resource | Estimate | Assumptions |
|---|---|---|
| Engineering effort | [e.g., 6–8 weeks, 2 engineers] | [e.g., No major infrastructure changes required] |
| Product and design | [e.g., 2 weeks scoping, 1 week UX] | [e.g., Design system already established] |
| External costs | [e.g., $X in infrastructure or vendor fees] | [e.g., Based on current pricing tier] |
| Ongoing maintenance | [e.g., ~X hrs/month] | [e.g., Estimated from similar feature] |

### 6.2 Opportunity Cost
[What will the organization *not* be doing while pursuing this initiative?
What is being deprioritized to make room for this?
This is often the most honest measure of what something actually costs —
especially in organizations where capacity, not budget, is the primary constraint.]

---

## 7. Risks
> What could go wrong — and how would we respond?
> Reference Organizational-Risk-and-Compliance.md for known organizational risk context.
> A risk that isn't named can't be managed.

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| [e.g., Scope expands beyond estimate] | Medium | High | [e.g., Define explicit phase boundaries in Product Build Record] |
| [e.g., Customer adoption lower than projected] | Medium | Medium | [e.g., Pilot with Reference Customer before full rollout] |
| [e.g., Regulatory or compliance requirement missed] | Low | High | [e.g., Review against Organizational Risk and Compliance before build] |

---

## 8. Recommendation and Decision Request
> State the recommendation clearly. Don't bury it.
> This section tells the reader exactly what is being asked of them,
> what the next step is if approved, and what happens if the decision is delayed.
>
> If the recommendation is "do not pursue," document the reasoning here.
> This record belongs in Institutional-Knowledge.md so the decision and its
> rationale are preserved for the organization.

**Recommendation**: [Proceed / Proceed with conditions / Do not proceed / Defer to [date]]

**What approval authorizes**:
[What specifically is being approved — a full build, a discovery phase, a pilot,
a budget allocation? Be precise. Approval of a Business Case is not the same as
approval of full scope — the Product Build Record defines that.]

**Next step if approved**:
[e.g., Begin Product Build Record scoping — estimated completion YYYY-MM-DD]
[e.g., Allocate engineering resources in next sprint planning]
[e.g., Schedule discovery phase with Reference Customer X]

**Cost of delay**:
[What is lost or risked if this decision is postponed?
If delay has no meaningful cost, say so — it's honest and helps prioritization.]

---

## 9. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | | | | |
