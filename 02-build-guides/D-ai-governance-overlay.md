# Build Guide D: AI Governance Overlay

## 1. What this process is for

AI systems change what "the process" means: part of the behavior being governed is produced by a model rather than written by a person, it can change with data and updates and it can act at machine speed. This guide applies the same 20 elements to that reality. It is an overlay, not a separate program: an organization that builds AI governance as a silo repeats the failure the GRC Capability Model™ exists to fix. Framework references in this guide are current as of 2026-07-04; verify against the applicable texts before reliance.

## 2. Elements invoked

All four components, with AI-specific emphasis: **L1** (a fast-moving regulatory landscape), **L2** (an AI system inventory, the single most commonly missing artifact), **A3/A4** (AI-specific identification and assessment), **A5/P1** (lifecycle controls and human oversight points), **P2** (AI use policy), **P6 to P8** (AI incident intake and response), **R1** (model monitoring), **R2** (AI audits and conformity assessment) and **R3** (model change as the improvement loop).

## 3. Process design

| Step | Owner | Input | Output | Cadence |
|---|---|---|---|---|
| 1. Inventory | GRC function + IT | Procurement, system, vendor and shadow-use scans | AI system registry: one row per system with purpose, model type, data, autonomy level, affected persons, owner | Continuous; full sweep quarterly |
| 2. Regulatory mapping | Counsel + GRC | L1 scan of applicable AI frameworks per jurisdiction | Obligations rows per system class (guide C pipeline) | Quarterly + on change |
| 3. Classify | System owners + GRC | Registry, applicable classification schemes | Risk classification per system with reasoning recorded | Per system + on change |
| 4. Assess | System owners + GRC | Classification, AI harm taxonomy (safety, rights, security, economic, information integrity), lifecycle stage | Assessed entries in the risk register with objective linkage | Per system; high classifications quarterly |
| 5. Design lifecycle controls | A5 owner | Assessments | Controls at each lifecycle checkpoint (section 4), including named human oversight points with real authority | Per system |
| 6. Policy | P2 owner | Obligations, classifications | AI use policy: permitted uses, prohibited uses, approval paths, disclosure rules, data handling | Standing; review annually |
| 7. Operate and evidence | System owners | Controls | Evaluation records, deployment gate decisions, oversight logs | Continuous |
| 8. Monitor | R1 owner | Deployed systems | Performance, drift, misuse and incident indicators with thresholds and escalation | Continuous |
| 9. Incident intake and response | P6/P7/P8 owners | Reports, monitoring detections | AI incident log, inquiries, remediation, regulator notification where required | On event |
| 10. Assure | R2 provider | High-classification systems | Independent audits or conformity assessments with evidence-based conclusions | Per assurance plan |
| 11. Change management | R3 + system owners | Model updates, retraining, findings | Re-assessment triggers fired; controls re-verified after material change | Per change |

## 4. Lifecycle control checkpoints

Design P1 controls at minimum at these points, with evidence at each:

1. **Data sourcing:** provenance, rights to use, representativeness review, personal data handling.
2. **Build or buy:** vendor due diligence for procured systems; development standards for built ones.
3. **Evaluation:** pre-deployment testing against defined acceptance criteria, including failure and misuse testing proportionate to classification.
4. **Deployment gate:** a named human decision, recorded, with authority to say no.
5. **Operation:** monitoring per step 8; human oversight points that can actually intervene.
6. **Change:** any material model, data or use change re-fires steps 3 to 5.
7. **Retirement:** decommissioning with data disposition and dependent-process updates.

## 5. Framework touchpoints

**ISO/IEC 42001 (AI management systems), clause families mapped to components:**

| ISO/IEC 42001 clause family | Model component and elements |
|---|---|
| 4 Context | LEARN (L1, L2, L4) |
| 5 Leadership | A1 Direction |
| 6 Planning, incl. AI risk and impact assessment | A2 to A5 |
| 7 Support | P3, P4, P5 |
| 8 Operation | P1, P2 (with A4 for impact assessment in operation) |
| 9 Performance evaluation | R1, R2 |
| 10 Improvement | R3 |

**NIST AI RMF functions mapped to components:**

| NIST AI RMF | Model component and elements |
|---|---|
| GOVERN | Cross-cutting: A1, A5, P2, accountability structures |
| MAP | LEARN + A3 (context and identification) |
| MEASURE | A4 + R1 (assessment and measurement) |
| MANAGE | A5 + P1 + P8 (treatment, operation, response) |

**Statutory and regulatory regimes** (EU AI Act risk-tiering and conformity duties, Korea's AI framework legislation, US federal and state measures and sectoral rules) enter through the guide C pipeline: source, applicability, decomposition, mapping. Classification duties land in steps 2 and 3; conformity assessment and audits in step 10; post-market monitoring in step 8; serious incident reporting in step 9. Do not hard-code any regime's thresholds into this guide; hard-code the pipeline that keeps up with them.

## 6. Measures and the REVIEW loop

R1 indicators: registry coverage (systems found outside the registry is the key negative indicator), percentage of high-classification systems with current evaluations, deployment gate bypasses (target zero), drift and incident rates, oversight interventions and their outcomes, change events that skipped re-assessment. R2 provides independent conclusions on the systems that matter most, with evidence a third party could re-trace. R3 treats every model change as a governance event, not an IT ticket.

## 7. Failure modes

1. **Shadow AI.** Systems in use that no registry knows. Inventory is step 1 for a reason; procurement, expense and network signals all feed it.
2. **One-time conformity theater.** Assessed at deployment, never re-assessed through a year of updates. The change trigger in step 11 is the difference between a certificate and a capability.
3. **Oversight without authority.** A named human who cannot actually stop the system is a compliance decoration. The deployment gate and intervention points must carry recorded authority.
4. **Monitoring without a response path.** Drift alarms that route to nobody. Every indicator in step 8 names its escalation.
5. **Vendor opacity accepted.** "The provider handles that" recorded nowhere, verified never. Procured systems get due diligence artifacts or compensating controls.

## 8. Reading the equation against this build

This is Ω conditioned by SP1 with the topic set to AI, and it is the overlay case that proves the model's generality: nothing in C changed, only the content flowing through it. The Universal Outcomes most exercised: U8 (sense and respond, at the pace this field moves) and U6 (prevent, detect and correct, now including harms produced at machine speed). The equation's test: an organization with certified paperwork and an incomplete inventory has UO pointing one way and reality pointing another, and the registry gap is where the two will meet.

## 9. Prompts for this guide

`../03-prompts/L1-external-context.md` (regulatory scan), `../03-prompts/L2-internal-context.md` (inventory build), `../03-prompts/A3-identification.md` and `../03-prompts/A4-assessment.md` (AI risk work), `../03-prompts/A5-design.md` (lifecycle controls), `../03-prompts/P6-notification.md` and `../03-prompts/P8-response.md` (AI incidents), `../03-prompts/R2-assurance.md` (audit scoping).

---

**Final Liability rests with the Human.**
