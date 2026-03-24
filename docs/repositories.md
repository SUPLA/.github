# Repository index

This document is the routing map for the SUPLA GitHub organization.
It helps contributors, users, and integrators land in the correct repository quickly.

## Primary repositories

| Repository | Description | Use it when... | Notes |
|---|---|---|---|
| `supla-core` | Core server and system components of the SUPLA smart home platform. | you work on core server or protocol-side components | Structurally central repository |
| `supla-cloud` | Cloud web application and REST API for the SUPLA open smart home platform. | you work on the Cloud backend, public REST API, or web UI | Active repo with local community docs |
| `supla-device` | Embedded device SDK for building SUPLA-compatible smart home devices. | you build or modify custom devices | Active repo with local docs and `LLM.md` |
| `supla-android` | Android client application for the SUPLA open smart home platform. | you work on the Android app | Official mobile client |
| `supla-ios` | iOS client application for the SUPLA open smart home platform. | you work on the iOS app | Official mobile client |
| `supla-docker` | Docker-based deployment for running your own SUPLA instance. | you want to self-host or deploy a full SUPLA stack | Practical deployment entry point |
| `api-client-php` | PHP client for the SUPLA public REST API. | you integrate with the public API from PHP | Generated client; not the source of API truth |

## Legacy, transition, or compatibility repositories

| Repository | Role today | Migration note |
|---|---|---|
| `supla-arduino` | historical Arduino-era repository | use `supla-device` |
| `supla-espressif-esp` | older ESP8266 / ESP8285 source tree | use only when that legacy tree is explicitly required |
| `ESP8266` | compatibility landing page | points to `supla-espressif-esp` |

## Supporting or auxiliary repositories

These repositories are not primary entry points for most users and contributors.
Examples visible from the organization overview include:

- `esp32-owb` - forked dependency
- `OpenSSL-for-Android` - build or dependency support

## Routing rules

Use these rules consistently in docs, issues, and discussions:

- deployment questions -> `supla-docker`
- backend or public API issues -> `supla-cloud`
- device SDK questions -> `supla-device`
- Android app issues -> `supla-android`
- iOS app issues -> `supla-ios`
- protocol or low-level core work -> `supla-core`
- PHP client usage -> `api-client-php`

