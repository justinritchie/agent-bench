# Multi-agent tasks: which coding agent

A weekly routing table for multi-agent work: which coding-agent CLI (Claude Code, Codex CLI, Antigravity CLI, Grok CLI) and model to use for five task classes (coding, agentic, research, reading, writing), with coding and agentic work also ranked by kind (for example bug fixing, frontend, terminal work). This repository holds the generated site; it is refreshed weekly.

## Files

- `index.html`: the page for people.
- `bench.md`: compact Markdown table for agents; start here.
- `bench.json`: every ranked candidate with its scoring inputs and the method (schema_version 6).
- `llms.txt`: pointers for language models.
- `history/`: one `bench.json` snapshot per week.

## How the ranking works

`priority = 0.45*public_norm + 0.25*own_success + 0.15*speed_rank + 0.15*cost_rank` (weights public 0.45, own success 0.25, speed 0.15, cost 0.15; every input 0-1).

- Public: results from public leaderboards for the models each CLI runs, scaled across the candidates; a score measured in another agent's harness counts at 0.8x.
- Own success: aggregate outcomes of our own dispatched jobs over the last 28 days, with quality from a weekly random sample of jobs graded against their own instructions.
- Speed: median minutes of our own jobs, else a public output-speed figure.
- Cost: estimated list-price cost per successful job, ranked on a log scale; the $ to $$$$ tier is the model's list price alone.
- Evidence first: Proven means at least 5 own jobs in the window. An unproven entry ranks above a proven one only with a clearly better public score, never on cost or speed alone.

Only aggregate job counts, success rates and median minutes are published; no prompts, job details, grades or dollar amounts.

## Public sources

- [Terminal-Bench 4.0](https://github.com/harbor-framework/terminal-bench/blob/main/leaderboard/leaderboard.yaml)
- [SWE-bench](https://www.swebench.com/)
- [DeepResearch Bench](https://huggingface.co/spaces/muset-ai/DeepResearch-Bench-Leaderboard)
- [Arena (text, document, search, webdev, agent)](https://arena.ai/leaderboard)
- [OpenRouter model prices](https://openrouter.ai/api/v1/models)
