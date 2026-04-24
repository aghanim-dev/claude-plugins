# Changelog

All notable user-facing changes to the Aghanim Claude Code marketplace and
its plugins are documented here. Format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/); this marketplace
and its plugins use date-based version numbers of the form
`YYYY.MM.DD.N`, where `N` is a zero-indexed counter for multiple
releases on the same day.

## [Unreleased]

## [2026.04.24.1]

### Changed
- Marketplace README quick-start now includes `/reload-plugins` between
  `/plugin install newton@aghanim` and `/newton:aghanim-webhooks-quick-start`,
  and uses the namespaced command form so the workflow runs correctly
  on first install.

## [2026.04.24.0]

### Added
- `/aghanim-webhooks-quick-start` slash command in the `newton`
  plugin that invokes the `aghanim-webhooks-quick-start` skill.
- Quick-start section in the marketplace README covering
  marketplace registration, `newton` plugin install, and running
  `/aghanim-webhooks-quick-start`.

### Fixed
- `newton` plugin MCP server URL corrected from
  `https://newton.aghanim.com/sse` to `https://mcp.aghanim.dev/sse`.
  The previous host was wrong, so `/plugin install newton@aghanim`
  users could not reach the Newton MCP server.

## [2026.04.23.3]

### Fixed
- `plugins[0].source` in `marketplace.json` now uses the full relative
  path `./plugins/newton` instead of the bare `newton` shorthand.
  Claude Code's schema validator rejected the shorthand form with
  `plugins.0.source: Invalid input`, blocking `/plugin marketplace add`.
  Dropped the unused `metadata.pluginRoot` shorthand at the same time.

## [2026.04.23.2]

### Changed
- Trimmed the marketplace README to the single install path relevant
  to users: `/plugin marketplace add aghanim-dev/claude-plugins`.

## [2026.04.23.1]

### Changed
- Relicensed the marketplace and the `newton` plugin from Proprietary
  to `AGPL-3.0-or-later`. Added full license text at `LICENSE` and
  `Copyright (C) 2026 Aghanim, Inc` attribution in the LICENSE header
  and both READMEs.

## [2026.04.23.0]

### Added
- `aghanim` marketplace catalog at `.claude-plugin/marketplace.json`.
- `newton` plugin with Newton MCP server (`mcp__aghanim__*`) for Aghanim
  docs and API lookups, and the `aghanim-webhooks-quick-start` skill.
