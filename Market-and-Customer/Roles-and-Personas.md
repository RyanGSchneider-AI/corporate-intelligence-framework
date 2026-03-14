# Roles and Personas

> Part of the Corporate Intelligence Framework — Market and Customer
>
> A research artifact describing the full range of people who influence whether a product gets built, bought, adopted, and sustained — not named individuals, but role archetypes grounded in real observation.
>
> Six role types are distinguished because each has a different relationship to the product and a different influence on decisions across product design, go-to-market, and delivery:
>
> - **User** — does the work with the product; drives UX and functional design
> - **Buyer** — controls the budget and makes the final purchase decision; drives Business Case framing and pricing
> - **Gatekeeper** — can block or accelerate a deal without being the economic decision maker; drives objection handling and compliance readiness
> - **Champion** — an internal advocate inside the customer organization who works to bring others along; drives sales cycle velocity
> - **Internal Affected Party** — an employee or team whose workflows change as a result of the product, even if they don't use it; drives change management and internal adoption
> - **External Affected Party** — a person outside the organization impacted by the product's existence or output without being a user or buyer; drives compliance, trust, and regulatory positioning
>
> Not every product or use case will have all six types. Capture the ones that are present and meaningful. Leave the rest out rather than forcing a persona where none exists.
>
> **Governance note:** Personas are governed by research and market understanding. Every attribute should be grounded in interviews, data, or direct observation — not assumption. For named individuals within specific accounts, see Reference-Customers-and-Champions (champions and buyers) and Internal-Stakeholders (internal affected parties).

---

## Document Control

| Field | Value |
|---|---|
| **Organization / Company** | |
| **Maintainer** | |
| **Status** | Active |
| **Last Updated** | YYYY-MM-DD |

> **Connected artifacts:**
> - **Reference-Customers-and-Champions** — named champions and buyers at specific accounts are tracked there; role archetypes are defined here
> - **Internal-Stakeholders** — named internal affected parties and their concerns are tracked there; the internal affected party role type is defined here
> - **Product-Build-Record** — Section 3 (Users and Personas) references the relevant user and affected party personas from this document
> - **Business-Case** — buyer and gatekeeper personas inform the organizational fit and risk sections
> - **Go-to-Market** — buyer triggers, gatekeeper concerns, and champion dynamics inform channel strategy and sales motion
> - **Sales-Playbook** — gatekeeper objections and buyer criteria here feed directly into discovery and objection handling there
> - **Competitive-Intelligence** — competitive positioning should be tested against how each role type evaluates alternatives

> **Significant Change Log**
> A record of meaningful changes to this document — entries made when the content shifts in a way that would affect how a reader interprets decisions made against it. Routine updates (adding a new persona, correcting a detail) do not require a log entry. A log entry is warranted when: a role type is added or retired, a core persona is significantly revised, the mix of role types changes in a way that reflects a market shift, or a reader a year from now would need to know that this document meant something different before this date.
>
> When writing an entry, capture not just what changed but what the document reflected *before* — so the log itself is recoverable context, not just a changelog.

| Date | What Changed | What It Was Before | Why It Changed | Connected Artifacts Affected |
|---|---|---|---|---|
| YYYY-MM-DD | [One sentence: the thing that is now different] | [One sentence: what this section or field reflected before this change] | [The organizational event, decision, or learning that prompted it] | [Artifact names if other documents should be read differently in light of this change] |

---

## 1. How to Use This Document

### 1.1 Role Types and Where They Show Up

Each role type has a different influence on the organization's work. Use this map to know where each persona is most relevant:

