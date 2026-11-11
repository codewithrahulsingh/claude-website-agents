# Website Dev Agents (plugin)

Website development system for Claude: 16 specialist agents, orchestrator, token-saver and progress bar.

## Install once (works in every session)

**Claude app (Cowork / cloud sessions):** open the `website-dev-agents.plugin` file in chat and press Install.

**Claude Code (terminal / desktop):**
```
/plugin marketplace add codewithrahulsingh/claude-website-agents
/plugin install website-dev-agents@codewithrahulsingh
```

Update later: `/plugin marketplace update codewithrahulsingh`

## Use
- `/new-website <brief>` – new project, full pipeline
- `/full-audit <url>` – audit an existing site (report only)
- `/progress` – progress table

Optional: copy `templates/CLAUDE.md` into a website project folder for project rules.

## Contents
- `agents/` – 16 agents
- `skills/` – project-orchestrator, token-saver, progress-tracker, new-website, full-audit, progress
- `README-full-guide.md` – full documentation
