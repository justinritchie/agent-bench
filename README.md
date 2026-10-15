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
- Evidence first: Proven means at least 5 own jobs in the window. An unproven entry ranks above a proven one only with a clearly better public score, never on cost or speed alone, and leads at all only with a public score within 0.05 of the best.

Only aggregate job counts, success rates and median minutes are published; no prompts, job details, grades or dollar amounts.

## Public sources

- [Terminal-Bench 4.0](https://www.tbench.ai/): terminal tasks an agent completes
- [SWE-bench Verified](https://www.swebench.com/verified.html): real repo issues resolved
- [SWE-bench Multilingual](https://www.swebench.com/multilingual.html): repo issues resolved in nine languages
- [Artificial Analysis coding index](https://artificialanalysis.ai/): composite coding score
- [Arena Text: coding](https://arena.ai/leaderboard/text): people's votes on coding prompts
- [Arena WebDev](https://arena.ai/leaderboard/webdev): people's votes on built web apps
- [Artificial Analysis agentic index](https://artificialanalysis.ai/): composite agentic score
- [Arena Agent: bash reliability](https://arena.ai/blog/agent-arena-methodology/): shell work in real agent sessions
- [Arena Agent: bash recovery](https://arena.ai/blog/agent-arena-methodology/): recovering from a failed shell command
- [Arena Agent: tool calls](https://arena.ai/blog/agent-arena-methodology/): not calling tools that do not exist
- [Arena Agent: task outcome](https://arena.ai/blog/agent-arena-methodology/): users marking the task done
- [DeepResearch Bench](https://deepresearch-bench.github.io/): long research reports
- [Arena Search](https://arena.ai/leaderboard/search): people's votes on search answers
- [Arena Document](https://arena.ai/leaderboard/document): people's votes on answers about PDFs
- [Arena Text: creative writing](https://arena.ai/leaderboard/text): people's votes on creative writing
- [Arena Text](https://arena.ai/leaderboard/text): people's votes on all text prompts
- [Artificial Analysis output speed](https://artificialanalysis.ai/methodology): output tokens per second
- [OpenRouter prices](https://openrouter.ai/models): list price per token