| Role Type | Product Design | Business Case | Go-to-Market | Sales Playbook | Change Management |
|---|---|---|---|---|---|
| **User** | Primary — functional requirements, UX, jobs to be done | Adoption and retention assumptions | Messaging and positioning | Discovery and demo | Internal rollout |
| **Buyer** | Pricing sensitivity, packaging | ROI framing, risk tolerance, approval process | Segment strategy, channel selection | Economic qualification, closing | Budget and sponsorship |
| **Gatekeeper** | Compliance, security, integration requirements | Risk section, implementation constraints | Proof points and certifications | Objection handling, procurement navigation | Policy and IT alignment |
| **Champion** | Feature advocacy, feedback quality | Internal sponsorship assumption | Reference activity, case studies | Deal velocity, multi-threading | Adoption sponsorship |
| **Internal Affected Party** | Downstream workflow effects, data handling | Change management cost, adoption risk | Not directly | Not directly | Primary — communication, training, process change |
| **External Affected Party** | Data handling, ethical design, accessibility | Regulatory risk, compliance cost | Trust and brand positioning | Not directly | Regulatory and community engagement |

### 1.2 How Personas Are Validated

A persona is only as good as the research behind it. Each persona includes a Last Validated date and a Research Basis field. When a persona has not been validated against real data within the past 12 months, treat its content as hypothesis rather than fact — and flag it for review.

Validation methods by role type:
- **User** — direct interviews, usability sessions, support ticket analysis, session recordings
- **Buyer** — win/loss interviews, sales call recordings, deal retrospectives
- **Gatekeeper** — procurement process reviews, implementation retrospectives, IT/Legal debrief interviews
- **Champion** — relationship conversations, reference customer interviews, CS check-ins
- **Internal Affected Party** — change management retrospectives, internal surveys, manager interviews post-implementation
- **External Affected Party** — regulatory guidance, community feedback, compliance reviews, third-party research

### 1.3 Persona Depth

Two template depths are available for each role type:

**Full persona** — for role types that are well-researched and directly influence product or GTM decisions. Use when the organization has direct evidence for each field.

**Lightweight persona** — for role types that are present but not yet fully researched, or secondary to the primary use case. Enough to inform a conversation or a decision, not enough to build a product strategy on.

---

## 2. User Personas

> The people who do the work with the product day to day. User personas drive functional requirements, UX decisions, jobs-to-be-done prioritization, and adoption assumptions.
>
> A single product may have multiple distinct user types — e.g., an administrator who configures the system and a front-line worker who operates it. Capture each as a separate persona.

---

### 2.1 Full User Persona Template

---

**Persona Name**: [A memorable label — e.g., "The Field Operations Supervisor"]
**Use Case**: [e.g., Logistics company managing last-mile delivery coordination across multiple depots]
**Role / Title Range**: [e.g., Operations Supervisor / Dispatch Manager / Fleet Coordinator]
**Organization Type**: [e.g., Regional logistics operator, 200–2,000 employees]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 12 user interviews, 3 usability sessions, support ticket analysis Q2 YYYY]

#### Who They Are
> 2–3 sentences. What they are responsible for, who they report to, and what a typical day looks like.

[e.g., A Field Operations Supervisor at a regional logistics company, responsible for coordinating driver assignments, managing delivery exceptions, and reporting daily on-time performance to the operations director. They spend most of their day in reactive mode — fielding calls from drivers, resolving exceptions, and updating status in multiple disconnected systems.]

#### Jobs to Be Done
> What outcomes are they trying to achieve? Frame as results, not features.

