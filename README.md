# grc

**Version 2.0 · 2026-07-04**

This repository is a working method for governance, risk management and compliance (GRC). It is built on the GRC Capability Model™ (Red Book) version 3.5 published by OCEG® and it exists to do three things:

1. Explain the model in operating terms, not just in outline.
2. Show how to build real processes and systems from it, with four worked guides.
3. Supply model-agnostic prompts and templates so the build work can start today.

The goal of the whole apparatus is Principled Performance®: the reliable achievement of objectives while addressing uncertainty and acting with integrity. Everything in this repository points at that goal. See `NOTICE.md` for attribution and trademark information.

## Core equation

**PP ≈ Ω(C | SP) ↑ UO**

## How to read the notation

This is mnemonic notation, not mathematics. The operators borrow the feel of conditioning and limits to say something precise in one line: Principled Performance emerges when a complete capability set is cycled continuously, from wherever you actually start, in the direction of ten defined outcomes.

| Symbol | Read as | Meaning here |
|---|---|---|
| **PP** | Principled Performance | The goal state: reliably achieve objectives, address uncertainty and act with integrity |
| **≈** | is approached through | PP is an emergent outcome of sustained operation, not a computed result |
| **Ω** | the operating cycle | LEARN → ALIGN → PERFORM → REVIEW, run continuously with feedback loops |
| **C** | the capability set | The 20 functional elements available to the cycle |
| **\| SP** | given starting point | The entry condition that shapes sequencing and emphasis |
| **↑ UO** | oriented toward Universal Outcomes | Ten outcomes that guide and constrain the entire process |

A worked reading: a company that has just settled an enforcement action enters at SP4 (Crisis). Ω begins with inquiry and response already running, then rebuilds backward into LEARN and ALIGN so that the fix is anchored to objectives rather than to the last headline. The Universal Outcomes tell it when the rebuild is real: not when the file closes, but when U6 (prevent, detect and correct) and U3 (improve culture) show evidence.

## Definitions of variables and symbols

- **PP (Principled Performance):** The ultimate goal to reliably achieve objectives, address uncertainty and act with integrity.
- **≈ (Is approached or achieved through):** Principled Performance emerges from the effective and sustained operation of the GRC system.
- **Ω (GRC Operating Cycle):** Continuous, iterative application of four components with feedback loops: **LEARN → ALIGN → PERFORM → REVIEW ↻**.
- **C (Set of GRC Capabilities/Elements):** The complete set of **20** functional elements used within **Ω**.
  - **Learn (L):** {L1 External Context, L2 Internal Context, L3 Culture, L4 Stakeholders}
  - **Align (A):** {A1 Direction, A2 Objectives, A3 Identification, A4 Assessment, A5 Design}
  - **Perform (P):** {P1 Controls, P2 Policies, P3 Communication, P4 Education, P5 Incentives, P6 Notification, P7 Inquiry, P8 Response}
  - **Review (R):** {R1 Monitoring, R2 Assurance, R3 Improvement}
- **| SP (Conditioned by / Initiated and focused by):** **Ω** is influenced and initially shaped by the specific starting point (**SP**): {SP0 Blank Canvas, SP1 Topical, SP2 Discipline, SP3 Element, SP4 Crisis}. Starting point names follow the Red Book.
- **↑ UO (Guided and constrained by / Aspiring toward):** The entire GRC process is directed by and aims to achieve ten Universal Outcomes (**UO**), expanded in `01-method/principled-performance.md`.

## Repository map

```
grc/
|-- README.md                        This file: equation, notation, routing
|-- LICENSE.md                       CC BY-SA 4.0
|-- NOTICE.md                        OCEG attribution, trademarks, derivation scope
|-- CHANGELOG.md                     Version history
|-- 01-method/
|   |-- principled-performance.md    PP, the ten Universal Outcomes, vocabulary
|   |-- operating-cycle.md           Omega in operation: cadence, accountability, failure modes
|   |-- elements.md                  All 20 elements: purpose, inputs, activities, outputs, measures
|   `-- starting-points.md           SP0 to SP4: entry conditions and first-90-days plans
|-- 02-build-guides/
|   |-- A-policy-management.md       PERFORM-heavy walkthrough (P2 core)
|   |-- B-risk-and-opportunity.md    ALIGN-heavy walkthrough (A2 to A5 core)
|   |-- C-obligations-register.md    LEARN-heavy walkthrough (L1 core)
|   `-- D-ai-governance-overlay.md   The model applied to AI systems
|-- 03-prompts/
|   |-- usage.md                     Design rules, input hygiene, review gate
|   |-- L1 ... R3 (20 files)         One capability prompt per element
|   `-- M0-maturity-self-assessment.md
`-- 04-templates/
    |-- objectives-register.md       risk-register.md      obligations-register.md
    `-- control-matrix.md            policy-template.md    review-assurance-plan.md
```

How the pieces fit: `01-method/` explains the model, `02-build-guides/` shows it building something, `03-prompts/` accelerates the drafting work inside each build and `04-templates/` receives the outputs as operating artifacts. The cycle then runs on those artifacts.

## Quick start: route by starting point

| Your situation | SP | Read first | First prompts | First templates |
|---|---|---|---|---|
| No formal capability exists | SP0 | `starting-points.md`, then `operating-cycle.md` | L1, L2, A2 | objectives-register, obligations-register |
| One topic is burning (AI, privacy, sanctions) | SP1 | Build guide C or D | L1, A3, A4 | obligations-register, risk-register |
| You run one discipline and need integration | SP2 | `operating-cycle.md`, then `elements.md` | A2, A5, R1 | control-matrix, review-assurance-plan |
| One element is broken (policies, hotline, training) | SP3 | That element in `elements.md` | That element's prompt | The matching template |
| An incident or enforcement event just happened | SP4 | `starting-points.md` SP4, then guides A and B | P6, P7, P8, then A3, A4 | risk-register, review-assurance-plan |

## Conventions

1. **Terminology.** GRC expands to governance, risk management and compliance throughout this repository. US English spelling is used.
2. **Identifiers.** Cross-references use these prefixes: OBJ (objective), RSK (risk), OPP (opportunity), OBL (obligation), CTL (control), POL (policy), ISS (issue). Templates define the fields.
3. **Depth.** Element treatments here are summaries in original wording. The authoritative model, including detailed practices, is the Red Book itself, available from OCEG at oceg.org.
4. **Prompts.** Every prompt is model agnostic, requires declared inputs and ends in a mandatory human review gate. Prompts produce drafts. Humans own decisions.

## Companion resources

Maintained by the same author and designed to interoperate with this method:

- [GRC Workbook](https://github.com/rolldabones/grc-workbook): module-by-module workbook with a scored Governance Test and artifact index.
- [GRCnext™ Copilot](https://github.com/rolldabones/grcnext-copilot): a build framework for GRC copilots on five primitives (Services, Tolerances, Pipes, Switches, Exits).
- [Slow AI Kitchen](https://github.com/rolldabones/slow-ai-kitchen): a 12-step methodology for deliberate AI adoption.
- [AI Audit DD Checklist](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip/blob/main/AI_Audit_Due_Diligence_Checklist_v4_7.md): 187-question due diligence instrument (App I).
- [AI GRC Master Reference](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip/blob/main/AI_GRC_Master_Reference_v7_7.md): consolidated regulatory and framework reference (App J).

## License and attribution

Original content in this repository is licensed under CC BY-SA 4.0 (`LICENSE.md`). The GRC Capability Model™ is the work of OCEG®; see `NOTICE.md` for attribution, trademark and derivation scope.

---

**Final Liability rests with the Human.**
