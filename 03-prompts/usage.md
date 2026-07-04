# Prompt Pack: Usage Rules

This directory contains 21 capability prompts: one per element (L1 to R3) plus M0, a maturity self-assessment. Every prompt produces a **draft for human review**. None of them produces a decision. Read this page before running any of them.

## 1. Model-agnostic by design

Prompts are plain text. They use no vendor-specific features, tools or formatting tricks, so they run on any capable large language model, hosted or local. If your model supports system prompts, place the ROLE block there; otherwise paste the prompt whole. Expect quality to vary by model; the quality checks inside each prompt are your first filter, not your last.

## 2. Anatomy

Every prompt has the same six blocks:

1. **ROLE:** what the model is acting as and the standing constraint that it drafts and never decides.
2. **CONTEXT + REQUIRED INPUTS:** the numbered inputs you must supply. Each prompt instructs the model to stop and list missing inputs rather than fabricate. Honor that: if it asks for your calibrated scales, give it your scales.
3. **TASK:** numbered steps.
4. **OUTPUT:** a fixed, lettered schema. Fixed schemas make outputs comparable across runs and routable into the templates in `../04-templates/`.
5. **QUALITY CHECKS:** verifications the model performs before responding.
6. **HUMAN REVIEW GATE:** a mandatory closing line marking the output as a draft under human authority.

## 3. Input hygiene

1. **No secrets, no credentials, no personal data beyond necessity.** Redact names and identifiers that the task does not require. Aggregate wherever the analysis allows, especially for L3 culture work.
2. **Confidentiality and privilege.** Treat prompts and outputs as records: they may be retained, discoverable or requestable. For investigation support (P7) and anything touching legal exposure, work under counsel direction and follow counsel's instructions on what enters any model at all. When in doubt, the answer is ask counsel first, not paste first.
3. **Data residency and vendor terms.** Know where the model runs and what its provider retains before regulated or sensitive material goes in. If you cannot answer that, use a model you can answer it for.
4. **Retention.** Decide where prompt outputs live and for how long, the same as any other working paper.

## 4. Evidence discipline

1. The model may use **only the inputs provided**. Every claim in an output should trace to an input; each prompt's quality checks enforce this.
2. Anything the model asserts without input support must be marked **UNVERIFIED**. Treat UNVERIFIED items as leads, never as findings.
3. **No invented citations.** Authority citations in any output are verified by a human against the source before use. A citation you did not check is a citation you do not have.
4. Where inputs conflict, the model is instructed to surface the conflict, not to resolve it silently.

## 5. The human review gate

Every prompt ends by instructing the model to close with:

> DRAFT FOR HUMAN REVIEW. Decision authority and final liability rest with the accountable human owner.

This is not a disclaimer; it is the operating rule. A named human reviews the draft, corrects it, decides and owns the decision. Wiring these prompts into unattended automation defeats the gate and is outside their intended use. The gate is also your audit marker: any artifact carrying that line and no reviewer's name is unfinished work.

## 6. Chaining along the cycle

Prompts compose in the order Ω runs. Typical chains by starting point (see `../01-method/starting-points.md`):

1. **SP0:** L2 → L1 → A2 → A3 → A4 → A5 → P2/P1 → R1.
2. **SP1 (topical):** L1 → A3 → A4 → A5 → P2 → R1, scoped to the topic.
3. **SP2 (integration):** A2 → A4 (recalibration) → R1 → R2.
4. **SP3 (element fix):** that element's prompt, plus its upstream adjacency from `../01-method/elements.md`.
5. **SP4 (crisis):** P6 → P7 → P8 → A3/A4 → A5 → R1.
6. **Whole-capability snapshot:** M0 across all elements, feeding R3.

Chain by feeding one prompt's reviewed output into the next prompt's inputs. Feed reviewed outputs, not raw ones; the gate sits between every link.

## 7. Prompts are controlled documents

Treat this pack the way P2 treats policies: each prompt has an owner, a version and a change history once you adapt it. Record local modifications; a prompt that drifted silently produces outputs nobody can interpret later. Re-test after model changes: the same prompt on a new model is a new combination.

## 8. Terminology and localization

Prompts use the vocabulary in `../01-method/principled-performance.md`. Where your organization's controlled vocabulary differs, edit the prompts to match and record the mapping. Translate freely; keep the six-block anatomy and the review gate intact in any language.

## 9. Limits

These prompts accelerate drafting. They do not confer expertise, they do not know your organization beyond what you paste and they do not carry accountability. The element documentation in `../01-method/elements.md` tells you what good looks like; the prompts just help you type toward it faster.

---

**Final Liability rests with the Human.**
