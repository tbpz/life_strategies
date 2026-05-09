# DM-OS — Step 2: Self-Assessment

> **Purpose:** An honest reflection on current practice across all 10 DM functions, measured against the professional standards documented in Step 1. Rating scale: **Yes / Partially / No / Never considered.**

---

## Function 1: Engagement Setup

**What professional standards require:**

- Map all stakeholders within 48h: who has authority, who has opinion, who has information → **Partially.** Relevant stakeholders are identified quickly, but mapping is done by technical role only — who is the developer, the QA, the Product Manager, the client. The central authority and information source for any given project is typically the Product Manager or someone on their team, so this identification happens intuitively rather than systematically.
- Locate or create the core project artifacts: charter/scope doc, backlog, team roster, contract/SOW → **Partially.** The only artifact consistently created at project start is a product requirements document, and occasionally a UX wireframe when the enhancement involves UI/UX changes. Other artifact types — charter, backlog, team roster, SOW — are unfamiliar in practice.
- Run a listening session (not a meeting) with each key stakeholder — goal is information, not status → **Partially.** The primary listening source at project start is the PM, since all requirements originate from that role. The tech lead is the second source, providing input on feasibility and resource needs.
- Identify the biggest unspoken risk within the first week — the one everyone knows but hasn't named → **Never considered.** After gathering available information, obvious risks are identified and addressed — for example, pushing the product team to clarify vague requirements. No particularly complex cases have surfaced where the critical risk was deeply hidden and required significant time to uncover.
- Establish communication channels and cadences *before* the first status update → **Partially.** At Zalo, this was done more proactively — creating a group chat and setting up a weekly meeting within the project team. At Orange Logic, it is done less consistently. A team chat group is still created, but daily or weekly meetings are rarely needed because the company tracks time and progress through an internal Jira-like tool. Even so, direct check-ins are still necessary to understand the full picture. A personal schedule is maintained to know when to follow up with each team member.
- Define what "done" looks like for the first milestone — get explicit alignment, not assumed consensus → **No.** The working assumption is that "done" is already defined by the product requirements document.
- Set recurring delivery cadence (stand-up, weekly sync, steering committee) within Week 1 → **Partially.** As noted above, formal cadences are rarely established at OL because the company favors deep, focused work and reflects progress in the internal tool. There is a weekly sync between the DM team and the CTO covering project risks.
- Understand the internal approval chain before making any commitments → **Partially.** The approval chain tends to be straightforward in environments worked in so far, and it has never been written down. Understanding emerges during project execution, and this approach has not caused visible consequences to date.

---

## Function 2: Scope & Requirements Governance

**What professional standards require:**

- Maintain a single, version-controlled source of truth for scope (requirements doc, backlog, SOW appendix) → **Yes.** Requirements are written in a formal document accessible to all relevant stakeholders.
- Ensure every requirement has: an owner, an acceptance criterion, and a priority → **Partially.** Owner is not explicitly defined because requirements always originate from the PM. Acceptance criteria and priority are usually absent. Requirements documents typically describe feature behaviors without structured metadata.
- Establish a formal (or at minimum explicit) process for *how* new requirements enter the backlog — not by informal conversation → **Partially.** The process is not fully informal, but also not formal. The typical flow: verbal discussion with the requester → team assessment for effort and estimation → mutual agreement on approach → written summary or email requesting requester confirmation.
- Conduct regular scope reviews with stakeholders to confirm alignment hasn't drifted → **Partially.** Reviews are not on a regular cadence. When something feels misaligned, a targeted check-in is initiated with the relevant stakeholder to confirm understanding.
- Document what is explicitly *out of scope* — as important as what's in scope → **Partially.** Done occasionally, not consistently.
- Ensure delivery team understands scope boundaries and knows to flag ambiguities before starting work → **Yes.** A project kick-off is held within the team to plan the work and surface ambiguities before execution begins.
- Link requirements to business goals — "what problem does this solve?" prevents gold-plating → **Yes.** Business goals are typically articulated by the PM. When acting as PM, the rationale is captured in the requirements document.

