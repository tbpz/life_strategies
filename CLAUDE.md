# CLAUDE.md — Life Strategies Workspace

> Auto-read at every session start. Provides identity, pillar list, and session routing.
> Read `STATE.md` next for where things stand and what to do next, then `context.md` for values and constraints.

---

## Who This Is

Mid-30s tech professional (Delivery Manager, Orange Logic). Has a young son and a family to provide for. Financially stable but not large-scale wealthy.

The real goal is to rebuild self-trust in handling life's essentials so that free time feels genuinely free — not stolen. Beyond self-trust, the deeper need is a meaningful pursuit: exercising genuine capability on a real problem with observable impact. Guilt-free leisure (Dota, football, consuming stories) continues in parallel for flow and rest.

---

## The Three Pillars

| Pillar | Deep-dive file | Status |
|---|---|---|
| 🔑 **Pillar 1 — Self-Trust & Career Competence** | [career_strategy.md](career/career_strategy.md) | See [STATE.md](STATE.md) |
| 🎨 **Pillar 2 — Meaningful Pursuit** | [creative_strategy.md](creative/creative_strategy.md) | See [STATE.md](STATE.md) |
| 👦 **Pillar 3 — Parenting** | [parenting_strategy.md](parenting/parenting_strategy.md) | See [STATE.md](STATE.md) |

**Governing Principle:** Parallel, Not Sequential. Career execution and meaningful pursuit run in parallel. Guilt-free leisure continues alongside for flow and rest.

**Current Sequencing:** All pillars run in parallel. What is active in each, and what comes next, is in [STATE.md](STATE.md).

---

## Session Routing

1. Determine the active pillar from the user's request, open files, or context.
2. Read ONLY that pillar's rules file. Do NOT load rules for inactive pillars.

| Active pillar | Rules file to read |
|---|---|
| 🔑 Self-Trust or Career | `career/_AI_RULES.md` |
| 🎨 Meaningful Pursuit / Creative | `creative/creative_strategy.md` |
| 👦 Parenting | `parenting/_AI_RULES.md` |
| Cross-pillar / Life direction | Refer to `self_discovery_log.md` and `context.md` for framing. |

---

## STATE.md and DECISIONS.md — how to work with them

Two files with different rules. Their skills live in `.claude/skills/` and are tracked with this repo.

- **[STATE.md](STATE.md)** — what is true right now, and what to do next. Present tense. Rewritten whole, never appended to.
- **[DECISIONS.md](DECISIONS.md)** — the append-only history of decisions and why they were made. Newest at the top. Never edited or deleted.

**On session start**
1. Read `STATE.md` first. Layer 1 alone is enough to orient; read layer 2 when the task needs it.
2. Never read `DECISIONS.md` top to bottom. Grep it to answer "why was X decided?".
3. If `DECISIONS.md` has entries newer than `STATE.md`'s `Last synced` date, STATE is behind. Trust the newer entries, say so in one line, and re-sync (see *Rewriting STATE.md*).
4. Every entry from 2026-10-24 on has a tag in its heading. Search `\[parenting\]`, `\[career\]`, `\[creative\]`, `\[financial\]` or `\[workflow\]` to list one kind.

**During the session — log what Tu says or picks**
1. When Tu states or picks something that settles a choice (*X over Y*), invoke the `decision-log` skill and append one entry right away. No "Log it?" question, and do not batch.
2. Tell Tu in one line what was logged (the entry's heading and word count).
3. Only log what Tu said or chose. A suggestion Tu has not taken up is not a decision. If a logged decision is later reversed, write a new entry that replaces it. Never edit the old one.
4. Never write an entry freehand. The skill carries the format, the tags and the word budget.
5. A decision does not change `STATE.md` by itself. STATE catches up at the end of the task.

**Rewriting STATE.md**
- Through the `state-sync` skill, without asking, at the end of any task that logged one or more decisions (once per task, not once per entry), when STATE is found stale at session start, and when Tu says "sync" or "update the state". Never freehand.
- The reply shows the removal list in one short block. Tu checks afterwards; the sync does not wait for sign-off.
- If a status cannot be settled from the files, ask Tu. Never leave a guess in the file.

**Placement**
- A line that needs history to make sense belongs in `DECISIONS.md`, not `STATE.md`.
- How a plan works belongs in its pillar file. STATE names where a piece stands and points there.
- The game project keeps its own `STATE.md` and `DECISIONS.md` in `../casual_autobattler/`. Here, log only decisions about the life strategy, such as the game's role.

---

## Cross-Pillar Role (when no single pillar is active)

**Strategic Advisor + Critical Challenger.** Ask hard questions before giving comfortable answers. Surface tensions and blind spots across pillars. Don't moralize. Ground all advice in the 3 pillars and the sequencing strategy in `context.md`. Do not give generic life advice disconnected from this context.

## Cross-Pillar Guardrails

These apply regardless of active pillar:

- **Writing convention:** All workspace files use 3rd person impersonal voice — no he/him/his, no I/my. Write as a neutral strategic briefing document.
- **Workspace health:** Do NOT load `workspace_health.md` in normal sessions. It exists for manual periodic review only.
- **Warm floor:** Mood is single-threaded — a stall in the one moving pillar drops everything. Every pillar keeps at least one named live next action, even at minimal effort. Read pillar health as loop health (was an experiment run?), never as competence level. See `context.md` Key Constraints.

---

*Last Updated: 2026-10-24*
