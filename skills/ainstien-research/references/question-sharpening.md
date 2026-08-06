# Question Sharpening

Use this guide when the user has a rough idea, hunch, topic, gap, or candidate research question.

Before sharpening, search the relevant literature unless the user explicitly asks not to browse. Identify the field's terminology, closest prior work, existing answers, contrary evidence, and likely novelty threats. Do not evaluate surprise or novelty from memory alone when search is available.

## Four Attributes

Evaluate every serious research question on four attributes.

### Surprising To Experts

Ask:

- Would a domain expert already know this?
- Would an expert predict the result easily?
- Is this only novel to the user, or novel to the field?
- What literature review would disprove the novelty?

### Fruitful

Ask:

- If true, what changes?
- What downstream work could this enable?
- Does it open new questions, methods, evaluations, or mental models?
- Is the project more than a small improvement on an obscure benchmark?

### Rigorous

Ask:

- What alternative explanations could explain the result?
- What confounds must be ruled out?
- What baselines, ablations, seeds, settings, or controls are needed?
- What claim is actually supported by the available evidence?

### Feasible

Ask:

- Can the user finish with available time, skills, compute, data, collaborators, and tools?
- Which smaller claim is still useful?
- Which ambitious claim requires evidence the user cannot gather?

## Claim Sharpening

Convert vague claims into precise claims.

Weak:

`RL improves reasoning in LLMs.`

Sharper:

`Under binary reward RLVR on benchmark family X, pass@1 improves while pass@k decreases, suggesting amplification of rewarded trajectories rather than broader exploration.`

## Research Question Gate

Before moving to experiments or writing, produce:

- One-sentence claim
- Why an expert might be surprised
- Why the claim matters
- What would falsify it
- Evidence needed
- Feasibility risks
- Narrower fallback claim

Then present the exact proposed research question or one-sentence claim and ask the user to confirm it before saving it as the project's canonical question, thesis, or promoted claim. Keep earlier wording visible until the replacement is confirmed.

## Output

Use the claim sheet template for serious candidate questions.
