# DM-OS — Step 1: Framework Research Reference

> **Purpose:** A research-grounded reference document covering the universal standards, professional expectations, common failure modes, and context adaptations for all 10 core DM functions. This is the input scaffold for Step 2 (Self-Assessment). Sources: PMI PMBOK 7th ed., PRINCE2, Agile Delivery frameworks (SAFe, Scrum), outsourcing industry practice, EPAM/Accenture/Capgemini DM job posting patterns.

---

## Function 1: Engagement Setup
*What to do in Week 1 of any new project or company*

**Why it matters:**
The first two weeks establish the operational baseline for everything that follows. DMs who skip structured engagement spend months in reactive fire-fighting. Poor engagement setup is the single most-cited cause of delivery failure in the first quarter of a project — not technical problems, not scope creep, but unestablished foundations.

**What professional standards require:**

- Map all stakeholders within 48h: who has authority, who has opinion, who has information
- Locate or create the core project artifacts: charter/scope doc, backlog, team roster, contract/SOW
- Run a listening session (not a meeting) with each key stakeholder — goal is information, not status
- Identify the biggest unspoken risk within the first week — the one everyone knows but hasn't named
- Establish communication channels and cadences *before* the first status update
- Define what "done" looks like for the first milestone — get explicit alignment, not assumed consensus
- Set recurring delivery cadence (stand-up, weekly sync, steering committee) within Week 1
- Understand the internal approval chain before making any commitments

**Common failure modes:**
- Jumping to execution before understanding the political landscape
- Inheriting someone else's structure without questioning if it works
- Not establishing your own communication rhythm — you end up fitting into others' chaos
- Treating "engagement setup" as a one-time checklist rather than an active listening phase
- Failing to name the elephant in the room early — it becomes harder to raise later

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| New company (not just new project) | Add: understand org chart, internal politics, who the real decision-makers are (vs. official ones) |
| Mid-flight inherited project | Add: pre-mortem — what's already broken that no one is saying out loud? |
| Outsourcing / client-facing | Add: timezone + async protocol established Day 1; clarify client's internal DM equivalent |
| Small team (≤5) | Lighter structure; direct relationships replace comms matrix |
| Fixed-price contract | Scope baseline must be locked and documented before any work begins |

---

## Function 2: Scope & Requirements Governance
*How to define, protect, and manage what is being built*

**Why it matters:**
Scope is the contract between delivery and expectation. Every unmanaged scope change either silently expands work (burning budget/time) or creates a gap between what's built and what was wanted. Scope governance is what separates DMs who deliver predictably from those who are perpetually surprised.

**What professional standards require:**

- Maintain a single, version-controlled source of truth for scope (requirements doc, backlog, SOW appendix)
- Ensure every requirement has: an owner, an acceptance criterion, and a priority
- Establish a formal (or at minimum explicit) process for *how* new requirements enter the backlog — not by informal conversation
- Conduct regular scope reviews with stakeholders to confirm alignment hasn't drifted
- Document what is explicitly *out of scope* — as important as what's in scope
- Ensure delivery team understands scope boundaries and knows to flag ambiguities before starting work
- Link requirements to business goals — "what problem does this solve?" prevents gold-plating

**Common failure modes:**
- Requirements defined only in verbal conversations — no written baseline to refer back to
- "Yes" given to new requests without impact assessment on timeline/budget
- Scope documents that exist but are never consulted after Week 1
- No distinction between must-have and nice-to-have — everything treated as equal priority
- Delivery team interpreting ambiguous requirements independently rather than raising to DM
- Acceptance criteria defined at delivery time, not at requirements time — leads to rework disputes

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Fixed-price outsourcing | Scope baseline is a legal document; changes must trigger formal change control |
| Agile / product | Backlog is the scope artifact; refinement sessions are the governance mechanism |
| US/EU client facing | Clients often have their own BA or PO — clarify who owns requirements authority |
| Legacy or evolving system | Add: assumption log for undocumented behaviors; scope must account for unknowns |
| Small team / startup context | Lighter process, but written user stories minimum — verbal only is a trap |

