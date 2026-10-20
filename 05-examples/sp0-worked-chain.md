# Worked Example: the SP0 Chain, Prompt by Prompt

**Fictional and illustrative.** Ganada Trading Co. is an invented company; every name, figure, date, scale and document below is invented for this example. Nothing here describes a real organization or a real run. The outputs are written by hand to show what each prompt's schema asks for after human review; they are not model output and not a logged test run. The run record is in [`../tests.md`](../tests.md).

**grc v2.3.4 · 20 October 2026 (KST)**

## What this example is for

`../03-prompts/usage.md` section 6 gives the SP0 chain as L2 → L1 → A2 → A3 → A4 → A5 → P2/P1 → R1 and says to feed reviewed outputs, not raw ones, from each prompt into the next. This file walks that chain once, from the inputs a reader would paste to the reviewed output that goes forward, and lands on the sample rows the six templates already carry: OBJ-001 (objectives register), RSK-014 and OPP-003 (risk register), OBL-021 (obligations register), CTL-052 (control matrix) and POL-007 (policy template). It is also the fixture for the pack's tests: the blocks marked "fixture" are pasted verbatim as the inputs of the test cases in `../tests.md`.

Each step shows three things: the inputs supplied, the output in the prompt's lettered schema (abridged where marked) and what the human reviewer changed at the gate before the output moved on. Every output ends with the gate line `DRAFT FOR HUMAN REVIEW. Decision authority and final liability rest with the accountable human owner.`; it is shown once, at step 1; later steps omit it.

## The fictional organization

Ganada Trading Co. imports and distributes industrial consumables in Korea. About 240 staff in four units (Finance, Sales, Procurement, Operations). Its order-to-cash process holds customer contact and payment data for Korean business customers and their staff. Starting point: SP0, Blank Canvas; no formal governance, risk management and compliance capability exists. The risk register already holds RSK-001 to RSK-013 and OPP-001 to OPP-002 from an earlier informal exercise, which is why the new items below are numbered RSK-014 and OPP-003.

## Step 1. L2 Internal Context

**Inputs supplied (abridged).** 1. Organization chart: CEO; CFO (S. Kim); Finance lead (J. Park); Procurement lead (D. Lee); Operations lead; IT and data protection officer (H. Choi). 2. Inventory: order-to-cash process on one ERP; 12 key suppliers supplying the top 20 stock lines; customer contact and payment data in the ERP. 3. Strategy summary: improve working capital (enterprise objective OBJ-E02). 4. Constraints: no new headcount in FY2026; GRC budget limited to existing staff time.

**Output (abridged).**

A. Internal context brief: Ganada runs one ERP-centered order-to-cash process; fulfillment depends on 12 key suppliers; personal data of customer staff sits in the same ERP.

B. Capability and asset inventory table:

| Item | Type (process, system, data, third party) | Owner if known | Relevance |
|---|---|---|---|
| Order-to-cash | process | J. Park | Drives OBJ-E02 |
| ERP | system | H. Choi | Holds orders, invoices and customer contact data |
| Customer contact and payment data | data | H. Choi | Personal data of Korean residents |
| 12 key suppliers | third party | D. Lee | Fulfillment of the top 20 stock lines |

C. Enablers and constraints table: one row, "No new headcount | constraint | GRC capability | Input 4".

D. Inventory gaps: no supplier criticality ranking (source: Procurement); no record of personal data flows (source: H. Choi).

E. Change triggers: a new ERP module; a change to the key supplier list.

F. Open questions: who owns the supplier list?

DRAFT FOR HUMAN REVIEW. Decision authority and final liability rest with the accountable human owner.

**At the gate.** S. Kim confirms the inventory and assigns supplier list ownership to D. Lee.

## Step 2. L1 External Context

**Inputs supplied (abridged).** 1. Profile: industrial consumables, Korea only, business customers, direct sales. 2. Scope: legal and regulatory, economic; horizon 12 months. 3. Objectives: OBJ-E02 improve working capital. 4. Watchlist: none. 5. FOUR-FRAMES reading: not used.

**Output (abridged).**

B. Force table:

| Force | Domain | Relevance to which objective | Trend | Re-assessment trigger |
|---|---|---|---|---|
| Sector credit tightening among mid-size manufacturers | economic | OBJ-E02, through supplier failure | rising | A key supplier misses a payment to its own creditors |
| New customs pre-clearance channel for registered importers | legal and regulatory | OBJ-E02, through faster inbound clearance | new | Channel registration opens for Ganada's goods class |

C. Candidate authority sources:

| Source | Type | Jurisdiction | Applicability question to resolve |
|---|---|---|---|
| Data protection statute | Statute | KR | Does Ganada act as controller for customer staff data in the ERP, and which breaches must it notify? |

