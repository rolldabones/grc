# The 20 Elements (C)

The capability set **C** contains 20 functional elements across four components: LEARN (4), ALIGN (5), PERFORM (8) and REVIEW (3). This document treats each element in operating terms: what it is for, what it consumes, what it does, what it produces, how to measure it and what it connects to. Treatments are summaries in original wording; the Red Book carries the detailed practices.

Each element links to its capability prompt in `../03-prompts/` and, where applicable, to a template in `../04-templates/`.

---

## LEARN

### L1 External Context

**Purpose.** Understand the world the organization operates in: legal and regulatory, market and competitive, technological, economic, social and geopolitical forces, so that objectives, assessments and designs rest on current reality.

**Inputs:** organization profile, jurisdictions and markets, prior context briefs, authority source watchlist.

**Activities:**
1. Scan defined external domains on a set cadence and on trigger.
2. Identify forces, their relevance to objectives and their direction of travel.
3. Extract candidate authority sources and obligations for decomposition.
4. Maintain a watchlist with explicit re-assessment triggers.

**Outputs:** external context brief, force inventory, candidate authority source list, watchlist.
**Measures:** scan cycle time, percentage of obligations traceable to a scanned source, count of changes that arrived as surprises.
**Feeds / fed by:** feeds L4, A2, A3 and the obligations register; fed by R3 triggers and P6 signals.
**Prompt:** `../03-prompts/L1-external-context.md` · **Template:** `../04-templates/obligations-register.md`

### L2 Internal Context

**Purpose.** Understand the organization itself: structure, strategy, people, processes, technology, information and resources, including what enables and what constrains the capability.

**Inputs:** organization charts, strategy documents, process and system inventories, resource plans.

**Activities:**
1. Map structures, key processes, systems and information flows.
2. Identify enablers and constraints relevant to objectives and to the GRC capability itself.
3. Define change triggers (reorganization, acquisition, new system) that force a refresh.

**Outputs:** internal context brief, capability and asset inventory, constraint and enabler analysis.
**Measures:** inventory coverage, staleness of the brief versus last material change.
**Feeds / fed by:** feeds A2, A5 and every build guide; fed by R3 and organizational change events.
**Prompt:** `../03-prompts/L2-internal-context.md`

### L3 Culture

**Purpose.** Understand the climates that decide how work really gets done: ethical climate, risk climate and governance culture, including any gap between stated values and lived incentives.

**Inputs:** survey results, interview and focus group notes, speak-up and case statistics, exit data.

**Activities:**
1. Assess leadership tone and its consistency with stated values.
2. Assess workforce willingness to raise concerns and perceived retaliation risk.
3. Compare stated values with what incentives, promotions and consequences actually reward.
4. Define desired-state culture objectives for ALIGN.

**Outputs:** culture assessment, climate trend lines, tone gap analysis.
**Measures:** speak-up volume and disposition mix, retaliation signals, survey trends by unit.
**Feeds / fed by:** feeds A1, P5 and P3; fed by P6 and P7 patterns.
**Prompt:** `../03-prompts/L3-culture.md`

### L4 Stakeholders

**Purpose.** Know who has a stake, what they need and expect, how much influence they carry and how the organization will engage them.

**Inputs:** stakeholder lists (owners, workforce, customers, suppliers, regulators, communities), interaction history.

**Activities:**
1. Identify and classify stakeholders by influence and interest.
2. Document needs, expectations and the commitments made to each.
3. Build and run an engagement plan with owners and cadence.

**Outputs:** stakeholder map, expectations inventory, engagement plan.
**Measures:** engagement plan execution, unmet-commitment count, materiality coverage.
**Feeds / fed by:** feeds A1, A2 and P3; fed by L1 changes and P6 input.
**Prompt:** `../03-prompts/L4-stakeholders.md`

---

## ALIGN

### A1 Direction

**Purpose.** Establish mission, vision, values, decision-making principles and appetite so that every downstream choice has something to align to.

**Inputs:** LEARN outputs, board and executive input, existing charters and codes.

**Activities:**
1. Draft or refresh direction statements grounded in LEARN outputs.
2. Draft appetite statements by category with tolerance language for calibration.
3. Set decision-making principles that name who decides what, on what criteria.