---

## Function 3: RAID Management
*Risks, Assumptions, Issues, Dependencies — proactive delivery control*

**Why it matters:**
RAID is the single most-cited differentiator between DMs who prevent crises and those who manage them after the fact. Explicitly required in PRINCE2, PMI PMBOK, and the majority of outsourcing DM job descriptions. Most often done superficially — a spreadsheet that no one updates after Week 2.

**What professional standards require:**

- Maintain a live RAID log reviewed every sprint or week — not a static document
- **Risk:** Probability × Impact → Priority → Owner → Mitigation action → Review date
- **Assumption:** Written explicitly, dated, assigned someone to validate by a specific date; revisited regularly
- **Issue:** Raised, assigned an owner, tracked to resolution — never "parked" indefinitely
- **Dependency:** Mapped directionally (what we need from others; what others need from us), with dates and owners
- Separate risk (potential future problem) from issue (problem that has already materialized)
- Escalate risks before they become issues — not after
- Communicate RAID status in stakeholder updates, not just in the log itself

**Common failure modes:**
- RAID log created at project start, never updated — becomes a historical artifact
- Issues logged but never escalated — DM absorbs problems instead of surfacing them
- Assumptions never re-validated — they quietly become invisible constraints
- Dependencies tracked but not actively chased — DM waits for other teams to self-report
- Risks rated at project start, never re-rated as context changes
- No clear owner per item — RAID becomes a shared responsibility and therefore no one's

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Fixed-price / outsourcing | Assumptions and dependencies are high-stakes — unvalidated = future scope disputes |
| Agile sprint-based | RAID review embedded into retrospective; issues surfaced in daily stand-up |
| Multi-team / program | Dependencies matrix becomes critical; need cross-team dependency owner |
| Solo DM without PMO | Simplify: 1-page log, owner + date + status, reviewed weekly |
| US/EU client | Risks must be communicated proactively in client reports, not just in internal log |

---

## Function 4: Stakeholder Communication
*Who gets what information, how often, and in what format*

**Why it matters:**
Delivery confidence is built or destroyed through communication, not just outcomes. Stakeholders who feel informed are forgiving of problems. Stakeholders who feel surprised become adversarial — even when results are good. Communication is not a soft skill; it is a delivery mechanism.

**What professional standards require:**

- Build a stakeholder map: identify each stakeholder's interest, influence, and preferred communication style
- Define a communication matrix: who gets what, how often, in what format (email, dashboard, meeting, Slack)
- Distinguish between *informing* and *decision-making* communications — mix them and both suffer
- Status reports must cover: accomplishments, upcoming work, risks/issues, decisions needed
- Cadence must be predictable — stakeholders should never need to chase for updates
- Tailor depth by audience: executives want headlines + red flags; team leads want detail + decisions
- Bad news must travel faster than good news — surface problems before stakeholders hear from other sources
- Written async updates reduce the meeting load and create a paper trail

**Common failure modes:**
- Over-communicating to everyone equally — executives get buried in detail, team gets ignored
- Communication only when things go wrong — no baseline rhythm, so silence = assumed success
- Status updates that report activity ("team worked on X") without progress or signal ("X is 80% done, on track")
- Verbal-only updates — no written record, alignment evaporates by next meeting
- Failing to identify the informal influencer who isn't on the org chart but shapes decisions
- Treating communication as a reporting task rather than a trust-building activity

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| US/EU client | Async-first (written updates); Loom or written summary before video calls |
| Executive steering committee | One-pager max; RAG status; decisions needed highlighted |
| Technical delivery team | Detail-oriented; blockers surfaced fast; daily stand-up is primary channel |
| Multiple stakeholder groups | Separate comms per group; never let one group's priorities contaminate another's update |
| Difficult / high-anxiety stakeholders | Over-communicate temporarily to rebuild trust; then normalize |

---

## Function 5: Team & Resource Management
*How to lead, unblock, and organize the delivery team*