D. Watchlist update: add both forces and the statute. E. Open questions: none.

**At the gate.** H. Choi confirms the statute question for build guide C; the citation stays "(verify)" until checked against the source.

## Step 3. A2 Objectives

**Inputs supplied (fixture `A2`).**

<!-- fixture:A2:start -->
```text
1. Strategy material (FY2026 plan, extract): "Our enterprise objective OBJ-E02
   is to improve working capital. In Finance this means getting paid faster:
   we will bring the order-to-cash cycle down to 30 days on a monthly average
   during FY2026, and Finance will escalate if the monthly average runs more
   than 5 days over that. J. Park, Finance lead, runs order-to-cash."
2. Direction statement and appetite summary from A1: low appetite for failures
   that stop customer fulfillment; moderate appetite for process changes that
   need no new budget.
3. Unit list for cascading: Finance, Sales, Procurement, Operations. Cascade
   only to Finance for this exercise.
4. Existing objectives register: one enterprise row, OBJ-E02 "Improve working
   capital", owner S. Kim (CFO), no unit rows. Number new unit objectives from
   OBJ-001.
```
<!-- fixture:A2:end -->

**Output (reviewed).**

A. Objectives register rows:

| OBJ-id | Objective | Owner | Unit | Parent OBJ | Measure | Target | Tolerance | Time frame | Linked RSK/OPP | Linked OBL | Review cadence | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| OBJ-001 | Reduce order-to-cash cycle to 30 days | J. Park (candidate) | Finance | OBJ-E02 | Days, monthly average | 30 | +5 days before escalation | FY2026 | pending A3 | pending A3 | Quarterly | Proposed |

B. Unmeasurable as stated: none. C. Coverage note: the one row is a growth objective; the register has no preservation objective for Finance yet. D. Open questions: is the 30-day target measured from invoice date or delivery date?

**At the gate.** J. Park confirms ownership and the measure (from invoice date). The row becomes Active with Owner "J. Park". The linked columns are filled after step 4, which gives the template's sample row: `| OBJ-001 | Reduce order-to-cash cycle to 30 days | J. Park | Finance | OBJ-E02 | Days, monthly average | 30 | +5 days before escalation | FY2026 | RSK-014, OPP-003 | OBL-021 | Quarterly | Active |`.

## Step 4. A3 Identification

**Inputs supplied (abridged).** 1. The reviewed OBJ-001 row. 2. The L2 and L1 outputs above. 3. The existing register (RSK-001 to RSK-013, OPP-001 to OPP-002; none on suppliers or customs). 4. Scope: OBJ-001.

**Output (abridged).**

A. Identified items table:

| Temp-id | Type (opportunity, obstacle, obligation) | Statement | Linked OBJ-id | Source in inputs |
|---|---|---|---|---|
| T1 | obstacle | Key supplier insolvency, caused by sector credit tightening, resulting in fulfillment failure on OBJ-001 | OBJ-001 | L1 force 1; L2 inventory row 4 |
| T2 | opportunity | Early adoption of the new customs pre-clearance channel, enabling 4-day cycle reduction on OBJ-001 | OBJ-001 | L1 force 2 |
| T3 | obligation | Notify the authority of qualifying breaches of customer staff data held in the order-to-cash ERP within the statutory window | OBJ-001 | L1 source 1; L2 inventory row 3 |

B. Obligations routing list: T3, data protection statute, KR. C. De-duplication: none. D. Coverage note: OBJ-001 has three items. E. Open questions: is the 4-day reduction in T2 measured or estimated?

**At the gate.** T1 becomes RSK-014 (category Third party) and T2 becomes OPP-003 (category Regulatory). T3 goes to build guide C, where it is decomposed into OBL-021 with owner H. Choi; the obligations register's sample row is that entry.

## Step 5. A4 Assessment

**Inputs supplied (fixture `A4`).**

