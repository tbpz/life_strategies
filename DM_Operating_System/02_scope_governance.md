# Function 2: Scope & Requirements Governance
*How to define, protect, and manage what is being built*

**Principle:** Scope is the contract between delivery and expectation. Every unmanaged scope change either silently expands work or creates a gap between what was wanted and what was built.

---

## Method

*At Project Start:*
- Create a single requirements document that all stakeholders can access and reference
- For every requirement, record at minimum: description, priority (High/Medium/Low), and acceptance criterion ("this is done when...")
- Add an explicit "Out of Scope" section — even a short bullet list prevents future disputes
- Confirm the document with the PM or equivalent owner before work begins

*During Execution:*
- When a new requirement arrives, run it through the intake process before responding: understand it, assess team effort/impact, then confirm in writing before execution begins
- If something feels misaligned — scope drifting, stakeholder expectations diverging — initiate a targeted check-in, do not wait for it to surface in a crisis
- Conduct a brief scope alignment with the key stakeholder every 2–4 weeks: "Here is what we are building. Has anything changed in your priorities?"

---

## Cadence

Requirements document created at project start. Scope alignment check every 2–4 weeks, or when scope change requests arrive.

---

## Artifact

Requirements document with priority + acceptance criteria + out-of-scope section. Written confirmation (email or comment) for every new requirement accepted.

---

## Adaptation Notes

| Context | Adjustment |
|---|---|
| Outsourcing / fixed-price | Scope baseline is a legal document; changes must trigger formal change control, not verbal agreement |
| Agile / product | Backlog is the scope artifact; refinement sessions are the governance mechanism |
| Legacy / evolving system | Add an assumption log for undocumented behaviors; scope must account for unknowns |

---

## Self-Check

- Does a single written source of truth for scope exist and is it current?
- Does every requirement have a priority and an acceptance criterion?
- Is there an out-of-scope section?

---

## Gap to Close

Build the habit of acceptance criteria as a non-negotiable field in every requirement. Vague requirements ("it should work") are a sign that the requirement is not yet ready to be built.

---

*Part of DM-OS | [← Engagement Setup](./01_engagement_setup.md) | [Next: RAID Management →](./03_raid_management.md)*
