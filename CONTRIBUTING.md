# Contributing to SUPLA

Thank you for contributing.

SUPLA is a multi-repository platform.
Before opening an issue or pull request, make sure you are working in the correct repository.

## Choose the correct repository first

Use the organization profile and repository index to route work correctly:

- Organization profile: [`profile/README.md`](profile/README.md)
- Repository index: [`docs/repositories.md`](docs/repositories.md)
- Architecture overview: [`docs/architecture.md`](docs/architecture.md)

Common routing examples:

- deployment / self-hosting → `supla-docker`
- cloud backend / REST API / web UI → `supla-cloud`
- server core / protocol → `supla-core`
- device-side SDK / firmware building blocks → `supla-device`
- Android application → `supla-android`
- iOS application → `supla-ios`
- generated PHP API client → `api-client-php`

## Before you start

Please:

- search existing issues and pull requests,
- read the target repository `README.md`,
- read any local `Development.md`, `SECURITY.md`, or repository-specific contribution notes,
- check whether the repository is active, legacy, or archived,
- use the correct support channel for usage questions.

For setup or usage questions, use the channels listed in [`SUPPORT.md`](SUPPORT.md) instead of opening a bug immediately.

## Branches

Do **not** assume the same branch model across the entire organization.

Historical reality:

- some repositories use `main`,
- some repositories use `master`,
- some repositories may also use `develop` for unreleased work.

Contribution rule:

- target the repository's current development branch,
- if maintainers ask for `develop`, use `develop`,
- otherwise, target the default branch unless local documentation says otherwise.

More detail: [`docs/branch-policy.md`](docs/branch-policy.md)

## Pull requests

Keep pull requests focused.

A good pull request should:

- describe the problem clearly,
- explain the chosen solution,
- mention affected repositories or components,
- describe how the change was tested,
- include screenshots for UI changes when relevant,
- mention compatibility impact, migrations, or breaking behavior,
- update related docs when behavior changes.

Avoid mixing unrelated refactors with functional changes.

## API, protocol, and compatibility expectations

Some repositories are public integration surfaces.
Changes there need extra care.

Examples:
- public REST API
- device/server protocol behavior
- client-visible behavior
- deployment contracts and configuration

When changing shared or public behavior:

- prefer backward compatibility,
- document compatibility risk explicitly,
- update changelog / release notes where relevant,
- update dependent repositories if the change spans multiple components.

## Generated repositories

Some repositories are generated artifacts rather than hand-maintained sources.

Example:
- `api-client-php` is generated from the SUPLA Cloud OpenAPI definition.

For generated repositories:

- do not submit large manual edits to generated output unless maintainers explicitly request it,
- prefer changing the source definition or generator inputs,
- mention the source repo and source version in the pull request.

## Documentation changes

Documentation updates are welcome, including:

- fixing incorrect setup or build steps,
- clarifying repository scope,
- improving architecture explanations,
- adding migration notes for legacy repositories.

If a change affects how the whole organization is explained or routed, update:

- `profile/README.md`
- `docs/repositories.md`
- `docs/architecture.md`

If a change only affects a single component, keep the detailed docs in that repository.

## Legacy and archived repositories

Some repositories remain visible for compatibility or migration reasons.

Rules:
- do not propose new feature work in archived repositories,
- prefer migrating users to the successor repository,
- keep redirect / deprecation notes accurate,
- treat legacy repositories as reference material unless maintainers explicitly reactivate them.

See [`docs/legacy-and-archived.md`](docs/legacy-and-archived.md).

## Security issues

Do **not** open public issues for vulnerabilities.

Use the process described in [`SECURITY.md`](SECURITY.md).

## Conduct

By participating, you agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
