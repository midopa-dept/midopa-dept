# Junha Kang

Independent researcher. I work on how coding agents can take on long-running work with clear limits: what they can reach, when work counts as done, and what evidence is left behind.

## Interests

- Agentic software engineering: specification for agent workflows (authority, task state, verification, acceptance)
- Reliability of AI-assisted work: independent review, evidence, recovery after interruption
- Security for coding agents and for local LLMs in air-gapped environments

## Projects

### Agent workflows

| Repository | What it shows |
| --- | --- |
| [cairn-harness](https://github.com/midopa-dept/cairn-harness) | A small declarative contract that Claude Code and Codex follow for authority, task state, verification, acceptance, and recovery. Release candidate (`1.0.0-candidate.5`), observed on a small cross-runtime fixture; the design notes keep the review history behind it. |
| [agent-workspace-hardening](https://github.com/midopa-dept/agent-workspace-hardening) | Managed settings and a git-guard hook that narrow what coding agents can reach on a personal Mac, with test findings on where permission rules did not behave as expected. Tested on specific tool versions. |

### Learning material

| Repository | What it shows |
| --- | --- |
| [education-harness](https://github.com/midopa-dept/education-harness) | Rules for producing course material with coding agents (textbook, slides, scripts, assessment, offline delivery), learned from building one real air-gapped course. |
| [local-ai-textbook](https://github.com/midopa-dept/local-ai-textbook) | The textbook from that course (Korean, 161 pages): information-security practitioners run a small local LLM on offline Windows PCs and learn to check its answers against sources, up to tool calling, agents, and harnesses. |
| [ai-knowledge-atlas](https://github.com/midopa-dept/ai-knowledge-atlas) | Knowledge graph and learning objectives for a Korean AI textbook in progress, with standard-library validators and tests, plus its first chapter (Attention and Transformer) as a review candidate. |

Most documents are written in Korean. Every repository above except local-ai-textbook has an English README.

ORCID: https://orcid.org/0009-0006-9062-8353
