# Preliminary product backlog — rebuild the current prototype

**Confirmed scope:** reproduce the current bacs-planner. See [FEATURE-PARITY.md](../../00-Project-Control/FEATURE-PARITY.md) for the 24 baseline checks. Six people and September–December 2026 are confirmed. All stories below are Not started in the team rebuild; generated resources/prototype features do not count as completed team work.

Effort bands are preliminary focused team hours, excluding general coordination/learning time. Refine into small tasks before commitment. Must is requested baseline scope; confirm capacity against TEAM-AND-CAPACITY.md. DDP-28–30 are outside-scope parking-lot ideas, not sprint work.

Board: Backlog → Ready → In progress → Review → Done. Ready means understood criteria/dependencies/owner/estimate. Done means criteria demonstrated, reviewed, checked, pushed and accepted.

| ID | Story | Priority | Target | Owner | Dependencies | Effort |
|---|---|---|---|---|---|---|
| DDP-01 | Repository and team setup | Must | S1 | TD | None | 4–6 h |
| DDP-02 | Student application shell | Must | S1 | S1 | 01 | 3–5 h |
| DDP-03 | Scope and source authority | Must | BL | PD | 01 | 2–4 h |
| DDP-04 | Reference curriculum contract and seed data | Must | S2 | S2 | 03 | 4–6 h |
| DDP-05 | Searchable course explorer | Must | S2 | S1 | 02, 04 | 3–5 h |
| DDP-06 | Course details and official links | Must | S2 | S1 | 05 | 2–4 h |
| DDP-07 | Accessible multi-year term planner | Must | S2 | S1 | 04, 06 | 5–8 h |
| DDP-08 | Local saving and recovery | Must | S2 | S2 | 07 | 3–5 h |
| DDP-09 | Versioned JSON export | Must | S2 | S2 | 07 | 2–3 h |
| DDP-10 | Validated plan import | Must | S2 | S2 | 09 | 3–5 h |
| DDP-11 | Student slice review and QA | Must | S2 | PD | 05, 06, 07, 08, 09, 10 | 2–4 h |
| DDP-12 | AND/OR prerequisites and chronology | Must | S3 | S2 | 04, 07 | 5–8 h |
| DDP-13 | Grades and co-requisites | Must | S3 | S2 | 12 | 3–5 h |
| DDP-14 | Checks panel and workload guidance | Must | S3 | S1 | 12, 13 | 2–4 h |
| DDP-15 | Dependency map | Must | S3 | S1 | 12, 06 | 5–8 h |
| DDP-16 | Requirement progress | Must | S3 | S2 | 04, 13 | 4–6 h |
| DDP-17 | Drag/drop with alternative controls | Must | S4 | S1 | 07, 14 | 3–5 h |
| DDP-18 | Admin hosting and API contract | Must | S3 | TD | 03, 04 | 2–4 h |
| DDP-19 | Admin authentication and authorization | Must | S4 | TD | 18 | 6–8 h |
| DDP-20 | Course admin editing | Must | S4 | S1 | 19, 04 | 5–8 h |
| DDP-21 | Degree and rule admin editing | Must | S4 | S2 | 20, 12, 16 | 6–8 h |
| DDP-22 | Preserve and review reference data coverage | Must | S4 | S2 | 03, 04, 16 | 4–8 h |
| DDP-23 | Usability and accessibility review | Must | S4 | S1 | 15, 17 | 3–5 h |
| DDP-24 | Deployment and regression | Must | S4 | TD | 19, 20, 21, 22, 23 | 4–8 h |
| DDP-25 | Presentation and demonstration | Must | PR | PD | 11; update with 24 | 3–5 h |
| DDP-26 | Executable and acceptance package | Must | EX | TD | 24 | 4–6 h |
| DDP-27 | Handover and individual declarations | Must | HO | PD | 26 | 3–5 h |
| DDP-28 | Live timetable availability integration | Stretch | Future | TD | 18; client approval | Discovery first |
| DDP-29 | Transfer/repeat/equivalence audit | Stretch | Future | S2 | 22; client approval | Discovery first |
| DDP-30 | PDF plan export | Could | Future | S1 | 09, 23 | 3–5 h |

