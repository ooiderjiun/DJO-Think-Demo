# D–J–O THINK — Architecture Overview

## Product principle

D–J–O THINK is not an AI tutor. Students interact with an ordinary chatbot-style interface. The intelligence layer is intended to observe and analyse the student's interaction in the background without interrupting the conversation or supplying coaching during it.

**Core thesis:** AI platforms generate answers. D–J–O THINK documents how students work with those answers.

## Learning sequence

- **Draft:** establish an initial, pre-AI baseline of student understanding.
- **Judge:** examine observable questioning, evaluation, verification, and justified decisions about AI contributions.
- **Own:** examine the student's final synthesis, reasoning, and reflection.

## Orchestration model

One central orchestrator coordinates eight specialist agents. In the proposed workflow, Evidence Capture records events synchronously; specialist analysis is queued and processed asynchronously so that analysis does not add latency to the student's chatbot interaction.

| Role | Responsibility | Boundary |
|---|---|---|
| Orchestrator | Routes events and coordinates agents | Does not grade student competence |
| 1. Evidence Capture | Records drafts, interaction events, submissions, timestamps, and provenance | Captures evidence; does not judge quality |
| 2. Independent Thinking | Establishes the pre-AI baseline | Does not infer unrecorded thoughts |
| 3. Critical Questioning | Analyses student-originated questions and challenges | Question count is not a critical-thinking score |
| 4. Evaluation & Verification | Examines assessment of claims and source checking | Reported checking is not authenticated checking |
| 5. Judgement & Decision | Analyses justified acceptance, rejection, or modification | Requires student-originated rationale |
| 6. Intellectual Ownership | Examines synthesis, reflection, and draft-to-final development | Textual change alone does not prove learning |
| 7. Evidence Validation | Challenges unsupported inferences, duplicate evidence, conflicts, and rubric misalignment | Can lower confidence or abstain; is not a truth detector |
| 8. Assessment Synthesis | Maps validated evidence to cognitive levels and competencies | Produces provisional outputs for lecturer review |

## Event-driven workflow

1. Pre-AI draft submitted → Evidence Capture and Independent Thinking.
2. Student question or challenge recorded → Evidence Capture and Critical Questioning.
3. Source or verification record submitted → Evidence Capture and Evaluation & Verification.
4. Student accepts, rejects, or modifies AI content → Evidence Capture and Judgement & Decision.
5. Final answer and reflection submitted → Evidence Capture and Intellectual Ownership.
6. Sufficient evidence available → Evidence Validation.
7. Validated evidence available → Assessment Synthesis and lecturer review.

## Evidence validation

The proposed validation layer combines adversarial review with deterministic checks. It checks whether findings are grounded in student-originated evidence, whether one evidence item has been double-counted, whether source links and identifiers are traceable, and whether interpretations align with the rubric. Where evidence is incomplete or conflicting, confidence should be downgraded or the system should abstain.

Source status is distinguished as:

1. **Reported:** the student says a source was consulted.
2. **Documented:** an identifiable citation, source, or passage is supplied.
3. **Authenticated:** the source is inspected directly and shown to support the claim.

## Lecturer-facing outputs

The Cognitive Development & Contribution Map presents four linked stages: student baseline → AI contribution (context) → student judgement → final synthesis. Longitudinal Draft, Judge, and Own indicators are kept separate. These are evidence summaries, not validated psychometric measurements or proof of causal learning gains.

Assessment synthesis is provisional. The lecturer retains final authority and can inspect the evidence, change a score, or decide that evidence is insufficient.

## Post-interaction checks

The concept includes an optional short diagnostic and targeted micro-viva after the normal chatbot interaction. These are supplementary ways to seek clarification in selected cases. A flag is not evidence of misconduct, and an asynchronous diagnostic cannot by itself prove independent authorship.

## Prototype versus production

The HTML prototype simulates the interface, scripted interaction, evidence panels, agent architecture, workflow, contribution map, and sample scoring. It does **not** implement live agents, a live LLM, asynchronous queues, authentication, database persistence, source authentication, or production assessment. All displayed learner records and scores are fictional.
