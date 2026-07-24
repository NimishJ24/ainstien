# AInstien

AInstien is a portable research companion for coding agents.

Use it with Codex, Cursor, Claude, Antigravity/Gemini-style agents, or any agent that reads `AGENTS.md`. It helps you live through the research journey: from messy curiosity to source-backed research output.

It is not a one-shot paper generator. It helps a researcher read deeply, discuss papers, notice patterns, incubate ideas, plan experiments, calibrate evidence, and decide when a project is ready to become a paper.

## Why AInstien

Most AI research workflows jump too quickly from topic to answer. AInstien keeps the actual research process alive:

```text
papers/discussion -> questions/confusions -> idea-bank -> claim-sheet -> experiment-plan -> experiment-log -> evidence-audit -> paper-readiness
```

The core loop is recursive:

```text
CHOOSE -> READ -> THINK -> HYPOTHESIZE -> EXPERIMENT -> VALIDATE -> COMMUNICATE
```

## Agent Support

AInstien ships the same core research workflow through multiple agent adapters:

| Agent or host | Entry file |
| --- | --- |
| Codex skill | `skills/ainstien-research/SKILL.md` |
| Codex plugin | `.codex-plugin/plugin.json` |
| Cursor | `.cursor/rules/ainstien-research.mdc` |
| Claude | `CLAUDE.md` and `.claude-plugin/plugin.json` |
| Antigravity / Gemini-style agents | `gemini-extension.json` and `.agents/rules/ainstien-research.md` |
| Generic coding agents | `AGENTS.md` |

The canonical source of behavior is always:

```text
skills/ainstien-research/SKILL.md
```

## What It Helps With

- Start and maintain multiple research journeys in parallel
- Keep separate project folders for NLP, mechanistic interpretability, RAG, benchmarks, or any other topic
- Read papers, articles, notes, and documents actively without turning reading into form-filling
- Build durable project-specific `research-state.md`, `reading-log.md`, and `discussion-notes.md` files
- Map literature across foundations, methods, evaluations, disagreements, and gaps
- Capture hunches and possible directions in `idea-bank.md`
- Turn promising ideas into precise research questions and claims
- Plan and log experiments against specific claims
- Evaluate questions for surprise, fruitfulness, rigor, and feasibility
- Calibrate evidence to claim breadth
- Decide whether a project is ready for a paper, memo, literature review, or position piece
- Frame AI/ML research as insight, tool, synthesis, or position work

## Multi-Project State

AInstien keeps each research journey separate. These are possible journey artifacts; AInstien creates them when the workflow calls for them.

```text
research-states/
  research-index.md
  nlp-synthetic-data/
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
  mech-interp-circuits/
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

If you continue an existing project, AInstien updates that project's folder. If your request is ambiguous, it should ask which journey to use before updating state.

## Install

### Codex Skill

Copy the skill folder into your Codex skills directory:

```powershell
Copy-Item -Recurse .\skills\ainstien-research $env:USERPROFILE\.codex\skills\
```

Invoke it with:

```text
Use $ainstien-research to start a research journey on mechanistic interpretability.
```

### Cursor

Open this repository in Cursor. Cursor should pick up:

```text
.cursor/rules/ainstien-research.mdc
```

Then ask Cursor to use AInstien for research work in the repo.

### Claude

Open this repository with Claude Code or another Claude-based coding agent. Claude should see:

```text
CLAUDE.md
.claude-plugin/plugin.json
```

Ask Claude to read `skills/ainstien-research/SKILL.md` before research tasks.

### Antigravity / Gemini-Style Agents

Use the extension metadata and generic rule files:

```text
gemini-extension.json
.agents/rules/ainstien-research.md
```

### Generic Agents

For agents that read repository guidance, use:

```text
AGENTS.md
```

## Example Prompts

```text
Use AInstien to start a new journey called nlp-synthetic-data about whether synthetic data improves reasoning robustness in small language models.
```

```text
Use AInstien to start a separate journey called mech-interp-circuits about finding circuits for refusal behavior.
```

```text
Continue nlp-synthetic-data. Here are five papers I read. Update my research state and tell me what pattern is emerging.
```

```text
Continue mech-interp-circuits. This paper made me wonder whether SAE features are stable across tasks. Add it to my idea bank and tell me how to sharpen it.
```

```text
Turn my best idea into an experiment plan with baselines, controls, falsification criteria, and expected confounds.
```

```text
Log these experiment results and audit whether my evidence supports my claim or whether I am overclaiming.
```

```text
Decide whether nlp-synthetic-data is paper-ready.
```

## Design Principles

- Research is not paper production. Paper writing comes after discovery.
- Reading should produce taste, not just summaries.
- Reading-log fields are reflective lenses, not mandatory interrogation prompts.
- Questions asked during paper discussion are part of the research record.
- Early ideas should be preserved before being judged.
- Experiments should test claims, not just produce impressive numbers.
- Claims should be precise enough to be wrong.
- Evidence should scale with ambition.
- Multiple research journeys should never overwrite each other.
- Good research changes the reader's cognitive state.
- The research state is the companion's memory surface.

## Repo Structure

```text
ainstien/
  AGENTS.md
  CLAUDE.md
  README.md
  gemini-extension.json
  package.json
  .agents/rules/ainstien-research.md
  .claude-plugin/plugin.json
  .codex-plugin/plugin.json
  .cursor/rules/ainstien-research.mdc
  skills/ainstien-research/
    SKILL.md
    agents/openai.yaml
    references/
    assets/templates/
```

## Status

Early public draft. The skill is designed to be extended with more examples, real research states, and community templates.
