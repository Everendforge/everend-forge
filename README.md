# Everend Forge

Everend Forge is an open source narrative creation suite for portable worldbuilding, branching narrative design, and engine runtime integration.

The suite is built around an open format rather than a single app. Canon lives in Markdown vaults, interactive stories export to JSON/YAML runtime packages, and engine plugins consume those packages without depending on authoring tools.

## Start Here

- [Roadmap](ROADMAP.md): staged plan for the suite.
- [Architecture](docs/architecture.md): how the parts fit together.
- [Repository map](docs/repo-map.md): where each project lives.
- [Monetization](docs/monetization.md): open source friendly business options.
- [Contributing](CONTRIBUTING.md): how to choose the right repo for a change.
- [Governance](GOVERNANCE.md): early stewardship rules.

## Repositories

- [spec](https://github.com/SoleipDreams/spec): shared contracts for vaults, branching graphs, runtime packages, and validation reports.
- [worldnotion](https://github.com/SoleipDreams/worldnotion): desktop worldbuilding vault app.
- [pathbranching](https://github.com/SoleipDreams/pathbranching): visual branching narrative editor.
- [plugins](https://github.com/SoleipDreams/plugins): runtime plugin coordination and engine adapter roadmap.

## Principles

- Users own their files.
- Canon stays portable and readable in Markdown tools such as Obsidian.
- Runtime packages are data, not app-private state.
- Authoring apps are independent clients over the spec.
- The open source core remains useful without proprietary lock-in.
- Public examples use synthetic content, not private canon.

## Current Status

Everend Forge is in early foundation work. The first milestone is to stabilize Everend Spec v0.1 and then build Everend WorldNotion against it.

## Local Workspace

If you clone all Everend Forge repositories as sibling folders, open [everend-forge.code-workspace](everend-forge.code-workspace) in VS Code-compatible editors to work across the suite.

## License

This portal repository is documentation-first. Documentation is licensed under CC BY 4.0. Code snippets and future code in this repository should use MIT OR Apache-2.0 unless stated otherwise.
