# Multi-agent tasks: which coding agent

Which engine, model and reasoning effort to send a job to, and the fallback. Generated 2026-11-13 UTC, rebuilt about weekly; source snapshots 2026-11-12 to 2026-11-12; own jobs: the 28 days before. First choices changed since 2026-11-02: research claude-fable-5.1 -> claude-fable-5.2; reading claude-fable-5.1 -> claude-fable-5.2; writing Claude Code / claude-fable-5.1 -> Antigravity CLI / gemini-4-argon; and 5 more (/bench.json `changes`).

For task class X, use the first choice; if it cannot run right now, the next fallback, in the order listed. The order is the ranking: with few own jobs, the evidence and tie rules can put a lower score first. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; probation = a new model version counting its predecessor's jobs and public scores for 28 days; effort = the reasoning effort to run at, lowest to highest low, medium, high, xhigh, max (a fallback's follows its cost tier; '(config)' = the CLI's own config; '· source' = moved by a leaderboard gap of 0.03+).

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.76); Codex CLI / gpt-6.1-sol $$$ xhigh (config) (0.70) | 0.82 | 76 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | medium | Codex CLI / gpt-6.1-sol $$$ xhigh (config) (0.59); Claude Code / claude-opus-5.5 $$$$ medium (0.53) | 0.65 | 25 | proven |
| coding / features | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.75); Claude Code / claude-sonnet-5.5 $$$ medium (0.74) | 0.81 | 12 | probation |
| coding / frontend | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.66); Antigravity CLI / claude-opus-5.5 $$$$ high (0.67) | 0.62 | 2 | unproven |
| coding / multilang | Codex CLI / gpt-6.1-sol $$$ | xhigh (config) | - | 0.50 | 2 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.51); Claude Code / claude-fable-5.2 $$$$ medium (0.53) | 0.60 | 20 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-haiku-5.5 $ high (0.79); Claude Code / claude-opus-5.5 $$$$ medium (0.74) | 0.83 | 26 | proven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.69); Claude Code / claude-fable-5.2 $$$$ medium (0.67) | 0.79 | 10 | proven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | medium | - | 0.50 | 1 | unproven |
| agentic / browser | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.42) | 0.57 | 1 | unproven |
| agentic / tools | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ medium (0.65); Antigravity CLI / claude-sonnet-5.5 $$$ high (0.67) | 0.65 | 0 | unproven |
| research | Claude Code / claude-fable-5.2 $$$$ | medium | Codex CLI / gpt-6.1-sol $$$ xhigh (config) (0.61); Claude Code / claude-sonnet-5.5 $$$ medium (0.56) | 0.79 | 35 | probation |
| reading | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-haiku-5.5 $ high (0.62); Codex CLI / gpt-6.1-sol $$$ xhigh (config) (0.57) | 0.88 | 42 | probation |
| writing | Antigravity CLI / gemini-4-argon $$$ | high | Claude Code / claude-fable-5.2 $$$$ medium (0.73); Claude Code / claude-sonnet-5.5 $$$ medium (0.73) | 0.85 | 12 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; multilang = repo work outside Python: JS/TS, Go, Rust, Java, PHP; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; browser = driving web pages and forms; tools = multi-step work through APIs and tool connectors.

Is a higher effort worth it? One step up in effort: Artificial Analysis Intelligence Index points gained / times the list-price cost per task (a general index, in no score here; the cost of its tasks, not of our jobs). Every level: /bench.json `cost_curve`.

| model | low to medium | medium to high | high to xhigh | xhigh to max |
|---|---|---|---|---|
| claude-fable-5.2 | +2.5 / 1.2x | +5.4 / 2.4x | +0.4 / 1.6x | +2.4 / 1.8x |
| claude-opus-5.5 | +13.4 / 2.5x | +3.6 / 1.4x | +5.6 / 1.7x | +1.7 / 1.7x |
| claude-sonnet-5.5 | +5.2 / 1.5x | +10.7 / 2.1x | +8.4 / 2.5x | +4.6 / 2.4x |
| claude-haiku-5.5 | +6.0 / 2.1x | +5.3 / 1.7x | +4.7 / 1.6x | +1.9 / 1.7x |
| gpt-6.1-sol | +11.5 / 2.2x | +4.0 / 1.6x | +2.2 / 1.3x | +2.1 / 1.7x |

Own jobs of one model at two effort levels, per class. Not a controlled test: the effort was chosen per job. What the leaderboards gain per level: /bench.json `classes.X.effort_evidence`. No source gives tokens per level.
- coding: Claude Opus 5.5 in Claude Code: 71 of 74 finished cleanly at medium, 51 of 51 at high.
- agentic: Claude Sonnet 5.5 in Claude Code: 17 of 17 finished cleanly at medium, 9 of 9 at high.
- research: Claude Opus 5.5 in Claude Code: 13 of 14 finished cleanly at medium, 16 of 16 at high.
- reading: Claude Sonnet 5.5 in Claude Code: 56 of 56 finished cleanly at medium, 17 of 17 at high.
- writing: Claude Opus 5.5 in Claude Code: 10 of 10 finished cleanly at medium, 12 of 12 at high.

Where a number comes from (/bench.json): `classes.X.first_choice.inputs` (a score's inputs, each public metric with its source and link), `sources` (snapshot dates), `method.fields` (definitions).
