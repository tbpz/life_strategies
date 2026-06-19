# Function 3: RAID Management
*Risks, Assumptions, Issues, Dependencies*

**Principle:** RAID is the difference between DMs who prevent crises and DMs who manage them after the fact. A RAID log created once and never updated is a historical document, not a delivery tool. Risk, Assumption, and Issue are the same uncertainty at three moments in time — an assumption is simply a risk you haven't noticed you're taking.

---

## Method

*Maintain a Live RAID Log:*
A simple table with four sections. Minimum fields per item:

| Field | Risk | Assumption | Issue | Dependency |
|---|---|---|---|---|
| Description | What might go wrong | What is being assumed as true | What has already gone wrong | What is needed from/by another party |
| Owner | Who is responsible for mitigation | Who will validate this | Who is resolving it | Who owns the dependency |
| Due/Review Date | When to reassess | When to validate by | When to resolve by | When it is needed by |
| Status | Open / Mitigating / Closed | Unvalidated / Confirmed / Invalidated | Open / Resolving / Closed | Pending / Met / At Risk |

*The lifecycle — same uncertainty, three moments:*

| State | What it is | Action |
|---|---|---|
| Assumption | A belief treated as true without proof | Validate |
| Risk | That belief might be false and would hurt | Mitigate |
| Issue | It turned out false and is hurting now | Resolve |

One uncertainty = one line. Log it where the *next action* lives. Never double-log the same thing.

*What earns a line:*
- **Risks & Assumptions** are infinite — triage hard: log only if (a) wrong → material damage **and** (b) cheaper to act now than after it breaks. ~3–5 per project, not 50.
- **Issues:** log if it's actually damaging delivery; trivial ones, just fix.
- **Dependencies:** log every real cross-party one — the seam between people is where things fall.

*Spotting risks (sweep, don't brainstorm):*
- 5 questions: depend on & don't control? · single point of failure? · new / never-done? · critical path, no slack? · unclear / likely to change?
- Pre-mortem: "It's the deadline and we failed — why?"
- Check your scar list — past blindsides, logged by class, not by name.

*Spotting assumptions (distrust your own certainty):*
- Tell-words: "should / just / as long as / they'll / by then / obviously".
- Decompose each date: "what must be true for this to hold?"
- Fact vs. inference: "did someone confirm it, or am I inferring?" (silence ≠ agreement).
- Master sensor: "What am I treating as settled that nobody confirmed?"

*Surface status, not blame:*
- A RAID entry names a task + date + status — never a verdict on a person. You can't be "wrong" about a date.
- Private-first is fine, but set a tripwire: "if not back on track by [date], it goes in the shared log as At Risk."
- Silent absorption removes the cheap fixes and lands the surprise on you.

*Weekly RAID Review (15 minutes):*
- Review each open item: status changed? Owner still right? Date still realistic?
- Add new items surfaced during the week.
- Communicate material changes to relevant stakeholders at the next sync — RAID stays in the log AND in verbal updates.

---

## Cadence

Spot at: kickoff (run the sweep) · every estimate/date accepted · every handoff · every scope change. Updated whenever a new item is identified. Formal review weekly or each sprint. Communicated in stakeholder syncs.

---

## Artifact

A RAID log (spreadsheet, Notion table, or equivalent) — shared with relevant stakeholders, not kept privately.

---

## Adaptation Notes

| Context | Adjustment |
|---|---|
| Outsourcing / fixed-price | Assumptions and dependencies are high-stakes — unvalidated = future scope dispute |
| Multi-team / program | Dependencies matrix becomes critical; need a cross-team dependency owner |
| Solo DM without PMO | Simplify: 1-page log, owner + date + status, reviewed weekly |

---

## Self-Check

- Is the log updated this week, every open item with an owner + date?
- Have I decomposed my key dates into "what must be true"?
- Any assumption now proven shaky — has it been promoted to a risk?
- Any risk materialized into an issue without being re-categorized?

---

## Gap to Close

Stop brainstorming risks from memory. Run the fixed sweep (5 questions + pre-mortem + scar list) at every kickoff, and decompose every accepted date into required-truths. Coverage should come from a checklist, not a good day.

---

*Part of DM-OS | [← Scope Governance](./02_scope_governance.md) | [Next: Stakeholder Communication →](./04_stakeholder_communication.md)*
