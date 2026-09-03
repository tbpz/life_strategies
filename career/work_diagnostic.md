# Current-Role Diagnostic — Weakness Register

> **Status:** Active. Supersedes `work_audit_experiment.md` (2026-06-26), which sat at "Data collection" with an empty log for ~10 weeks and is folded into this file rather than discarded.
> **Purpose:** Convert the feeling "I'm not doing well at Orange Logic" into a short, evidence-backed, hard-capped Weakness Register — or into an honest verdict that performance is already adequate. Retrospective throughout: every instrument here is completable in one sitting from existing traces, not a forward-logging exercise.
> This file is self-contained and can resume in a fresh session.

---

## Background — Why This Instrument Exists (carried over, still correct)

The original work-audit experiment (2026-06-26) reached three conclusions before any data was collected, in response to a persistent feeling that "too much time goes to busy, unimportant operational work, leaving no room for the work that actually builds capability":

1. **There is no separate "important" vs. "unimportant" work competing for time.** There is one stream of operational delivery work, run in one of two modes:
   - **Manual mode:** acting personally as the follow-up, the router, the safety net, the reviewer. Regenerates endlessly; does not compound.
   - **Leveraged mode:** a system, an owner, or a forcing-function carries the handoff. Shrinks itself over time; *is* the capability being built.
2. **"Unimportant" is the wrong axis.** The correct axis: **did this need ME specifically (judgment / authority / relationship), or does it merely route through me by default?**
3. **The feeling is not yet evidence.** The conviction "there must be waste" was reached *before* looking. Per the Anxiety Engine (`career_strategy.md`), "busy and inefficient" is a baseline hum, independent of actual efficiency.

**Where this instrument was mis-filed:** the Me-test axis measures whether delivery work has been *systematized* — that is a **process-management** question (job part 2), not a project-management one. It sat under the wrong half of the job for 10 weeks. This file gives it its correct place: it is now the evidence source for failure mode **F2** below, not a freestanding experiment.

---

## Job Model (context for both instruments)

The role has two parts. Only part 1 has an existing framework (`DM_Operating_System/`); part 2 has none, and is deliberately kept small here rather than mirrored into a second 10-function playbook.

| Part | What it is | Authority |
|---|---|---|
| **1. Project management** | Specific projects delivered on time at required quality | Full DM authority over the project |
| **2. Process management** | Improve the delivery process; notice recurring failure classes, design and propose interventions | **Advisory only — others decide and roll out** |

**Guardrail (also in `career/_AI_RULES.md`):** because part 2 is advisory, adoption and rollout outcomes are excluded from scoring by rule. Being accountable for a process outcome without the authority to cause it is the Zalo double-bind in miniature — never let this instrument measure that.

---

## Sitting 0 — The Incident Sheet (30–45 min, do this first, zero dependencies)

Write 5–8 specific real events from the last 90 days where the feeling "I'm not doing well" actually fired. One line each, pure retrieval — no scoring, no tagging, no DM-OS references yet:

| Date | What happened | The exact trigger moment | What was done | Outcome | Who else noticed |
|---|---|---|---|---|---|
| | | | | | |

**This step is self-diagnosing — there is no null result.** 8 retrievable incidents with specific triggers means there is something real to name and feed into Sittings 2–3. A thin, vague, or reconstructed-after-the-fact sheet is *already* Verdict C evidence — a baseline hum has no incidents attached to it.

**Also settle this while here (one line):** did any RAID log / two-line change record / acceptance-criteria habit actually happen informally between June and September, even if never logged in `career_strategy.md`? The record currently contradicts itself — `self_discovery_log.md` (June 20–21 session) credits "DM-OS applied at work, producing real results" while the habit table has read all-⬜ since 2026-06-12. One of two things is true: informal practice happened and went unrecorded, or the confidence lift came from *writing* DM-OS rather than *practicing* it. This answer feeds Sitting 4's habit disposition.

---