**Outputs:** direction statement, appetite framework, decision principles.
**Measures:** decisions citing the criteria, exceptions to appetite and their approval trail.
**Feeds / fed by:** feeds A2, A4, A5 and P2; fed by L1 to L4 and R2 results.
**Prompt:** `../03-prompts/A1-direction.md`

### A2 Objectives

**Purpose.** Define measurable objectives, cascaded to owners, each with measures, targets and tolerances. Objectives are the spine: every risk, opportunity, obligation and control ultimately attaches here.

**Inputs:** strategy, direction statement, unit plans, prior objectives register.

**Activities:**
1. Draft objectives that are measurable, owned and time-bound.
2. Cascade to units without losing traceability to the enterprise level.
3. Set tolerances that define acceptable variation before escalation.

**Outputs:** objectives register.
**Measures:** percentage of objectives with owner, measure and tolerance; orphan activity count (work traceable to no objective).
**Feeds / fed by:** feeds A3, R1 and every register; fed by A1 and L2.
**Prompt:** `../03-prompts/A2-objectives.md` · **Template:** `../04-templates/objectives-register.md`

### A3 Identification

**Purpose.** For each objective, identify what could help (opportunities), what could hinder (obstacles) and what must be met (obligations). Identification is objective-first: no orphan risks, no orphan rules.

**Inputs:** objectives register, LEARN outputs, event history, workshop and interview material.

**Activities:**
1. Run objective-by-objective identification using multiple techniques (workshops, data, external sources).
2. Record each item with source, owner candidate and objective linkage.
3. Route obligations to decomposition and the obligations register.

**Outputs:** populated risk, opportunity and obligation inventories, each item linked to an objective.
**Measures:** items per objective, source diversity, orphan item count.
**Feeds / fed by:** feeds A4 directly; fed by L1 to L4, P6 and R1.
**Prompt:** `../03-prompts/A3-identification.md` · **Templates:** `../04-templates/risk-register.md`, `../04-templates/obligations-register.md`

### A4 Assessment

**Purpose.** Analyze and evaluate identified items so that priority reflects reality: likelihood, impact, velocity and the effect of existing controls, judged against appetite and tolerance.

**Inputs:** identified inventories, calibrated assessment scales, appetite framework, control matrix.

**Activities:**
1. Assess items on the organization's calibrated scales, inherent and residual.
2. Evaluate against appetite and tolerance to produce a prioritized queue.
3. Record the treatment decision required for each priority item.

**Outputs:** assessed and prioritized registers, treatment decision queue.
**Measures:** assessment currency, calibration drift between assessors, items above appetite without a treatment decision.
**Feeds / fed by:** feeds A5 and R1 thresholds; fed by A3 and P1 control effectiveness data.
**Prompt:** `../03-prompts/A4-assessment.md` · **Template:** `../04-templates/risk-register.md`

### A5 Design

**Purpose.** Design the integrated set of actions and controls (proactive, detective, responsive) and the capability itself: what will exist, who will run it, what it will cost and in what order it will be built.

**Inputs:** prioritized registers, treatment decisions, internal context, resource constraints.

**Activities:**
1. Design treatments per priority item with a deliberate mix of control types.
2. Trace every designed action to the item and objective it serves.
3. Sequence implementation with owners, resources and dates.
4. Design changes to the capability itself when REVIEW findings require it.

**Outputs:** control architecture, treatment plans, resourced implementation roadmap.
**Measures:** design coverage of priority items, implementation on-time rate, controls with no traced item.
**Feeds / fed by:** feeds P1 to P8; fed by A4 and R3.
**Prompt:** `../03-prompts/A5-design.md` · **Template:** `../04-templates/control-matrix.md`

---

## PERFORM

### P1 Controls

**Purpose.** Operate the designed management actions and controls across human, process, physical and technical layers, with evidence that they ran.

**Inputs:** control architecture, control matrix, operating procedures.

**Activities:**
1. Implement controls with named operators and defined frequency.
2. Produce and retain the evidence each control specifies.
3. Detect and report control failures and design gaps (risks with no control, controls with no risk).