- [e.g., Know the real-time status of all active deliveries without calling drivers]
- [e.g., Reassign routes when exceptions occur without rebuilding the entire schedule]
- [e.g., Close out the day's delivery report without spending an hour pulling data from multiple systems]

#### Pain Points
> What frustrates, slows down, or blocks them today?

- [e.g., No single view of delivery status — they maintain a personal spreadsheet because the system doesn't show what they need]
- [e.g., Exception handling is entirely manual — a missed delivery requires phone calls, texts, and system updates across three tools]
- [e.g., End-of-day reporting takes 45–60 minutes because data lives in disconnected systems]

#### Buying Triggers
> What causes someone in this role to start evaluating a new solution?

- [e.g., A high-profile delivery failure that reached executive attention]
- [e.g., Volume growth that made manual coordination visibly unsustainable]
- [e.g., A peer recommendation from someone who solved the same problem]

#### Adoption Drivers
> What makes this persona embrace a new product once it's in place?

- [e.g., Immediate time savings on tasks they do every day]
- [e.g., Feeling less reactive — the system surfaces problems before they escalate]
- [e.g., Peer adoption — they follow early adopters on the team]

#### Adoption Risks
> What causes this persona to resist, abandon, or work around a new product?

- [e.g., Any increase in the number of steps to complete a task they do frequently]
- [e.g., Training requirements that take them away from their primary job]
- [e.g., System unreliability — one bad day of downtime creates lasting distrust]

#### Success Looks Like
> How does this persona define a win?

[e.g., They stop maintaining their personal spreadsheet because the system shows everything they need. Exceptions surface automatically. End-of-day reporting takes 5 minutes.]

#### Notes
[Industry variation, org size sensitivity, regional considerations, anything that affects how this persona manifests differently across segments.]

---

### 2.2 Lightweight User Persona Template

---

**Persona Name**: [e.g., "The Clinical Care Coordinator"]
**Use Case**: [e.g., Healthcare network managing patient scheduling and care team communication]
**Role / Title Range**: [e.g., Care Coordinator / Patient Navigator / Scheduling Specialist]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 4 interviews, 1 job shadow]

**Who They Are**: [e.g., A care coordinator at a regional hospital network, responsible for scheduling patient appointments, coordinating between care teams, and ensuring follow-up tasks don't fall through the cracks.]

**Jobs to Be Done**:
- [e.g., Keep all open patient care tasks visible without maintaining a personal tracking system]
- [e.g., Communicate status changes to care team members without phone tag]

**Pain Points**:
- [e.g., Tasks assigned in one system don't appear in the system the care team actually uses]
- [e.g., No visibility into whether follow-up tasks were completed until something is missed]

**Adoption Risks**:
- [e.g., Any tool that requires manual data entry on top of existing documentation requirements will be abandoned]

**Notes**: [e.g., HIPAA compliance requirements affect what data can be surfaced in which contexts — product design must account for this at the data layer, not just the UI layer.]

---

> Add user personas by copying the full or lightweight template above.
> Label each as ### 2.X [Persona Name] — [Use Case].

---

## 3. Buyer Personas

> The people who control the budget and make the final purchase decision. Buyers may never touch the product — their relationship to it is through outcomes, risk, and organizational fit.
>
> Buyer personas drive Business Case framing, pricing and packaging decisions, channel strategy, and economic qualification in sales.

---

### 3.1 Full Buyer Persona Template

---

**Persona Name**: [e.g., "The VP of Operations"]
**Use Case**: [e.g., Mid-market manufacturer evaluating operational visibility solutions]
**Role / Title Range**: [e.g., VP Operations / COO / Director of Operations]
**Organization Type**: [e.g., Mid-market manufacturer, $50M–$500M revenue]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 8 win/loss interviews, 5 sales call recordings, 3 deal retrospectives]

#### Who They Are
> 2–3 sentences. What they are accountable for, what success looks like in their role, and how they are evaluated.

[e.g., A VP of Operations at a mid-market manufacturer, accountable for production efficiency, cost per unit, and on-time delivery performance. Their bonus is tied to margin improvement and operational uptime. They own the budget for operational technology and report to the COO or CEO.]

#### What They Are Buying
> What does this buyer think they are purchasing? Frame in their language, not product language.

- [e.g., Reduced operational risk — fewer surprises that reach the executive layer]
- [e.g., A defensible ROI they can present to the CFO]
- [e.g., Proof that their team can operate more efficiently without headcount additions]

#### Evaluation Criteria
> How does this buyer evaluate options? What makes them choose or not choose?

- [e.g., Total cost of ownership over 3 years — they will build a spreadsheet]
- [e.g., Reference customers in their industry at similar scale — they will call them]
- [e.g., Implementation risk — they have been burned before and will ask detailed questions about rollout]
- [e.g., Vendor stability — they will not buy from a company they think might not exist in 2 years]

#### Approval Process
> How does the purchase actually get made? Who else is involved?

[e.g., Decisions above $50K require CFO sign-off and a formal vendor security review from IT. Contracts above $100K require board notification. Typical cycle from evaluation to signed contract is 90–120 days at this org size.]

#### Risk Tolerance
> What risks are acceptable, and what risks will kill the deal?

- **Acceptable**: Implementation timeline slipping slightly if vendor communicates proactively
- **Acceptable**: Starting with a pilot before full rollout
- **Deal-killer**: Any data security concern raised by IT that the vendor cannot resolve
- **Deal-killer**: Reference customers who report poor implementation support

#### Objections
> What will this buyer push back on?

- [e.g., "Your implementation timeline is longer than we planned for — we have a board review in Q3"]
- [e.g., "We already have a system for this — why is yours better than what we have?"]
- [e.g., "My CFO is going to ask what the payback period is — can you give me numbers I can defend?"]

#### Buying Triggers
> What causes someone in this role to enter an active evaluation?

- [e.g., A production failure or missed delivery commitment with executive visibility]
- [e.g., A strategic initiative (expansion, acquisition) that exposes the limits of current systems]
- [e.g., A peer recommendation from a VP at a comparable company]

#### Notes
[Segment variation, industry-specific considerations, anything that changes how this buyer type behaves in different contexts.]

---

### 3.2 Lightweight Buyer Persona Template

---

**Persona Name**: [e.g., "The Practice Administrator"]
**Use Case**: [e.g., Multi-location healthcare practice evaluating patient communication tools]
**Role / Title Range**: [e.g., Practice Administrator / Operations Director / Office Manager]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 4 win/loss interviews]

**Who They Are**: [e.g., A Practice Administrator responsible for day-to-day operations across multiple clinic locations, including staff scheduling, vendor management, and technology decisions up to a defined budget threshold.]

**What They Are Buying**: [e.g., A solution that reduces front-desk call volume and no-show rates without requiring significant staff training or IT involvement.]

**Evaluation Criteria**:
- [e.g., Ease of implementation — they do not have IT support on staff]
- [e.g., Monthly cost relative to the staff hours they expect to save]

**Approval Process**: [e.g., Decisions under $1,000/month are within their authority. Above that, they need physician partner sign-off — which typically adds 4–6 weeks.]

**Objections**:
- [e.g., "We tried something like this before and the patients didn't use it"]
- [e.g., "Our EMR vendor says they're building this — should we just wait?"]

**Notes**: [e.g., Extremely risk-averse due to past implementation failures. References from comparable practice sizes are the most effective credibility tool.]

---

> Add buyer personas by copying the full or lightweight template above.
> Label each as ### 3.X [Persona Name] — [Use Case].

---

## 4. Gatekeeper Personas

> People who can block or significantly slow a purchase or implementation without being the economic decision maker. Gatekeepers evaluate through the lens of their specific function — risk, compliance, legal, technical fit — and their concerns must be addressed on their terms, not the buyer's.
>
> Common gatekeeper roles: IT / Security, Legal / Procurement, Finance / CFO office, Compliance / Risk, Clinical or Regulatory Affairs.
>
> Gatekeeper personas feed directly into the Sales Playbook objection handling section and the risk and constraints sections of the Business Case.

---

### 4.1 Full Gatekeeper Persona Template

---

**Persona Name**: [e.g., "The IT Security Reviewer"]
**Function**: [e.g., IT / Information Security]
**Use Case**: [e.g., Enterprise technology procurement review]
**Role / Title Range**: [e.g., IT Manager / CISO / Security Architect / VP of IT]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 6 implementation retrospectives, 3 procurement process interviews]

