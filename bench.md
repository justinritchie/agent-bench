# Multi-agent tasks: which coding agent (generated 2026-10-13)

For task class X, use the first choice; if it cannot run right now (plan limit, engine unavailable), use the next fallback. score 0-1; evidence = own jobs in 28 days; full data /bench.json

| class | first choice | fallbacks | score | evidence | status |
|---|---|---|---|---|---|
| coding | Claude Code / claude-opus-5.5 | Claude Code / claude-fable-5.1 (0.80); Claude Code / claude-sonnet-5.5 (0.79) | 0.96 | 15 | proven |
| agentic | Claude Code / claude-opus-5.5 | Claude Code / claude-sonnet-5.5 (0.72); Codex CLI / gpt-6.1-sol (0.69) | 0.75 | 0 | unproven |
| research | Codex CLI / gpt-5.6-sol | Claude Code / claude-sonnet-5.5 (0.62); Claude Code / claude-haiku-5.5 (0.60) | 0.75 | 0 | unproven |
| reading | Claude Code / claude-fable-5.1 | Claude Code / claude-sonnet-5.5 (0.60); Codex CLI / gpt-6.1-sol (0.49) | 0.75 | 0 | unproven |
| writing | Claude Code / claude-sonnet-5.5 | Claude Code / claude-opus-5.5 (0.65); Antigravity CLI / claude-opus-5.5 (0.75) | 0.64 | 2 | proven |

Plan limits are checked live when a job is dispatched; this table does not track them.
