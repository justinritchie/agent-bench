# Multi-agent tasks: which coding agent (generated 2026-10-13)

For task class X, use the first choice; if it cannot run right now (plan limit, engine unavailable), use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1; evidence = own jobs in 28 days; full data /bench.json

| class | first choice | fallbacks | score | evidence | status |
|---|---|---|---|---|---|
| coding | Claude Code / claude-opus-5.5 | Claude Code / claude-fable-5.1 (0.80); Claude Code / claude-sonnet-5.5 (0.79) | 0.96 | 15 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 | Antigravity CLI / gpt-oss-120b (0.50) | 0.65 | 13 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 | Claude Code / claude-opus-5.5 (0.65); Antigravity CLI / claude-opus-5.5 (0.75) | 0.90 | 17 | proven |
| coding / frontend | Antigravity CLI / claude-opus-5.5 | Claude Code / claude-opus-5.5 (0.75); Claude Code / claude-sonnet-5.5 (0.68) | 0.75 | 0 | unproven |
| coding / review | Claude Code / claude-opus-5.5 | Claude Code / claude-fable-5.1 (0.58); Claude Code / claude-sonnet-5.5 (0.57) | 0.75 | 13 | proven |
| agentic | Claude Code / claude-opus-5.5 | Claude Code / claude-sonnet-5.5 (0.72); Codex CLI / gpt-6.1-sol (0.69) | 0.75 | 0 | unproven |
| agentic / terminal | Claude Code / claude-opus-5.5 | Claude Code / claude-sonnet-5.5 (0.72); Antigravity CLI / claude-opus-5.5 (0.70) | 0.73 | 0 | unproven |
| agentic / tools | Codex CLI / gpt-6.1-sol | Antigravity CLI / claude-opus-5.5 (0.66); Claude Code / claude-opus-5.5 (0.66) | 0.71 | 0 | unproven |
| research | Codex CLI / gpt-5.6-sol | Claude Code / claude-sonnet-5.5 (0.62); Claude Code / claude-haiku-5.5 (0.60) | 0.75 | 0 | unproven |
| reading | Claude Code / claude-fable-5.1 | Claude Code / claude-sonnet-5.5 (0.60); Codex CLI / gpt-6.1-sol (0.49) | 0.75 | 0 | unproven |
| writing | Claude Code / claude-sonnet-5.5 | Claude Code / claude-opus-5.5 (0.65); Antigravity CLI / claude-opus-5.5 (0.75) | 0.64 | 2 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; tools = multi-step work through APIs and tool connectors.

Plan limits are checked live when a job is dispatched; this table does not track them.
