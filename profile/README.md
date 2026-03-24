<h1 align="left">
  <a href="https://www.supla.org/">
    <img src="https://github.com/SUPLA/supla-device/raw/main/docs/assets/supla-logo.svg" alt="SUPLA logo" width="30" style="vertical-align: middle; margin-right: 6px;" />
  </a>
  SUPLA
</h1>
SUPLA is an open smart home platform that brings together hardware manufacturers, the community, and users.

A complete setup is built from multiple parts: device software, communication layer, cloud backend, applications, and deployment.

---

## If you are a user

If you want to use SUPLA (not work on its development):

* You can use SUPLA with public cloud services (no self-hosting required)
* You can also run your own instance using self-hosting

For typical usage, start with:

* [https://www.supla.org](https://www.supla.org)
* [https://forum.supla.org](https://forum.supla.org)

If you are a software developer or a power user, continue below.

---

## How SUPLA is structured

SUPLA is divided into layers with clear responsibilities:

* device software
* core (server, protocol, communication)
* cloud (user interface, configuration, API)
* mobile applications
* deployment and infrastructure

These layers are developed independently. This is a deliberate design choice.

---

## How the system works

In simplified form:

**device → core (server) → cloud → mobile application**

1. Devices run SUPLA-compatible software
2. Core components handle device connections, protocol, and data exchange
3. Cloud provides user interface, configuration, accounts, and API access
4. Applications connect to the system through server/core and cloud interfaces

This separation is key to understanding the system.

---

## Start from your goal

### Run SUPLA (self-hosting)

→ [https://github.com/supla/supla-docker](https://github.com/supla/supla-docker)

Infrastructure and deployment setup.

---

### Build or integrate a device

→ [https://github.com/supla/supla-device](https://github.com/supla/supla-device)

Device-side software and SDK.

---

### Work on cloud (user interface, configuration, API)

→ [https://github.com/supla/supla-cloud](https://github.com/supla/supla-cloud)

User-facing cloud interface, configuration, and API.

---

### Work on core system (server, communication, system logic)

→ [https://github.com/supla/supla-core](https://github.com/supla/supla-core)

Central system component responsible for device connections, communication, and core system logic.

---

### Work on mobile applications

→ [https://github.com/supla/supla-android](https://github.com/supla/supla-android)  
→ [https://github.com/supla/supla-ios](https://github.com/supla/supla-ios)

User applications.

---

## What SUPLA is not

SUPLA is not:

* a single deployable system from one repository
* a closed ecosystem tied to one manufacturer
* a monolithic codebase combining all layers

Understanding this avoids most confusion when working with the platform.

---

## For contributors

Choose the layer you want to work on:

* Devices → [https://github.com/supla/supla-device](https://github.com/supla/supla-device)
* Core system (server, communication, logic) → [https://github.com/supla/supla-core](https://github.com/supla/supla-core)
* Cloud (UI, configuration, API) → [https://github.com/supla/supla-cloud](https://github.com/supla/supla-cloud)
* Mobile applications → [https://github.com/supla/supla-android](https://github.com/supla/supla-android) / [https://github.com/supla/supla-ios](https://github.com/supla/supla-ios)
* Deployment → [https://github.com/supla/supla-docker](https://github.com/supla/supla-docker)

Each repository defines its own scope and contribution rules.

---

## Legacy repositories

Some repositories are no longer part of the current development path.

If something looks outdated, archived, or inconsistent with the structure above, treat it as historical.