---

## Function 3: RAID Management

**What professional standards require:**

- Maintain a live RAID log reviewed every sprint or week — not a static document → **Never considered.** Risks, issues, and dependencies are tracked informally on a day-to-day basis, with attention directed at the most immediate or highest-priority item. A complete, structured RAID log has never been maintained.
- **Risk:** Probability × Impact → Priority → Owner → Mitigation action → Review date → **Partially.** The structured risk model is not applied. Risks are identified and mitigation actions are defined. If action is required from someone else, a follow-up date is set and escalated until resolved.
- **Assumption:** Written explicitly, dated, assigned someone to validate by a specific date; revisited regularly → **Never considered.** Assumptions are not tracked as a formal category.
- **Issue:** Raised, assigned an owner, tracked to resolution — never "parked" indefinitely → **Yes.** Issues are tracked personally, not shared broadly with stakeholders. The view is that issues are routine; stakeholders only need to be informed of critical ones.
- **Dependency:** Mapped directionally (what we need from others; what others need from us), with dates and owners → **Partially.** No dependency map exists at project start. Blockers involving external teams are identified as they surface, tracked, resolved, and then no longer maintained.
- Separate risk (potential future problem) from issue (problem that has already materialized) → **No.** Both are treated as work that needs to be done, without formal distinction.
- Escalate risks before they become issues — not after → **Yes.** This approach is applied instinctively.
- Communicate RAID status in stakeholder updates, not just in the log itself → **Yes.** In weekly syncs with the PM and line manager, the current risk situation, the planned mitigation, and the expected timeline are communicated verbally.

---

## Function 4: Stakeholder Communication

**What professional standards require:**

- Build a stakeholder map: identify each stakeholder's interest, influence, and preferred communication style → **Partially.** No written map exists. Understanding of stakeholders is built through extended working relationships. For new stakeholders, information is gathered through other channels, but remains informal and kept mentally rather than documented.
- Define a communication matrix: who gets what, how often, in what format (email, dashboard, meeting, Slack) → **Never considered.** No formal communication matrix has been defined.
- Distinguish between *informing* and *decision-making* communications — mix them and both suffer → **Yes.**
- Status reports must cover: accomplishments, upcoming work, risks/issues, decisions needed → **Partially.** Updates tend to be brief. Some elements are included at times, but the full structured format is not applied consistently.
- Cadence must be predictable — stakeholders should never need to chase for updates → **Partially.** Current sync cadences are typically initiated by stakeholders themselves. There have been cases where stakeholders had to ask for updates because a proactive cadence was not established.
- Tailor depth by audience: executives want headlines + red flags; team leads want detail + decisions → **Yes.**
- Bad news must travel faster than good news — surface problems before stakeholders hear from other sources → **Partially.** There is a tendency to attempt resolution independently before escalating — partly out of concern that escalating too quickly signals an inability to make decisions, rather than a DM exercising judgment.
- Written async updates reduce the meeting load and create a paper trail → **Partially.** Applied inconsistently; no clear personal rule governs when written updates are used versus not.

---

## Function 5: Team & Resource Management

**What professional standards require:**

- Maintain clear role clarity — every team member knows what they own, who they depend on, and what "done" means for their work → **Partially.** Role clarity in software development teams is generally assumed to be established from the start, so this is not actively managed.
- Identify and remove blockers actively — don't wait for stand-up to discover them → **Yes.** This is the area of highest confidence. A natural orientation toward risk means blockers tend to be detected early. The approach is instinct-based rather than framework-based.
- Track utilization without micromanaging — know who is overloaded, who is underutilized → **Partially.** Utilization is tracked closely, but with a tendency toward micromanagement. At Zalo, the absence of a unified tracking platform meant physically checking in with team members frequently, which interrupted their work. At OL, the internal platform provides time-tracking by ticket, but status in the system does not always reflect reality — the habit of direct check-ins persists as a result.
- Resolve team conflicts early — escalate interpersonal issues before they damage delivery → **Partially.** Early detection of interpersonal tension is possible, but resolving human conflicts is a different and less developed skill.
- Create conditions for psychological safety — team members must feel safe raising problems → **Partially.** Team members are consistently told they can raise issues freely, and feedback is always delivered constructively. Whether they actually feel psychologically safe is uncertain.
- Know each team member's constraints (skills, availability, competing priorities) → **Yes.** This knowledge is developed over time through direct experience working with each person.
- Distinguish between team problems the DM can solve vs. ones that need HR/leadership escalation → **No.** No clear framework for this distinction exists. The lesson from Zalo was to tackle every problem that affects the delivery objective, regardless of whether it was a team or organizational issue.
- Ensure onboarding of new team members is covered — uncovered onboarding = weeks of lost productivity → **No.** Onboarding is minimal in practice: a brief introduction to the project, assignment of initial tasks, and an instruction to ask for help when unclear. There is no structured onboarding process.

