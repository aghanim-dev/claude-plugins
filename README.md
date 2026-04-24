# Aghanim Claude Code Marketplace

A [Claude Code plugin marketplace](https://docs.claude.com/en/docs/claude-code/plugins)
containing Aghanim's plugins for Claude Code.

## Quick start

From inside Claude Code, run:

```text
/plugin marketplace add aghanim-dev/claude-plugins
/plugin install newton@aghanim
/aghanim-webhooks-quick-start
```

The first command registers this marketplace, the second installs the
`newton` plugin, and the third launches the webhook quick-start
workflow that scaffolds Aghanim's `player.verify`, `item.add`, and
`item.remove` handlers in the current project. The very first
`mcp__aghanim__*` call opens a browser for Aghanim SSO login — complete
it once and the session persists.

## Add this marketplace

```text
/plugin marketplace add aghanim-dev/claude-plugins
```

## Plugins

| Plugin | Install | Description |
| --- | --- | --- |
| [`newton`](plugins/newton/README.md) | `/plugin install newton@aghanim` | Search Aghanim's docs and the Aghanim public API via the Newton MCP server, plus a webhook quick-start skill. |

## Support

Contact your Aghanim representative.

## License

Copyright (C) 2026 Aghanim, Inc — released under [AGPL-3.0-or-later](LICENSE).
