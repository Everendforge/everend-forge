# Everend Forge Roadmap

## 0.1 Foundation

- Define Everend Spec v0.1 as Markdown contracts plus examples.
- Publish a synthetic demo vault.
- Define runtime package examples for branching narrative.
- Establish repo roles and contribution conventions.

## 0.2 WorldNotion MVP

- Open local Markdown vaults.
- Browse file trees.
- Render and edit Markdown.
- Parse YAML frontmatter.
- Resolve wikilinks and backlinks.
- Search entities and content.
- Report broken links and missing required metadata.

## 0.3 PathBranching Design

- Define graph model.
- Reference canon entities by stable IDs.
- Export JSON/YAML runtime packages.
- Validate missing references and broken transitions.

## 0.4 Unity Runtime Prototype

- Load runtime package.
- Start node.
- Show current line and choices.
- Select choices.
- Get/set variables.
- Emit events.
- Save/load runtime state.

## 0.5 Beta Suite Preparation

- Keep WorldNotion and PathBranching useful as standalone apps.
- Expose stable public app components for future suite mounting.
- Keep shared universe files portable and versioned through Everend Spec.
- Confirm PathBranching can read the same universe folder WorldNotion edits.
- Avoid coupling the future suite to private React state or private Tauri command details.

## 0.6 Everend Forge Suite Shell

- Convert the portal into a Tauri + React suite app while preserving documentation.
- Mount WorldNotion as the World workspace page.
- Mount PathBranching as the Branch workspace page.
- Share one active universe folder across both pages by default.
- Pin WorldNotion and PathBranching by compatible version or commit when integrating, rather than tracking moving development branches automatically.

## Later

- Godot plugin.
- Unreal plugin.
- Optional cloud services for sync, backup, collaboration, or hosted previews.