---

## Function 6: Financial & Commercial Awareness

**What professional standards require:**

- Understand the contract structure: fixed-price vs. T&M vs. retainer — each changes risk allocation entirely → **No.** All experience to date has been in product companies, not outsourcing contexts. Contract structures and their implications are not a practical area of knowledge.
- Track burn rate against budget regularly — know the financial health of the project, not just the delivery health → **No.** Same context — product company delivery does not surface budget as a tracked metric.
- Recognize early warning signs: budget overrun trajectory, scope expanding without budget adjustment, team billing that doesn't match deliverables → **No.** In a product company context, achieving outcomes is the primary objective. When scope expansion is necessary to reach the goal, it is pursued without reference to a budget ceiling.
- Understand what triggers a change order — and know when to raise one vs. absorb the cost → **Yes.** The rationale behind any change is examined before accepting it. When a change is requested, the requester is consulted to assess whether it is truly necessary and how it should be handled.
- Be able to report on financial status in client conversations without depending entirely on a PM or Finance team → **No.** No exposure to this requirement.
- Flag margin risks to leadership before they become P&L problems → **No.**
- Know the commercial implications of timeline slippage: delay ≠ just schedule problem, it may = penalty clause → **No.**

---

## Function 7: Delivery Cadence & Tracking

**What professional standards require:**

- Define the delivery rhythm at project start: sprint length, milestone dates, review cadence → **Yes.** This is done naturally at the start of every project.
- Track progress against plan weekly — not monthly, not in retrospect → **Yes.** Progress is tracked daily. A personal calendar tracks the next action for each project. If the next action depends on someone else, a commitment date is obtained and followed up on when due. If no date can be committed, follow-up occurs daily.
- Use leading indicators (work started, blockers count, velocity trend) not just lagging indicators (tasks completed) → **No.** Only the next action per project is tracked. Leading indicators as a category are not used.
- Maintain a realistic forecast: if current velocity continues, when do we finish? → **Yes.** Remaining work and time are assessed, and instinct is applied to judge whether the deadline is at risk. The forecast is not formally calculated.
- Surface schedule risk as soon as trajectory diverges from plan — not when the date is missed → **Yes.** When velocity slips, the risk is immediately visible and flagged.
- Burn-down / burn-up charts, milestone trackers, or equivalent — visible to team and stakeholders → **No.** No shared tracking artifact is maintained. The DM holds the most complete picture of the project. When stakeholders want a status update, they come for a report. At OL, the internal tool maintains some visibility through status fields.
- Distinguish between output (features shipped) and outcome (value delivered) in tracking → **Yes.** Business outcomes are understood and used as the measure of whether what was shipped actually addressed the underlying need.

---

## Function 8: Quality Assurance

**What professional standards require:**