**Why it matters:**
A DM who cannot manage the team is just a reporter. Delivery happens through people. Keeping the team unblocked, motivated, and correctly utilized is the most direct lever a DM has on output velocity and quality.

**What professional standards require:**

- Maintain clear role clarity — every team member knows what they own, who they depend on, and what "done" means for their work
- Identify and remove blockers actively — don't wait for stand-up to discover them
- Track utilization without micromanaging — know who is overloaded, who is underutilized
- Resolve team conflicts early — escalate interpersonal issues before they damage delivery
- Create conditions for psychological safety — team members must feel safe raising problems
- Know each team member's constraints (skills, availability, competing priorities)
- Distinguish between team problems the DM can solve vs. ones that need HR/leadership escalation
- Ensure onboarding of new team members is covered — uncovered onboarding = weeks of lost productivity

**Common failure modes:**
- Assuming role clarity exists when it hasn't been explicitly established
- Waiting for blockers to surface in stand-up rather than proactively asking in between
- Over-relying on top performers and leaving weak links unaddressed
- Treating remote team members as second-class participants in meetings and decisions
- Allowing conflict to fester — "they're adults, they'll figure it out" rarely ends well
- Not knowing team members' actual skills vs. their stated skills until a critical task reveals the gap

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Outsourced / vendor team | Relationship management = a delivery input; invest in rapport early |
| Cross-cultural team | Communication norms, directness, and hierarchy expectations differ; map them explicitly |
| Remote-first | Async check-ins; documented decisions; deliberate informal touchpoints |
| Mixed seniority | Junior members need closer oversight; seniors need autonomy + clear outcomes |
| Under-resourced team | Resource gap must be escalated early with impact analysis, not absorbed silently |

---

## Function 6: Financial & Commercial Awareness
*Budget, burn rate, contract basics, and knowing when numbers are off*

**Why it matters:**
DMs in outsourcing contexts are often the closest person to both the client relationship and the financials. Not understanding the commercial model means being blind to the biggest delivery risk — the one that triggers contract disputes, early terminations, and loss of client trust. Financial awareness is not optional for senior DMs.

**What professional standards require:**

- Understand the contract structure: fixed-price vs. T&M vs. retainer — each changes risk allocation entirely
- Track burn rate against budget regularly — know the financial health of the project, not just the delivery health
- Recognize early warning signs: budget overrun trajectory, scope expanding without budget adjustment, team billing that doesn't match deliverables
- Understand what triggers a change order — and know when to raise one vs. absorb the cost
- Be able to report on financial status in client conversations without depending entirely on a PM or Finance team
- Flag margin risks to leadership before they become P&L problems
- Know the commercial implications of timeline slippage: delay ≠ just schedule problem, it may = penalty clause

**Common failure modes:**
- Treating budget as Finance's problem — DM "doesn't do numbers"
- Discovering overrun only at end-of-month finance review rather than week-by-week tracking
- Not knowing the SOW/contract well enough to identify when a client request is out of scope
- Confusing "team is busy" with "budget is being used effectively"
- Absorbing out-of-scope work to avoid difficult client conversations

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Fixed-price contract | Budget management is the highest-stakes function; every untracked hour is margin erosion |
| T&M (time & materials) | Focus on billing accuracy and client transparency on hours consumed |
| Product company (internal) | Budget = headcount + vendor costs; focus on ROI framing rather than cost control |
| Startup / resource-scarce | Cost efficiency is a delivery constraint, not just a finance metric |
| US/EU enterprise client | Finance reporting may be a contractual requirement with a defined format |

---

## Function 7: Delivery Cadence & Tracking
*Sprint/milestone rhythm, progress measurement, and forecasting*

**Why it matters:**
Delivery without tracking is hope without evidence. Cadence creates predictability. Tracking creates visibility. Forecasting creates credibility. Together, they are what allows a DM to say "we will hit the date" with confidence — or to say "we won't" early enough to matter.

**What professional standards require:**

