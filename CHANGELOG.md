# Changelog

All notable user-facing changes to the Aghanim Claude Code marketplace and
its plugins are documented here. Format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/); this marketplace
and its plugins use date-based version numbers of the form
`YYYY.MM.DD.N`, where `N` is a zero-indexed counter for multiple
releases on the same day.

## [Unreleased]

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
