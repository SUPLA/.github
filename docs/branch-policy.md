# Branch policy

SUPLA has mixed branch naming across repositories.

## Current reality

Across important repositories, both `main` and `master` are used as default branches.
Some repositories may also use `develop` for unreleased work.

This means contributors should **not** assume one universal target branch.

## Organization-level rules

### 1. Default branch = stable public entry point

The default branch of a repository is the canonical public entry point for:

- organization profile links,
- repository routing,
- stable README links,
- user-facing references.

### 2. `develop` is allowed for unreleased work

A repository may use `develop` for:

- upcoming release work,
- integration changes that are not yet released,
- documentation that describes unreleased behavior.

## Pull request targeting guidance

For contributors:

1. Read the repository `README.md` and any local development docs.
2. Check the default branch and local maintainer guidance.
3. If the repository uses `develop` for active work, target `develop`.
4. Otherwise, target the default branch unless maintainers request something else.

