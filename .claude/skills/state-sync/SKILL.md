---
name: state-sync
description: Regenerate STATE.md wholesale from the current STATE plus newer DECISIONS entries. Use at the end of a task that logged a decision, when STATE is found stale, or when the user asks to "sync", "re-sync", "update the state", or "regenerate STATE.md". No need to ask first. Carries the reader framework, the removal-list step, the four sizing rules that replace a word budget, and the required section skeleton.
---

# Regenerating STATE.md

`STATE.md` is the snapshot of what is true *right now* across the three pillars. It is rewritten wholesale, never appended to. This skill is the only place the full regeneration protocol lives — `CLAUDE.md` just points here.

## Who it is for

Two readers, one file, two depths:

- **The user**, re-orienting after a break or when direction feels lost. Reads **layer 1** — the top four sections — and stops. Target: 60 seconds to say what this workspace is for, what it is betting on, and what the next actions are.
- **Claude**, at session start, advising across pillars. Reads both layers, then follows pointers into the pillar files and `DECISIONS.md` for whatever the session needs.

Both readers know the pillars. So STATE never explains a strategy — it says where a piece stands and names the file.

## The reader framework

The questions a reader arrives with, in the order they ask them. Every line in STATE answers one; a line answering none is cut or moved.

| # | Question | Home |
|---|---|---|
| 1 | What is this, for whom? | STATE — layer 1 |
| 2 | What is the workspace trying to make true? | STATE — layer 1 |
| 3 | Where does it stand? | STATE — both layers |
| 4 | What comes next? | STATE — layer 1 |
| 5 | What is still open? | STATE — layer 2 |
| 6 | What must not be undone, and why? | **`DECISIONS.md` — STATE carries a pointer, never the content** |
| 7 | How does work happen here? | STATE — layer 2 |

Question 6 is the one STATE does not answer. Settled ground and its reasons are `DECISIONS.md`'s whole job; restating them in STATE is what bloats it.

## The four sizing rules

These replace a word budget. **Each is checkable while writing a single line**, not after drafting.

1. **Admission test.** A line earns its place only if it would change what the reader does next session. Three failure modes, each with a destination:
   - *how a rule or plan works* → the pillar file (`career/career_strategy.md`, `creative/creative_strategy.md`, `parenting/parenting_strategy.md`, `financial/financial_checklist.md`)
   - *reasoning, history, "a move from X to Y"* → `DECISIONS.md`
   - *unchanged across two syncs and never used* → cut, or move to `context.md`
2. **Slots, not words.** Each section has a hard **item count**, listed in the skeleton below. Item 5 is known the moment item 5 is typed.
3. **One line, one claim.** Every bullet and every table cell is a single line. If it wants a second sentence, that sentence goes to `DECISIONS.md` or a pillar file, and the item keeps a pointer.
4. **Pointer over restatement.** Name the file or the DECISIONS entry. Never paraphrase it and then cite it too.

**Length is an output, not a target.** Do not count words, do not report a count, and do not trim to hit a number. If a draft comes out long, the admission test was applied too loosely — fix that.

## The two litmus tests (apply while drafting)

1. **Checkable-claim test:** the claim a line makes must be true or false on its face — "the checklist is closed" is checkable; "career is going well" is not. The detail behind the claim is a pointer.
2. **Different-path test:** would this line be written the same way if the workspace had reached today's state by a different route? If it only makes sense as a contrast with what came before — "as of June...", "no longer...", "up from..." — it is history. Cut it; `DECISIONS.md` already holds it.

## The regeneration protocol

1. **Build a removal list first** — before drafting, go through the current `STATE.md` and mark every line that fails the admission test or either litmus test. Sync is subtractive by default.
2. **Rewrite `STATE.md` from scratch** — not line by line. Regenerate the whole file from the current STATE *minus the removal list*, plus the `DECISIONS.md` entries added since its last sync.
3. **Ask, do not guess.** Status that the files cannot settle (a habit that may have lapsed, a stage that may have changed) is asked of the user before drafting. Never leave a `(?)` in the file.
4. **One pass.** Draft once, applying the sizing rules per line. No second trimming pass.
5. **Deprecated ideas fall away by omission.** No tombstones; deprecations live in `DECISIONS.md`.
6. Keep it **present tense, one fact in one place**. Keep the section headers stable across rewrites.
7. **`Where it stands` is a snapshot, not a chronicle.** At most 4 present-tense sentences. No dates, no "first X, then Y".
8. `Last synced` is a bare date: `> **Last synced:** YYYY-MM-DD`.
9. **Check every cross-reference.** Every "see X" must name a `##` header that exists verbatim in the rewritten file, and every file path named must exist on disk.
10. Write the file, then show the removal list in the reply for the user to check afterwards — do not wait for sign-off. The user maintains nothing by hand — draft, they verify.

## The section skeleton

Stable headers. Layer 1 is the 60-second read and ends at the rule; layer 2 is the working index.

| Section | Shape | Slots |
|---|---|---|
| What this is | what the workspace is, for whom | ≤4 lines |
| What is being bet on | the real goal as one quote, then what it rests on | quote + ≤4 lines |
| Where it stands | present-tense prose across the pillars | ≤4 sentences |
| Next up | ordered; #1 unambiguous and doable today; a pillar with no step says so | ≤5 lines |
| *— layer break (`---`) —* | | |
| Status by piece | table: Piece \| State \| Where it lives | one row per piece |
| Unverified bets | beliefs that could still turn out wrong | ≤5 lines |
| Open questions | only ones that block a Next up item or shape how it is done | ≤5 lines |
| How to work here | read order, decision rule, pointers | ≤6 lines |

**State words** for the status table: `not started`, `active`, `paused`, `dropped`, `done`, `upcoming`. A short note may follow after a semicolon.

## Guardrails

- Never repeat the same fact in two places in STATE.
- **Live status lives in exactly one place:** `Status by piece`. Every other mention points there.
- STATE never explains a strategy. If a reader needs the reasoning, they open the pillar file or `DECISIONS.md`.
- `context.md` is **not** regenerated by a sync. It holds the values, constraints and pillar descriptions that rarely change, and is edited only when actually wrong.
- Sections may be renamed as the workspace changes, but the shape — two layers, one status table, one bets list, one open-questions list — should stay.
- The game project keeps its own `STATE.md` in `../casual_autobattler/`. This file points at it; a sync never copies its content.
- All text follows the workspace writing rule: third person, no pronouns, plain words (`CLAUDE.md`).
