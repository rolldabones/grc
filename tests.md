# grc prompt pack: tests

**Cases, known defects and the run record for the 21 prompts in [`03-prompts/`](03-prompts/) · v2.3.0 · 18 October 2026 (KST)**

`03-prompts/usage.md` section 7 says to re-test after model changes. This file is what that re-test runs against. The fixture is the worked SP0 chain, [`05-examples/sp0-worked-chain.md`](05-examples/sp0-worked-chain.md): its blocks marked "fixture" are pasted verbatim as each case's input, after the opening line "Here are the required inputs." A run passes when every case it exercises passes; a case not exercised in a run is recorded as not run, never as passed.

**How a case is run.** Following `usage.md` section 1 ("If your model supports system prompts, place the ROLE block there; otherwise paste the prompt whole"), the prompt for the step, the fenced text block under "## Prompt" in its file, is loaded whole and byte for byte as the system prompt, and the user turn is the line "Here are the required inputs." followed by the fixture block verbatim. Loading the whole prompt rather than the ROLE block alone keeps the instruction text as published; the file's masthead and closing line, which sit outside the fence, are not loaded.

## Cases

The cases test the one property a reader cannot check by eye across runs: that an output lands in its template column for column. Only A2 and A4 have an output table that maps onto a template one to one; the other chain steps are listed under Known defects.

| ID | Prompt | Rule in the prompt | Input | Pass condition |
| --- | --- | --- | --- | --- |
| G1 | [A2 Objectives](03-prompts/A2-objectives.md) | "A. Objectives register rows, in exactly these 13 columns, in this order, with these headers (the columns of the objectives register template)" | Fixture `A2` | Table A's header row is exactly `OBJ-id, Objective, Owner, Unit, Parent OBJ, Measure, Target, Tolerance, Time frame, Linked RSK/OPP, Linked OBL, Review cadence, Status`, in that order, with no column added or missing, and every row of table A has 13 cells. |
| G2 | [A4 Assessment](03-prompts/A4-assessment.md) | "A. Assessment rows, in exactly these 14 columns, in this order, with these headers (the risk register template's columns from Id to Appetite position)" | Fixture `A4` | Table A's header row is exactly `Id, Type, Statement, Linked OBJ, Category, Inherent L, Inherent I, Velocity, Existing CTLs, Control effectiveness, Residual L, Residual I, Rating, Appetite position`, in that order, with no column added or missing, and every row of table A has 14 cells. |

Content, for the reader, not the pass condition: the worked chain's reviewed rows are one reading of the fixture, not an answer key. Where a score rests on judgment the prompt marks it CALIBRATE for the human owner, so two runs (or a run and the worked chain) can differ on those cells and both be within the prompt's rules (see the run T5 notes below).

## Known defects

Recorded 18 October 2026 (KST). None is fixed at v2.3.0.

- **K1: three more chain outputs do not map one to one onto their templates.** A5's treatment design table has no Linked OBL, Linked POL, Last test result or Status column against the control matrix and names "Operator candidate" for Operator; R1's indicator table names "Owner candidate" for Owner and has no Status column against the review and assurance plan's indicator set; A3's identified items carry no Category, which A4 then needs. The worked chain maps them by hand. A case for each would fail today.
- **K2: the stop rule and the optional inputs.** Every prompt says "If any numbered input is missing, stop and list the missing items", and several numbered inputs read "if any" or "if used" (A2 input 4, A4 input 2 velocity, L1 inputs 4 and 5). Whether an absent optional input stops the prompt is not stated. The fixtures state every input, so the cases do not exercise this.
- **K3: the template sample rows cohere by identifier, not wholly by reason.** CTL-052 (breach severity rubric) is linked to RSK-014 (supplier insolvency); OBL-021 lists CTL-053, which the control matrix does not hold; OPP-003's Appetite position reads "Pursuit within appetite" where the risk register's field definition 5 allows Above, At or Within. The worked chain shows P1's gap check finding the first two. The sample rows are left as published pending the owner's decision.

## Last run

**Run T5, 18 October 2026 (KST).** Configuration: the fenced prompt block of each step as the API system prompt, byte for byte (A2 SHA-256 `c09cb31e3fc47283855f2014f4ba85071b9f1a80d176e13c3bc2d86bce5e7cd7`, A4 SHA-256 `1975e3c289899ba1c26451bcb088d10f7e9231f3bacb840ad4d3b849826568fe`, the v2.3.0 text); the line "Here are the required inputs." and the fixture block as the one user turn; no tools; max_tokens 16000; tested model `claude-opus-5-5`; scorer `claude-sonnet-5-5`. Evidence: [`evidence/transcripts-2026-10-18-T5/`](evidence/transcripts-2026-10-18-T5/README.md). LLM scoring is developer testing, not independent assurance.

| ID | Scorer verdict | Session review | Reason |
| --- | --- | --- | --- |
| G1 | PASS | spot-checked, concur | Table A's header row equals the objectives register template's header row character for character (checked by script against `04-templates/objectives-register.md`); both data rows have 13 cells; stop_reason end_turn; gate line last |
| G2 | PASS | spot-checked, concur | Table A's header row equals the risk register template's first 14 headers character for character (checked by script against `04-templates/risk-register.md`); both data rows have 14 cells; stop_reason end_turn; gate line last |

Counts: scorer 2 PASS, 0 FAIL. Session review: 2 concur; 0 dissent; 0 instrument defect; 0 case defect.

Notes on content, not scored. G1 also drafted a row for the existing enterprise objective OBJ-E02, with its measure, target and tolerance flagged as not stated, and proposed a monthly review cadence where the worked chain has quarterly. G2 scored five cells differently from the worked chain (RSK-014 Inherent I 5 and Residual L 3; OPP-003 Inherent L 4, Velocity High and Residual L 4 against 3) and marked each CALIBRATE with its reasoning, which is the prompt's rule for a judgment score; rating and appetite position agree with the worked chain.

Acceptance under this file's rule ("A run passes when every case it exercises passes"): the run passes, 2 of 2. Reviewer: Michael Paik, 19 October 2026 (KST), concurs. Accepted: yes, 19 October 2026 (KST).

History: no earlier run of any prompt in this pack is published. Whether the prompts were tested against a fixture before 18 October 2026 is Unknown.

---

**Final Liability rests with the Human.**
