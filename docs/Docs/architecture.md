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

## Future suite shell

Everend Forge will remain contract-first while gaining a suite shell after the authoring apps reach beta stability. The shell should be a Tauri + React desktop app that mounts WorldNotion and PathBranching as internal workspace pages instead of replacing either app.

The intended first pages are:

- World: WorldNotion's Markdown vault and canon workspace.
- Branch: PathBranching's branching narrative graph workspace.

The shell should share one active universe folder by default. WorldNotion remains responsible for editing canon Markdown, while PathBranching reads that canon and writes branching metadata under `.everend/.pathbranching`.

Suite integration must depend on public app exports and stable file/runtime contracts. It should not read private React state, depend on private Tauri command internals, or require the standalone WorldNotion and PathBranching apps to stop working.

Until both apps have beta-quality public integration surfaces, `everend-forge` should document and coordinate this direction rather than importing live source from moving development branches.