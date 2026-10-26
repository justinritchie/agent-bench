# Multi-agent tasks: which coding agent (generated 2026-10-26)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; effort = reasoning effort for the first choice (standing default; '(config)' = the CLI's config; '· source' = moved by a leaderboard gap of 0.03+); full data /bench.json

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.76); Codex CLI / gpt-6.1-sol $$$ (0.71) | 0.78 | 72 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / gpt-oss-120b $ (0.57); Claude Code / claude-opus-5.5 $$$$ (0.35) | 0.67 | 13 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.65); Antigravity CLI / gemini-4-argon $$$ (0.70) | 0.78 | 30 | proven |
| coding / frontend | Antigravity CLI / claude-opus-5.5 $$$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.59); Claude Code / claude-sonnet-5.5 $$$ [xhigh · Arena] (0.71) | 0.69 | 0 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | high | Codex CLI / gpt-6.1-sol $$$ (0.55); Claude Code / claude-fable-5.1 $$$$ (0.39) | 0.56 | 26 | proven |
| agentic | Claude Code / claude-opus-5.5 $$$$ | high | Claude Code / claude-sonnet-5.5 $$$ (0.64); Claude Code / claude-fable-5.1 $$$$ (0.67) | 0.68 | 0 | unproven |
| agentic / terminal | Claude Code / claude-opus-5.5 $$$$ | high | Claude Code / claude-sonnet-5.5 $$$ (0.63); Antigravity CLI / claude-sonnet-5.5 $$$ (0.66) | 0.67 | 0 | unproven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | high | - | 0.50 | 1 | unproven |
| agentic / tools | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / claude-sonnet-5.5 $$$ (0.69); Antigravity CLI / claude-opus-5.5 $$$$ (0.66) | 0.68 | 1 | unproven |
| research | Claude Code / claude-fable-5.1 $$$$ | medium | Codex CLI / gpt-6.1-sol $$$ (0.54); Claude Code / claude-sonnet-5.5 $$$ (0.49) | 0.80 | 51 | proven |
| reading | Claude Code / claude-fable-5.1 $$$$ | medium | Codex CLI / gpt-6.1-sol $$$ (0.64); Claude Code / claude-sonnet-5.5 $$$ (0.51) | 0.92 | 41 | proven |
| writing | Claude Code / claude-opus-5.5 $$$$ | high | Claude Code / claude-fable-5.1 $$$$ (0.76); Claude Code / claude-sonnet-5.5 $$$ (0.59) | 0.88 | 13 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; tools = multi-step work through APIs and tool connectors.

Sources (what each benchmark measures, its weight and snapshot date) and the raw base data per model: /bench.json `sources` and `base_data`.
