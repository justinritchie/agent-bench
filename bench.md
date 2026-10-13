# Agent routing benchmark, generated 2026-10-13: for task class X, use the first choice unless it is gated, else the next fallback. score 0-1; evidence = own jobs in 28 days; full data /bench.json

| class | first choice | fallbacks | score | evidence | status |
|---|---|---|---|---|---|
| coding | Claude Code / claude-opus-5.5 | Claude Code / claude-fable-5.1 (0.80); Claude Code / claude-sonnet-5.5 (0.79) | 0.96 | 15 | proven |
| agentic | Claude Code / claude-opus-5.5 | Claude Code / claude-sonnet-5.5 (0.72); Codex CLI / gpt-6.1-sol (0.69) | 0.75 | 0 | unproven |
| research | Codex CLI / gpt-5.6-sol | Claude Code / claude-sonnet-5.5 (0.62); Claude Code / claude-haiku-5.5 (0.60) | 0.75 | 0 | unproven |
| reading | Claude Code / claude-fable-5.1 | Claude Code / claude-sonnet-5.5 (0.60); Codex CLI / gpt-6.1-sol (0.49) | 0.75 | 0 | unproven |
| writing | Claude Code / claude-sonnet-5.5 | Claude Code / claude-opus-5.5 (0.65); Antigravity CLI / claude-opus-5.5 (0.75) | 0.64 | 2 | proven |

## Usage

| engine | seat | 5h used | weekly used | weekly resets | status |
|---|---|---|---|---|---|
| Claude Code | seat 1 | 5% | 22% | 2026-10-19T05:00 | ok |
| Claude Code | seat 2 | 0% | 77% | 2026-10-15T15:00 | ok |
| Claude Code | seat 3 | 69% | 9% | 2026-10-17T02:00 | ok |
| Codex CLI | seat 1 | 15% | 5% | 2026-10-20T06:37 | ok |
| Antigravity CLI | gemini models | 0% | 0% | 2026-10-20T20:02 | ok |
| Antigravity CLI | claude and gpt models | 0% | 0% | 2026-10-20T20:02 | ok |
| Grok CLI | seat 1 | - | - | - | no reading |

## Feeds

| source | fetched | status | url |
|---|---|---|---|
| Terminal-Bench 4.0 | 2026-10-13 | ok | https://github.com/harbor-framework/terminal-bench/blob/main/leaderboard/leaderboard.yaml |
| SWE-bench | 2026-10-13 | ok | https://www.swebench.com/ |
| DeepResearch Bench | 2026-10-13 | ok | https://huggingface.co/spaces/muset-ai/DeepResearch-Bench-Leaderboard |
| Arena (text, document, search) | 2026-10-13 | ok | https://arena.ai/leaderboard |
| Artificial Analysis | - | no data | https://artificialanalysis.ai/ |
