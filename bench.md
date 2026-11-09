# Multi-agent tasks: which coding agent (generated 2026-11-09)

For task class X, use the first choice; if it cannot run right now, use the next fallback. A `class / kind` row ranks one kind of coding or agentic work; prefer it when the task clearly fits. score 0-1 (cheaper wins when quality is close); $-$$$$ = list-price cost tier; evidence = own jobs in 28 days; proven = at least 5; effort = reasoning effort for the first choice (standing default; '(config)' = the CLI's config; '· source' = moved by a leaderboard gap of 0.03+); full data /bench.json

| class | first choice | effort | fallbacks | score | evidence | status |
|---|---|---|---|---|---|---|
| coding | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.73); Claude Code / claude-fable-5.1 $$$$ (0.75) | 0.75 | 83 | proven |
| coding / bugfix | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.45); Antigravity CLI / gpt-oss-120b $ (0.57) | 0.66 | 33 | proven |
| coding / features | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.75); Claude Code / claude-sonnet-5.5 $$$ (0.74) | 0.79 | 11 | proven |
| coding / frontend | Claude Code / claude-opus-5.5 $$$$ | medium | Antigravity CLI / claude-opus-5.5 $$$$ (0.70); Antigravity CLI / claude-sonnet-5.5 $$$ (0.66) | 0.75 | 3 | unproven |
| coding / multilang | Codex CLI / gpt-6.1-sol $$$ | xhigh (config) | - | 0.50 | 1 | unproven |
| coding / review | Claude Code / claude-sonnet-5.5 $$$ | medium | Codex CLI / gpt-6.1-sol $$$ (0.49); Claude Code / claude-fable-5.1 $$$$ (0.51) | 0.54 | 21 | proven |
| agentic | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-haiku-5.5 $ (0.78); Claude Code / claude-opus-5.5 $$$$ (0.64) | 0.84 | 14 | proven |
| agentic / terminal | Claude Code / claude-sonnet-5.5 $$$ | medium | Claude Code / claude-opus-5.5 $$$$ (0.66); Antigravity CLI / claude-sonnet-5.5 $$$ (0.65) | 0.85 | 10 | proven |
| agentic / data | Claude Code / claude-sonnet-5.5 $$$ | medium | - | 0.50 | 1 | unproven |
| agentic / browser | Claude Code / claude-opus-5.5 $$$$ | medium | Claude Code / claude-fable-5.1 $$$$ (0.42) | 0.57 | 1 | unproven |
| agentic / tools | Claude Code / claude-sonnet-5.5 $$$ | medium | Antigravity CLI / claude-sonnet-5.5 $$$ (0.69); Antigravity CLI / claude-opus-5.5 $$$$ (0.66) | 0.67 | 1 | unproven |
| research | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-haiku-5.5 $ (0.65); Codex CLI / gpt-6.1-sol $$$ (0.54) | 0.80 | 43 | proven |
| reading | Claude Code / claude-fable-5.1 $$$$ | medium | Claude Code / claude-sonnet-5.5 $$$ (0.59); Claude Code / claude-haiku-5.5 $ (0.62) | 0.92 | 44 | proven |
| writing | Claude Code / claude-fable-5.1 $$$$ | medium | Antigravity CLI / gemini-4-argon $$$ (0.81); Claude Code / claude-opus-5.5 $$$$ (0.67) | 0.81 | 15 | proven |

Kinds: bugfix = finding and fixing defects in existing code; features = new features, tools and restructuring; frontend = web pages, UI components and styling; multilang = repo work outside Python: JS/TS, Go, Rust, Java, PHP; review = code review, audits and tests; terminal = shell, installs, configuration, server upkeep; data = data processing and one-off scripts; browser = driving web pages and forms; tools = multi-step work through APIs and tool connectors.

Sources (what each benchmark measures, its weight and snapshot date) and the raw base data per model: /bench.json `sources` and `base_data`.
