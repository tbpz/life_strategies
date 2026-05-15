# Function 8: Quality Assurance
*How to ensure what is delivered actually works and meets expectations*

**Principle:** Quality failures are the most visible form of delivery failure. A DM who does not own QA outcomes will be blindsided by them.

**Current State:** The strongest function in current practice. The method is already effective — it needs formalization, not rebuilding.

---

## Method

*Before Development:*
- Define success criteria: "This feature is done when [specific, testable behavior] is confirmed"
- Confirm the testing assignment: who tests, what types (unit, integration, UAT, regression), in what sequence
- Include QA time in the timeline estimate — it is not the time left over after development

*During Development:*
- Track defect count, severity (Critical / High / Medium / Low), and resolution time
- A rising defect count or unresolved Critical defects is a quality risk — flag it
- Do not treat all defects equally: prioritize by severity, not by volume

*Before Release — Go/No-Go Checklist:*
- [ ] All acceptance criteria met?
- [ ] No unresolved Critical or High defects?
- [ ] UAT completed and signed off (or PM confirmation received)?
- [ ] Rollback plan defined if release fails?

The go/no-go decision is owned by the DM — input gathered from PM and dev team, decision made independently.

---

## Cadence

Quality standards defined before development. Defect tracking throughout. Go/no-go decision at release gate.

---

## Artifact

Acceptance criteria in requirements doc. Defect log with severity. Go/no-go checklist.

---

## Adaptation Notes

| Context | Adjustment |
|---|---|
| Outsourcing / client delivery | UAT and formal sign-off are contractual requirements; document everything |
| Agile sprint-based | QA is part of the sprint; no separate test phase; done = tested |
| Product with high user volume | Performance and load testing added; regression suite critical |
| Regulated industry (finance, health) | Compliance requirements add formal test documentation and audit trails |

---

## Self-Check

- Is there a written acceptance criterion for every feature in the current release?
- Are Critical defects resolved or have they been explicitly accepted by the decision authority?
- Who owns the go/no-go decision — is it clear?

---

*Part of DM-OS | [← Delivery Cadence & Tracking](./07_delivery_cadence_tracking.md) | [Next: Change Control →](./09_change_control.md)*
