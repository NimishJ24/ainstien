# Experiment Cycle

Use this guide when the user wants to plan, run, interpret, debug, or record experiments.

## Purpose

Experiments exist to test claims, not to produce impressive numbers. Keep every experiment tied to a question, hypothesis, or falsification attempt.

## Planning Pass

Before running an experiment, capture:

- Research question
- Hypothesis
- Claim being tested
- What result would support the claim
- What result would weaken or falsify the claim
- Dataset, model, benchmark, or environment
- Baselines
- Controls and ablations
- Metrics
- Seeds or repetitions
- Expected confounds
- Feasibility constraints

## Execution Log

During or after experiments, capture:

- Date or run id
- Setup
- Changes from previous run
- Results
- Unexpected observations
- Failures or bugs
- Interpretation
- Alternative explanations
- Follow-up run

## Interpretation Rules

- Narrow the claim when evidence is narrow.
- Treat surprising positive results as suspicious until checked.
- Separate engineering success from scientific evidence.
- Record failed experiments because they shape the research map.
- Prefer one decisive falsification test over decorative rigor.

## Output

Use `experiment-plan.md` before running. Use `experiment-log.md` during or after running. Use `evidence-audit.md` when interpreting results against a claim.
