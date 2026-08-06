# Research Journey

Use this guide when starting or continuing a research project.

## Core Philosophy

Good research discovers knowledge that is both novel and impactful. The goal is not to merely build something, collect papers, or produce a publication. The goal is to form precise claims about a phenomenon and gather enough evidence for those claims to matter.

The journey is recursive:

`CHOOSE -> READ -> THINK -> HYPOTHESIZE -> EXPERIMENT -> VALIDATE -> COMMUNICATE`

## Multi-Journey Setup

Pass the research-home gate in `research-home.md` before creating or updating journey files. Treat each research project as a separate journey inside the confirmed home so the user can run multiple projects in parallel without mixing state.

Recommended possible layout:

```text
research-states/
  research-index.md
  <project-slug>/
    research-state.md
    reading-log.md
    discussion-notes.md
    literature-map.md
    idea-bank.md
    claim-sheet.md
    experiment-plan.md
    experiment-log.md
    evidence-audit.md
    paper-outline.md
```

Create `research-state.md` and update `research-index.md` when starting a journey. Create the other artifacts only when the workflow calls for them or the user asks for a full workspace.

Use a short slug that is stable across sessions. Examples:

- `nlp-synthetic-data`
- `mech-interp-circuits`
- `rag-evaluation-failures`

If the user says "continue my NLP work" and there are multiple NLP journeys, ask which one. If there is only one clear match, continue it.

## Stage Guide

### Choose

Help the user pick a domain they are genuinely curious about. Favor curiosity that can sustain many days or weeks of reading and thinking.

When the user starts with a raw idea or question, run a brief literature reconnaissance before treating the framing as settled. Find the closest prior work, field vocabulary, and obvious novelty threats.

Capture:

- Project name and slug
- Domain
- Why it matters
- Initial curiosity
- Known constraints
- Possible research type: insight, tool, synthesis, experiment, literature review, or position

### Read

Push for deep reading until marginal new insight declines. Track what has been read, what was learned, what remains unclear, and what gaps are emerging.

### Think

Look for patterns, contradictions, repeated assumptions, untested explanations, brittle evaluations, missing baselines, and places where experts may be wrong or uncertain.

### Hypothesize

Convert observations into precise, falsifiable candidate claims. Do not accept vague claims such as "X improves reasoning" when a narrower claim is more honest.

### Experiment

Design tests that could support or falsify the claim. Keep claim scope and evidence scope aligned.

### Validate

Search for bugs, confounds, alternative explanations, random-seed effects, p-hacking, narrow benchmarks, and mismatched baselines. Treat good results as suspicious until checked.

### Communicate

Write only when there is a cohesive story. The paper should make precise, evidence-backed claims and leave the reader in a different cognitive state.

## Research State Update Rules

When updating the research state:

- Select the correct journey folder before editing.
- Preserve useful prior context.
- Mark uncertainty explicitly.
- Separate facts from interpretations.
- Preserve the user's original wording for raw ideas and questions.
- Label agent paraphrases as unconfirmed interpretations.
- Before saving or replacing core curiosity, best research question, one-sentence thesis, promoted candidate claim, or project objective, show the exact sentence and wait for user confirmation.
- Keep stale claims visible until rejected or superseded.
- Record the next best action.
- Update the research index after meaningful stage, readiness, or next-action changes.

## Paper Readiness Scale

- **0 - Exploration**: Domain and curiosity exist, but no sharp question.
- **1 - Emerging gap**: Patterns or gaps are visible, but claim is unclear.
- **2 - Candidate claim**: A falsifiable claim exists, but evidence plan is weak.
- **3 - Active validation**: Evidence is being gathered and alternatives are being tested.
- **4 - Cohesive story**: Claim, evidence, and contribution type align.
- **5 - Write-ready**: The work can be communicated as a paper, report, or position.

