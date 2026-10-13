# Agent Bench

A living benchmark of how we route work across coding agents (Claude Code, Codex, Antigravity, Grok), refreshed weekly.

Each week a script combines public benchmark results with aggregate outcomes from our own dispatched jobs and each engine's plan usage, ranks the engines for a handful of task kinds, and commits the result here. Cloudflare Pages publishes it at https://bench.jritchie.com.

- `index.html`: the readable page.
- `bench.json`: the same data for agents to read.
- `history/`: one snapshot per week.

Nothing here describes the work itself: no prompts, job names, file paths, clients or accounts. Only engine and model names, public benchmark figures with their sources, and aggregate counts and rates.