<!-- fixture:A4:start -->
```text
1. Items to assess (reviewed A3 output):
   | Id | Type | Statement | Linked OBJ | Category |
   | RSK-014 | Obstacle | Key supplier insolvency, caused by sector credit tightening, resulting in fulfillment failure on OBJ-001 | OBJ-001 | Third party |
   | OPP-003 | Opportunity | Early adoption of the new customs pre-clearance channel, enabling 4-day cycle reduction on OBJ-001 | OBJ-001 | Regulatory |
   Evidence: two of the 12 key suppliers reported losses in their last two
   filings; sector lenders have tightened terms this year (L1 force 1). The
   customs channel has opened for Ganada's goods class; the 4-day reduction
   is the customs authority's published estimate for registered importers.
2. Calibrated scales (verbatim):
   Likelihood within 12 months: 1 Rare (under 5%); 2 Unlikely (5% to under
   20%); 3 Possible (20% to under 50%); 4 Likely (50% to under 80%);
   5 Almost certain (80% or more).
   Impact on the OBJ-001 measure (adverse for obstacles, favorable for
   opportunities): 1 Minimal (under 1 day); 2 Minor (1 to under 3 days);
   3 Moderate (3 to under 5 days); 4 Major (5 to under 10 days, or one key
   customer lost); 5 Severe (10 days or more, or fulfillment stopped for more
   than a week).
   Velocity: High (impact within one week of the event); Medium (within one
   month); Low (later than one month).
   Rating rule, on residual scores: High where Residual I is 4 or 5 and
   Residual L is 2 or more; otherwise Medium where Residual L times Residual I
   is 6 to 12; otherwise Low.
3. Appetite and tolerance statements:
   Third party: a residual rating of High on any supplier risk to a
   customer-facing objective is above appetite; Medium is at appetite; Low is
   within appetite.
   Regulatory opportunities: an opportunity rated Medium or Low that needs no
   new budget is within appetite for pursuit.
4. Existing controls:
   RSK-014: CTL-030, quarterly financial health review of the 12 key
   suppliers by Procurement (two of 12 reviews missed last quarter);
   CTL-031, approved alternate supplier list for the top 20 stock lines,
   refreshed semiannually (covers 14 of 20 lines). Effectiveness evidence:
   second-line review graded the pair "Partially effective" in May 2026.
   Supplier failure would stop fulfillment of the affected lines within days.
   OPP-003: no controls exist.
```
<!-- fixture:A4:end -->

**Output (reviewed).**

A. Assessment rows:

| Id | Type | Statement | Linked OBJ | Category | Inherent L | Inherent I | Velocity | Existing CTLs | Control effectiveness | Residual L | Residual I | Rating | Appetite position |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| RSK-014 | Obstacle | Key supplier insolvency, caused by sector credit tightening, resulting in fulfillment failure on OBJ-001 | OBJ-001 | Third party | 3 | 4 | High | CTL-030, CTL-031 | Partially effective | 2 | 4 | High | Above |
| OPP-003 | Opportunity | Early adoption of the new customs pre-clearance channel, enabling 4-day cycle reduction on OBJ-001 | OBJ-001 | Regulatory | 3 | 3 | Medium | n/a | n/a | 3 | 3 | Medium | Within |

B. Evidence notes (abridged): RSK-014 Inherent L 3, "two of the 12 key suppliers reported losses"; Residual L 2, CTL-030 and CTL-031 graded Partially effective; OPP-003 Inherent I 3, the published 4-day estimate falls in "3 to under 5 days".

C. Treatment decision queue:

| Id | Appetite position | Decision required | Owner candidate |
|---|---|---|---|
| RSK-014 | Above | Reduce, avoid, transfer or accept | S. Kim |
| OPP-003 | Within | Pursue, enhance, share or decline | J. Park |

D. CALIBRATE list: RSK-014 Velocity High rests on the statement that failure would stop fulfillment "within days", not on a measured lead time. E. Scale application issues: none. F. Open questions: may the second-line grade cover two controls jointly?

**At the gate.** S. Kim decides Reduce for RSK-014 on 2026-06-15 and names D. Lee action owner, due 2026-09-30; she decides Pursue for OPP-003 the same day with J. Park as action owner, due 2026-08-31. Those are the human columns of the risk register's sample rows. One wording difference remains: the template's sample row for OPP-003 reads "Pursuit within appetite" where the template's own field definition 5 and the A4 prompt allow Above, At or Within; this example uses "Within" and `../tests.md` records the difference.

## Step 6. A5 Design

**Inputs supplied (abridged).** 1. The step 5 queue with decisions. 2. The L2 extract. 3. Control matrix extract: CTL-030, CTL-031. 4. Envelope: existing staff time only.

**Output (abridged).**

A. Treatment design table:

| Item id | OBJ-id | Action or control statement | Type | Nature | Frequency | Operator candidate | Evidence produced | Test method | Reused CTL-id or NEW |
|---|---|---|---|---|---|---|---|---|---|
| RSK-014 | OBJ-001 | Every one of the 12 key suppliers receives a financial health review each quarter, signed by the reviewer | Detective | Manual | Quarterly | Procurement analyst | Signed review per supplier per quarter | Second line checks 12 of 12 signatures each quarter | CTL-030 |
| RSK-014 | OBJ-001 | The alternate supplier list covers all top 20 stock lines | Proactive | Manual | Semiannual | D. Lee | Dated list with a named alternate per line | Second line samples 5 lines | CTL-031 |
| RSK-014 | OBJ-001 | On a supplier failure signal, open orders for the affected lines move to the listed alternate within 2 business days | Responsive | Hybrid | Per event | D. Lee | Switch log with timestamps | Tabletop once a year | NEW |
| OPP-003 | OBJ-001 | Register for the customs pre-clearance channel and route eligible inbound lots through it | Proactive | Manual | Once, then per lot | Operations lead | Registration record; lot clearance times | Compare cycle days before and after | NEW |

