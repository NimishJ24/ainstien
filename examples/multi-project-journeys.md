# Example: Multiple Research Journeys

Prompt:

```text
Use $ainstien-research to start two separate research journeys: one called nlp-synthetic-data about whether synthetic data improves reasoning robustness in small language models, and one called mech-interp-circuits about finding circuits for refusal behavior.
```

Expected behavior:

- Create or propose `research-states/research-index.md`.
- Create one folder per journey.
- Keep each journey's `research-state.md` separate.
- Ask before updating if the user later says something ambiguous like "continue my NLP research" and multiple NLP journeys exist.
- End with the selected journey slug, current stage, paper readiness, and next best action.
