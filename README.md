# D–J–O THINK — Agentic Learning Environment

A self-contained, browser-based demonstration prototype for a management presentation. The demo uses a Biochemistry case study on Antimycin A and Complex III inhibition.

## Live demo

This is a static site and can be published with GitHub Pages. Open `index.html` locally or publish the repository using the steps below.

## What the prototype demonstrates

1. **Draft** — captures a student's initial hypothesis before substantive AI exposure.
2. **Orchestrate** — displays a central orchestrator coordinating specialised agents.
3. **Judge** — offers multiple perspectives and captures the student's critical evaluation.
4. **Refine** — records how the student's explanation develops.
5. **Own & evaluate** — captures a student-authored final answer and produces an illustrative process report.

## Agent roles shown

- Draft Guardian
- Biochemistry Expert
- Perspective Agent
- Critical Challenger
- Evidence Checker
- Learning Analyst
- Ownership Evaluator

## Important prototype disclosure

**This version simulates agent orchestration locally in the browser.** It does not call live LLMs, a production multi-agent runtime, or the Jev framework. The routing is a transparent, predefined demonstration sequence inspired by typed decision routing. Assessment values are illustrative placeholders, not validated grades. No student data is sent to a server; the prototype does not persist records after the browser session.

A production implementation would require model/API integration, authenticated student accounts, secure persistence, consent and retention controls, validated assessment rubrics, educator moderation, and evaluation of routing accuracy and fairness.

## Publish with GitHub Pages

1. Create a new GitHub repository, e.g. `djo-think-demo`.
2. Upload `index.html` and `README.md` to the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**.
4. Select `main` and `/ (root)`, then save.
5. Wait for the Pages deployment and open the published URL.

## Run locally

Simply open `index.html` in a modern browser. No build tools or dependencies are required.

## Suggested next technical milestone

Replace the local simulation with an orchestrator service that routes structured tasks to specialist agents, records execution events, and uses a typed decision layer. Keep the pedagogical D–J–O workflow independent of any one agent framework or model provider.
