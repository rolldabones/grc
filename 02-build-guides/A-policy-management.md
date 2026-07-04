# Build Guide A: Policy Management

## 1. What this process is for

Policies convert obligations and leadership decisions into stated expectations that people can follow, attest to and be trained on. A policy management process exists so that every policy has a reason, an owner and a lifecycle. It equally exists so that no obligation needing a policy lacks one. The deliverable is not a document library. It is bidirectional traceability: obligation to policy to control to evidence and back.

## 2. Elements invoked

Core: **P2 Policies**. Upstream: **A1 Direction** (what leadership has decided), **L1 External Context** and the obligations register (what must be met), **A5 Design** (where a policy is the chosen treatment). Alongside: **P3 Communication** and **P4 Education** (a policy nobody knows is not a control). Downstream: **P1 Controls** (policies state expectations that controls enforce), **R1 Monitoring** and **R3 Improvement**.

## 3. Process design

| Step | Owner | Input | Output | Cadence |
|---|---|---|---|---|
| 1. Mandate check | Policy owner | Obligation, risk or A1 decision requiring a policy | Documented mandate with OBL/RSK/decision reference | On trigger |
| 2. Draft | Policy owner (author) | `policy-template.md`, obligations extract, related controls | Draft in template structure | On trigger |
| 3. Traceability check | GRC function | Draft | Every policy statement traced to an obligation, risk or decision; untraceable statements cut or justified | Per draft |
| 4. Stakeholder review | Named reviewers | Draft | Consolidated comments with dispositions | Per draft |
| 5. Approval | Designated approver per hierarchy | Reviewed draft | Approved policy, version stamped | Per draft |
| 6. Publish | GRC function | Approved policy | Published to the single authoritative location; register updated | Per approval |
| 7. Communicate and train | P3/P4 owners | Published policy | Targeted communication; role-based training where required | Per publication |
| 8. Attest | Affected workforce | Published policy | Attestation records | Per publication and annually |
| 9. Exceptions | Requester + approver | Exception request | Approved exception with expiry and compensating measure, logged | On request |
| 10. Periodic review | Policy owner | Register review-date trigger | Reconfirmed, revised or retired; register updated | Per policy, at least every 2 years |
| 11. Retire | Policy owner + approver | Obsolete policy | Retirement record; dependent training and controls updated | On trigger |

## 4. System requirements (tool-agnostic)

Any system supporting this process, from a spreadsheet plus a document repository to a dedicated platform, must provide:

1. **A policy register** as the single source of truth, one row per policy, with the fields in section 5.
2. **One authoritative publication location** per policy. Copies elsewhere are convenience, never authority.
3. **Workflow states:** Draft, In review, Approved, Published, Under revision, Retired. State changes are logged with actor and timestamp.
4. **Traceability fields** in both directions: policy to OBL/RSK/CTL identifiers, and those registers back to POL identifiers.
5. **Attestation capture** by person, policy version and date, queryable by role and unit.
6. **Exception records** with approver, expiry date and compensating measure, with expiry alerts.
7. **Review-date alerting** to the policy owner and the GRC function.
8. **Version history** preserving every published version and its effective window (audits ask what applied on a date).

## 5. Artifacts and templates

- Policy documents: `../04-templates/policy-template.md`.
- Policy register fields: POL-id, title, owner, approver, hierarchy level (policy, standard, procedure), status, version, effective date, next review date, linked OBL ids, linked RSK ids, linked CTL ids, attestation scope, exception count.
- Attestation and exception logs as defined in section 4.

## 6. Measures and the REVIEW loop

R1 indicators: attestation rate by unit, overdue reviews, exceptions past expiry, orphan policies (no OBL/RSK/decision link), obligations flagged as policy-requiring with no policy. R2 examines lifecycle discipline and traceability integrity on a sample. R3 receives every finding: repeated exception patterns usually mean the policy is wrong, not the people.

## 7. Failure modes

1. **Orphan policies.** Statements with no traceable mandate accumulate until nobody can say what is actually required. The traceability check at step 3 exists to stop this at the door.
2. **Shelfware.** Published, never communicated, never trained, attested by reflex. Attestation rate looks fine; comprehension is zero. Pair every publication with step 7 or admit the policy is decorative.
3. **Unowned policies.** The author left; the policy persists. Ownership is a register field with an alert, not a memory.
4. **Version sprawl.** Copies in mail, drives and decks. One authoritative location, everything else linked.
5. **Exception rot.** Exceptions without expiry become the real policy. Expiry and compensating measures are mandatory fields.

## 8. Reading the equation against this build

Ω engaged here runs L1 and A1 into A5, expresses the decision through P2, carries it out through P3 and P4 and closes through R1 and R3. The starting point is commonly SP3 (the policy element is broken) or SP1 (a topic forces new policy). The Universal Outcomes most exercised: U6 (prevent, detect and correct) and U10 (honor and express values). The test the equation imposes: if the register is clean but attestation is theater, P2 is succeeding while U3 fails, and the capability is spinning without motion.

## 9. Prompts for this guide

`../03-prompts/P2-policies.md` (drafting), `../03-prompts/L1-external-context.md` (obligation sourcing), `../03-prompts/P3-communication.md` and `../03-prompts/P4-education.md` (rollout), `../03-prompts/R1-monitoring.md` (indicators).

---

**Final Liability rests with the Human.**
