# Senior Developer 2 — Sprint 2

Assignee: Name TBD. Due date: **2026-10-11**. Assessment weight: 20%.

Your focus: Main domain coder: curriculum data, plan state, validation, import/export and admin integration. Mentor Junior Developer 2.

Start with [the assessment brief](../README.md), then work through these tasks in order. Use [CHECKLIST.md](CHECKLIST.md) and [EVIDENCE.md](EVIDENCE.md). Dependencies come from the [backlog](../../02-Project-Backlog/Deliverables/BACKLOG.md); ask the owner for a stable interface before starting dependent work.

### S2-S2-01: Implement plan state

Create usePlan and pure state updates for adding, moving and removing entries; keep curriculum data separate.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 / Technical Director.
### S2-S2-02: Implement export and validated import

Use versioned JSON; reject malformed, duplicate or unknown records before replacing the current plan; confirm replacement.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 / Technical Director.
### S2-S2-03: Add browser saving

Persist student plans locally with a visible saved/error state; coordinate failure handling with TD.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 / Technical Director.
### S2-S2-04: Test state and import boundaries

Check export/reimport equality, cancellation, invalid input and preservation of the old plan on failure; review Junior 2 source records.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 / Technical Director.

## Handoff and support

Keep the task/issue board current; mention what is done, what remains and what is blocked. Send your reviewer the issue link, changed files and checks performed. Junior developers should ask their paired senior after about 20 minutes stuck; authentication, academic interpretation and graph algorithms need senior/TD support.

Before this milestone closes, demonstrate your result and record your own contribution honestly. Code changes use the [Git walkthrough](../../09-Team-Library/GIT-WORKFLOW.md). For no-code work, link the reviewed document, meeting record or executed QA result instead of claiming a software test was run.

- [ ] **PAR-02 — Prototype parity:** Preserve version-1 export/import compatibility and the example/confirmed-reset flow (P04/P14); cross-import a prototype export.