- Define the delivery rhythm at project start: sprint length, milestone dates, review cadence
- Track progress against plan weekly — not monthly, not in retrospect
- Use leading indicators (work started, blockers count, velocity trend) not just lagging indicators (tasks completed)
- Maintain a realistic forecast: if current velocity continues, when do we finish?
- Surface schedule risk as soon as trajectory diverges from plan — not when the date is missed
- Burn-down / burn-up charts, milestone trackers, or equivalent — visible to team and stakeholders
- Distinguish between output (features shipped) and outcome (value delivered) in tracking

**Common failure modes:**
- Tracking only what's done, not what's at risk
- Velocity measured but never used to forecast — data collected but not converted to signal
- Milestone dates treated as aspirational rather than managed
- "Green" status maintained past the point where it's honest — status inflation
- Progress reported by team self-assessment only — no independent DM view
- No mechanism to catch when small slippages are accumulating into a larger miss

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Agile sprint-based | Velocity, sprint goals, and burn-down are primary tracking tools |
| Waterfall / phase-gate | Milestone and deliverable completion is the tracking currency |
| Outsourcing / client-facing | Client-visible tracking artifact required (weekly report, dashboard, shared project tracker) |
| Multiple parallel streams | Program-level view needed; individual stream tracking rolls up |
| Research or ambiguous scope | Track learning milestones, not just feature completion |

---

## Function 8: Quality Assurance
*How to ensure what is delivered actually works and meets expectations*

**Why it matters:**
Quality failures are the most visible form of delivery failure — they reach clients, create rework cycles, erode trust rapidly, and (in outsourcing) can trigger SLA penalties or contract review. A DM who does not own QA outcomes is a DM who will be blindsided by them.

**What professional standards require:**

- Define quality standards and acceptance criteria *before* development begins — not at review time
- Ensure a testing strategy exists: who tests, what types (unit, integration, UAT, regression), when
- Track defect rate, severity, and resolution time as delivery health metrics
- Include QA effort in timeline estimates — QA is not "the time left after development"
- Facilitate UAT (User Acceptance Testing) with actual stakeholders — not just internal sign-off
- Ensure Definition of Done includes quality gates, not just feature completion
- Own the go/no-go decision for releases — DM asserts readiness, doesn't just defer to dev team

**Common failure modes:**
- QA treated as the final phase rather than integrated throughout
- Acceptance criteria defined vaguely — "it should work" — leading to subjective sign-off disputes
- Testing effort under-resourced because development ran long
- Bug backlog grows but severity isn't tracked — all bugs treated equally
- UAT conducted superficially (rubber-stamp review) rather than actual user testing
- DM not involved in quality decisions — "that's the tech team's domain"

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Outsourcing / client delivery | UAT and formal sign-off are contractual requirements; document everything |
| Agile sprint-based | QA is part of the sprint; no separate test phase; done = tested |
| Product with high user volume | Performance and load testing added; regression suite critical |
| Small team | DM may need to facilitate testing personally, not just oversee it |
| Regulated industry (finance, health) | Compliance requirements add formal test documentation and audit trails |

---

## Function 9: Change Control
*How to handle scope changes, timeline shifts, and surprises*

**Why it matters:**
Change is inevitable. Unmanaged change is how projects fail. Change control is not bureaucracy — it is the mechanism that converts surprises into decisions, and decisions into updated plans. DMs without a change control habit absorb changes silently until the project is unrecognizable from its original scope and timeline.

**What professional standards require:**

- Define the change control process at project start: how changes are submitted, evaluated, approved, and communicated
- Assess every change request for impact on: scope, timeline, budget, resource, risk
- No change proceeds without explicit approval from the appropriate authority (client, sponsor, steering committee)
- Document all approved changes and update the baseline plan accordingly
- Communicate the impact of changes to all affected parties — team and stakeholders
- Distinguish between a change request (new work) and a defect fix (work that should have been done correctly) — these have different approval paths
- Track the cumulative impact of changes — individual changes look small; combined, they can double the project