PD = Project Director; TD = Technical Director; S1/S2 = seniors; J1/J2 = juniors. BL = backlog; PR = presentation; EX = executable; HO = handover. Dependencies refer to DDP IDs.

## DDP-01 — Repository and team setup

As a contributor I can run the project and submit a reviewed change.

- **Acceptance:** All confirmed members can clone, run and push a branch; one small reviewed PR each; README names runtime and commands.
- **Owner:** TD; **support/review:** All.
- **Target:** S1; **priority:** Must; **effort:** 4–6 h; **dependencies:** None.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-02 — Student application shell

As a student I can identify DDP and navigate its main views.

- **Acceptance:** DDP/Dal branding and existing logo; responsive sidebar/mobile drawer; four views with hash navigation, skip link and help; compare reference keyboard/mobile paths.
- **Owner:** S1; **support/review:** J1.
- **Target:** S1; **priority:** Must; **effort:** 3–5 h; **dependencies:** 01.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-03 — Scope and source authority

As a project team we know which curriculum and users we support.

- **Acceptance:** Client questions logged; BACS intake year and source approver requested; unresolved assumptions visible; scope decisions linked.
- **Owner:** PD; **support/review:** TD, S2, J2.
- **Target:** BL; **priority:** Must; **effort:** 2–4 h; **dependencies:** 01.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-04 — Reference curriculum contract and seed data

As a student I can see course data with source and review status.

- **Acceptance:** Use reference course IDs and curriculum shape (revision, updatedAt, courses, rules, ruleSources, degree); preserve source-year and unknown/reviewed-empty distinctions; no live timetable feed.
- **Owner:** S2; **support/review:** J2, TD.
- **Target:** S2; **priority:** Must; **effort:** 4–6 h; **dependencies:** 03.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-05 — Searchable course explorer

As a student I can find a course by code or title.

- **Acceptance:** Case-insensitive code/title search, category and level filters, hide-planned option, active-course filtering and empty state match the reference.
- **Owner:** S1; **support/review:** J1.
- **Target:** S2; **priority:** Must; **effort:** 3–5 h; **dependencies:** 02, 04.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-06 — Course details and official links

As a student I can inspect requirements and reach official sources.

- **Acceptance:** Details show credits, reviewed rule text/status and source year; calendar/timetable links work; dialog closes with focus restored.
- **Owner:** S1; **support/review:** J1.
- **Target:** S2; **priority:** Must; **effort:** 2–4 h; **dependencies:** 05.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-07 — Accessible multi-year term planner

As a student I can add, move and remove a course without logging in.

- **Acceptance:** Four-year Fall/Winter grid, optional Summer and all-years view; labelled example and confirmed blank reset; add/move/remove and grade controls; move does not duplicate or discard an existing grade; term totals update.
- **Owner:** S1; **support/review:** S2.
- **Target:** S2; **priority:** Must; **effort:** 5–8 h; **dependencies:** 04, 06.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-08 — Local saving and recovery

As a student I can return to my plan in this browser.

- **Acceptance:** Reload restores plan; storage failure shows feedback without losing in-memory edits; invalid stored data handled; browser-only limitation stated.
- **Owner:** S2; **support/review:** TD.
- **Target:** S2; **priority:** Must; **effort:** 3–5 h; **dependencies:** 07.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-09 — Versioned JSON export

As a student I can keep a portable backup.

- **Acceptance:** Export matches reference version:1/isExample/entries courseId-termId-grade format and filename; blank grade is an empty string; reference and rebuilt exports cross-import.
- **Owner:** S2; **support/review:** J2.
- **Target:** S2; **priority:** Must; **effort:** 2–3 h; **dependencies:** 07.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-10 — Validated plan import

As a student I can restore a saved plan safely.

- **Acceptance:** Valid cross-import preserves entries; malformed/over-1MB/unsupported-version/unknown-ID/invalid-grade/duplicate input rejected; cancellation or failure preserves current plan; replacement confirmed.
- **Owner:** S2; **support/review:** TD, J2.
- **Target:** S2; **priority:** Must; **effort:** 3–5 h; **dependencies:** 09.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-11 — Student slice review and QA

