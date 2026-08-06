# Research Home

Use this guide before any research-state read or write when a stable research home has not been confirmed.

## Resolution Order

1. Use a path explicitly supplied by the user.
2. Otherwise, reuse the current workspace when it contains `research-states/research-index.md`.
3. Otherwise, ask the user to choose a stable directory. Do not initialize automatically.

Ask:

`No stable AInstien research home is configured. Which persistent directory should contain your research-states folder? You may choose this workspace if it is a long-lived project, or provide another path.`

## Reject Unsafe Defaults

Do not initialize by default in:

- Temporary directories.
- Generated date-based Codex workspaces, including paths containing `Codex/<YYYY-MM-DD>/`.
- The cloned AInstien source repository containing `skills/ainstien-research/SKILL.md`.
- Any location the user describes as disposable, session-specific, or short-lived.

Explain the risk and ask for a stable alternative. Proceed only if the user explicitly overrides the warning.

## Verify The Home

Before writing state:

1. Resolve the intended path.
2. Confirm that it exists or that the user wants it created.
3. Confirm that the agent can write there.
4. Confirm that the user expects to reopen or reuse it across sessions.
5. Create or update `research-states/research-index.md` and record the home metadata.

If filesystem access is blocked, do not choose another path silently. Ask the user to open the directory as the workspace or grant access.

## Long-Lived Projects

Keep one project slug for the lifetime of the research journey, even when it spans months or years. Put dates inside reading logs, discussion notes, experiment logs, and `Last Updated` metadata. Never fork state merely because a new Codex thread, workspace, day, month, or year begins.
