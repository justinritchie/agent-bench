# Multi-agent tasks: which coding agent

Which engine, model and reasoning effort to send a job to, and the fallback. Generated 2026-11-20 UTC, rebuilt about weekly; source snapshots 2026-11-20 to 2026-11-20; own jobs: the 28 days before. First choices changed since 2026-11-13: agentic claude-haiku-5.5 -> claude-sonnet-5.5; writing Antigravity CLI / gemini-4-argon -> Claude Code / claude-fable-5.2; coding / multilang Codex CLI / gpt-6.1-sol -> none; and 2 more (/bench.json `changes`).

For task class X, use the first choice; if it cannot run right now, the next fallback, in the order listed. The order is the ranking: with few own jobs, the evidence and tie rules can put a lower score first. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; probation = a new model version counting its predecessor's jobs and public scores for 28 days; effort = the reasoning effort to run at, lowest to highest low, medium, high, xhigh, max (a fallback's follows its cost tier; '(config)' = the CLI's own config; '· source' = moved by a leaderboard gap of 0.03+).

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | medium | Codex CLI / gpt-6.2-sol $$$ xhigh (config) (0.79); Claude Code / claude-opus-5.5 $$$$ medium (0.70) | 0.81 | 77 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.52); Antigravity CLI / gpt-oss-120b $ medium (0.57) | 0.68 | 25 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.70); Antigravity CLI / gemini-4-neon $$$$ high (0.72) | 0.77 | 11 | proven |
| coding / frontend | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.58); Antigravity CLI / claude-opus-5.5 $$$$ high (0.71) | 0.65 | 6 | probation |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.48); Codex CLI / gpt-6.2-sol $$$ xhigh (config) (0.51) | 0.54 | 9 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-haiku-5.5 $ high (0.71); Claude Code / claude-fable-5.2 $$$$ medium (0.67) | 0.70 | 65 | proven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ medium (0.72); Claude Code / claude-haiku-5.5 $ high (0.67) | 0.78 | 10 | proven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | medium | - | 0.50 | 2 | unproven |
| agentic / browser | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.42) | 0.57 | 1 | unproven |
| agentic / tools | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.2 $$$$ medium (0.57); Antigravity CLI / gemini-4-neon $$$$ high (0.61) | 0.55 | 5 | proven |
| research | Claude Code / claude-fable-5.2 $$$$ | medium | Codex CLI / gpt-6.2-sol $$$ xhigh (config) (0.64); Claude Code / claude-sonnet-5.5 $$$ medium (0.59) | 0.74 | 31 | probation |
| reading | Claude Code / claude-fable-5.2 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ medium (0.63); Claude Code / claude-haiku-5.5 $ high (0.60) | 0.73 | 38 | probation |
| writing | Claude Code / claude-fable-5.2 $$$$ | medium | Antigravity CLI / gemini-4-argon $$$ high (0.76); Claude Code / claude-opus-5.5 $$$$ medium (0.69) | 0.76 | 76 | probation |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; browser = driving web pages and forms; tools = multi-step work through APIs and tool connectors.

Is a higher effort worth it? One step up in effort: Artificial Analysis Intelligence Index points gained / times the list-price cost per task (a general index, in no score here; the cost of its tasks, not of our jobs). Every level: /bench.json `cost_curve`.

| model | low to medium | medium to high | high to xhigh | xhigh to max |
|---|---|---|---|---|
| claude-fable-5.2 | +2.5 / 1.2x | +5.4 / 2.4x | +0.4 / 1.6x | +2.4 / 1.8x |
| claude-opus-5.5 | +13.4 / 2.5x | +3.6 / 1.4x | +5.6 / 1.7x | +1.7 / 1.7x |
| claude-sonnet-5.5 | +5.2 / 1.5x | +10.7 / 2.1x | +8.4 / 2.5x | +4.6 / 2.4x |
| claude-haiku-5.5 | +6.0 / 2.1x | +5.3 / 1.7x | +4.7 / 1.6x | +1.9 / 1.7x |
| gpt-6.2-sol | +12.1 / 2.2x | +2.2 / 1.4x | +0.8 / 1.1x | +1.6 / 1.6x |
| gemini-4-argon | - | +2.8 / 1.2x | - | - |
| gemini-4-neon | +10.8 / 2.6x | +4.7 / 2.0x | +1.8 / 1.7x | - |

Own jobs of one model at two effort levels, per class. Not a controlled test: the effort was chosen per job. What the leaderboards gain per level: /bench.json `classes.X.effort_evidence`. No source gives tokens per level.
- coding: Claude Opus 5.5 in Claude Code: 134 of 187 finished cleanly at medium, 41 of 43 at high.
- agentic: Claude Opus 5.5 in Claude Code: 10 of 22 finished cleanly at medium, 8 of 8 at high.
- research: Claude Opus 5.5 in Claude Code: 14 of 16 finished cleanly at medium, 12 of 12 at high.
- reading: Claude Opus 5.5 in Claude Code: 16 of 19 finished cleanly at medium, 77 of 91 at high.
- writing: Claude Sonnet 5.5 in Claude Code: 15 of 16 finished cleanly at medium, 16 of 17 at high.

Where a number comes from (/bench.json): `classes.X.first_choice.inputs` (a score's inputs, each public metric with its source and link), `sources` (snapshot dates), `method.fields` (definitions).