As a director I can demonstrate completed student outcomes.

- **Acceptance:** Search→details→add→move→reload→export/import executed on release commit; defects linked; individual work pushed before Oct. 11.
- **Owner:** PD; **support/review:** All.
- **Target:** S2; **priority:** Must; **effort:** 2–4 h; **dependencies:** 05, 06, 07, 08, 09, 10.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-12 — AND/OR prerequisites and chronology

As a student I can identify courses planned before their prerequisites.

- **Acceptance:** All groups required; any alternative can satisfy its group; earlier term required unless concurrent allowed; missing/unknown cases visible; synthetic tests cover branches.
- **Owner:** S2; **support/review:** TD.
- **Target:** S3; **priority:** Must; **effort:** 5–8 h; **dependencies:** 04, 07.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-13 — Grades and co-requisites

As a student I can distinguish pending from earned eligibility.

- **Acceptance:** C and C+ thresholds compared correctly in synthetic tests; blank grade is pending; below minimum blocks; co-requisite allows same term only where reviewed rule permits.
- **Owner:** S2; **support/review:** TD, J2.
- **Target:** S3; **priority:** Must; **effort:** 3–5 h; **dependencies:** 12.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-14 — Checks panel and workload guidance

As a student I can understand what to change in my plan.

- **Acceptance:** Issues identify course/term and reason in text; fix recalculates promptly; workload warning labelled guidance; no unsupported graduation guarantee.
- **Owner:** S1; **support/review:** J1, S2.
- **Target:** S3; **priority:** Must; **effort:** 2–4 h; **dependencies:** 12, 13.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-15 — Dependency map

As a student I can explore ancestors and dependent courses.

- **Acceptance:** Selected course highlights reachable prerequisites/dependents; traversal terminates on cycles; unknown rules visible; keyboard course buttons and text list available.
- **Owner:** S1; **support/review:** TD, J1.
- **Target:** S3; **priority:** Must; **effort:** 5–8 h; **dependencies:** 12, 06.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-16 — Requirement progress

As a student I can distinguish planned coverage from earned credit.

- **Acceptance:** Match reference planned category/option progress, earned-credit summary and elective guidance; preserve warnings that counts do not establish graduation eligibility; no new full elective audit.
- **Owner:** S2; **support/review:** J2.
- **Target:** S3; **priority:** Must; **effort:** 4–6 h; **dependencies:** 04, 13.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-17 — Drag/drop with alternative controls

As a student I can quickly rearrange courses.

- **Acceptance:** Drop adds/moves only a valid course to a valid term; credits/checks update; labelled add/move controls remain usable by keyboard/touch.
- **Owner:** S1; **support/review:** J1.
- **Target:** S4; **priority:** Must; **effort:** 3–5 h; **dependencies:** 07, 14.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-18 — Admin hosting and API contract

As a maintainer I know how admin changes persist.

- **Acceptance:** FCS runtime/storage/HTTPS confirmed or blocker recorded; API/schema/error/version contract and hosting ADR reviewed; no assumption that static hosting runs a server.
- **Owner:** TD; **support/review:** S2.
- **Target:** S3; **priority:** Must; **effort:** 2–4 h; **dependencies:** 03, 04.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-19 — Admin authentication and authorization

As an authorized admin I can access editing tools.

- **Acceptance:** Server verifies credentials with appropriate password hashing and protected sessions; unauthorized writes denied; session/logout and CSRF controls tested; credentials excluded from frontend/repo.
- **Owner:** TD; **support/review:** S2 review.
- **Target:** S4; **priority:** Must; **effort:** 6–8 h; **dependencies:** 18.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-20 — Course admin editing

As an admin I can add, edit and archive a course.

- **Acceptance:** All reference course fields, fixed code on edit, search and active/archived/all filters supported; create/edit/archive/restore validated server-side; save persists across restart; shared curriculum, stale-edit protection and activity history match.
- **Owner:** S1; **support/review:** TD, S2.
- **Target:** S4; **priority:** Must; **effort:** 5–8 h; **dependencies:** 19, 04.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-21 — Degree and rule admin editing

As an admin I can maintain approved requirements.

