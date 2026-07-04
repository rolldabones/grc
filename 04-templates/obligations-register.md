# Template: Obligations Register

One row per assignable requirement, never per instrument. Elements: L1, A3. Prompt: `../03-prompts/L1-external-context.md`. Build guide C is the operating manual for this template.

## Register

| OBL-id | Authority source | Type | Citation | Jurisdiction | Entity scope | Requirement summary | Applicability | Applicability reasoning | Owner | Linked POLs | Linked CTLs | Evidence of compliance | Change trigger | Last verified | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| OBL-021 | Data protection statute | Statute | Art. 00(0) (verify) | KR | All KR entities | Notify the authority of qualifying breaches within the statutory window | Applies | Processes personal data of KR residents as controller | H. Choi | POL-007 | CTL-052, CTL-053 | Incident response test records, notification runbook | Amendment or new enforcement guidance | 2026-05-10 | Mapped |

## Field definitions

1. **Type.** Statute, regulation, official guidance, contract, standard, voluntary commitment. This is the authority hierarchy; conflicts resolve upward, with counsel.
2. **Citation.** Exact provision, human-verified against the source. A citation nobody checked is marked (verify) until someone has.
3. **Requirement summary.** Original-wording summary of the discrete demand, decomposed to what one owner can be accountable for.
4. **Applicability and reasoning.** The verdict and the analysis. The reasoning is what gets re-tested when the business changes.
5. **Linked POLs, CTLs, Evidence.** How compliance happens and how you know. The links run both directions; orphans must be visible from either end.
6. **Change trigger and Last verified.** The change pipeline hooks. Verification means the evidence was checked, not that the row was reread. Every row inside 12 months.
7. **Status.** Identified, Under analysis, Mapped, Gap (treatment underway), Retired.

## Guidance

1. Decompose before assigning; "comply with the statute" is not a requirement, it is a wish.
2. Voluntary commitments and contract clauses are obligations too; L4 feeds this register.
3. Every surprise change (learned from a regulator or headline rather than the watchlist) gets a root cause in the scanning design.
