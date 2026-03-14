# Claude Code Integration

The Agency was built for Claude Code. No conversion needed — agents work
natively with the existing `.md` + YAML frontmatter format.

## Install

```bash
# Clone the repo
git clone https://github.com/msitarzewski/agency-agents
cd agency-agents

# Install all agents to ~/.claude/agents/
./scripts/install.sh --tool claude-code

# Or manually copy a specific category
cp engineering/*.md ~/.claude/agents/
cp design/*.md ~/.claude/agents/
```

## Activate an Agent

In any Claude Code session, reference an agent by name:

```
Use the Frontend Developer agent to help me build a React component.
```

```
Activate the Reality Checker and verify this feature is production-ready.
```

```
Switch to the Backend Architect to design this API.
```

```
Use the Security Engineer to review this authentication code.
```

Claude Code will automatically load the matching agent from `~/.claude/agents/`
and adopt its persona, workflows, and communication style for the session.

## Agent Directory

Agents are organized into divisions. See the [main README](../../README.md) for
the full current roster.

| Division | Directory |
|----------|-----------|
| Engineering | `engineering/` |
| Design | `design/` |
| Marketing | `marketing/` |
| Paid Media | `paid-media/` |
| Sales | `sales/` |
| Product | `product/` |
| Project Management | `project-management/` |
| Testing | `testing/` |
| Support | `support/` |
| Spatial Computing | `spatial-computing/` |
| Game Development | `game-development/` |
| Specialized | `specialized/` |