**Outputs:** operating controls, control performance records, failure reports.
**Measures:** control execution rate, evidence completeness, failure detection-to-fix time.
**Feeds / fed by:** feeds R1 and A4 (effectiveness data); fed by A5.
**Prompt:** `../03-prompts/P1-controls.md` · **Template:** `../04-templates/control-matrix.md`

### P2 Policies

**Purpose.** Maintain a policy framework that converts obligations and decisions into stated expectations: a hierarchy (policy, standard, procedure), a lifecycle and traceability in both directions.

**Inputs:** obligations register, direction statement, control architecture, policy register.

**Activities:**
1. Draft and maintain policies in which every statement traces to an obligation, risk or decision.
2. Run the lifecycle: draft, review, approve, publish, attest, review, retire.
3. Manage exceptions with approval, expiry and compensating measures.

**Outputs:** policy set, policy register, attestation and exception records.
**Measures:** attestation rate, overdue reviews, exceptions past expiry, orphan policies.
**Feeds / fed by:** feeds P3, P4 and P1; fed by A1, A5 and the obligations register.
**Prompt:** `../03-prompts/P2-policies.md` · **Template:** `../04-templates/policy-template.md`

### P3 Communication

**Purpose.** Keep expectations, values and channels known: the right message, to the right audience, at the right time, with a way to talk back.

**Inputs:** policy set, culture assessment, stakeholder map, communication history.

**Activities:**
1. Build an audience-message-channel plan with cadence and owners.
2. Communicate policies, values and intake channels in plain language.
3. Check comprehension, not just delivery.

**Outputs:** communication plan, campaign records, comprehension results.
**Measures:** reach, comprehension scores, intake channel awareness.
**Feeds / fed by:** feeds P6 awareness and L3; fed by P2 and L4.
**Prompt:** `../03-prompts/P3-communication.md`

### P4 Education

**Purpose.** Build the competence roles actually need: curriculum mapped from role to obligation and risk, delivered and evaluated for effect, not attendance.

**Inputs:** role inventory, obligations and risk registers, incident lessons.

**Activities:**
1. Map roles to the obligations and risks they touch, then to learning objectives.
2. Deliver role-based training at onboarding and on a cycle.
3. Evaluate effectiveness with assessment and behavior signals, then revise.

**Outputs:** training plan, completion and efficacy records, curriculum map.
**Measures:** completion by role, assessment pass quality, correlation of training with incident patterns.
**Feeds / fed by:** feeds P1 operator competence and L3; fed by P2, A5 and P8 lessons.
**Prompt:** `../03-prompts/P4-education.md`

### P5 Incentives

**Purpose.** Align what the organization rewards with what it claims to value: performance management, compensation, recognition and consequences, screened for perverse incentives.

**Inputs:** compensation and performance criteria, promotion data, culture assessment, case outcomes.

**Activities:**
1. Review incentive structures against stated values and appetite.
2. Identify perverse incentives and quantify their exposure.
3. Align consequence frameworks so outcomes are consistent and proportionate.

**Outputs:** incentive review, consequence framework, recognition records.
**Measures:** consistency of consequences across levels, perverse-incentive findings closed.
**Feeds / fed by:** feeds L3 and U3 evidence; fed by L3 and P7 patterns.
**Prompt:** `../03-prompts/P5-incentives.md`

### P6 Notification

**Purpose.** Maintain always-open pathways for anyone, inside or outside, to report concerns, exceptions and events, with triage that routes fast and protects reporters.

**Inputs:** channel inventory, triage taxonomy, severity rubric, anti-retaliation safeguards.

**Activities:**
1. Operate multiple intake channels with acknowledged service levels.
2. Triage by taxonomy and severity, routing to P7 or direct resolution.
3. Protect reporters and monitor for retaliation.

**Outputs:** intake log, triage records, acknowledgment trail.
**Measures:** channel volume and mix, acknowledgment SLA performance, retaliation signals.
**Feeds / fed by:** feeds P7, R1 and L3; fed by P3 awareness work.
**Prompt:** `../03-prompts/P6-notification.md`

### P7 Inquiry

**Purpose.** Establish what actually happened: scoped, fair, evidence-based investigation of notifications and detections, plus proactive inquiry where signals warrant it.

**Inputs:** intake records, investigation protocols, evidence handling standards, counsel direction where applicable.

