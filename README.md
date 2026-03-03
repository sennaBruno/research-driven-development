# research-driven-development

A Claude Code skill that enforces research-validated development across the full product lifecycle.

## What This Does

This skill adds **mandatory research and validation gates** to every phase of development. No code gets written without first researching best practices, validating findings against multiple sources, and creating research-informed specifications.

### The Pipeline

```
RESEARCH → VALIDATE → PLAN → IMPLEMENT → REVIEW → VERIFY → DELIVER
```

Each phase produces an artifact. Each artifact is validated before the next phase begins. Phases cannot be skipped.

## Why This Exists

Most AI coding workflows jump straight from idea to implementation. This leads to:
- Wrong technology choices discovered too late
- Patterns that contradict community best practices
- Architectures that don't fit the existing codebase
- Costly rework when better approaches existed all along

Research-Driven Development fixes this by making research the **foundation** of every decision.

## What Makes This Different

This skill **orchestrates** existing skills (superpowers TDD, code review, verification, etc.) while adding the missing pieces:

- **Mandatory research** before any planning or implementation
- **Multi-source validation** against community best practices
- **Research-informed specs** (plans reference findings, not assumptions)
- **Model routing** based on task complexity (ACR scoring)
- **Full lifecycle coverage** including delivery and infrastructure
- **Explicit quality gates** between every phase

## Installation

### Claude Code

```bash
# Copy the skill to your Claude Code skills directory
mkdir -p ~/.claude/skills/research-driven-development
cp SKILL.md ~/.claude/skills/research-driven-development/
```

### Other AI Coding Tools

This skill follows the open SKILL.md standard and is compatible with:
- Claude Code
- OpenAI Codex CLI
- Gemini CLI
- Cursor
- Any tool supporting SKILL.md format

## Companion Skills

This skill works best with:
- [superpowers](https://github.com/obra/superpowers) — Core development skills (TDD, debugging, planning, code review)
- [estimating-agent-tasks](https://github.com/sennaBruno/estimating-agent-tasks) — ACR complexity scoring for model selection

## Research Sources

This skill was designed based on extensive research of community patterns and industry best practices:

- [Anthropic 2026 Agentic Coding Trends Report](https://resources.anthropic.com/2026-agentic-coding-trends-report)
- [Spec-Driven Development (GitHub)](https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/)
- [How to Write a Good Spec for AI Agents (Addy Osmani)](https://addyosmani.com/blog/good-spec/)
- [Multi-Agent Workflows That Don't Fail (GitHub Blog)](https://github.blog/ai-and-ml/generative-ai/multi-agent-workflows-often-fail-heres-how-to-engineer-ones-that-dont/)
- [Agentic Workflows for Software Development (McKinsey/QuantumBlack)](https://medium.com/quantumblack/agentic-workflows-for-software-development-dc8e64f4a79d)
- [Quality Gates for AI Code Reviews (CodeRabbit)](https://www.coderabbit.ai/blog/coderabbit-series-b-60-million-quality-gates-for-code-reviews)

Community frameworks studied: Metaswarm, Spec-Flow, cc-sdd, sudocode, gbFinch/agentic-orchestration, Conductor-Orchestrator, Claude-Octopus, wshobson/agents, and 10+ others.

## License

MIT
