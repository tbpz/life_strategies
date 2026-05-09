# Function 3: RAID Management
*Risks, Assumptions, Issues, Dependencies*

**Principle:** RAID is the difference between DMs who prevent crises and DMs who manage them after the fact. A RAID log that is created once and never updated is a historical document, not a delivery tool.

---

## Method

*Maintain a Live RAID Log:*
The log is a simple table with four sections. Minimum fields per item:

| Field | Risk | Assumption | Issue | Dependency |
|---|---|---|---|---|
| Description | What might go wrong | What is being assumed as true | What has already gone wrong | What is needed from/by another party |
| Owner | Who is responsible for mitigation | Who will validate this | Who is resolving it | Who owns the dependency |
| Due/Review Date | When to reassess | When to validate by | When to resolve by | When it is needed by |
| Status | Open / Mitigating / Closed | Unvalidated / Confirmed / Invalidated | Open / Resolving / Closed | Pending / Met / At Risk |

*Distinguish risk from issue:*
- **Risk** = something that might happen and would damage delivery. Mitigation is the action.
- **Issue** = something that has already happened and is damaging delivery. Resolution is the action.
- Treating both as the same category means reacting to everything. The RAID log forces this distinction.

*Weekly RAID Review (15 minutes):*
- Review each open item: has status changed? Is the owner still the right person? Is the date still realistic?
- Add any new items surfaced during the week
- Communicate material changes to relevant stakeholders at the next sync — RAID stays in the log AND in verbal updates

---

## Cadence

RAID log updated whenever a new item is identified. Formal review weekly or each sprint. Communicated in stakeholder syncs.

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

- Is the RAID log updated this week?
- Are all open items assigned to an owner with a date?
- Have any risks materialized into issues without being re-categorized?

---

## Gap to Close

Begin tracking assumptions formally. Every time something is assumed to be true at the start of a project, write it down and assign a person to validate it by a specific date.

---

*Part of DM-OS | [← Scope Governance](./02_scope_governance.md) | [Next: Stakeholder Communication →](./04_stakeholder_communication.md)*
