# D–J–O THINK

**Agentic Interaction Intelligence for Education**  
*Making student thinking visible in AI-assisted learning*

D–J–O THINK is a concept demonstrator for an educational intelligence layer that captures and analyses observable evidence of how students work with generative AI. It is designed around the **Draft–Judge–Own (D–J–O™)** learning framework.

> **DEMO / SAMPLE:** This repository contains a front-end simulation with fictional, illustrative content. It is not a production learning platform and does not connect to live LLMs, autonomous agents, a database, or a learning management system.

## Open the demo

- Open `index.html` directly in a modern web browser, or
- Publish the repository with **GitHub Pages** (instructions below).

The demo is a self-contained HTML file. It requires no build step, package installation, API key, or server-side service.

## What the prototype demonstrates

### Student workspace

1. **Draft** — students record an initial, pre-AI explanation.
2. **Judge** — students interact with a scripted chatbot exchange and can question or evaluate AI-generated claims. The chatbot flow is illustrative, not a live AI connection.
3. **Own** — students prepare a final answer and reflection, documenting whether they accepted, rejected, or modified AI contributions.

### Lecturer workspace

- An evidence view showing the student's initial draft, final answer, source statement, and reflection.
- An eight-specialist-agent architecture coordinated by one orchestrator.
- An event-driven workflow in which evidence capture is represented as synchronous, while specialist analysis is represented as asynchronous.
- An **Evidence Validation** auditor that illustrates adversarial review, unsupported-inference checks, double-counting checks, rubric alignment, confidence downgrading, and abstention.
- Three-tier source verification: **Reported**, **Documented**, and **Authenticated**.
- A **Cognitive Development & Contribution Map** showing the sequence from student baseline to AI contribution, student judgement, and final synthesis.
- Separate illustrative Draft, Judge, and Own indicators across four fictional assignments.
- A proposed post-interaction 60-second diagnostic and targeted human micro-viva workflow.
- Illustrative cognitive and scientific-competency rubric scoring for lecturer review.

## Agent architecture shown

The concept uses one orchestrator and eight specialist agents:

1. Evidence Capture
2. Independent Thinking
3. Critical Questioning
4. Evaluation & Verification
5. Judgement & Decision
6. Intellectual Ownership
7. Evidence Validation (adversarial auditor)
8. Assessment Synthesis

The orchestrator coordinates the workflow; it does not independently grade students. Evidence Capture records events and does not assess thinking quality. Assessment outputs are provisional and intended for lecturer review. The lecturer retains final assessment authority.

## Important interpretation and safeguards

- The system analyses **observable evidence in the captured interaction**, not private thoughts or internal cognition.
- A relevant question is evidence of questioning, not proof of deep critical thinking.
- A student-reported source check is not equivalent to authenticated verification.
- Missing evidence means **not observed in this record**, not that the student lacks the ability.
- A diagnostic or micro-viva flag is a request for clarification, not a misconduct finding.
- Prompt count, conversation length, and textual change alone are not valid measures of critical thinking or learning gain.
- All student records, scores, timelines, and assignments in this demo are fictional and illustrative.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in Chrome, Edge, Firefox, or Safari.
3. Switch between **Student workspace** and **Lecturer workspace** to explore the flow.

No build command is required.

## Publish with GitHub Pages

1. Push the repository to GitHub.
2. Open the repository's **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder, then save.
5. Wait for GitHub Pages to publish the site. The public URL will appear in the Pages settings.

Keep the visible **DEMO · SAMPLE** watermark when publishing or sharing this prototype.

## Repository structure

```text
DJO_THINK_GitHub_Release/
├── index.html
├── README.md
├── .gitignore
└── docs/
    ├── ARCHITECTURE.md
    └── DJO-THINK-Presentation.pdf
```

## Status and next steps

This is a **front-end concept prototype**. A production implementation would require, at minimum, secure authentication, consent and privacy controls, a persistent event store, model/API integration, orchestration and queue infrastructure, source retrieval and verification, audit logging, access controls, and evaluation against expert-annotated evidence. These capabilities are not implemented in this repository.

## Intellectual property and reuse

The D–J–O™ framework and D–J–O THINK concept are presented for demonstration. No open-source licence is granted by this repository unless a separate licence is added by the rights holder. Please seek permission before reusing the framework, branding, or materials beyond evaluation and demonstration.