#### Who They Are and What They Own
> What is this gatekeeper responsible for, and what is the risk they are protecting against?

[e.g., The IT Security Reviewer is responsible for ensuring that any new vendor or system that touches company data meets the organization's security standards. They are protecting the organization from data breach, compliance violation, and the reputational and financial consequences that follow. A failed security review is a career event for them — their default posture is skeptical.]

#### Their Specific Concerns
> What does this gatekeeper evaluate? What questions do they always ask?

- [e.g., Where is data stored, and in which geographic regions?]
- [e.g., What certifications does the vendor hold — SOC 2 Type II, ISO 27001, HIPAA BAA?]
- [e.g., What is the vendor's penetration testing cadence and when was the last test?]
- [e.g., How is access provisioned and deprovisioned — and does it integrate with our SSO?]
- [e.g., What happens to our data if we terminate the contract?]

#### What Resolves Their Concern
> What evidence, documentation, or process satisfies this gatekeeper?

- [e.g., A current SOC 2 Type II report shared under NDA]
- [e.g., A completed vendor security questionnaire — they will send their own]
- [e.g., A signed Data Processing Agreement before the contract is executed]
- [e.g., A reference call with a peer IT leader at a comparable organization]

#### Blocking Behaviors
> What causes this gatekeeper to block or indefinitely delay a purchase?

- [e.g., Any unresolved finding in the security questionnaire — they will not approve until every item is addressed]
- [e.g., Vendor unwillingness to provide documentation — opacity is treated as a red flag]
- [e.g., A data residency requirement the vendor cannot meet]

#### How to Engage Them
> When and how should this gatekeeper be brought into the sales process?

[e.g., Engage IT Security as early as the technical evaluation stage — waiting until legal review adds 30–60 days to the cycle. Provide the security overview and certifications proactively before they ask. Assign a technical resource on the vendor side as their counterpart — they do not want to talk to Sales.]

#### Notes
[Variation by org size, industry-specific compliance requirements, anything that changes how this gatekeeper behaves in different contexts.]

---

### 4.2 Lightweight Gatekeeper Persona Template

---

**Persona Name**: [e.g., "The Procurement Officer"]
**Function**: [e.g., Finance / Procurement]
**Use Case**: [e.g., Enterprise contract review and vendor approval]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 4 deal retrospectives]

**Who They Are**: [e.g., A Procurement Officer responsible for vendor evaluation, contract negotiation, and ensuring all purchases comply with the organization's vendor management policy. They are process-oriented and timeline-driven — their job is to protect the organization from unfavorable terms, not to evaluate the product itself.]

**Their Specific Concerns**:
- [e.g., Payment terms — they default to Net 60 and will push back on anything shorter]
- [e.g., Liability and indemnification clauses — Legal must approve before they sign]
- [e.g., Auto-renewal provisions — they flag any contract that auto-renews without notification]

**What Resolves Their Concern**: [e.g., A clean, standard MSA with minimal redlines. Vendors who respond quickly to redlines and don't escalate minor points move through procurement faster.]

**Blocking Behaviors**: [e.g., They will not move a contract forward if Legal has not signed off. Any unusual term — unlimited liability, IP ownership provisions, data retention disagreements — goes back to Legal and adds weeks.]

**Notes**: [e.g., Building a relationship with Procurement before the legal review stage dramatically reduces cycle time. They respond well to vendors who treat them as a professional counterpart rather than an obstacle.]

---

> Add gatekeeper personas by copying the full or lightweight template above.
> Label each as ### 4.X [Persona Name] — [Function / Use Case].

---

## 5. Champion Personas

> An internal advocate inside the customer organization who wants the product to succeed and actively works to bring others along. Champions are not always the user, not always the buyer — they are the person who has decided this matters and is willing to spend political capital to make it happen.
>
> Champion personas inform sales cycle strategy, reference customer development, and the conditions under which deals accelerate or stall. Named champions at specific accounts are tracked in Reference-Customers-and-Champions — this section defines what a champion looks like as a role archetype.

---

### 5.1 Full Champion Persona Template

---

**Persona Name**: [e.g., "The Internal Operator"]
**Use Case**: [e.g., Mid-market SaaS purchase driven by an operational leader who identified the problem independently]
**Role / Title Range**: [e.g., Director of Operations / Senior Manager / Team Lead — someone with credibility but not final budget authority]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 10 post-sale champion interviews, 5 win retrospectives]

#### Who They Are
> What is their role, and what makes them a champion rather than just a user or an interested party?

[e.g., The Internal Operator is a senior individual contributor or manager who has felt the pain of the problem directly, has the organizational credibility to be heard by leadership, and has enough initiative to drive an internal evaluation without being asked. They identified the problem, found potential solutions, and are now navigating internal approval. They are not the economic buyer — but without them, the deal likely doesn't happen.]

#### Why They Champion
> What motivates them to spend internal capital on this?

- [e.g., They are accountable for an outcome that the current state prevents them from achieving]
- [e.g., They have tried to solve this problem before and failed — this feels like the first real solution]
- [e.g., They see this as an opportunity to lead a visible organizational improvement]

#### How They Champion
> What do they actually do to move the purchase forward?

- [e.g., Schedules internal demos and brings the right stakeholders to each]
- [e.g., Builds the internal business case — often using materials and data the vendor provides]
- [e.g., Manages the gatekeeper review process from the inside]
- [e.g., Maintains momentum during long procurement cycles by keeping the vendor informed of internal dynamics]

#### What They Need from the Vendor
> What does the vendor need to provide to make this champion effective?

- [e.g., A clear, defensible ROI narrative they can present to their CFO — in the CFO's language, not product language]
- [e.g., Reference customers at comparable organizations who will take a call]
- [e.g., Prompt, substantive responses to every internal question — delays undermine their credibility]
- [e.g., A named point of contact they can reach directly, not a support queue]

#### Champion Risk Signals
> What indicates the champion is losing traction or commitment?

- [e.g., Response times slow significantly — they are deprioritizing the evaluation]
- [e.g., They stop attending meetings or send a delegate]
- [e.g., They ask for a pause "while we sort out some internal things"]
- [e.g., They stop sharing internal context they previously shared freely]

#### Notes
[What causes a champion to emerge vs. not emerge. Industry or org-size variation. How to identify a potential champion early in a sales cycle.]

---

### 5.2 Lightweight Champion Persona Template

---

**Persona Name**: [e.g., "The IT Modernizer"]
**Use Case**: [e.g., Enterprise IT transformation initiative driven by a senior IT leader]
**Role / Title Range**: [e.g., IT Director / VP of Technology / Enterprise Architect]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 5 post-sale interviews]

**Who They Are**: [e.g., A senior IT leader who has been tasked with reducing technical debt and consolidating the vendor landscape. They champion solutions that fit their modernization roadmap — and will actively block solutions that don't.]

**Why They Champion**: [e.g., This purchase is aligned with a strategic initiative they own. Success is visible. Failure is also visible.]

**What They Need from the Vendor**:
- [e.g., A credible technical architecture review — they will scrutinize integration approach and scalability]
- [e.g., A roadmap conversation — they want to know the vendor is building toward where they're going]

**Champion Risk Signals**: [e.g., Their modernization initiative loses executive sponsorship — at which point their internal influence drops and the deal stalls regardless of product quality.]

**Notes**: [e.g., This champion type can shift to a gatekeeper if the product doesn't fit their technical standards. Treat early technical conversations as a qualification exercise for both parties.]

---

> Add champion personas by copying the full or lightweight template above.
> Label each as ### 5.X [Persona Name] — [Use Case].

---

## 6. Internal Affected Party Personas

> Employees, teams, or functions whose workflows, data, responsibilities, or performance metrics are affected by the product — even if they don't use it directly and had no role in the purchase decision.
>
> Internal affected party personas are primarily relevant for product design (downstream workflow effects, data handling, system dependencies), change management (communication, training, process redesign), and implementation planning (who needs to be engaged, when, and how).
>
> Named internal affected parties and their specific concerns are tracked in Internal-Stakeholders. This section defines the role archetype — what it looks like when a function is affected by a product without being a user or buyer.

---

### 6.1 Full Internal Affected Party Template

---

**Persona Name**: [e.g., "The Finance Team Member"]
**Function**: [e.g., Finance / Accounting]
**Use Case**: [e.g., Operations platform that changes how cost and performance data flows into financial reporting]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 5 post-implementation interviews with Finance stakeholders across 3 customer organizations]

#### Who They Are and How They Are Affected
> What does this person do, and what changes for them when the product is in place?

[e.g., A Finance team member responsible for month-end close, cost reporting, and variance analysis. Before the product, they receive a manual export from Operations each month that they reformat and load into the financial system. After the product, data flows automatically — which eliminates their manual step but requires them to trust a new data source and update their reconciliation process. They were not involved in the purchase decision.]

#### Their Concerns
> What does this person worry about as a result of the change?

- [e.g., Data accuracy — if the new system calculates cost differently than their manual export, month-end numbers will not reconcile]
- [e.g., Audit trail — they need to be able to trace every number back to a source for audit purposes]
- [e.g., Timeline — if the new data feed is delayed, their close process is delayed]

#### What They Need
> What does this person need from the product and from the implementation team?

- [e.g., A period of parallel running — old process and new data source simultaneously — before they are willing to retire the manual step]
- [e.g., Documentation of how key calculations are performed — not UI documentation, calculation logic]
- [e.g., A named contact for reconciliation questions during the first close cycle]

#### Change Management Implications
> What does the organization need to do to bring this person along?

- [e.g., Involve Finance in acceptance testing — specifically the reconciliation of output data against existing reports]
- [e.g., Communicate the change and the rationale before go-live — surprises create resistance]
- [e.g., Plan for at least one full close cycle of parallel running before cutover]

#### Resistance Signals
> What indicates this person is not accepting the change?

- [e.g., They continue maintaining their manual process in parallel beyond the agreed transition period]
- [e.g., They escalate data discrepancies to their manager rather than the implementation team]
- [e.g., They raise concerns about data accuracy to the buyer after go-live]

#### Notes
[Function-specific variation, org size considerations, anything that affects how this affected party type manifests differently across implementations.]

---

### 6.2 Lightweight Internal Affected Party Template

---

**Persona Name**: [e.g., "The Customer Support Agent"]
**Function**: [e.g., Customer Support / Service Desk]
**Use Case**: [e.g., Product change that alters the customer-facing workflow Support is trained to explain]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., 3 post-launch interviews]

**Who They Are and How They Are Affected**: [e.g., A Customer Support Agent who handles inbound questions about the product. When a product change is released, their existing knowledge base is partially wrong — and they receive a spike in tickets before updated documentation and training reach them.]

**Their Concerns**:
- [e.g., Being caught off-guard by customer questions they cannot answer]
- [e.g., Being measured on resolution time during a period when they lack the information to resolve quickly]

**What They Need**:
- [e.g., Pre-release briefing and updated knowledge base articles before go-live, not after]
- [e.g., A clear escalation path for questions they cannot resolve during the transition period]

**Change Management Implications**: [e.g., Support must be included in launch communication plans — not as an afterthought but as a primary internal audience. Launch timing should account for Support readiness, not just product readiness.]

**Notes**: [e.g., Support resistance often surfaces publicly — in customer interactions and in ticket data. A Support team that is not prepared for a launch creates a visible customer experience problem within days of go-live.]

---

> Add internal affected party personas by copying the full or lightweight template above.
> Label each as ### 6.X [Persona Name] — [Function / Use Case].

---

## 7. External Affected Party Personas

> People outside the organization who are impacted by the product's existence or output without being users or buyers. External affected parties have no direct voice in the purchase or design process — which is exactly why they must be explicitly considered.
>
> Common examples: end consumers in a B2B2C model, individuals whose data is processed, community members affected by operational changes, downstream partners whose workflows change, regulated populations.
>
> External affected party personas are primarily relevant for compliance and regulatory positioning, ethical product design, trust and brand considerations, and go-to-market messaging in regulated or socially sensitive markets.

---

### 7.1 Full External Affected Party Template

---

**Persona Name**: [e.g., "The Patient"]
**Context**: [e.g., Healthcare platform where the buyer is a clinic and the patient is the person whose data is processed and whose care coordination is affected]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., Regulatory guidance review, 3 patient advocacy organization interviews, secondary research on patient experience in care coordination contexts]

#### Who They Are and How They Are Affected
> Who is this person, and what is the nature of their relationship to the product?

[e.g., A patient at a healthcare clinic that uses the platform to manage scheduling, care coordination, and follow-up communication. The patient did not choose this platform — it was chosen by their care provider. They interact with it through automated appointment reminders, care team messages, and follow-up surveys. Their health data is processed by the platform. Their experience of care is partly shaped by how well or poorly the platform supports their care team's coordination.]

#### Their Interests and Concerns
> What does this person care about, even if they have no direct voice in product decisions?

- [e.g., That their personal health information is handled securely and not used in ways they didn't consent to]
- [e.g., That automated communications are clear, timely, and not confusing or alarming]
- [e.g., That errors in the system — a missed follow-up, an incorrect appointment record — don't result in gaps in their care]

#### Regulatory and Compliance Implications
> What obligations does the organization have toward this affected party, and how do they affect product design?

- [e.g., HIPAA governs data handling — minimum necessary access, breach notification, patient rights to access and correct their records]
- [e.g., Communications sent on behalf of the clinic are subject to patient communication regulations — opt-out must be honored, certain content requires specific disclosures]
- [e.g., Accessibility requirements apply to any patient-facing interface — WCAG compliance at minimum]

#### Product Design Implications
> How should awareness of this affected party change how the product is designed?

- [e.g., Data minimization by design — collect and retain only what is necessary for the care coordination function]
- [e.g., Error handling must account for the downstream human consequence — a missed follow-up is not a UX failure, it is a care gap]
- [e.g., Patient-facing communications must be reviewable and correctable by the care team before sending]

#### Trust and Brand Implications
> How does the organization's treatment of this affected party affect brand and market position?

[e.g., In healthcare, patient trust is a buyer evaluation criterion — clinics are sensitive to solutions that could create a patient relations problem. A platform that generates patient complaints about data handling or communication quality creates churn risk at the buyer level, not just the affected party level. Positive patient experience, conversely, becomes a reference point in the sales cycle.]

#### Notes
[Regulatory variation by geography or context, anything that changes how this affected party's interests should be weighted in product decisions.]

---

### 7.2 Lightweight External Affected Party Template

---

**Persona Name**: [e.g., "The End Consumer"]
**Context**: [e.g., B2B2C retail platform where the buyer is a retailer and the consumer is the person whose purchase experience is affected]
**Last Validated**: YYYY-MM-DD
**Research Basis**: [e.g., Secondary research, retailer feedback on consumer response]

**Who They Are and How They Are Affected**: [e.g., A consumer who shops at a retailer using the platform for inventory management and fulfillment. The consumer never interacts with the platform directly — but they experience its effects through product availability accuracy, delivery timing, and order communication quality. If the platform performs poorly, the retailer's customer experience suffers.]

**Their Interests**:
- [e.g., Accurate product availability — they want to know if something is in stock before they drive to the store]
- [e.g., Reliable delivery estimates — a missed window erodes trust in the retailer, not the platform]

**Product Design Implications**:
- [e.g., Data accuracy at the consumer-facing layer is a downstream consequence of inventory data quality — product design must treat consumer-visible outputs as first-class quality requirements]

**Trust and Brand Implications**: [e.g., Retailer churn is often preceded by consumer complaints that reach the retailer's leadership. Poor platform performance that reaches the consumer layer creates reputational pressure on the buyer relationship.]

**Notes**: [e.g., Consumer-facing effects are often invisible to the buyer until they surface as customer complaints or churn. Proactively surfacing consumer experience data — delivery accuracy rates, availability accuracy — as a platform metric creates a differentiation opportunity.]

---

> Add external affected party personas by copying the full or lightweight template above.
> Label each as ### 7.X [Persona Name] — [Context].

---

## 8. Open Questions

| # | Question | Owner | Due Date | Resolution |
|---|---|---|---|---|
| 1 | [e.g., Are there role types present in our market that are not yet represented in this document?] | | | |
| 2 | [e.g., Which personas are overdue for validation — Last Validated date older than 12 months?] | | | |
| 3 | [e.g., Are the gatekeeper personas current relative to how procurement processes have changed in our primary segments?] | | | |
| 4 | [e.g., Do external affected party personas reflect current regulatory requirements in all markets we operate in?] | | | |