**Activities:**
1. Plan each inquiry: scope, custodians, evidence, interviews, timeline.
2. Gather and preserve evidence; conduct fair interviews.
3. Report findings as supported or not supported by evidence, with recommendations.

**Outputs:** investigation plans, evidence records, findings reports.
**Measures:** cycle time by severity, substantiation rate, quality review results.
**Feeds / fed by:** feeds P8 and R3; fed by P6 and R1 detections. Run under counsel direction where privilege or legal exposure is in play.
**Prompt:** `../03-prompts/P7-inquiry.md`

### P8 Response

**Purpose.** Correct and recover: remediate confirmed issues, apply consequences, make disclosure decisions with counsel, manage crises and convert root causes into improvement.

**Inputs:** findings reports, response plans, disclosure obligations, crisis criteria.

**Activities:**
1. Execute remediation with owners and dates; verify closure with evidence.
2. Apply the consequence framework consistently.
3. Assemble disclosure decision packages for counsel and leadership.
4. Feed root causes into R3 and design changes into A5.

**Outputs:** remediation records, consequence records, disclosure log, root cause analyses.
**Measures:** remediation on-time rate, recurrence rate, disclosure timeliness.
**Feeds / fed by:** feeds R3 and A5; fed by P7 and crisis triggers.
**Prompt:** `../03-prompts/P8-response.md`

---

## REVIEW

### R1 Monitoring

**Purpose.** Watch the capability and the objectives continuously: defined indicators (performance, risk, control), thresholds tied to tolerance and escalation that actually escalates.

**Inputs:** objectives register, assessed registers, control matrix, data sources.

**Activities:**
1. Define indicators with owner, source, frequency, threshold and escalation path.
2. Report on cadence; escalate threshold breaches immediately.
3. Watch for gaming and stale indicators; retire what no longer informs.

**Outputs:** indicator definitions, dashboards, escalation log.
**Measures:** indicator coverage of priority items, breach-to-action time, stale indicator count.
**Feeds / fed by:** feeds A4, P7 (detections) and R3; fed by P1 evidence and A2 tolerances.
**Prompt:** `../03-prompts/R1-monitoring.md` · **Template:** `../04-templates/review-assurance-plan.md`

### R2 Assurance

**Purpose.** Provide independent, objective conclusions on design and operating effectiveness: internal audit, external audit, certifications and reviews, planned on risk and coordinated on a map.

**Inputs:** assessed registers, assurance inventory, prior findings, independence requirements.

**Activities:**
1. Maintain an assurance map: what is assured, by whom, at what depth, when.
2. Plan engagements on risk; scope to conclusions that matter.
3. Report with evidence sufficient for a third party to reach the same conclusion.

**Outputs:** assurance plan and map, engagement reports, opinions.
**Measures:** coverage of high-rated areas, findings accepted and closed, repeat finding rate.
**Feeds / fed by:** feeds R3, A1 and stakeholder confidence (U4); fed by A4 ratings and R1 signals. Independence from operation and design is the non-negotiable.
**Prompt:** `../03-prompts/R2-assurance.md` · **Template:** `../04-templates/review-assurance-plan.md`

### R3 Improvement

**Purpose.** Close the loop: consolidate findings from monitoring, assurance and events into a prioritized backlog, drive changes into ALIGN and PERFORM and prove closure with evidence.

**Inputs:** findings from R1 and R2, root causes from P8, context triggers from LEARN.

**Activities:**
1. Consolidate and de-duplicate findings into one backlog.
2. Prioritize on impact, effort and risk; assign owners and dates.
3. Route changes to A5 (design) or P-elements (operation); verify closure with evidence.

**Outputs:** improvement backlog, change records, closure evidence.
**Measures:** backlog throughput, aging, recurrence of closed items.
**Feeds / fed by:** feeds A5 and all P-elements; fed by everything. R3 is where the cycle either loops or leaks.
**Prompt:** `../03-prompts/R3-improvement.md`

---

## Using this document

Read the element you are building, open its prompt, prepare the declared inputs and route the output into the matching template. The build guides in `../02-build-guides/` show several elements composed into complete processes. For a whole-capability snapshot, run `../03-prompts/M0-maturity-self-assessment.md` across all 20.

---

**Final Liability rests with the Human.**
