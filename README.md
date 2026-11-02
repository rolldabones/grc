# grc

**Version 2.3.7 · 2026-11-03 · [CHANGELOG](CHANGELOG.md)**

**Acceptance status ([ACCEPTANCE.md](https://github.com/rolldabones/rolldabones/blob/main/ACCEPTANCE.md), 26 October 2026, KST, unchanged at v2.3.7 of 3 November 2026):** Accepted. Run T5 (18 October 2026) passed both cases, G1 and G2, on prompts A2 and A4; neither is critical. The other 19 prompts in 03-prompts/ have no case and carry no acceptance. The account's status table is in [ECOSYSTEM.md](https://github.com/rolldabones/rolldabones/blob/main/ECOSYSTEM.md#instrument-status).

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

**Method and build guides.**

| File | What it holds |
|---|---|
| [01-method/principled-performance.md](01-method/principled-performance.md) | Principled Performance, the ten Universal Outcomes, vocabulary |
| [01-method/operating-cycle.md](01-method/operating-cycle.md) | Omega in operation: cadence, accountability, failure modes |
| [01-method/elements.md](01-method/elements.md) | All 20 elements: purpose, inputs, activities, outputs, measures |
| [01-method/starting-points.md](01-method/starting-points.md) | SP0 to SP4: entry conditions and first-90-days plans |
| [02-build-guides/A-policy-management.md](02-build-guides/A-policy-management.md) | PERFORM-heavy walkthrough (P2 core) |
| [02-build-guides/B-risk-and-opportunity.md](02-build-guides/B-risk-and-opportunity.md) | ALIGN-heavy walkthrough (A2 to A5 core) |
| [02-build-guides/C-obligations-register.md](02-build-guides/C-obligations-register.md) | LEARN-heavy walkthrough (L1 core) |
| [02-build-guides/D-ai-governance-overlay.md](02-build-guides/D-ai-governance-overlay.md) | The model applied to AI systems |
| [FOUR-FRAMES.md](FOUR-FRAMES.md) | Four-frames geopolitical sense-making entry |

**Prompts.** [03-prompts/usage.md](03-prompts/usage.md) gives the design rules, input hygiene and the review gate; one capability prompt per element follows, with [M0 Maturity self-assessment](03-prompts/M0-maturity-self-assessment.md) beside them.

- **LEARN:** [L1 External context](03-prompts/L1-external-context.md) · [L2 Internal context](03-prompts/L2-internal-context.md) · [L3 Culture](03-prompts/L3-culture.md) · [L4 Stakeholders](03-prompts/L4-stakeholders.md)
- **ALIGN:** [A1 Direction](03-prompts/A1-direction.md) · [A2 Objectives](03-prompts/A2-objectives.md) · [A3 Identification](03-prompts/A3-identification.md) · [A4 Assessment](03-prompts/A4-assessment.md) · [A5 Design](03-prompts/A5-design.md)
- **PERFORM:** [P1 Controls](03-prompts/P1-controls.md) · [P2 Policies](03-prompts/P2-policies.md) · [P3 Communication](03-prompts/P3-communication.md) · [P4 Education](03-prompts/P4-education.md) · [P5 Incentives](03-prompts/P5-incentives.md) · [P6 Notification](03-prompts/P6-notification.md) · [P7 Inquiry](03-prompts/P7-inquiry.md) · [P8 Response](03-prompts/P8-response.md)
- **REVIEW:** [R1 Monitoring](03-prompts/R1-monitoring.md) · [R2 Assurance](03-prompts/R2-assurance.md) · [R3 Improvement](03-prompts/R3-improvement.md)

**Templates and example.** [Objectives register](04-templates/objectives-register.md) · [Risk register](04-templates/risk-register.md) · [Obligations register](04-templates/obligations-register.md) · [Control matrix](04-templates/control-matrix.md) · [Policy template](04-templates/policy-template.md) · [Review and assurance plan](04-templates/review-assurance-plan.md) · [05-examples/sp0-worked-chain.md](05-examples/sp0-worked-chain.md), the SP0 chain worked prompt by prompt (fictional).

**Repository files.** [tests.md](tests.md) (prompt pack cases, known defects, run record) · [NOTICE.md](NOTICE.md) (OCEG attribution, trademarks, derivation scope) · [CHANGELOG.md](CHANGELOG.md) · [CITATION.cff](CITATION.cff) · [LICENSE.md](LICENSE.md) (CC BY-SA 4.0) · [evidence/transcripts-2026-10-18-T5/](evidence/transcripts-2026-10-18-T5/README.md), the logged run transcripts, listed last because they sit behind the instruments.

How the pieces fit: `01-method/` explains the model, `02-build-guides/` shows it building something, `03-prompts/` accelerates the drafting work inside each build and `04-templates/` receives the outputs as operating artifacts. The cycle then runs on those artifacts. `05-examples/` walks one chain from inputs to reviewed outputs, and `tests.md` uses it as the fixture for re-testing the prompts. Only A2 and A4 of the 21 prompts have test cases; the other 19 are untested. `FOUR-FRAMES.md` stands upstream of all four: a sense-making entry that reads the external environment through four mythological system-hypotheses with pre-registered discriminators, used alongside PESTLE and STEEPLE, whose weighted readings feed L1 External Context; its first exhibit is Carney's Davos Rupture (20 January 2026), which predates the pre-registration and is excluded from scoring, and its public exposition is [*The Gods of the New Great Game*](https://redcaps.substack.com/p/the-gods-of-the-new-great-game).

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

## Part of the ecosystem

This method repository is one component of a larger body of AI governance, risk management and compliance work. The canonical map of all repositories is [ECOSYSTEM.md](https://github.com/rolldabones/rolldabones/blob/main/ECOSYSTEM.md) in the profile repository.

Nearest neighbors:
- [grc-workbook](https://github.com/rolldabones/grc-workbook): the module-by-module workbook built on this method, with a scored Governance Test and artifact index
- [GRCnext-Copilot](https://github.com/rolldabones/GRCnext-Copilot): the optionality assessor: evidence-led scoring of Global Optionality across critical services (Pipes, Switches, Exits)
- [slow-ai-kitchen](https://github.com/rolldabones/slow-ai-kitchen): the 12-step methodology for deliberate, governed AI adoption
- [definition-of-done](https://github.com/rolldabones/definition-of-done): the acceptance doctrine, how done is defined before work begins and confirmed before reliance
- [AI-Impact-Assessment-Tool](https://github.com/rolldabones/AI-Impact-Assessment-Tool): pre-deployment and lifecycle impact assessment aligned to the EU AI Act, NIST AI RMF, ISO/IEC 42001 and ISO/IEC 42005

Book-appendix instruments:
- [AI Audit DD Checklist v5.2](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip/blob/main/AI_Audit_Due_Diligence_Checklist_v5_2.md): 199-question due diligence instrument with stable question IDs (App I)
- [AI GRC Master Reference v7.13](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip/blob/main/AI_GRC_Master_Reference_v7_13.md): consolidated regulatory and framework reference (App J)

## License and attribution

Original content in this repository is licensed under CC BY-SA 4.0 (`LICENSE.md`). The GRC Capability Model™ is the work of OCEG®; see `NOTICE.md` for attribution, trademark and derivation scope.

## How to Cite

> Paik, Son-U Michael. *grc*, v2.3.7. GRC Solutions Korea, 2026. https://github.com/rolldabones/grc

A machine-readable citation is in [CITATION.cff](CITATION.cff).

---

**Final Liability rests with the Human.**
