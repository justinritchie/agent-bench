# Multi-agent tasks: which coding agent (generated 2026-10-19)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; effort = reasoning effort for the first choice (standing default; '(config)' = the CLI's config; '· source' = moved by a leaderboard gap of 0.03+); full data /bench.json

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.76); Codex CLI / gpt-6.1-sol $$$ (0.62) | 0.77 | 59 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / gpt-oss-120b $ (0.57); Claude Code / claude-opus-5.5 $$$$ (0.35) | 0.65 | 13 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / gemini-4-argon $$$ (0.71); Antigravity CLI / claude-opus-5.5 $$$$ (0.69) | 0.78 | 26 | proven |
| coding / frontend | Antigravity CLI / claude-opus-5.5 $$$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.59); Claude Code / claude-sonnet-5.5 $$$ [xhigh · Arena] (0.71) | 0.69 | 0 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | high | Codex CLI / gpt-6.1-sol $$$ (0.47); Claude Code / claude-fable-5.1 $$$$ (0.39) | 0.61 | 18 | proven |
| agentic | Claude Code / claude-opus-5.5 $$$$ | high | Claude Code / claude-sonnet-5.5 $$$ (0.71); Codex CLI / gpt-6.1-sol $$$ (0.67) | 0.70 | 0 | unproven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.69); Antigravity CLI / claude-sonnet-5.5 $$$ (0.69) | 0.71 | 0 | unproven |
| agentic / tools | Codex CLI / gpt-6.1-sol $$$ | xhigh (config) | Antigravity CLI / claude-opus-5.5 $$$$ (0.67); Claude Code / claude-opus-5.5 $$$$ (0.66) | 0.69 | 0 | unproven |
| research | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ (0.49); Codex CLI / gpt-6.1-sol $$$ (0.40) | 0.57 | 42 | proven |
| reading | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ (0.41); Codex CLI / gpt-6.1-sol $$$ (0.36) | 0.91 | 27 | proven |
| writing | Claude Code / claude-sonnet-5.5 $$$ | high | Antigravity CLI / gemini-4-argon $$$ (0.68); Claude Code / claude-fable-5.1 $$$$ (0.65) | 0.65 | 10 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; tools = multi-step work through APIs and tool connectors.

Sources (what each benchmark measures, its weight and snapshot date) and the raw base data per model: /bench.json `sources` and `base_data`.