- **Acceptance:** Match reference reviewed/unknown rule toggle, AND/OR groups, grade/timing/source fields and degree/group/elective editing; revision conflicts visible; invalid totals/fields denied; saves appear in activity history.
- **Owner:** S2; **support/review:** TD, S1.
- **Target:** S4; **priority:** Must; **effort:** 6–8 h; **dependencies:** 20, 12, 16.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-22 — Preserve and review reference data coverage

As a student I know which rules have been verified.

- **Acceptance:** Preserve existing catalogue and clearly labelled review gaps; verify sources for changed records; document coverage; no new transfer/elective audit or invented C+ rule.
- **Owner:** S2; **support/review:** J2, PD.
- **Target:** S4; **priority:** Must; **effort:** 4–8 h; **dependencies:** 03, 04, 16.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-23 — Usability and accessibility review

As a student I can use the main flows on a narrow screen and keyboard.

- **Acceptance:** Agreed student tasks observed; focus/dialog/labels/status messages checked; issues prioritized and fixed or documented; feedback identifies build used.
- **Owner:** S1; **support/review:** J1, PD.
- **Target:** S4; **priority:** Must; **effort:** 3–5 h; **dependencies:** 15, 17.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-24 — Deployment and regression

As a stakeholder I can use a stable release candidate.

- **Acceptance:** Clean build/applicable tests; actual host-path smoke check; student fallback when API unavailable; VITE_FRONTEND_ONLY=true static build has bundled data and disabled admin; full backend restart/persistence/restore tested when available; parity results recorded.
- **Owner:** TD; **support/review:** S1, S2, J2.
- **Target:** S4; **priority:** Must; **effort:** 4–8 h; **dependencies:** 19, 20, 21, 22, 23.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-25 — Presentation and demonstration

As a stakeholder I can understand delivered results.

- **Acceptance:** Date/rubric confirmed; timed rehearsal completed; demo matches release and has fallback; every member contribution represented truthfully.
- **Owner:** PD; **support/review:** All.
- **Target:** PR; **priority:** Must; **effort:** 3–5 h; **dependencies:** 11; update with 24.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-26 — Executable and acceptance package

As a non-technical stakeholder I can open and test the product.

- **Acceptance:** Release/tag, start guide, acceptance steps and known issues supplied; another person follows install; actual acceptance outcomes recorded; package submitted Dec. 9.
- **Owner:** TD; **support/review:** PD, All.
- **Target:** EX; **priority:** Must; **effort:** 4–6 h; **dependencies:** 24.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-27 — Handover and individual declarations

As a client I receive materials and maintenance knowledge.

- **Acceptance:** Six reviewed declarations, repo/release/docs/access inventory, walkthrough and acknowledgement recorded; open work assigned; exact deadline confirmed.
- **Owner:** PD; **support/review:** All.
- **Target:** HO; **priority:** Must; **effort:** 3–5 h; **dependencies:** 26.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-28 — Live timetable availability integration

As a student I can see synchronized offerings if a supported source exists.

- **Acceptance:** Supported source/permission and refresh semantics agreed; stale/error states visible; term coverage tested; no scraping assumption.
- **Owner:** TD; **support/review:** S2.
- **Target:** Future; **priority:** Stretch; **effort:** Discovery first; **dependencies:** 18; client approval.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-29 — Transfer/repeat/equivalence audit

As a student I can model more complex academic cases.

- **Acceptance:** Advisor-approved semantics and fixtures precede implementation; repeated attempts and equivalents avoid double credit; exclusions reported.
- **Owner:** S2; **support/review:** TD.
- **Target:** Future; **priority:** Stretch; **effort:** Discovery first; **dependencies:** 22; client approval.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.

## DDP-30 — PDF plan export

As a student I can share a readable plan document.

- **Acceptance:** Printable plan includes terms/credits/check limitations and source version; long labels remain readable; JSON backup still supported.
- **Owner:** S1; **support/review:** J1.
- **Target:** Future; **priority:** Could; **effort:** 3–5 h; **dependencies:** 09, 23.
- **Status:** Not started. **Issue/PR:** TBD. **Actual outcome and acceptance date:** TBD.
