# Template: Review and Assurance Plan

REVIEW made concrete: the indicator set, the assurance map and the improvement backlog on three connected tables. Elements: R1, R2, R3. Prompts: `../03-prompts/R1-monitoring.md`, `../03-prompts/R2-assurance.md`, `../03-prompts/R3-improvement.md`.

## 1. Indicator set (R1)

| Indicator | Type | Item id | Definition and calculation | Source | Frequency | Owner | Threshold | Escalation (who, when) | Status |
|---|---|---|---|---|---|---|---|---|---|
| Requirements mapped to evidenced controls | KCI | OBL register | Mapped rows / total applicable rows | Obligations register | Monthly | GRC lead | Below 95 percent | GC within 5 business days | Active |

Field notes: **Type** is KPI (performance), KRI (risk) or KCI (control). **Threshold** derives from a stated tolerance; a threshold nobody set is a threshold nobody defends. **Escalation** names a role and a clock. Retire indicators that inform no decision.

## 2. Assurance map (R2)

| Area | Rating | Management activity | Oversight activity | Independent assurance | Provider | Depth | Last | Next |
|---|---|---|---|---|---|---|---|---|
| Third party risk | High | Supplier reviews per CTL-030 | Second-line QA sampling | Internal audit engagement | Internal audit | Design and operating effectiveness | 2025-11 | 2026-11 |

Field notes: assurance effort sits where risk sits; the map exposes high-rated areas with no independent line and low-rated areas assured repeatedly. **Depth** states what the conclusion covers: design, operating effectiveness or both. Independence is structural: the provider examines what it neither operates nor designed.

## 3. Improvement backlog (R3)

| Item | Sources merged | Priority | Route (element) | Owner | Due | Closure evidence | Status |
|---|---|---|---|---|---|---|---|
| Automate obligation change alerts | R2 finding 2026-03, two R1 breaches | High | A5 design | H. Choi | 2026-09-30 | Alert log with SLA report over one full quarter | Open |

Field notes: **Closure evidence** is defined at intake, not at closing time; closure is an artifact, not an assertion. Recurrence of a closed item means the closure was cosmetic; flag it and reopen the root cause.

## Guidance

1. The three tables reference each other: indicators surface findings, assurance tests what indicators cannot, the backlog closes what both discover.
2. Report the plan on one page monthly; the cycle is alive when all three tables have moved.
