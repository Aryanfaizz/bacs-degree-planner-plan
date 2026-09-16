# Presentation outline and demo script

Date, duration, slide limit and submission format: TBD with instructor. The sequence below is a proposal; scale timing once the allotted duration is known.

| Slide | Content | Suggested speaker |
|---|---|---|
| 1 | DDP, client, team and student planning problem | PD |
| 2 | Confirmed scope and user needs | PD |
| 3 | Architecture and why student plans need no login | TD |
| 4 | Search → details → term plan → dependency map | S1 |
| 5 | Rules, grade thresholds, pending/unknown states and export | S2 |
| 6 | UI accessibility contribution and what was learned | J1 |
| 7 | Source review and acceptance evidence | J2 |
| 8 | Admin workflow, deployment status and known limits | TD |
| 9 | Delivered outcomes, remaining backlog and handover | PD |

## Demo sequence

1. Open the exact release build and start with a labelled synthetic plan.
2. Search/open a course and show its source/timetable link.
3. Place a dependent course too early; explain the resulting warning.
4. Move its prerequisite earlier. Show pending when the grade is unknown, then enter a sufficient synthetic grade.
5. Inspect the dependency map and its text alternative.
6. Export and reimport the plan; show the result is preserved.
7. If admin is implemented, log in using a dedicated test account, change a synthetic course and show validation/persistence. If unfinished, state that clearly.

Reset steps, build commit, sample-plan location and backup recording: TBD before rehearsal. Do not expose real credentials in slides/video. Test the local student fallback before presenting. Log timings and rehearsal defects in the package record.
