# Institutional Knowledge
> Part of the Corporate Intelligence Framework — Institutional Knowledge
> A living repository of organizational learning. Fed from retros, reviews, post-mortems,
> architecture discussions, escalations, and any other source of accumulated insight.
>
> This is not a top-down document — it is a receiver. Anyone can contribute an entry.
> Entries are not required to fit a single category; most will span multiple aspects.
> The value of this artifact grows over time as entries accumulate and connect.
>
> **Audience**: New team members, AI agents, executive leadership, and any reader
> who needs context before making a decision or taking action.

---

## Document Control

| Field | Value |
|---|---|
| **Organization / Company** | |
| **Maintainer** | |
| **Status** | Active |
| **Last Updated** | YYYY-MM-DD |

> Note: Unlike other framework artifacts, this document has a **Maintainer** rather than an Author.
> It is collectively owned — the Maintainer ensures entries are captured consistently,
> not that they are solely responsible for the content.


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### Contributing an Entry
> Anyone can add an entry. Entries do not need to be polished — clarity matters more than prose.
> Use the entry template in Section 2. Fill in the fields that apply and leave the rest blank.
> Tag each entry with one or more aspects so it can be found in context.

### Aspect Tags
> Each entry is tagged with the aspects it touches. Tags are not mutually exclusive.

| Tag | What it captures |
|---|---|
| `#decision` | A significant choice that was made — what was decided, why, and what was ruled out |
| `#lesson` | Something that worked, didn't work, or would be done differently next time |
| `#constraint` | A technical, architectural, regulatory, or organizational boundary that shapes what is possible |
| `#process` | How something actually gets done — the real workflow, not the documented one |

### Reading an Entry
> Entries are written to be useful to any reader — a new hire, an AI agent parsing context,
> or an executive reviewing a decision made two years ago. When reading:
> - Trust the entry as a point-in-time record — check the date before applying it
> - If something has changed, add a follow-up entry rather than editing the original
> - Use the Initiative tag to filter entries relevant to a specific project

---

## 2. Entry Template

> Copy this block for each new entry. Delete fields that don't apply.
> Entries should be added in reverse chronological order — most recent first.

---

**Entry ID**: IK-[sequential number, e.g., IK-001]
**Date**: YYYY-MM-DD
**Contributor**: [Name / Role]
**Source**: [e.g., Sprint retro, Architecture review, Customer escalation, Leadership offsite, Post-mortem]
**Initiative**: [Related project or initiative, or "General" if not initiative-specific]
**Aspect Tags**: `#decision` `#lesson` `#constraint` `#process` ← delete tags that don't apply

#### Summary
[One sentence. What does someone need to know from this entry?]

#### Detail
[The full context. What happened, what was learned, what was decided, or what constraint was identified.
Write as if the reader has no prior context. Be specific — vague entries lose value quickly.]

#### Why This Decision Was Made
[Optional. The real reasoning behind the decision — not just the stated rationale.
Include organizational context, timing pressures, constraints that shaped the choice,
alternatives that were considered and ruled out, and any factors that were weighted
but not formally documented. Future readers need to understand not just what was
decided but why — especially if the decision looks questionable in hindsight.]

#### Implications
[Optional. What does this mean for future work, decisions, or team members who encounter this situation?]

#### Follow-Up Entries
[Optional. List IDs of related entries that update, contradict, or expand on this one.]

---

## 3. Decision Log

> All entries tagged `#decision` are listed here for quick reference.
> Full entry detail lives in Section 4. This is an index, not a duplicate.

| Entry ID | Date | Initiative | Decision Summary | Contributor |
|---|---|---|---|---|
| IK-001 | YYYY-MM-DD | [Initiative] | [One sentence] | [Name] |

---

## 4. Knowledge Entries

> All entries in reverse chronological order. Most recent first.
> Use Ctrl+F / Cmd+F to search by tag, initiative, or keyword.

---

**Entry ID**: IK-001
**Date**: YYYY-MM-DD
**Contributor**: [Name / Role]
**Source**: [e.g., Architecture review]
**Initiative**: [e.g., Third-party data platform integration]
**Aspect Tags**: `#decision` `#constraint`

#### Summary
[e.g., Decided to integrate via existing processor API rather than direct network connection due to certification timeline.]

#### Detail
[e.g., Direct integration with the vendor's core platform would require 6–9 months of certification and dedicated engineering. Their published API provides equivalent access in weeks with minimal overhead. Performance difference is negligible at current data volumes.]

#### Why This Decision Was Made
[e.g., Direct integration with the vendor's core platform would require 6–9 months of certification and dedicated engineering. Their published API provides equivalent access in weeks with minimal overhead. Performance difference is negligible at current data volumes. Timeline pressure from a committed customer delivery date was the deciding factor.]

#### Implications
[e.g., Future RTP features are dependent on processor API roadmap. Negotiate API access terms carefully at next contract renewal.]

#### Follow-Up Entries
—

---

> Add new entries above this line, in reverse chronological order.

---

## 5. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | | | | |
