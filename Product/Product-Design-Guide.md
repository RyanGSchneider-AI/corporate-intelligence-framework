# Product Design Guide: [Product Name]
> Part of the Corporate Intelligence Framework — Product
>
> The Product Design Guide is the governance layer for how this product looks,
> behaves, and feels. It defines the standard — aspirational and directional —
> that all product changes are held against.
>
> This is not a component library, a Figma file, or a technical specification.
> It references those artifacts where precision is needed, but its purpose is
> higher-level: to ensure that every team member, every Product Build Record author, and every
> AI agent working on this product understands the design intent before making
> changes.
>
> **Relationship to other artifacts:**
> - Informed by **Product-Chronicle.md** — design principles and customer lens
>   are the source of truth for *why* standards exist
> - Referenced by every **Product Build Record** that touches UI/UX — the record documents
>   what is being built; this guide governs how it should behave and feel
> - Links to external design assets (Figma, Storybook, component libraries)
>   for technical implementation detail
>
> **This guide is aspirational.** It documents the standard we are building
> toward. Where the current product diverges from this standard, that gap is
> a known design debt — not a reason to lower the standard.
>
> **One Guide per product.** For a product suite, maintain a shared guide
> for cross-product standards and a separate guide for product-specific patterns.

---

## Document Control

| Field | Value |
|---|---|
| **Product Name** | |
| **Product Owner** | |
| **Design Lead** | |
| **Maintainer** | |
| **Last Updated** | YYYY-MM-DD |
| **Design Assets** | [Link to Figma / Storybook / component library] |
| **Accessibility Standard** | [e.g., WCAG 2.1 AA] |


> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (correcting a date, adding a new entry to a register) do not require a log entry. A log entry is warranted when: the document's overall picture has changed, a core definition or principle has shifted, organizational context that drove earlier decisions has been replaced, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it — e.g., Board approved Series B / New CRO hired, replacing VP Sales / Product-Build-Record-XX retrospective revealed assumption was wrong] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. Design Intent
> The governing philosophy behind all design decisions for this product.
> This section is derived directly from the Product Chronicle's design principles
> and customer lens. If those change, this section should be revisited.
>
> A reader who understands this section should be able to make a reasonable
> design judgment on a new feature without consulting anyone — that's the test.

