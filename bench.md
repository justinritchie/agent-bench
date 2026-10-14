# Multi-agent tasks: which coding agent (generated 2026-10-14)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; effort = reasoning effort for the first choice (standing default; '(config)' = the CLI's config; '· source' = moved by a leaderboard gap of 0.03+); full data /bench.json

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | high | Codex CLI / gpt-6.1-sol $$$ (0.65); Claude Code / claude-opus-5.5 $$$$ (0.67) | 0.86 | 46 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / gpt-oss-120b $ (0.57) | 0.55 | 13 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / claude-opus-5.5 $$$$ (0.67); Claude Code / claude-opus-5.5 $$$$ (0.61) | 0.79 | 18 | proven |
| coding / frontend | Claude Code / claude-opus-5.5 $$$$ | high | Antigravity CLI / claude-opus-5.5 $$$$ (0.67); Claude Code / claude-sonnet-5.5 $$$ [xhigh · Arena] (0.64) | 0.68 | 0 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | high | Codex CLI / gpt-6.1-sol $$$ (0.52); Claude Code / claude-fable-5.1 $$$$ (0.42) | 0.72 | 13 | proven |
| agentic | Claude Code / claude-opus-5.5 $$$$ | high | Claude Code / claude-sonnet-5.5 $$$ (0.74); Codex CLI / gpt-6.1-sol $$$ (0.70) | 0.71 | 0 | unproven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.70); Antigravity CLI / claude-sonnet-5.5 $$$ (0.68) | 0.73 | 0 | unproven |
| agentic / tools | Codex CLI / gpt-6.1-sol $$$ | xhigh (config) | Claude Code / claude-opus-5.5 $$$$ (0.57); Antigravity CLI / claude-opus-5.5 $$$$ (0.54) | 0.71 | 0 | unproven |
| research | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ (0.49); Codex CLI / gpt-6.1-sol $$$ (0.38) | 0.54 | 30 | proven |
| reading | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-fable-5.1 $$$$ (0.65); Codex CLI / gpt-6.1-sol $$$ (0.51) | 0.65 | 5 | proven |
| writing | Claude Code / claude-opus-5.5 $$$$ | high | Antigravity CLI / claude-opus-5.5 $$$$ (0.67); Claude Code / claude-fable-5.1 $$$$ (0.66) | 0.69 | 2 | unproven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; tools = multi-step work through APIs and tool connectors.
