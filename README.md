# MCP-Safeguard Skill

Claude Code skill for using [MCP-Safeguard](https://github.com/Li-Bailiang/mcp-safeguard)
to scan Model Context Protocol (MCP) servers, explain findings, suggest minimal
fixes, and add CI security gates.

The skill uses the published npm package `@mcp-safeguard/cli`. It does not
reimplement the scanner.

## Install

### Project skill

From the root of a project where you want Claude Code to use the skill:

```powershell
git clone https://github.com/Li-Bailiang/mcp-safeguard-skill .claude/skills/mcp-safeguard
```

### Personal skill

Windows PowerShell:

```powershell
git clone https://github.com/Li-Bailiang/mcp-safeguard-skill "$env:USERPROFILE\.claude\skills\mcp-safeguard"
```

macOS/Linux:

```bash
git clone https://github.com/Li-Bailiang/mcp-safeguard-skill ~/.claude/skills/mcp-safeguard
```

## Use

Ask Claude Code to use the skill, for example:

```text
Use the mcp-safeguard skill to scan this MCP server and explain the findings.
```

or:

```text
Use the mcp-safeguard skill to add GitHub Actions security scanning to this repository.
```

## Contents

- `SKILL.md` - Claude Code skill instructions.
- `references/ci-examples.md` - GitHub Actions examples.
- `references/remediation-guide.md` - Triage and remediation notes by finding category.

## Related

- Scanner repository: https://github.com/Li-Bailiang/mcp-safeguard
- npm package: https://www.npmjs.com/package/@mcp-safeguard/cli

