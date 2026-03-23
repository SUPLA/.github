# Security Policy

## Scope

This organization contains repositories with different maintenance states.

General rule:

- active repositories on their current maintained branches are in scope for security review,
- legacy repositories are reviewed on a best-effort basis,
- archived repositories are generally out of scope except for migration or deprecation guidance.

Repository-specific `SECURITY.md` files override this default when present.

## Reporting a vulnerability

Please **do not** report security vulnerabilities in public GitHub issues, pull requests, discussions, or forum posts.

Report vulnerabilities privately to:

- **security@supla.org**

Include, when possible:

- affected repository,
- affected branch, tag, or version,
- short summary of the issue,
- impact assessment,
- reproduction steps or proof of concept,
- configuration assumptions,
- suggested mitigation if known.

If you need an encrypted reporting path, mention that in the initial message and ask for a secure channel.

## What to expect

After receiving a report, maintainers will:

- review the report privately,
- confirm scope and severity,
- decide whether the fix belongs in one repository or across multiple repositories,
- coordinate disclosure when a fix is ready.

We may ask for additional reproduction details.

## Supported versions

This default policy is intentionally simple because maintenance differs by repository.

Default support expectation:

| Repository state | Security support |
|---|---|
| Active repository, maintained branch | Supported |
| Legacy repository kept for compatibility | Best effort |
| Archived repository | Not supported for feature/security maintenance |

Examples of repositories that are known to be legacy or archived should remain documented in [`docs/legacy-and-archived.md`](docs/legacy-and-archived.md).

## Public disclosure

Please give maintainers reasonable time to investigate, prepare a fix, and coordinate disclosure before publishing details.
