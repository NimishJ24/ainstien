# Example: Start A Research Journey

Prompt:

```text
Use $ainstien-research to start a research journey called nlp-synthetic-data about whether synthetic data improves reasoning robustness in small language models.
```

Expected behavior:

- Look for an existing `research-states/research-index.md`.
- If no stable research home is established, ask the user where to initialize it and wait for their answer.
- Reject temporary, date-based Codex workspaces and the cloned AInstien source repository as silent defaults.
- Verify that the confirmed research home is writable before creating state.
- Create or propose `research-states/nlp-synthetic-data/research-state.md`.
- Add the journey to `research-states/research-index.md`.
- Identify the current stage as exploration.
- Ask for or suggest seed sources.
- Separate curiosity from claim.
- Avoid jumping directly to paper writing.
- End with the selected journey slug, current stage, paper readiness, and next best action.