## Sitting 1 — Trace Pull (~45 min, before any self-scoring)

Pull these *before* scoring anything — the ordering is the main defence against self-assessment being an unreliable judge of its own performance (see `career_strategy.md`'s Anxiety Engine).

| Trace | What it answers |
|---|---|
| Slip/defect record, last 90 days (internal Jira-like tool) | Objective, non-introspective spine — what actually missed a date or needed rework |
| **Chase events** | Every time a stakeholder had to ask for a status that hadn't been sent — the single most diagnostic list available |
| Assignment trend, last 12 months | Are harder/messier/higher-stakes projects still arriving? Orgs don't route hard work to people they're preparing to replace |
| Weekly DM↔CTO risk sync | What gets pushed on *repeatedly* — the recurring unanswered question is the real gap |

**Pre-committed weighting:** where traces disagree with self-assessment, traces win for the register; the discrepancy itself gets recorded as a line item. Traces reading *more positive* than self-assessment is not noise — it is Verdict C evidence. Also record explicitly: absence of negative feedback, in a company with a standing weekly risk sync, is weak but real evidence against the replacement fear — not proof, but not nothing.

---

## Sitting 2 — Instrument P1: Project-Management Live-Gap Conversion (~60 min)

Do not re-score the DM-OS grid from scratch. Open `archive/dm_os_step2_reflection.md` and add **one column** to every row, with exactly three permitted values:

| Value | Bar to assign it |
|---|---|
| **Caused harm** | Must cite a specific incident by date from the Sitting 0 sheet |
| **No harm observed** | Real gap against professional standards, but no observable damage here — the default |
| **N/A at OL** | Standard doesn't apply in this environment; one-line reason required |

"Partially" is not a permitted value here — the axis is harm, not maturity. Maturity is unbounded and self-referential (every function can always be more mature — the Anxiety Engine's preferred shape); harm is bounded by the fixed 90-day window.

**Prediction, written down before scoring so the collapse counts as a result:** most "No / Never considered" rows in the May reflection will land in *No harm observed* or *N/A at OL*. The clearest expected N/A: **Function 6 (Financial & Commercial)**, scored almost entirely "No" — that gap is portability-shaped (product-company experience only) and portability is now a parked ambition, not an active target. Strike it and any similar rows outright with a one-line reason.

Record after scoring: did the shrinkage prediction hold? (Yes/no, and by how much — e.g., "~30 gaps → N named".)

---

## Sitting 3 — Instrument P2: Process-Management Failure Modes (~60 min)

No new 10-function framework — that repeats the mistake of building unexecutable documents. Process management is: *notice a recurring failure class → design an intervention → propose it → (others decide)*. Advisory authority truncates the chain at the proposal step, so only these seams are testable:

| # | Failure mode | Evidence test (one sitting) |
|---|---|---|
| **F0** | **Mandate ambiguity** — improvement is self-assigned, unrequested, unreviewed, uncredited | Is it in the role definition or review criteria? Has anyone ever *requested* one? Name one change that was recognised by someone else. |
| **F1** | **Class blindness** — recurring problems handled as one-offs, never named as a class | Take 3 problems from the Sitting 0 sheet / last 90 days: first occurrence or repeat? If repeat, was it ever named as a type? |
| **F2** | **Self-absorption of the gap** — becoming the router/follow-up/safety net personally, so the gap never becomes a process | Reconstruct the last ~10 working days retrospectively from written traces (ticket time-tracking, calendar, chat). Tag each meaningful chunk (≥15 min): **Me-test** (Y = genuinely needed this person's judgment/authority/relationship; N = merely routed through by default), **Origin** (Y = exists only because an earlier step lacked a system), **Recurrence** (Rec/One). Target: rows tagged `N / Rec`, especially `N / Y / Rec`. |
| **F3** | **Proposal quality** — proposals arrive unevidenced, unsized, or without a named owner | Name every process change proposed in the last 12 months. For each: was it evidenced, sized, and did it name an owner? |

**Score F0 first.** If the mandate is self-assigned and unmeasured, F1–F3 get read under a different frame — the felt failure may be against a KPI nobody set.

**Trade-off, stated honestly:** the F2 reconstruction is retrospective and will under-count small routing chunks — it is a **lower bound**. A positive finding (real `N/Rec` patterns show up even under-counted) is strong evidence. A null finding is *weaker* evidence for Verdict C than a live week-long log would have been — but an uncollected live log is not weaker evidence, it is *no* evidence, and 10 weeks already demonstrated which one actually materializes. Close on the lower bound either way; do not restart a prospective log "to be sure."

---

## Sitting 4 — Weakness Register, Verdict, Close (~45 min)

### The Register

One table. **Hard cap: 3 items.** The cap is the design, not a first pass — adding a 4th is prohibited until one of the three is closed.

| Rank | Gap | Source (P1 function / F-mode) | Citing incident (date) | Proposed fix (single artifact or rule) |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

### Pre-committed verdicts — declare exactly one

- **Verdict A — real, named, bounded capability gap.** ≥1 function or failure mode has a cited incident where a DM-controllable action or missing artifact was the proximate cause. → Fix the top 3 only, one at a time, each as a single artifact or a single rule — never a programme.
- **Verdict B — legibility gap, not a capability gap** *(predicted outcome — see reasoning below)*. Delivery outcomes are sound (traces neutral-to-positive, harder work still arriving) but nothing about the performance is visible outside one head, so competence can't be evidenced on demand. → Fix is not "get better at delivery" — it's 1–2 artifacts that make existing competence legible (e.g., a shared status artifact readable without contacting the DM; a running change record). This presents as "not doing well" but is actually **"cannot see myself doing well."**
- **Verdict C — performance is already adequate; the feeling is the Anxiety Engine.** No cited incidents with DM-controllable proximate causes; traces neutral-to-positive; `N/Rec` rows scarce or non-recurring. → Close the loop. Explicitly forbidden: hunting harder, launching a new live log "to be sure," expanding scope to a third job part.

**Anti-goalpost clause:** "still feeling unsafe after the register is written" is pre-classified as Verdict C evidence, never as a signal to gather more.

**Why Verdict B is the predicted outcome:** outside-view feedback was confirmed effectively absent (no formal review, no usable informal signal) when this instrument was designed. Against `mastery_infrastructure.md`'s six pillars, the DM role structurally scores **Clear metrics ❌** (no standard for "good DM" beyond shipped/not-shipped) and **Expert models ❌** (no calibration channel beyond the CTO risk sync). A role with no metrics and no calibration cannot generate the feeling of being good at it regardless of actual performance — that's an environment-design gap, not a performance gap, and it's the leading hypothesis for the "unsafe" feeling persisting with no evidence of real problems attached. (Optional deeper look: run the `mastery_infrastructure.md` scorecard against the DM role itself — but only *after* the register, never before, since it explains a B/C verdict rather than helping decide one, and is exactly the kind of interesting adjacent framework that could absorb the sitting the register needs.)

### Update on close

Once a verdict is declared, update `career/career_strategy.md`:
- Resolve the three legacy `⬜` habits per the Sitting 0 answer — dated disposition each, none left at `⬜`.
- If Verdict A or B: record the top 1–3 fixes as the new active focus.
- If Verdict C: apply the hard rule already in `career_strategy.md` — close the career worry loop, permission to not think about career safety until the next periodic check.

---

## How To Resume

Return with whatever sittings are complete. Resume from the next unfinished sitting in order (0 → 1 → 2 → 3 → 4). No need to re-explain context — this file is self-contained.

---

*Created: 2026-06-26 (as `work_audit_experiment.md`). Rewritten and re-scoped: 2026-09-03.*
*Part of the Career strategy, Phase 3 (Current-Role Diagnosis). Companion to `career_strategy.md`, `DM_Operating_System/`, and `archive/dm_os_step2_reflection.md`.*
