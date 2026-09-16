# Technical Director — Executable and acceptance package

Assignee: Name TBD. Due date: **2026-12-09**. Assessment weight: 25%.

Your focus: Architecture, infrastructure, complex implementation, integration and technical mentoring. Reserve time for coding and reviews.

Start with [the assessment brief](../README.md), then work through these tasks in order. Use [CHECKLIST.md](CHECKLIST.md) and [EVIDENCE.md](EVIDENCE.md). Dependencies come from the [backlog](../../02-Project-Backlog/Deliverables/BACKLOG.md); ask the owner for a stable interface before starting dependent work.

### EX-TD-01: Create the release from a clean checkout

Use the committed lockfile/runtime and app scripts; record commit, build commands and environment variable names.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### EX-TD-02: Package frontend and backend accurately

Static dist supports the student UI; an admin release also needs a running API, persistent storage and protected configuration. Do not tell users to double-click index.html.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### EX-TD-03: Verify installation and recovery

Have another member follow install steps, restart the service, restore a test backup and smoke-test the deployed path.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.
### EX-TD-04: Keep secrets out of delivery archives

Provide .env.example names only; transfer real admin access via the agreed private channel and test the recipient can use it.

Evidence: link the resulting PR, document, decision or executed test in EVIDENCE.md. Reviewer/support: Senior Developer 1 or 2.

## Handoff and support

Keep the task/issue board current; mention what is done, what remains and what is blocked. Send your reviewer the issue link, changed files and checks performed. Junior developers should ask their paired senior after about 20 minutes stuck; authentication, academic interpretation and graph algorithms need senior/TD support.

Before this milestone closes, demonstrate your result and record your own contribution honestly. Code changes use the [Git walkthrough](../../09-Team-Library/GIT-WORKFLOW.md). For no-code work, link the reviewed document, meeting record or executed QA result instead of claiming a software test was run.
