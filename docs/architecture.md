# Architecture

Everend Forge is organized around portable contracts rather than a single app.

## Source of truth

- Canon source: Markdown vaults with YAML frontmatter and wikilinks.
- Runtime source: JSON/YAML packages exported by authoring tools.
- Compatibility source: Everend Spec versions.

## Product boundaries

- Everend WorldNotion owns worldbuilding vault UX.
- Everend PathBranching owns branching narrative graph UX.
- Everend Plugins own runtime import, execution, and debugging.
- Everend Spec owns shared contracts and examples.

## Data flow

~~~text
Markdown Vault
  -> WorldNotion reads, edits, validates canon
  -> PathBranching references canon IDs
  -> PathBranching exports runtime package
  -> Engine plugins import and execute runtime package
~~~
