# Build Guide C: Obligations Register and Regulatory Change

## 1. What this process is for

The obligations register is the organization's answer to a simple question asked under pressure: what must we comply with, how do we comply and how do we know. This process finds authority sources, decomposes them into assignable requirements, maps each requirement to policies, controls and evidence and keeps the whole structure current as the sources change. Acting with integrity starts here, because you cannot honor obligations you have not identified.

## 2. Elements invoked

Core: **L1 External Context** (sourcing and horizon scanning) feeding **A3 Identification** (obligations are one of the three identified species). Downstream: **P2 Policies** and **P1 Controls** (how compliance happens), **R1 Monitoring** and **R2 Assurance** (how you know). **R3 Improvement** closes change loops. Internal sources matter too: **L4** surfaces contractual and voluntary commitments made to stakeholders.

## 3. Process design

| Step | Owner | Input | Output | Cadence |
|---|---|---|---|---|
| 1. Define scope | GRC function + counsel | Jurisdictions, activities, products, data types | Documented applicability scope | Annual + on change |
| 2. Source inventory | GRC function | Scope, L1 scans | Authority source list: statute, regulation, official guidance, contract, standard, voluntary commitment, each with citation and jurisdiction | Quarterly refresh |
| 3. Applicability analysis | Owner + counsel where needed | Source list | Applies / does not apply / conditional, with reasoning recorded | Per source |
| 4. Decompose | Requirement owners | Applicable sources | Discrete requirements: one obligation row per assignable demand, in original-wording summary with citation | Per source |
| 5. Map | Requirement owners + GRC | Requirements, policy register, control matrix | Each OBL linked to POL and CTL ids and to the evidence that demonstrates compliance | Per requirement |
| 6. Gap treatment | A5 owner | Unmapped requirements | Treatment plans: new or changed policy or control, with dates | Per gap |
| 7. Horizon scanning | L1 owner | Watchlist, official sources | Change alerts with trigger classification | Continuous |
| 8. Change impact assessment | Requirement owners | Change alert | Affected OBL rows identified; impact rated; change plan drafted | Per alert, within a defined SLA |
| 9. Implement change | Policy and control owners | Change plan | Updated policies, controls, training; register rows re-verified | Per plan |
| 10. Verify | GRC function | Register | Last-verified date refreshed with evidence checked | Rolling, all rows within 12 months |

## 4. System requirements (tool-agnostic)

1. **Register structure** per `../04-templates/obligations-register.md`: one row per requirement, not per statute. Citation-level dumping (one row saying "GDPR") is inventory theater.
2. **Applicability reasoning stored**, not just the verdict. When the business changes, the reasoning is what gets re-tested.
3. **Bidirectional links**: OBL to POL, CTL and evidence; POL and CTL back to OBL. Orphans visible from both ends.
4. **Change pipeline states**: Alert received, Impact assessed, Change planned, Implemented, Verified, with timestamps for SLA measurement.
5. **Last-verified date per row** with alerting; verification means evidence was checked, not that the row was reread.
6. **Jurisdiction and entity dimensions** so the register answers per-country and per-entity questions without a fire drill.
7. **Authority hierarchy captured** on every row: statute, regulation, official guidance, contract, standard, voluntary commitment. When sources conflict, hierarchy plus counsel decides.

## 5. Artifacts and templates

- `../04-templates/obligations-register.md` (the register), `../04-templates/control-matrix.md` and `../04-templates/policy-template.md` (the mapped ends).
- The applicability scope document and the watchlist with triggers (L1 outputs).

## 6. Measures and the REVIEW loop

R1 indicators: percentage of requirements mapped to at least one control with evidence (coverage), unmapped requirement count and aging, change SLA performance (alert to verified), rows past their verification window, surprises (changes that arrived without an alert, each one a scanning finding). R2 tests decomposition quality and evidence sufficiency on a sample: could a third party reach the same compliance conclusion from the linked evidence. R3 turns surprises and repeated gaps into scanning and design changes.

## 7. Failure modes

1. **The static register.** Built in a project, never touched again. The last-verified discipline and the change pipeline are what distinguish a register from a monument.
2. **Citation dumping.** Rows that name instruments instead of requirements cannot be assigned, mapped or evidenced. Decomposition is the work; skipping it just moves the work to the worst possible moment.
3. **Applicability by assumption.** "Surely that applies to us" and "surely that does not" both fail audits. The reasoning field is mandatory.
4. **Change surprise.** A requirement changed and the organization learned from a regulator or a headline. Every surprise gets a root cause in the scanning design.
5. **Evidence rot.** Links that point to evidence that no longer exists or no longer demonstrates the requirement. Verification checks the evidence, not the link.

## 8. Reading the equation against this build

This build is Ω entered through LEARN, the natural shape of SP1 (a topical mandate) and the backbone of integrity at every starting point. The Universal Outcomes most exercised: U8 (sense and respond to context) and U6 (prevent, detect and correct). The equation's test: a complete register with a dead change pipeline satisfies C while failing U8, and the gap will be discovered by exactly the party you would least choose.

## 9. Prompts for this guide

`../03-prompts/L1-external-context.md` (sourcing and scanning), `../03-prompts/A3-identification.md` (routing into the register), `../03-prompts/P2-policies.md` and `../03-prompts/P1-controls.md` (mapping ends), `../03-prompts/R2-assurance.md` (evidence sufficiency).

---

**Final Liability rests with the Human.**
