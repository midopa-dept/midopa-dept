[한국어](README.md) · English

# Junha Kang

Security practitioner and independent researcher. I build an agent runner for models you host yourself, and study how such runners should be measured.

## stewart

**A small agent runner that lets a model you host work on a local folder** · [repository](https://github.com/midopa-dept/stewart)

[![stewart hub: reproducing and fixing a checkout-total bug](https://github.com/midopa-dept/stewart/raw/main/docs/images/hero.en.png)](https://github.com/midopa-dept/stewart/blob/main/docs/demo.en.md)

- Connects to any OpenAI-compatible server (llama.cpp, vLLM) or the Anthropic Messages API.
- Runs in a browser hub (several conversations, branches and workers) or the terminal (`stewart chat`).
- A hub on an external API can run as its own named instance, with separate settings, state and memory, inside a macOS sandbox.
- Workdir bounds and approvals, memory and skills, and two-stage context compaction (mask old tool results, then summarize).
- With the same Claude model on the same tasks, it used 0.69–0.77× the cost per run and 0.72–0.80× the time of Claude Code, with no meaningful difference in success rate. This was an exploratory measurement on 16 of our own tasks, not a general performance claim.

[README](https://github.com/midopa-dept/stewart/blob/main/README.en.md) · [Demo screens](https://github.com/midopa-dept/stewart/blob/main/docs/demo.en.md) · [Research notes (Korean)](https://github.com/midopa-dept/stewart/blob/main/docs/research-notes.md)

Companion tool [stewart-cloud](https://github.com/midopa-dept/stewart-cloud) (v0.2.1): rent a GPU on Vast.ai, serve an open model with vLLM, reach it only from your own Tailscale network, and connect it to stewart.

## Current interests

- Runner design for small and local models: covering for a weak model with mechanisms on the runner side
- How to measure runners: plans written down in advance (preregistration), baselines, side-by-side runs on the same model
- Agents that improve from their own records: learning from run logs, and fine-tuning (in progress)
- Safety rails and isolation for agents that run shell commands
- Teaching local LLM use on air-gapped PCs (published textbook: local-ai-textbook)

## Other repositories

- [cairn-harness](https://github.com/midopa-dept/cairn-harness): a small declarative contract for projects where LLM agents change code over long periods (authority, task state, verification and acceptance, evidence, recovery after interruption). Release candidate `1.0.0-candidate.5`.
- [agent-workspace-hardening](https://github.com/midopa-dept/agent-workspace-hardening): managed settings and a git-guard hook that narrow what coding agents can reach on a personal Mac, with test findings on where permission rules did not behave as expected.
- [education-harness](https://github.com/midopa-dept/education-harness): rules for producing course material with coding agents, learned from building one two-day course where security practitioners run a local LLM on PCs without internet access.
- [local-ai-textbook](https://github.com/midopa-dept/local-ai-textbook): the textbook from that course (Korean, 161 pages). Exercises use a small model running on your own PC, and practice checking AI answers against source material.
- [ai-knowledge-atlas](https://github.com/midopa-dept/ai-knowledge-atlas): knowledge graph for a Korean non-linear AI textbook (504 concepts, 817 learning objectives) with validators, plus its first chapter (Attention and Transformer) as a review candidate.

Most documents are written in Korean. Every repository above except local-ai-textbook has an English README.

ORCID: https://orcid.org/0009-0006-9062-8353