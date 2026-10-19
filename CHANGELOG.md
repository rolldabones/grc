# Changelog

## v2.3.2 (2026-10-19)

Patch, from the weekly maintenance sweep of 19 October 2026 (KST) and Michael Paik's review of the T5 runs, completed 19 October 2026 (KST), on which he concurs with the scoring as recorded. No prompt, template or schema changes.

- **Logged run T5 accepted.** The run passed 2 of 2 (G1, G2); the named reviewer concurs and accepts the configuration. `tests.md` records the review and the acceptance.
- README masthead, How to Cite and `CITATION.cff` to v2.3.2.

## v2.3.1 (2026-10-18)

Link repair, session T8 of the whole-account review of 15 October 2026 (KST). Patch: the book repository reissued its two appendix instruments under new versioned filenames on the same day (AI Audit and Due Diligence Checklist v5.0, AI GRC Master Reference v7.11), and the superseded files are deleted there, so the two links in the README's related-instruments list would have broken.

- **`README.md`**: the Checklist link moves from `AI_Audit_Due_Diligence_Checklist_v4_11.md` to `AI_Audit_Due_Diligence_Checklist_v5_0.md` and names its stable question IDs; the Master Reference link moves from `AI_GRC_Master_Reference_v7_10.md` to `AI_GRC_Master_Reference_v7_11.md` (account guard pin `grc-master-reference-version`).
- Masthead, How to Cite and `CITATION.cff` to v2.3.1 in lockstep. All other files unchanged byte for byte.

## v2.3.0 (2026-10-18)

Prompt pack made testable, session T5 of the whole-account review of 15 October 2026 (KST); review doc section 5 and reviewer report 07. Minor release: three prompts and two templates change their instrument text, each with a dated amendment note.

- **A2 and A4 output schemas aligned to their templates (report 07, item B4).** A2's output A now carries the objectives register's 13 columns in its order and with its headers; it had produced nine, with "Owner candidate" for Owner. A2 drafts each row with the owner marked "(candidate)", both linked columns "pending A3" and Status "Proposed", and task step 2 adds a proposed review cadence. A4's output A now carries the risk register's columns from Id to Appetite position; it had produced "Inherent scores" and "Residual scores" against the template's Inherent L, Inherent I, Velocity, Residual L, Residual I and Rating. Evidence notes move to their own table B, the later outputs re-letter C to F and input 2 names the rating rule where one is used. Amendment notes in both prompt files.
- **Templates.** `objectives-register.md` adds the status Proposed (drafted by A2, owner not yet confirmed); both templates name the prompt output that fills them and point to the worked example.
- **L1 optional input 5 (report 07, item B5).** The weighted portfolio reading from the `FOUR-FRAMES.md` scoring log, if used; the README said FOUR-FRAMES readings feed L1 and neither the prompt nor `elements.md` took them. Amendment note in the prompt file; `elements.md` L1 inputs name it.
- **Worked SP0 chain (new, `05-examples/sp0-worked-chain.md`).** One fictional organization taken through L2, L1, A2, A3, A4, A5, P2, P1 and R1, from inputs to reviewed outputs, landing on the template sample rows OBJ-001, RSK-014, OPP-003, OBL-021, CTL-052 and POL-007. Labeled fictional and illustrative; not model output and not a test run.
- **`tests.md` (new).** Cases G1 (A2) and G2 (A4), whose pass condition is that the output table matches its template column for column, with the worked chain as the fixture; three known defects; the run record. `03-prompts/usage.md` sections 6 and 7 point to both files, closing the "re-test after model changes" line that had no fixture.
- **Logged run T5, 18 October 2026 (KST).** `claude-opus-5-5`, scored by `claude-sonnet-5-5`, API system prompt = the fenced prompt block, no tools, max_tokens 16000: G1 PASS, G2 PASS (2 of 2). Session review concurs on both; the exact header match was also checked by script against the two templates. The run passes under `tests.md`'s rule; acceptance is pending Michael Paik's review. G2 scored four judgment cells differently from the worked chain and marked each CALIBRATE, as the prompt requires; `tests.md` now says the worked chain is one reading of the fixture, not an answer key. Transcripts and `summary.json` in `evidence/transcripts-2026-10-18-T5/`, copied byte for byte with a closing line appended.
- **Records.** `FOUR-FRAMES.md` v0.5.2 strikes the completed ECOSYSTEM.md outstanding item, with a dated amendment note (report 07, item A8). Build guide D's currency line is re-dated with the statement that the guide carries no regime thresholds (report 07, item A11). The README map lists `tests.md` and `05-examples/`.
- **Findings by class (report 07, grc items).** Confirmed and edited: B4 (A2 and A4 schemas; the fixture), B5, A8, A11. Already fixed: A5 (count, v2.2.3), C1 (closing lines, v2.2.4), C6 grc parts (v2.2.4; the two "licence" lines are shipped history under ruling 7), C7 (v2.2.4). Not reproducible in full: the doc's statement that the five sample rows "already cohere" holds by identifier only (tests.md K3).
- **Deferred, with reasons.** A9 (a first scoring date for FOUR-FRAMES) needs the author's date; B6 and B7 (falsifiable discriminators, method and exhibit split) need the author's series and are content work; C2 (the symbol list) carries the element enumeration the table does not, so dropping it is a front-door decision for session T7; C3 (masthead trim or a single source for the 21 prompts) touches every prompt file and is left for a release of its own; K1 (A5, R1 and A3 schemas) is outside the two schemas the review named.
- Masthead, How to Cite and `CITATION.cff` to v2.3.0 in lockstep. All other files unchanged byte for byte.

