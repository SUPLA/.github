# SUPLA

> SUPLA - an open smart home platform that brings together hardware manufacturers, the community, and users.  
> Learn more at [supla.org](https://www.supla.org).

This organization contains the main source repositories of the SUPLA ecosystem: device software, server-side components, cloud services, mobile clients, deployment tooling, and integration clients.

## Start from your goal

- **Run your own SUPLA instance** -> [`supla-docker`](https://github.com/SUPLA/supla-docker)
- **Work on the Cloud backend or REST API** -> [`supla-cloud`](https://github.com/SUPLA/supla-cloud)
- **Work on core server and communication components** -> [`supla-core`](https://github.com/SUPLA/supla-core)
- **Build a SUPLA-compatible device** -> [`supla-device`](https://github.com/SUPLA/supla-device)
- **Work on the Android app** -> [`supla-android`](https://github.com/SUPLA/supla-android)
- **Work on the iOS app** -> [`supla-ios`](https://github.com/SUPLA/supla-ios)
- **Use the public REST API from PHP** -> [`api-client-php`](https://github.com/SUPLA/api-client-php)

## Main repositories

| Repository | Description |
|---|---|
| [`supla-core`](https://github.com/SUPLA/supla-core) | Core server and system components of the SUPLA smart home platform. |
| [`supla-cloud`](https://github.com/SUPLA/supla-cloud) | Cloud web application and REST API for the SUPLA open smart home platform. |
| [`supla-device`](https://github.com/SUPLA/supla-device) | Embedded device SDK for building SUPLA-compatible smart home devices. |
| [`supla-android`](https://github.com/SUPLA/supla-android) | Android client application for the SUPLA open smart home platform. |
| [`supla-ios`](https://github.com/SUPLA/supla-ios) | iOS client application for the SUPLA open smart home platform. |
| [`supla-docker`](https://github.com/SUPLA/supla-docker) | Docker-based deployment for running your own SUPLA instance. |
| [`api-client-php`](https://github.com/SUPLA/api-client-php) | PHP client for the SUPLA public REST API. |

## How the main parts fit together

- `supla-device` is used to build custom SUPLA-compatible devices.
- `supla-core` contains the server-side and communication foundations of the platform.
- `supla-cloud` provides the Cloud application, web UI, and public REST API.
- `supla-android` and `supla-ios` are the official client applications.
- `supla-docker` is the practical entry point for self-hosting and production deployment.
- `api-client-php` is an integration client for the public API.

## Legacy and compatibility repositories

Some repositories remain public for compatibility, migration, or historical reference.
They should not be treated as the primary entry point for new work.

- `supla-arduino` -> archived; use `supla-device`
- `ESP8266` -> compatibility landing page; see `supla-espressif-esp`
- `supla-espressif-esp` -> legacy ESP8266 / ESP8285 source tree

## More orientation

- [Architecture overview](../docs/architecture.md)
- [Repository index](../docs/repositories.md)
- [Branch policy](../docs/branch-policy.md)
- [Legacy and archived repositories](../docs/legacy-and-archived.md)
- [Contribution rules](../CONTRIBUTING.md)
- [Support](../SUPPORT.md)
- [Security reporting](../SECURITY.md)
