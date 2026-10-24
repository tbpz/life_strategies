---
name: decision-log
description: Append one entry to DECISIONS.md when the user states or picks a decision. Use whenever CLAUDE.md's DECISION protocol fires — no confirmation needed. Carries the entry budget, the one-claim-per-bullet rule, and the decision-not-diff test that keeps entries small and easy to grep.
---

# Appending to DECISIONS.md

`DECISIONS.md` is the append-only history of decisions and their reasons. This skill is the only place the full append protocol lives — `CLAUDE.md` just points here.

Append-only means entries are never edited or deleted once written. That makes what goes *into* an entry the only lever — get it wrong and it stays wrong, so the rules below matter.

## The two tests (apply while drafting)

**1. Decision, not diff.** An entry records the *principle adopted* and *the evidence that led to it* — not a list of what values changed.
- Numbers are allowed only as **frozen, dated evidence**: "the user confirmed on 2026-10-24 that the sprint was dropped" stays true forever.
- Numbers are **never** recorded as **current settings**: an amount, a window, a count that the next review will change. Those live in the pillar file (`financial/financial_checklist.md`, `parenting/stages/stage_2_toddler/kindergarten_plan.md`, and so on). Point there instead of restating them.
- If a line is fully recoverable from `git log -p <file>`, cut it and name the file instead.

**2. One claim per bullet.** Short bullets, one claim each — not one long bullet carrying the whole decision. `CLAUDE.md`'s "grep it, don't read it" rule only works if a grep hit is one line, not a block of prose.

## The append protocol

1. Fires only for a choice the user stated or picked — never for Claude's own suggestion that has not been taken up, never batched. No "Log it?" question first.
2. Draft the entry in the standard format: `## [YYYY-MM-DD] [tag] Title` → **Decision** / **Why** / **Replaces**, each as short one-claim bullets. The tag is part of the heading and is one of:
   - `career`, `creative`, `parenting`, `financial` — the decision settles something in that pillar.
   - `workflow` — the decision settles how the workspace itself runs (context files, skills, logging, process).
   - A decision that spans two pillars takes the one it changes most.
3. Apply both tests while drafting. Cut diff-shaped lines. Point at the pillar file for live details.
4. **Hold the budget: about 250 words, hard cap 350 words.** Report the word count in the one-line note that says what was logged.
5. Insert at the **top** of the log, directly below the header block — never at the bottom, never in the middle.
6. Never edit, reorder, or delete an existing entry to make room. If an old entry is now stale or contradicted, write a *new* entry that says so and points at the current pillar file.
7. **Backfilling** an old decision from a file or commit is allowed. Date it by when it was made (or when its file was dated), add a **Source** bullet naming the file, and say if the exact day is not recorded.

## Guardrails

- **Live status has no home in DECISIONS.** DECISIONS records why a choice was made, not what a plan currently says. Current status is `STATE.md`'s job.
- Every bullet should read clearly on its own, since that is the form a `grep` match returns it in.
- Plain words, third person, no pronouns, as the rest of the workspace (`CLAUDE.md`).
- Choices about the game project itself (its rules, numbers, screens) belong in `../casual_autobattler/DECISIONS.md`. Log here only decisions about the life strategy, such as what role the game plays.
