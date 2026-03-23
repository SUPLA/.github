# SUPLA architecture overview

This document explains the high-level relationship between the primary repositories in the SUPLA GitHub organization.
It is intentionally simple.
Detailed implementation and build instructions belong in the individual repositories.

## Big picture

SUPLA is split across several layers:

1. **server-side core and communication**
2. **cloud application and public API**
3. **device-side software**
4. **client applications and integrations**
5. **deployment tooling**

## Repository roles

| Layer | Repository | Role |
|---|---|---|
| Core and server | `supla-core` | Core server and system components of the SUPLA smart home platform |
| Cloud, API, and web UI | `supla-cloud` | Cloud web application and REST API for the SUPLA open smart home platform |
| Device SDK | `supla-device` | Embedded device SDK for building SUPLA-compatible smart home devices |
| Deployment | `supla-docker` | Docker-based deployment for running your own SUPLA instance |
| Android client | `supla-android` | Android client application for the SUPLA open smart home platform |
| iOS client | `supla-ios` | iOS client application for the SUPLA open smart home platform |
| PHP integration client | `api-client-php` | PHP client for the SUPLA public REST API |

## Important boundaries

### `supla-device`

`supla-device` is a device-side SDK.
It is not a ready-made firmware image.

### `supla-core`

`supla-core` contains low-level and server-side components.
It sits under the user-facing Cloud and client layers.

### `supla-cloud`

`supla-cloud` contains the Cloud backend, public REST API, and web UI.
It is central to the user-facing platform but is not the deployment entry point by itself.

### `supla-docker`

`supla-docker` is the practical entry point for running a full self-hosted SUPLA stack.

### Mobile applications

`supla-android` and `supla-ios` are official client applications.
They consume server and Cloud functionality rather than replace them.

### Generated clients

`api-client-php` should be treated as an integration artifact rather than the primary source of API truth.

