# Agreed build target — match the current bacs-planner

User confirmation: September 16, 2026. Team: six members, September–December 2026. **Rebuild the existing bacs-planner as it is now.** The original project remains unchanged. This is a feature/design baseline, not a request for a larger degree-audit platform.

The source snapshot and SHA-256 manifest in `09-Team-Library/prototype-reference/` freeze what “as of now” means. Compare the new app side by side with this reference. Source inspection established the inventory below; runtime parity still needs demonstration during the team build. Prototype screenshots may predate the current branding: the snapshot's source and running UI are the reference when screenshots differ.

| ID | Existing behavior to reproduce | Story / owner | Target | Verification |
|---|---|---|---|---|
| P01 | DDP naming, Dal black/gold theme and existing logo; desktop sidebar/mobile drawer | 02 / S1 + J1 | S1–S2 | Compare reference at desktop and narrow widths |
| P02 | Four main views: plan, curriculum map, course explorer, degree requirements; hash navigation, help, skip link | 02, 06 / S1 | S2 | Open each view; keyboard navigation and refresh |
| P03 | Four academic years, individual/all-years view, optional Summer terms | 07 / S1 | S2 | Switch years/all-years/Summer and preserve entries |
| P04 | Labelled initial example plan; confirm Start blank/reset | 07, 08 / S2 | S2 | First visit, cancel reset, confirm reset |
| P05 | Search code/title, level/category filters, hide planned courses and empty state | 05 / S1 + J1 | S2 | Combine filters and clear them |
| P06 | Course dialog: details, credits, grade, source year and official calendar/timetable links | 06 / S1 | S2 | Compare fields and link destinations |
| P07 | Add/move/remove via dialog; grade entry; course-grip drag/drop | 07, 13, 17 / S1 + S2 | S2–S4 | Move without duplication; grade preserved |
| P08 | Term credit counts, planned/earned summaries and workload warnings | 14, 16 / S2 | S3 | Compare same example plan totals |
| P09 | Earlier-term prerequisites; AND groups/OR alternatives; allowed co-requisites; minimum grades | 12, 13 / S2 + TD | S3 | Valid/invalid/pending synthetic scenarios |
| P10 | Unknown/unreviewed rule status and archived course warnings | 04, 14 / S2 | S3 | Missing rule differs from explicitly empty rule |
| P11 | Dependency map with selected ancestors/descendants and course details access | 15 / S1 + TD | S3 | Compare reachable course highlights |
| P12 | Required-group progress, option guidance, elective guidance and explicit audit limits | 16 / S2 | S3 | Match reference display; no new full elective audit |
| P13 | Browser-local plan saving, saved/error status and recovery messaging | 08 / S2 + TD | S2 | Reload and simulated unavailable storage |
| P14 | JSON export/import, version-1 format, confirmation, invalid/oversized-file protection | 09, 10 / S2 | S2 | Import a reference export and vice versa |
| P15 | Student access without login; plans stay local | 07, 08 / S2 | S2 | Fresh browser needs no student account |
| P16 | Admin sign-in/session/logout, busy/error states and return to planner | 19 / TD + S1 | S4 | Valid login, denied login, logout and direct unauthorized write |
| P17 | Admin course search; active/archived/all filter; create/edit/archive/restore | 20 / S1 + TD | S4 | Update persists and old plan displays archived record |
| P18 | Course fields: fixed code on edit, title, category, level, credits, minimum grade, description, official URL and required/active flags | 20 / S1 + TD | S4 | Compare every field to AdminCourseEditor |
| P19 | Reviewed/unknown toggle; prerequisite groups, alternatives, minimum grade, timing and source text | 21 / S2 + TD | S4 | Compare form and server validation |
| P20 | Degree name/credits/usual term credits/grade guidance; required-group targets and descriptions; elective guidance/counts | 21 / S2 + S1 | S4 | Save valid values; reject invalid totals |
| P21 | Curriculum revision conflict warning/reload and shared student updates | 20, 21 / S2 + TD | S4 | Two stale editors; conflict does not overwrite newer data |
| P22 | Admin activity history | 20, 21 / TD + S1 | S4 | Course/degree edits appear with user/time/action |
| P23 | Bundled curriculum fallback and offline notice when API unavailable | 04, 24 / S2 + TD | S4 | Disconnect API; reference student fallback is reproduced |
| P24 | Frontend-only mode: bundled data, no admin entry; direct admin view explains backend requirement | 24 / TD | S4 | Build VITE_FRONTEND_ONLY=true and smoke-test without API |

## Scope boundary

Reproduce the prototype's student and admin behavior, architecture style and visual identity. Preserve known data-review limitations. Source review, readable UTF-8 copy, tests and documentation support this rebuild; they do not authorize feature expansion. Full elective/transfer/repeat/equivalence audits, live timetable data, student accounts and PDF plan export are outside this baseline. Stories DDP-28–30 are parking-lot ideas only and consume no committed sprint capacity.

The prototype has an Express/SQLite admin implementation. Static preview comes first; final FCS hosting still depends on confirmed server capabilities. If hosted admin cannot be delivered, PD records an explicit client/instructor decision; do not claim the static preview is full parity.

## Compatibility contract

Plan export uses `{ version: 1, isExample: boolean, entries: [{ courseId, termId, grade }] }`; blank grade is `''`. Curriculum uses `revision`, `updatedAt`, `courses`, `rules`, `ruleSources`, `degree`. Reuse stable IDs from the reference. Do not introduce a new incompatible schema solely because an example uses different fields. Any deliberate migration requires a separate reviewed decision.

## Final parity sign-off

For each row record reference behavior, rebuilt result, screenshot/test/commit, reviewer and date in PARITY-RESULTS.csv. Begin with Not run. Known prototype bugs should be logged and fixed deliberately; do not reproduce defects simply to claim exactness.
