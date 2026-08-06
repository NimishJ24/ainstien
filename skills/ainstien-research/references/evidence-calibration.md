# Evidence Calibration

Use this guide when the user has claims, experiments, results, observations, or conclusions.

## Core Rule

Gather evidence in proportion to the scope of the claim. Broad claims require broad evidence. Narrow evidence should produce narrow claims.

## Evidence Audit

For each claim, check:

- What exactly is being claimed?
- What is the broadest version of the claim?
- What is the narrowest version supported by evidence?
- What evidence would falsify the claim?
- Has that falsifying test been run?
- What alternatives remain open?
- What bugs or measurement errors could explain the result?
- What would a skeptical reviewer ask first?

## Common Failure Modes

- Broad claim from a narrow benchmark
- Missing baselines
- Missing ablations
- Single random seed
- Evaluation leakage
- Cherry-picked tasks
- Hidden implementation bug
- Confounding method changes
- Treating engineering success as scientific evidence
- Reporting improvements without a thesis

## Alternative Explanations

Actively generate explanations that would weaken the claim:

- Dataset artifact
- Metric artifact
- Prompting or preprocessing artifact
- Random seed luck
- Baseline weakness
- Compute or scale confound
- Annotation or label issue
- Selection bias in examples

## Validation Posture

Treat promising results as provisional. Before making strong claims, rule out the most likely reasons the result should not hold.

## Output

Produce an evidence audit and recommend the next validation action.
