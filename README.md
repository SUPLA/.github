# SUPLA GitHub organization

> Part of SUPLA - an open smart home platform that brings together hardware manufacturers, the community, and users.  
> Learn more at [supla.org](https://www.supla.org).

This repository contains the organization-level profile, routing docs, and shared community files for the SUPLA GitHub organization.
Its role is to explain how the main repositories fit together and help contributors, integrators, self-hosters, and users land in the correct place.

## Main repositories

| Repository | Description | Open it when... |
|---|---|---|
| `supla-core` | Core server and system components of the SUPLA smart home platform. | you work on low-level server or protocol-side components |
| `supla-cloud` | Cloud web application and REST API for the SUPLA open smart home platform. | you work on the Cloud backend, public REST API, or web UI |
| `supla-device` | Embedded device SDK for building SUPLA-compatible smart home devices. | you build or modify device-side software |
| `supla-android` | Android client application for the SUPLA open smart home platform. | you work on the Android application |
| `supla-ios` | iOS client application for the SUPLA open smart home platform. | you work on the iOS application |
| `supla-docker` | Docker-based deployment for running your own SUPLA instance. | you want to self-host or deploy a full SUPLA stack |
| `api-client-php` | PHP client for the SUPLA public REST API. | you integrate with SUPLA Cloud from PHP |

## Reading order

- Start with [profile/README.md](profile/README.md) for the public organization entry.
- Use [docs/architecture.md](docs/architecture.md) for the high-level platform map.
- Use [docs/repositories.md](docs/repositories.md) for detailed routing.
- Use [docs/legacy-and-archived.md](docs/legacy-and-archived.md) to avoid routing people into historical repositories.

## Shared organization documents

- [CONTRIBUTING.md](CONTRIBUTING.md)
- [SECURITY.md](SECURITY.md)
- [SUPPORT.md](SUPPORT.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## Notes on repository state

The organization contains a mix of active, generated, legacy, and archived repositories.
Some repositories also use a `develop` branch for changes that are not yet released.
Use the default branch as the stable public entry point, and treat `develop` as pre-release when it exists.
