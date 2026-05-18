# Stage Document Guide

Read this before creating or editing any `00_stage_N_overview.md` file.

---

## Template

```
# Stage N: Name (age range) — STATUS

**Status:** [✅ Active | ⏳ Upcoming | ⏳ Future] — [one-line context]

**Develop:** [outcome 1] · [outcome 2] · [outcome 3]
**How:** [stage-level mechanism in one line]

---

### [emoji] Domain Name
*Build [developmental outcome] — [mechanism/approach].*

- [x] Established habit — brief description of what doing it looks like in practice
- [ ] Open action — specific task (window: Xmo) or (trigger: X)

### [repeat for all 6 domains: 🧠 Cognitive · 🗣️ Language · ❤️ Social-Emotional · 🏃 Physical · 🏥 Health · ⚖️ Moral]

---

**Avoid:** [single line]

→ **Why this approach:** [Rationale — focuses, actions, and the reasoning behind them](stages/stageN_name/rationale.md)

→ **Deep dive:** [link1] · [link2]

*Develop Stage N+1 at ~[age] based on observed [what to watch].*

---
*Last Updated: YYYY-MM-DD*
```

---

## Rules

### Stage header
- `Develop:` = developmental outcomes the stage builds — not activities, not strategies
- `How:` = the single overarching mechanism for this stage

### Required artifacts per stage

Each stage folder must contain:
- `00_stage_N_overview.md` — operational checklist (what to do)
- `rationale.md` — reasoning layer (why these focuses, why these actions)

The `rationale.md` stub is created when the stage folder is created. It is filled in when the stage becomes active — based on observed temperament at that time, not speculatively in advance.

### Domain strategy line
- Format: `*Build [what] — [how].*`
- "What" = the specific capacity being developed in this domain this stage
- "How" = the parenting posture or mechanism that produces it
- One line only. Deep-dive files hold the evidence.

### Action item types — two types only

| Type | Format | Meaning |
|---|---|---|
| Established habit | `- [x] Name — what doing it looks like` | Running continuously — visible for coverage confidence, not for doing |
| Pending action | `- [ ] Action (window: Xmo) or (trigger: X)` | One-time action with a real deadline or trigger |

Recurring behaviors are **never** `[ ]`. They are habits, captured as `[x]` once established. Only one-time decisions or setup tasks use `[ ]`.

### Active stage completeness rule
Every domain in the **active** stage must have at least one `[x]`. A blank domain signals an incomplete strategy, not an intentional omission.

### Future stages
No `[x]` items until the stage is active. Only `[ ]` upcoming actions (pre-work before the stage begins).

### Docsify link format
`basePath: '..'` in `parenting/web/index.html` means Docsify roots at `parenting/`. All inline links must be **absolute from that root**:

✅ `[checklist](stages/stage_1_infant/food_introduction_checklist.md)`  
❌ `[checklist](food_introduction_checklist.md)` — resolves to parenting root, not file's directory

---

## Current Stage Status

| Stage | File | Develop when |
|---|---|---|
| Stage 1: Infant (0–18mo) | `stage_1_infant/00_stage_1_overview.md` | ✅ Active |
| Stage 2: Toddler (18mo–3yr) | `stage_2_toddler/00_stage_2_overview.md` | ~16 months old |
| Stage 3: Pre-school (3–6yr) | `stage_3_preschool/00_stage_3_overview.md` | ~2.5 years old |
| Stage 4: School Age (6+) | `stage_4_school/00_stage_4_overview.md` | ~5.5 years old |