## v2.2.4 (2026-10-17)

Closing line and house style, session T3 of the whole-account review of 15 October 2026 (KST).

- **Closing line.** "Final Liability rests with the Human." added as the last line of the 21 prompt files, the six templates, `NOTICE.md` and this changelog, after the paste-ready fences so no prompt text changes. Found by reviewer report 07, item C1, and doc section 8.
- **`FOUR-FRAMES.md` v0.5.1**, with a dated amendment note: byline in the account form, "GRCnext" given its mark in Section 4, one serial comma removed in Section 9 (report 07, item C6). No frame, indicator or reading changed.
- **`README.md`.** The repository map lists `CITATION.cff` (report 07, item C7).
- Masthead, How to Cite and `CITATION.cff` to v2.2.4 in lockstep. All other files unchanged byte for byte.

## v2.2.3 (2026-10-15)

Pointer correction, session T1 of the whole-account review of 15 October 2026 (KST).

- **`README.md`, Book-appendix instruments.** The Checklist line read "187-question" against an instrument of 197 questions since v4.10 (13 August 2026) and 198 since v4.11 (15 October 2026); corrected to 198. Both links re-pointed to the reissued filenames, `AI_Audit_Due_Diligence_Checklist_v4_11.md` and `AI_GRC_Master_Reference_v7_10.md`, released the same day in `final-liability-rests-with-the-human-book-wip` v1.8.0. Found by reviewer report 05, item A17.
- Masthead, How to Cite and `CITATION.cff` to v2.2.3 in lockstep. All other files unchanged byte for byte.

## v2.2.2 (2026-09-06)

Citation infrastructure, doctrine citation line and lockstep maintenance. Session C of the September 2026 improvement pack, one patch release per repository across all 21 public repositories.

- **`CITATION.cff` added** in the house form settled at D-C1: no `type` field, `version` and `date-released` in lockstep with the README, `license` as the SPDX identifier for this repository's licence, `abstract` taken from this repository's ECOSYSTEM.md role line rather than newly written.
- **How to Cite block** aligned to this release and pointing at `CITATION.cff`.
- All other files in this repository are unchanged byte for byte.

## v2.2.1 (2026-08-23)

Link correction in the README's Part of the ecosystem section.

- The two book-appendix links pointed at superseded filenames (v4_7, v7_7). Corrected to AI_Audit_Due_Diligence_Checklist_v4_10.md and AI_GRC_Master_Reference_v7_9.md, the filenames in force in the book repository. The stale names entered with the v2.2.0 restoration, which reproduced the v2.1.0-era description without re-verifying the link targets.
- No other changes. README version header advanced to 2.2.1.

## v2.2.0 (2026-08-23)

