# Protomota agent skills

Skills that teach Claude Code and Codex how to install and use the MCP servers in
Protomota's Mac apps. Each skill covers setup (Claude Code first, Codex second), the
available tools, and safe day-to-day use.

| Skill | App | What it does |
| --- | --- | --- |
| [`jotley-mcp`](skills/jotley-mcp/SKILL.md) | [Jotley](https://jotley.ai) | Find, read, edit and organize voice notes and transcripts |
| [`inkspring-mcp`](skills/inkspring-mcp/SKILL.md) | [Inkspring](https://inkspring.ai) | Write posts, work post ideas, schedule, and draft newsletters |
| [`opentalon-mcp`](skills/opentalon-mcp/SKILL.md) | OpenTalon (coming soon) | Work tickets on a local Kanban board from start to Done |

PulseCanvas Studio's MCP is in development; its skill will be added when it ships.
Current MCP availability and full setup guides: https://protomota.com/mcp

## Install a skill

**Claude Code:** copy the skill folder into `~/.claude/skills/` (all projects) or
`.claude/skills/` in a project, then start a new session.

```bash
git clone https://github.com/protomota/skills.git
cp -R skills/skills/jotley-mcp ~/.claude/skills/
```

**Codex:** copy the skill folder into `~/.codex/skills/`, then start a new session.

```bash
cp -R skills/skills/jotley-mcp ~/.codex/skills/
```

**Claude.ai:** zip the skill folder and upload it under Settings → Capabilities → Skills.

Each app's MCP server runs locally on your Mac, so connect it from a local session
on the same computer. Cloud sessions can't reach it.

## License

MIT. See [LICENSE](LICENSE).