- Define quality standards and acceptance criteria *before* development begins — not at review time → **Yes.** Project objectives and success criteria are defined before work starts.
- Ensure a testing strategy exists: who tests, what types (unit, integration, UAT, regression), when → **Yes.** For software projects, testing is assigned to the QA team. For smaller or personal projects, a testing approach is kept mentally. A written strategy is only produced for complex projects.
- Track defect rate, severity, and resolution time as delivery health metrics → **Partially.** At OL, this is handled through the internal tool. At Zalo, only a defect list and severity were tracked; resolution time required daily follow-up with the QA team directly.
- Include QA effort in timeline estimates — QA is not "the time left after development" → **Yes.**
- Facilitate UAT (User Acceptance Testing) with actual stakeholders — not just internal sign-off → **Yes.** At Zalo, features were released to users and behavioral tracking data was observed. At OL, UAT opportunities are limited; PM confirmation serves as the closest equivalent.
- Ensure Definition of Done includes quality gates, not just feature completion → **Yes.** There is a strong personal conviction against shipping something that delivers no real value.
- Own the go/no-go decision for releases — DM asserts readiness, doesn't just defer to dev team → **Yes.** The go/no-go decision is actively owned — input is gathered from PM and dev teams, but the final call is made independently.

---

## Function 9: Change Control

**What professional standards require:**

- Define the change control process at project start: how changes are submitted, evaluated, approved, and communicated → **Partially.** Change is actively managed, but the process is not defined upfront. When a change arrives, it is reviewed in context and a decision is made based on the situation.
- Assess every change request for impact on: scope, timeline, budget, resource, risk → **Yes.**
- No change proceeds without explicit approval from the appropriate authority (client, sponsor, steering committee) → **Partially.** There is a clear understanding of who the official decision authority is. However, when a decision appears low-risk enough to make independently without significant downside, that call is made without escalating for formal approval.
- Document all approved changes and update the baseline plan accordingly → **No.** The tendency to move fast means documentation of changes is frequently missed. This has caused problems at Zalo when decisions were later disputed.
- Communicate the impact of changes to all affected parties — team and stakeholders → **Partially.** Occasionally, some team members or stakeholders affected by a change are overlooked in the communication.
- Distinguish between a change request (new work) and a defect fix (work that should have been done correctly) — these have different approval paths → **Yes.** Work that was not in the original scope is treated as a change request; work that should have been delivered correctly in scope is treated as a defect.
- Track the cumulative impact of changes — individual changes look small; combined, they can double the project → **No.** The concept of cumulative change impact is not something currently tracked or considered.

---

## Function 10: Escalation & Crisis Management

**What professional standards require:**

- Define escalation thresholds at project start: what types of problems go to whom → **No.** Like change control, escalation thresholds are not defined upfront. The approach is experiential — each situation is assessed based on past exposure.
- Escalate with: problem statement, impact, options considered, recommended action — not just "we have a problem" → **Yes.** Escalating without a clear framing would create unnecessary back-and-forth. The habit is to analyze the situation fully, identify options, and present a recommended path for the decision-maker to choose from. The cost of this thoroughness is that escalation sometimes takes longer than it should.
- Escalate early enough that leadership has time to act — not as a post-mortem → **Yes.** However, the same thoroughness that improves escalation quality sometimes delays the moment of escalation — the desire to bring a well-reasoned analysis can slow the timing.
- In a crisis: establish facts first, then communicate; don't speculate in stakeholder updates → **Partially.** Occasionally, a situation is held back longer than warranted while facts are being confirmed, partly because the initial read of the situation turns out to be wrong.
- Crisis response sequence: Contain → Communicate → Investigate → Remediate → Prevent recurrence → **Yes.**
- Protect the team during crisis — DM is the interface to leadership, not the conduit for blame → **Yes.** The Zalo experience reinforced this: the DM is accountable for everything within the product and project scope. Team members' failures are a management failure as well. This responsibility is accepted, though it can be exhausting.
- Know the difference between a delivery problem (DM owns) vs. a strategic problem (leadership owns) → **No.** No clear framework exists for this distinction.
- After any major escalation: conduct a brief retrospective to improve the system, not find scapegoats → **Partially.** There is no inclination to assign blame. However, dedicated retrospectives rarely happen in practice — the flow of continuous, back-to-back execution work tends to crowd them out. The importance is understood, but the time is never found.

---

*Created: 2026-05-09*
*Based on: DM-OS Step 1 Framework (dm_os_step1_framework.md)*