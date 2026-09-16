# Technical Director — Sprint 4

Assignee: Name TBD. Due date: **2026-11-29**. Assessment weight: 20%.

Your focus: Architecture, infrastructure, complex implementation, integration and technical mentoring. Reserve time for coding and reviews.

Start with [the assessment brief](../README.md), then work through these tasks in order. Use [CHECKLIST.md](CHECKLIST.md) and [EVIDENCE.md](EVIDENCE.md). Dependencies come from the [backlog](../../02-Project-Backlog/Deliverables/BACKLOG.md); ask the owner for a stable interface before starting dependent work.

### S4-TD-01: Build the admin security/backend foundation

Own password hashing, server sessions, server-side authorization, CSRF strategy, validation and persistent storage; review the prototype without copying credentials.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### S4-TD-02: Implement deployment and recovery

Configure environment variables and permitted paths, HTTPS/session settings and backup/restore; prove persistence across a restart.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### S4-TD-03: Integrate curriculum versioning

Expose read data to students and authorized updates to admin; define how existing plans handle renamed/archived courses and revised rules.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### S4-TD-04: Review release risks and mentor

Have a senior review your code. Run unauthorized-write/session tests and help seniors close integration defects.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.

## Handoff and support

Keep the task/issue board current; mention what is done, what remains and what is blocked. Send your reviewer the issue link, changed files and checks performed. Junior developers should ask their paired senior after about 20 minutes stuck; authentication, academic interpretation and graph algorithms need senior/TD support.

Before this milestone closes, demonstrate your result and record your own contribution honestly. Code changes use the [Git walkthrough](../../09-Team-Library/GIT-WORKFLOW.md). For no-code work, link the reviewed document, meeting record or executed QA result instead of claiming a software test was run.

- [ ] **PAR-03 — Prototype parity:** Reproduce activity history and VITE_FRONTEND_ONLY behavior; ensure static preview skips API/admin calls (P22/P24).