FOUR-FRAMES.md added: the four-frames geopolitical sense-making entry (entry version v0.5, final). The ecosystem section recorded in v2.1.0, found missing from the live README, is restored in the same release.

1. **Method entry (new).** Four mythological system-hypotheses (Greek, Norse, Kali Yuga, Mandate of Heaven) run as a portfolio with pre-registered discriminators, a quarterly scoring log and a standing bias register. Used alongside PESTLE and STEEPLE; feeds L1 External Context. First scored exhibit: Carney's Davos Rupture (19 January 2026).
2. **Public exposition.** *The Gods of the New Great Game* (23 August 2026): https://redcaps.substack.com/p/the-gods-of-the-new-great-game
3. **README.** Repository map and How-the-pieces-fit updated; version header advanced to 2.2.0 with a CHANGELOG link.
4. **Restoration.** The Part of the ecosystem section recorded in v2.1.0 was absent from the live README; restored before License and attribution, superseding Companion resources with every link preserved.
5. **No changes** to the method documents, build guides, prompts, templates, NOTICE or LICENSE.

## v2.1.1 (2026-08-13)

License metadata sweep. An `SPDX-License-Identifier: CC-BY-SA-4.0` line and the canonical Creative Commons legal code are now carried inside the existing license file. The filename is unchanged and the human-readable summary is retained above the legal code. This repository stays on ShareAlike rather than NonCommercial: its material adapts the OCEG GRC Capability Model 3.5, distributed under CC BY-SA, and a NonCommercial variant is not share-alike compatible with that source.

- The primary audience is automated intake and provenance tooling, which reads the SPDX tag rather than prose. Automated license detection previously reported nothing across all twenty-one repositories in this account.
- No change to the licence in force. The identifier records what was already true.

## v2.1.0 (2026-07-15)

Ecosystem integration release under the repository improvement program. Three-part semantic versioning applies from this release; prior releases retain their two-part labels.

1. **Part of the ecosystem section (new).** Links the canonical ECOSYSTEM.md in the profile repository plus five nearest neighbors (grc-workbook, GRCnext-Copilot, slow-ai-kitchen, definition-of-done, AI-Impact-Assessment-Tool) and the two book-appendix instruments, placed before License and attribution.
2. **Companion resources consolidated.** The prior Companion resources section is superseded by the ecosystem section; every link it carried is preserved there.
3. **Version header.** README header updated to 2.1.0 with a CHANGELOG link.
4. **No content changes.** The method, build guides, prompts, templates, NOTICE and LICENSE are unchanged.

## v2.0 (2026-07-04)

Full restructure from a single README to a complete method repository.

1. **Method (new).** Four documents: Principled Performance and the ten Universal Outcomes expanded with evidence and failure modes; the operating cycle with cadence, accountability and failure patterns; all 20 elements treated individually (purpose, inputs, activities, outputs, measures, adjacencies); starting points SP0 to SP4 with first-90-days plans.
2. **Build guides (new).** Four worked examples of building GRC processes and systems: policy management; risk and opportunity management; obligations register and regulatory change; and an AI governance overlay with ISO/IEC 42001 and NIST AI RMF touchpoints.
3. **Prompt pack (new).** 21 model-agnostic prompts: one per element plus a maturity self-assessment, each with declared inputs, fixed output schemas, quality checks and a mandatory human review gate. Usage rules cover input hygiene, evidence discipline and prompt version control.
4. **Templates (new).** Six operating templates: objectives register, risk register, obligations register, control matrix, policy template and review and assurance plan.
5. **Correction.** Element A4 renamed to **Assessment** per Red Book 3.5. Version 1 rendered it as Analysis.
6. **Governance files (new).** LICENSE (CC BY-SA 4.0), NOTICE (OCEG attribution, trademarks, derivation scope) and this changelog.
7. **Conventions.** Terminology standardized to governance, risk management and compliance; identifier scheme (OBJ, RSK, OPP, OBL, CTL, POL, ISS) defined; US English throughout.

## v1.0 (last updated 2026-01-27)

Initial release. Single README containing the core equation PP ≈ Ω(C | SP) ↑ UO, the 20-element enumeration, starting points SP0 to SP4 and the ten Universal Outcomes.

---

**Final Liability rests with the Human.**
