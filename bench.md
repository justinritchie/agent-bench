# Multi-agent tasks: which coding agent

Which engine, model and reasoning effort to send a job to, and the fallback. Generated 2026-11-20 UTC, rebuilt about weekly; source snapshots 2026-11-20 to 2026-11-20; own jobs: the 28 days before. First choices changed since 2026-11-13: agentic claude-haiku-5.5 -> claude-sonnet-5.5; coding / review Claude Code / claude-sonnet-5.5 -> Codex CLI / gpt-6.2-sol; coding / multilang Codex CLI / gpt-6.1-sol -> none; and 3 more (/bench.json `changes`).

For task class X, use the first choice; if it cannot run right now, the next fallback, in the order listed. The order is the ranking: with few own jobs, the evidence and tie rules can put a lower score first. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; probation = a new model version counting its predecessor's jobs and public scores for 28 days; effort = the reasoning effort to run at, lowest to highest low, medium, high, xhigh, max (a fallback's follows its cost tier; '(config)' = the CLI's own config; '· source' = moved by a leaderboard gap of 0.03+).

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | medium | Codex CLI / gpt-6.2-sol $$$ xhigh (config) (0.78); Claude Code / claude-opus-5.5 $$$$ medium (0.70) | 0.81 | 79 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.47); Claude Code / claude-fable-5.2 $$$$ medium (0.35) | 0.62 | 25 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | medium | Antigravity CLI / gemini-4-neon $$$$ high (0.71); Claude Code / claude-opus-5.5 $$$$ medium (0.63) | 0.77 | 11 | proven |
| coding / frontend | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.58); Antigravity CLI / claude-opus-5.5 $$$$ high (0.70) | 0.65 | 6 | probation |
| coding / review | Codex CLI / gpt-6.2-sol $$$ | xhigh (config) | Claude Code / claude-sonnet-5.5 $$$ medium (0.54); Claude Code / claude-fable-5.2 $$$$ medium (0.48) | 0.61 | 13 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-haiku-5.5 $ high (0.71); Claude Code / claude-fable-5.2 $$$$ medium (0.66) | 0.69 | 65 | proven |
| agentic / terminal | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-haiku-5.5 $ high (0.67); Claude Code / claude-sonnet-5.5 $$$ medium (0.63) | 0.72 | 4 | unproven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | medium | - | 0.50 | 2 | unproven |
| agentic / browser | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.42) | 0.57 | 1 | unproven |
| agentic / tools | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.57); Antigravity CLI / gemini-4-neon $$$$ high (0.60) | 0.55 | 5 | proven |
| research | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ medium (0.57); Grok CLI / grok-4.7 $$$ medium (config) (0.53) | 0.74 | 35 | probation |
| reading | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ medium (0.60); Claude Code / claude-opus-5.5 $$$$ medium (0.54) | 0.73 | 48 | probation |
| writing | Antigravity CLI / gemini-4-argon $$$ | high | Claude Code / claude-fable-5.2 $$$$ medium (0.73); Claude Code / claude-opus-5.5 $$$$ medium (0.68) | 0.82 | 14 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; browser = driving web pages and forms; tools = multi-step work through APIs and tool connectors.

Is a higher effort worth it? One step up in effort: Artificial Analysis Intelligence Index points gained / times the list-price cost per task (a general index, in no score here; the cost of its tasks, not of our jobs). Every level: /bench.json `cost_curve`.

| model | low to medium | low to high | medium to high | high to xhigh | xhigh to max |
|---|---|---|---|---|---|
| claude-fable-5.2 | +2.5 / 1.2x | - | +5.4 / 2.4x | +0.4 / 1.6x | +2.4 / 1.8x |
| claude-opus-5.5 | +13.4 / 2.5x | - | +3.6 / 1.4x | +5.6 / 1.7x | +1.7 / 1.7x |
| claude-sonnet-5.5 | +5.2 / 1.5x | - | +10.7 / 2.1x | +8.4 / 2.5x | +4.6 / 2.4x |
| claude-haiku-5.5 | +6.0 / 2.1x | - | +5.3 / 1.7x | +4.7 / 1.6x | +1.9 / 1.7x |
| gpt-6.2-sol | +12.1 / 2.2x | - | +2.2 / 1.4x | +0.8 / 1.1x | +1.6 / 1.6x |
| gemini-4-argon | - | - | +2.8 / 1.2x | - | - |
| grok-4.7 | - | +4.1 / 2.1x | - | +0.3 / 1.3x | - |
| gemini-4-neon | +10.8 / 2.6x | - | +4.7 / 2.0x | +1.8 / 1.7x | - |

Own jobs of one model at two effort levels, per class. Not a controlled test: the effort was chosen per job. What the leaderboards gain per level: /bench.json `classes.X.effort_evidence`. No source gives tokens per level.
- coding: Claude Opus 5.5 in Claude Code: 138 of 215 finished cleanly at medium, 42 of 46 at high.
- agentic: Claude Opus 5.5 in Claude Code: 12 of 25 finished cleanly at medium, 8 of 8 at high.
- research: Claude Opus 5.5 in Claude Code: 15 of 18 finished cleanly at medium, 11 of 11 at high.
- reading: Claude Opus 5.5 in Claude Code: 19 of 22 finished cleanly at medium, 87 of 105 at high.
- writing: Claude Sonnet 5.5 in Claude Code: 16 of 18 finished cleanly at medium, 17 of 18 at high.

Where a number comes from (/bench.json): `classes.X.first_choice.inputs` (a score's inputs, each public metric with its source and link), `sources` (snapshot dates), `method.fields` (definitions).
