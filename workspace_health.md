# Workspace Health — Split Signals

> **Purpose:** Monitor this file periodically to decide when the single-workspace approach is breaking down and a pillar should be split into its own workspace.
>
> **Review trigger:** Check this when a session feels unfocused, AI seems distracted, or a pillar directory feels crowded.
>
> **This file is NOT loaded in normal sessions.** Open and read manually when monitoring.

---

## Decision Rule

When **2 or more signals** fire for the same pillar → seriously consider splitting that pillar into its own workspace. When **3 or more** → split is overdue.

---

## Signals to Monitor

| # | Signal | How to detect |
|---|---|---|
| 1 | **File count in a pillar directory exceeds ~30** | Run `list_dir` on the pillar directory and count |
| 2 | **AI reads files from the wrong pillar during a session** | Notice AI referencing career docs during creative sessions or vice versa |
| 3 | **AI misidentifies the active pillar or loads wrong `_AI_RULES.md`** | First response in a session has the wrong role/tone |
| 4 | **Session context feels crowded or unfocused** | Subjective: "AI seems distracted" or responses feel generic despite clear context |
| 5 | **`_AI_RULES.md` for one pillar grows significantly larger than others** | That pillar's AI rules have become complex enough to warrant their own workspace identity |

---

## Current Baseline

*Last measured: 2026-06-11*

| Pillar | File count | Signal 1 | Signal 2 | Signal 3 | Signal 4 | Signal 5 |
|---|---|---|---|---|---|---|
| 🔑 Pillar 1 — Career/Self-Trust | ~13 | ⬜ | ⬜ | ⬜ | ⬜ | ⬜ |
| 🎮 Pillar 2 — Enjoyment | 1 | ⬜ | ⬜ | ⬜ | ⬜ | ⬜ |
| 👦 Pillar 3 — Parenting | ~16 | ⬜ | ⬜ | ⬜ | ⬜ | ⬜ |

*(Update this table when you review. Mark 🟡 for emerging, 🔴 for firing.)*

---

## Split Execution

If a split is triggered, refer to the hub+spoke plan archived in the conversation history (2026-05-23/24) or rebuild it from scratch — the approach is well understood.

---

*Created: 2026-05-24*
*Last Updated: 2026-06-11*
