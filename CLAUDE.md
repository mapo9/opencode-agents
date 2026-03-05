# Project Instructions

## Agent System

This project uses a multi-agent workflow via custom slash commands. Configuration is staged in `claude/` and deployed to `~/.claude/` for system-wide use.

### Router Commands (start here)
- `/docs` — Routes documentation tasks to the right specialist (docs-writer or agent-architect)
- `/code` — Routes coding tasks by complexity (junior / senior / architect)

### Direct Specialist Commands
- `/docs-writer` — Write end-user documentation (READMEs, guides) [haiku-optimized]
- `/nextflow-docs` — nf-core pipeline documentation [haiku-optimized]
- `/agent-architect` — Design agent systems and AGENTS.md (read-only analysis)
- `/code-review` — Review code for issues (read-only analysis)
- `/junior` — Small, single-file changes [haiku-optimized]
- `/senior` — Multi-file refactors and debugging
- `/architect` — System design and high-stakes changes

### Model Notes
Commands marked [haiku-optimized] were designed for lighter/cheaper models in the original opencode.json config. All others target sonnet-class capability. Claude Code uses a single model per session — switch models if cost matters for bulk documentation or simple tasks.

## Git Workflow
Follow the conventions in AGENTS.md for branching, commits, and pull requests.
