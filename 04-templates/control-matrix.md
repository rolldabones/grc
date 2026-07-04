# Template: Control Matrix

Every control with its reason, operator, evidence and test. Elements: A5, P1. Prompts: `../03-prompts/A5-design.md`, `../03-prompts/P1-controls.md`.

## Matrix

| CTL-id | Control statement | Type | Nature | Frequency | Operator | Linked RSK/OPP | Linked OBL | Linked POL | Evidence produced | Test method | Last test result | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| CTL-052 | Breach severity is assessed against the notification rubric within 24 hours of incident confirmation | Detective | Hybrid | Per incident | Incident manager on duty | RSK-014 | OBL-021 | POL-007 | Completed rubric with timestamp per incident | Sample incidents re-performed quarterly by second line | Pass 2026-04 | Operating |

## Field definitions

1. **Control statement.** Specific and observable: an independent person can tell whether it happened. "Management monitors X" is not a control statement.
2. **Type.** Proactive (prevents or promotes), Detective (finds promptly), Responsive (corrects and recovers). The portfolio needs all three; the matrix makes the mix visible.
3. **Nature.** Manual, automated, hybrid. Automated controls still need evidence and tests; they just fail differently.
4. **Operator.** The role that performs it. Unowned controls do not operate; they linger.
5. **Linked RSK/OPP, OBL, POL.** The reason the control exists. A control with no links is either missing its reason or spending money on nothing.
6. **Evidence produced.** What the control leaves behind, specified so a third party could reach the same conclusion from it.
7. **Test method and result.** How operation is independently verified, and the latest outcome with date.
8. **Status.** Designed, Implementing, Operating, Failed (remediation open), Retired.

## Guidance

1. Run the two-way gap check on cadence: linked items with no control; controls with no linked item.
2. When a control fails, the row shows it; hiding failures in email defeats the matrix.
3. Reuse before building; the matrix is also the catalog.