### 1.1 What This Product Feels Like
[Describe the intended experience in plain language. Not adjectives — outcomes.
What should a user feel after completing a task? What should they never feel?
Example: "A user should always know where they are, what just happened, and
what they can do next. They should never feel uncertain about whether an
action worked."]

### 1.2 Design Principles
> These are carried forward from the Product Chronicle and restated here
> in their UI/UX application. For the full rationale behind each principle,
> see Product-Chronicle.md Section 4.

- **[Principle]**: [How this principle applies specifically to UI/UX decisions.
  One or two sentences on what it means in practice for design.]

> Example:
> - **Clarity over cleverness**: Every interface element should communicate its
>   purpose without requiring explanation. If a label, icon, or interaction
>   needs a tooltip to be understood, reconsider the design before adding the tooltip.

### 1.3 Who We Are Designing For
[A brief restatement of the primary user — not a full persona, but enough
context to orient design decisions. Reference Customer-Personas.md for full detail.
Call out any meaningful differences between the buyer and the user where relevant —
these often create competing design pressures.]

---

## 2. Interaction Standards
> How the product behaves — the patterns users can rely on across all features.
> Consistency here is what makes a product feel coherent rather than assembled.
> Each standard below is the governing rule; link to design assets for
> implementation detail.

### 2.1 Core Interaction Principles
- **Predictability**: Similar actions should behave the same way everywhere.
  A user who learns how something works in one part of the product should
  not be surprised by how it works in another.
- **Reversibility**: Where possible, actions should be reversible. Destructive
  actions — delete, cancel, submit — require explicit confirmation.
- **Feedback**: Every user action should produce a visible response. The user
  should never wonder whether the system received their input.
- **Escape**: Users should always have a clear way to cancel, go back, or
  return to a known state without losing context unexpectedly.

### 2.2 Navigation
[How users move through the product. What is the primary navigation model?
What is persistent vs. contextual? How do users know where they are?
Reference design assets for implementation.]

### 2.3 Actions and Confirmations
[What requires confirmation before execution? What is reversible vs. permanent?
How are destructive actions treated differently from safe ones?
What is the standard pattern for multi-step actions?]

### 2.4 Loading and System States
[How does the product communicate that something is happening?
What is the standard for loading states, processing states, and long-running operations?
Users should never see a blank screen or frozen UI without explanation.]

### 2.5 Forms and Data Entry
[What are the standards for how users enter data?
Inline validation vs. on-submit? Required field treatment? Character limits?
How are complex forms broken into manageable steps?
Reference design assets for component-level detail.]

---

## 3. Feedback and Communication
> How the product talks to the user — in interface copy, system messages,
> and error states. Voice and tone are part of the experience, not an afterthought.

### 3.1 Voice and Tone
[How does this product communicate? What are the qualities of its voice?
Ground this in the customer — what tone does the user need in their context?
A financial product used by accountants during month-end close has different
tone requirements than a consumer app.

Define the voice in terms of what it IS and what it is NOT:
- IS: [e.g., Direct, confident, human]
- IS NOT: [e.g., Casual to the point of flippancy, technical without explanation,
  corporate to the point of distance]]

### 3.2 Error Messages
> Error messages are the moment the product is most likely to lose a user's trust.
> They should always tell the user what happened, why, and what to do next.
> "Something went wrong" is not an error message — it is an absence of one.

Standard error message structure:
- **What happened**: Plain language, no jargon, no blame
- **Why it happened** (when known and useful): Brief, honest
- **What to do next**: A specific, actionable path forward

[Add any product-specific error message standards or common error patterns here.]

### 3.3 Empty States
[What does the product show when there is no data to display?
Empty states are an opportunity — they can orient a new user, prompt an action,
or explain why something is empty. They should never just be blank.
What is the standard approach for first-use empty states vs. no-results states?]

### 3.4 Success and Confirmation Messages
[How does the product confirm that something worked?
What warrants a toast notification vs. an inline confirmation vs. a full confirmation screen?
Success messages should be specific — "Report generated" or "Changes saved" — not "Success."]

---

## 4. Visual Standards
> The governing principles for how the product looks.
> This section defines intent and standard — not hex codes and pixel values.
> For implementation detail, see design assets linked in Document Control.

### 4.1 Visual Hierarchy
[How does the product communicate what is most important on any given screen?
What are the principles for directing user attention?
How is the primary action distinguished from secondary and tertiary actions?]

### 4.2 Typography
[What are the governing principles for type use?
What makes something a heading vs. body vs. label vs. caption in this product?
Reference design assets for typeface, size scale, and weight specifications.]

### 4.3 Color
[What does color communicate in this product?
What is color used for — status, hierarchy, brand, data differentiation?
What is color never used as the sole means of communicating information?
Reference design assets for the full color system.]

### 4.4 Spacing and Density
[What is the governing philosophy on information density?
Does this product prioritize efficiency (more information visible) or
clarity (more whitespace, fewer elements)? How does that balance shift
across different contexts — dashboard vs. form vs. report?]

### 4.5 Iconography
[When are icons used vs. labels? When are both used together?
What is the standard for icon meaning — are icons product-specific or
drawn from a standard library? Reference design assets for the icon system.]

---

## 5. Accessibility
> Accessibility is not a feature — it is a standard that all design and
> development work is held against. This section defines the commitment
> and the minimum bar. Meeting this standard is not optional.

### 5.1 Governing Standard
[e.g., This product targets WCAG 2.1 Level AA compliance across all features.
New features should meet this standard at launch, not as a follow-up.
Reference Organizational-Risk-and-Compliance.md for any regulatory accessibility
obligations specific to this product's market.]

### 5.2 Core Commitments
- **Color contrast**: Text and interactive elements meet minimum contrast ratios.
  Color is never the sole means of conveying information or state.
- **Keyboard navigation**: All interactive elements are reachable and operable
  via keyboard. Focus states are always visible.
- **Screen reader support**: All meaningful content and interactions are
  accessible to assistive technology. Images have meaningful alt text.
  Form fields have labels.
- **Text scaling**: The interface remains usable at increased text sizes.
- **Motion**: Animations respect user preferences for reduced motion.

### 5.3 Known Gaps
[Honest accounting of where the current product falls short of the standard.
Each gap should have an owner and a remediation plan or timeline.
This section is not a place to normalize gaps — it is a place to track them
toward resolution.]

| Gap | Affected Area | Severity | Owner | Target Resolution |
|---|---|---|---|---|
| [e.g., Low contrast on secondary buttons] | [e.g., All forms] | Medium | | |

---

## 6. Motion and Animation
> Animation should serve the user — orienting them, confirming actions,
> and communicating system state. It should never be decorative at the
> expense of performance or clarity.

### 6.1 Governing Principles
- **Purposeful**: Every animation communicates something — state change,
  hierarchy, causality. If removing an animation would not confuse the user,
  reconsider whether it belongs.
- **Fast**: UI animations should feel immediate. Transitions should not make
  users wait. Loading animations should appear only when wait time is meaningful.
- **Respectful**: All motion respects `prefers-reduced-motion` settings.

### 6.2 Standard Patterns
[What are the standard animation patterns for this product?
What transitions are used for page/view changes, modal entry/exit,
expanding/collapsing content, and feedback states?
Reference design assets for timing and easing specifications.]

---

## 7. Platform and Context Considerations
> Design standards may need to adapt across platforms, screen sizes, or
> usage contexts without abandoning core principles.

### 7.1 Responsive Behavior
[What are the governing principles for how the product adapts across screen sizes?
What is the primary design target — desktop, mobile, or both equally?
What degrades gracefully vs. what requires a fundamentally different approach?]

### 7.2 Context-Specific Adaptations
[Are there usage contexts that require different design treatment?
e.g., A product used in a warehouse on a ruggedized tablet has different
interaction requirements than the same product used at a desk.
Document known contexts and the design adaptations they require.]

---

## 8. Design Debt Register
> Known divergences between this guide's standard and the current product.
> This register exists to make design debt visible and managed — not to
> normalize it. Every entry should have a path toward resolution.

| Area | Current State | Standard | Priority | Owner | Target Resolution |
|---|---|---|---|---|---|
| [e.g., Error messages] | [e.g., Generic system errors shown to user] | [e.g., Plain language errors with next steps] | High | | |

---

## 9. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | | | | |
