# Multi-agent tasks: which coding agent (generated 2026-10-13)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; full data /bench.json

| class | first choice | fallbacks | score | evidence | status |
|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | Codex CLI / gpt-6.1-sol $$$ (0.63); Claude Code / claude-opus-5.5 $$$$ (0.66) | 0.82 | 44 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | Antigravity CLI / gpt-oss-120b $ (0.57) | 0.55 | 13 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | Antigravity CLI / claude-opus-5.5 $$$$ (0.68); Claude Code / claude-opus-5.5 $$$$ (0.61) | 0.79 | 17 | proven |
| coding / frontend | Claude Code / claude-opus-5.5 $$$$ | Antigravity CLI / claude-opus-5.5 $$$$ (0.68); Claude Code / claude-sonnet-5.5 $$$ (0.64) | 0.68 | 0 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | Codex CLI / gpt-6.1-sol $$$ (0.50); Codex CLI / gpt-6-astra $$$$ (0.47) | 0.71 | 12 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | Claude Code / claude-opus-5.5 $$$$ (0.68); Codex CLI / gpt-6.1-sol $$$ (0.64) | 0.68 | 0 | unproven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | Antigravity CLI / claude-sonnet-5.5 $$$ (0.65); Claude Code / claude-opus-5.5 $$$$ (0.67) | 0.68 | 0 | unproven |
| agentic / tools | Codex CLI / gpt-6.1-sol $$$ | Claude Code / claude-opus-5.5 $$$$ (0.60); Antigravity CLI / claude-opus-5.5 $$$$ (0.60) | 0.67 | 0 | unproven |
| research | Codex CLI / gpt-5.6-sol $$$ | Claude Code / claude-fable-5.1 $$$$ (0.57); Claude Code / claude-sonnet-5.5 $$$ (0.53) | 0.70 | 0 | unproven |
| reading | Claude Code / claude-fable-5.1 $$$$ | Claude Code / claude-sonnet-5.5 $$$ (0.59); Codex CLI / gpt-6.1-sol $$$ (0.47) | 0.65 | 1 | unproven |
| writing | Antigravity CLI / gemini-3.8-flash $$ | Antigravity CLI / claude-opus-5.5 $$$$ (0.68); Claude Code / claude-opus-5.5 $$$$ (0.64) | 0.67 | 0 | unproven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; tools = multi-step work through APIs and tool connectors.
