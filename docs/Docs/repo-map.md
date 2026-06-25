# Repository Map

## Portal

- https://github.com/Everendforge/everend-forge

Main overview, roadmap, governance, contribution guide, and cross-repo coordination.

This repository is documentation-first during foundation work. After WorldNotion and PathBranching reach beta-quality integration surfaces, it is intended to also become the Everend Forge suite shell: a Tauri + React app that mounts the authoring apps as workspace pages while keeping them available as standalone tools.

## Spec

- https://github.com/Everendforge/spec

Shared contracts for vaults, entities, branching graphs, runtime packages, and validation reports.

## Apps

- https://github.com/Everendforge/worldnotion
- https://github.com/Everendforge/pathbranching

WorldNotion is the worldbuilding vault app. PathBranching is the visual branching narrative editor.

Both apps should continue to own their product areas and expose public integration surfaces for the future suite. The suite should consume those surfaces by compatible release or pinned commit, not by assuming every latest development change is immediately suite-safe.

## Runtime adapters

- https://github.com/Everendforge/plugins

Shared runtime adapter roadmap. Engine-specific repos may split out later.