B. Mix warnings: before the NEW responsive line, RSK-014 had prevention and detection only; the third line closes it. C. Roadmap, D. resource notes and E. open questions are omitted here.

**At the gate.** S. Kim approves; the two NEW lines enter the control matrix as Designed.

## Step 7. P2 Policies and P1 Controls

**P2 inputs supplied (abridged).** 1. Mandate: OBL-021, notify the authority of qualifying breaches within the statutory window. 2. Scope: all Korean entities and all staff handling customer data. 3. Related controls: CTL-052 (and CTL-053, listed in the OBL-021 row). 4. No existing policy; repository template structure.

**P2 output (abridged).** A. Policy draft: POL-007, Personal Data Breach Notification, status Draft, Linked OBL-ids OBL-021, Linked CTL-ids CTL-052 and CTL-053; statement 4.1, every suspected breach is reported to the incident manager on duty the same day; 4.2, breach severity is assessed against the notification rubric within 24 hours of confirmation; 4.3, qualifying breaches are notified to the authority within the statutory window by H. Choi. B. Traceability table:

| Statement number | OBL-id, RSK-id or decision | Related CTL-ids |
|---|---|---|
| 4.1 | OBL-021 | CTL-053 |
| 4.2 | OBL-021 | CTL-052 |
| 4.3 | OBL-021 | CTL-053 |

C. Untraceable statements: none.

**P1 inputs supplied (abridged).** 1. Control matrix extract: CTL-052 as in the template's sample row. 2. Linked items: RSK-014, OBL-021, POL-007. 3. Operating context: incident manager on duty, ERP incident log. 4. History: no incidents in scope.

**P1 output (abridged).** B. Test table: | CTL-052 | Re-perform the rubric on a sample of incidents | Severity matches and timestamp within 24 hours | Second line |. C. Gap check:

| Direction | Id | Description | Suggested action |
|---|---|---|---|
| Control lacking a fitting item | CTL-052 | Linked to RSK-014 (supplier insolvency), but its statement addresses breach severity; the item it serves is OBL-021 | Remove the RSK-014 link, or identify a breach risk under A3 and link that |
| Item lacking a control | OBL-021 | Lists CTL-053, which the control matrix does not hold | Design CTL-053 under A5 or remove it from the row |

**At the gate.** This is the gate doing its work: the two template sample rows were written to cross-reference by identifier, and P1's two-way check shows that one link carries no reason. The reviewer's decision is the owner's, not the example's; the template's sample row is left as published and the finding is recorded in `../tests.md`.

## Step 8. R1 Monitoring

**Inputs supplied (abridged).** 1. OBJ-001 with its tolerance; RSK-014 rated High; CTL-052. 2. Sources: ERP monthly report; Procurement review log; incident log. 3. Tolerance: +5 days on OBJ-001; no tolerance stated for the review log or the rubric. 4. No current indicators.

**Output (abridged).**

A. Indicator table:

| Indicator | Type | Item id | Definition and calculation | Source | Frequency | Owner candidate | Threshold | Escalation (who, when) |
|---|---|---|---|---|---|---|---|---|
| Order-to-cash cycle | KPI | OBJ-001 | Average days from invoice to cash, monthly | ERP monthly report | Monthly | J. Park | Above 35 days | S. Kim within 5 business days |
| Key supplier reviews completed | KRI | RSK-014 | Signed reviews / 12, quarterly | Procurement review log | Quarterly | D. Lee | CALIBRATE | S. Kim at quarter end |
| Rubric within 24 hours | KCI | CTL-052 | Incidents with rubric inside 24 hours / incidents | Incident log | Monthly | H. Choi | CALIBRATE | General counsel within 2 business days |

B. CALIBRATE list: the two thresholds without a stated tolerance. C. Anti-gaming: the cycle measure rewards writing off slow invoices; pair it with a write-off count.

**At the gate.** J. Park sets the KRI threshold at "below 12 of 12" and H. Choi the KCI threshold at "below 100 percent"; the indicator set enters `../04-templates/review-assurance-plan.md`.

## What the chain shows

1. Every artifact traces to OBJ-001, which is SP0's day-90 test in `../01-method/starting-points.md`.
2. The A2 and A4 outputs land in their templates column for column, since grc v2.3.0 aligned the two schemas; A5, P1 and R1 outputs still need light mapping into the control matrix and the review and assurance plan (recorded in `../tests.md`).
3. The gate moved something at every step; at step 7 it caught a link the templates had carried unexamined.

---

**Final Liability rests with the Human.**
