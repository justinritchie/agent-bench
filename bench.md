# Multi-agent tasks: which coding agent (generated 2026-11-02)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; effort = reasoning effort for the first choice (standing default; '(config)' = the CLI's config; '· source' = moved by a leaderboard gap of 0.03+); full data /bench.json

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-fable-5.1 $$$$ (0.76); Claude Code / claude-opus-5.5 $$$$ (0.69) | 0.74 | 100 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.35); Antigravity CLI / gpt-oss-120b $ (0.57) | 0.65 | 25 | proven |
| coding / features | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.70); Antigravity CLI / gemini-4-argon $$$ (0.70) | 0.78 | 36 | proven |
| coding / frontend | Antigravity CLI / claude-opus-5.5 $$$$ | high | Claude Code / claude-opus-5.5 $$$$ (0.59); Claude Code / claude-sonnet-5.5 $$$ (0.71) | 0.70 | 0 | unproven |
| coding / multilang | Codex CLI / gpt-6.1-sol $$$ | xhigh (config) | - | 0.50 | 1 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-fable-5.1 $$$$ (0.51); Codex CLI / gpt-6.1-sol $$$ (0.50) | 0.53 | 30 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.69); Claude Code / claude-haiku-5.5 $ (0.65) | 0.83 | 12 | proven |
| agentic / terminal | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ (0.69); Antigravity CLI / claude-sonnet-5.5 $$$ (0.65) | 0.74 | 3 | unproven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | medium | - | 0.50 | 1 | unproven |
| agentic / browser | Claude Code / claude-fable-5.1 $$$$ | medium | - | 0.50 | 1 | unproven |
| agentic / tools | Claude Code / claude-sonnet-5.5 $$$ | medium | Antigravity CLI / claude-sonnet-5.5 $$$ (0.70); Antigravity CLI / claude-opus-5.5 $$$$ (0.67) | 0.68 | 1 | unproven |
| research | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-haiku-5.5 $ (0.65); Claude Code / claude-sonnet-5.5 $$$ (0.51) | 0.79 | 58 | proven |
| reading | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-haiku-5.5 $ (0.62); Codex CLI / gpt-6.1-sol $$$ (0.57) | 0.89 | 45 | proven |
| writing | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.73); Antigravity CLI / gemini-4-argon $$$ (0.70) | 0.79 | 14 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; multilang = repo work outside Python: JS/TS, Go, Rust, Java, PHP; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; browser = driving web pages and forms; tools = multi-step work through APIs and tool connectors.

Sources (what each benchmark measures, its weight and snapshot date) and the raw base data per model: /bench.json `sources` and `base_data`.
