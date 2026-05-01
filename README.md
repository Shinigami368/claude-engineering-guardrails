# Claude Component Library

This repository is a plug-and-play Claude component library.

Browse the categorized source tree here, then copy only the components you
actually want into your own flat `~/.claude/` setup.

It is not a platform, not a starter app, and not a runtime workspace.
Do not run normal Claude sessions from this repository root.

## Why This Repository Exists

This repository is a depot and reference template for AI workflow components. It is not meant to be copied wholesale. Instead, it is designed to help you browse, select, and adapt useful skills, agents, hooks, rules, commands, and tips into your own AI-tooling setup or Claude-compatible configuration.

The components here reflect my local setup, real usage patterns, and the workflows I have built around day-to-day AI-assisted work. Some skills, agents, and hooks are actively used in my own setup; others were created, refined, and kept available as reusable starting points for future needs.

This repository was built and refined with AI assistance, but the practical direction, workflow ideas, structure, and operating principles come from my own long-term experience using AI tools in real work.

In my opinion, one of the most valuable parts of this repository is [TIPS.md](./TIPS.md). It contains practical lessons, habits, and mindset notes collected from years of working with AI tools. I hope it helps others avoid common mistakes, build a cleaner setup, and use AI tools more effectively.

Although the repository is organized around Claude-compatible components, many of the ideas, workflows, and operating principles can also be adapted to other AI coding tools and agentic workflows.

If you find this useful, have suggestions, or want to discuss AI-assisted workflows, you are welcome to contact me. Feedback, improvements, and practical recommendations are always appreciated.

## Start Here

1. Read [QUICKSTART.md](./QUICKSTART.md).
2. Read [TIPS.md](./TIPS.md) before installing many components globally.
3. Use [docs/recommended-components.md](./docs/recommended-components.md) to choose a starter set by role.
4. Use [docs/use-cases.md](./docs/use-cases.md) to choose by scenario.
5. Use [docs/skill-index.md](./docs/skill-index.md), [docs/agent-index.md](./docs/agent-index.md), [docs/command-index.md](./docs/command-index.md), [docs/hook-index.md](./docs/hook-index.md), and [docs/rule-index.md](./docs/rule-index.md) when you want the full catalog.

## Copy Model

- Source tree is categorized for browsing:
  - skills: `.claude/skills/<domain>/<skill-name>/`
  - agents: `.claude/agents/<domain>/<agent-name>.md`
- Install destination is flat in your own Claude setup:
  - skills: `~/.claude/skills/<skill-name>/`
  - agents: `~/.claude/agents/<agent-name>.md`
  - commands, rules, and most settings: flat files under `~/.claude/`
- Copy skills as whole directories.
- Copy agents, commands, and rules as files.
- Hooks and settings are optional. Enable them carefully and keep human approval for risky actions.
- Some business and self-improvement components can optionally create local context files such as `.claude/product-marketing-context.md`, `.claude/industry-context.md`, or `.claude/knowledge/`. These are user-owned local state in your own setup, not required repo files, and should stay uncommitted by default.
- Do not bulk-copy the entire catalog. Keep your active Claude setup small and maintainable.

## Copy Examples

```bash
mkdir -p ~/.claude/skills ~/.claude/agents ~/.claude/commands ~/.claude/rules

cp -R .claude/skills/meta-catalog/repo-navigator ~/.claude/skills/repo-navigator
cp .claude/agents/engineering/developer.md ~/.claude/agents/developer.md
cp .claude/commands/node-task.md ~/.claude/commands/node-task.md
```

## Docs Map

- Public user docs: [QUICKSTART.md](./QUICKSTART.md), [TIPS.md](./TIPS.md), [docs/getting-started.md](./docs/getting-started.md), [docs/recommended-components.md](./docs/recommended-components.md), [docs/use-cases.md](./docs/use-cases.md), and the catalog indexes under [`docs/`](./docs)
- Component authoring guidance: [docs/authoring/skill-authoring-checklist.md](./docs/authoring/skill-authoring-checklist.md)
- Governance/reference docs: [docs/governance/](./docs/governance/)