**Common failure modes:**
- Changes absorbed verbally without documentation or impact assessment
- "Sure, we can add that" said without checking against budget and timeline
- No formal approval from client — later disputed as "that wasn't agreed"
- Change log exists but is not maintained — changes fall through the cracks
- Team implements changes before approval — creates untracked scope and billing disputes
- DM not included in change conversations — client goes directly to tech lead

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| Fixed-price outsourcing | Change control is financial protection; every out-of-scope request = change order trigger |
| Agile / product | Changes enter backlog through refinement; prioritization is the governance mechanism |
| US/EU enterprise client | Formal change request form + paper trail often contractually required |
| Startup / early-stage | Lightweight process (Slack thread + written summary); adapt as project matures |
| High-frequency change environment | Batch changes into weekly review to avoid constant plan disruption |

---

## Function 10: Escalation & Crisis Management
*When and how to raise problems to leadership*

**Why it matters:**
Escalation is not failure — it is judgment. The DM who never escalates is absorbing problems that leadership needs to know about. The DM who escalates everything is abdicating decision-making. The skill is calibration: knowing what to resolve independently, what to escalate proactively, and how to do it in a way that generates solutions rather than blame.

**What professional standards require:**

- Define escalation thresholds at project start: what types of problems go to whom
- Escalate with: problem statement, impact, options considered, recommended action — not just "we have a problem"
- Escalate early enough that leadership has time to act — not as a post-mortem
- In a crisis: establish facts first, then communicate; don't speculate in stakeholder updates
- Crisis response sequence: Contain → Communicate → Investigate → Remediate → Prevent recurrence
- Protect the team during crisis — DM is the interface to leadership, not the conduit for blame
- Know the difference between a delivery problem (DM owns) vs. a strategic problem (leadership owns)
- After any major escalation: conduct a brief retrospective to improve the system, not find scapegoats

**Common failure modes:**
- Escalating too late — problem is already a crisis by the time leadership hears it
- Escalating without options — presenting the problem without any proposed path forward
- Not escalating at all — absorbing strategic-level problems at the DM level
- Panic communication during crisis — sending incomplete or inaccurate updates that create more confusion
- Framing escalations as personal failure rather than system signal
- Failing to follow up after escalation — problem raised, then dropped with no resolution tracking

**Adaptation by context:**

| Context | Adjustment |
|---|---|
| US/EU client-facing | Client must hear bad news from DM directly, before hearing from internal sources |
| Outsourcing firm (internal) | Both client-facing and internal escalation paths must be clearly defined |
| Small team / flat hierarchy | Escalation path is shorter; DM may escalate directly to CEO/CTO |
| High-stakes / regulated delivery | Crisis communication may have legal/contractual implications; involve legal if needed |
| Remote/async team | Crisis escalation cannot wait for a meeting; synchronous channel needed immediately |

---

## Step 1 Summary: Cross-Cutting Observations

These patterns appear across all 10 functions and represent the difference between a **system-based DM** and an **instinct-based DM**:

| Pattern | Instinct-Based (current risk) | System-Based (target state) |
|---|---|---|
| Documentation | Exists when convenient | Always exists; always current |
| Proactivity | Reacts when problems surface | Scans for problems before they surface |
| Communication | Informs when prompted | Communicates on a defined, predictable rhythm |
| Decision records | Verbal / implicit | Written, dated, attributed |
| Adaptation | Rebuilds from scratch each context | Has a portable framework, adapts parameters |
| Confidence | Dependent on familiarity with environment | Independent of environment |

**The central insight for the DM-OS:** Every function above can be executed informally and still produce results in a familiar environment. The DM-OS exists to make each function *explicit*, *teachable*, and *environment-independent* — so that confidence doesn't reset with every new company.

---

> **Next Step (Step 2):** Self-assessment. For each of the 10 functions above, answer:
> 1. Do I do this? (Yes / Partially / No / Never thought about it)
> 2. Is it a habit or a system?
> 3. Can I describe my method in 5 minutes to someone new?
> 4. What's my real example (the Career Story)?
> 5. Where is my actual gap vs. the standard above?

---
*Created: 2026-05-04*
*Source: PMI PMBOK 7th Ed., PRINCE2, SAFe, Agile Delivery practice, outsourcing industry DM patterns*
