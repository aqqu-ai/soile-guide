# soile-guide

Offline-first sovereign tourism platform: PWA mobile guide + edge AI infrastructure for GOVTECH and remote low-connectivity routes.

---

## Platform Architecture

![SOILE Platform Architecture](docs/architecture/soile_platform_architecture.svg)

---

## Overview

SOILE Guide is an offline-first tourism platform designed for regions with limited or unreliable internet connectivity.

The platform combines a Progressive Web Application (PWA) used by tourists with optional edge AI infrastructure deployed in remote locations.  
This architecture enables navigation, safety monitoring, and local intelligence without relying on continuous cloud connectivity.

Core design principles:

- offline-first operation
- minimal infrastructure requirements
- sovereign data control
- optional edge intelligence layer
- compatibility with GOVTECH tourism systems

---

## System Components

### Tourist Application (PWA)

A Progressive Web Application used directly on mobile devices.

Capabilities:

- offline navigation
- downloadable route packages
- local map rendering
- multilingual content
- safety notifications
- lightweight mobile operation

Supported environments:

- Android browsers
- iOS browsers
- desktop browsers

---

### Edge Intelligence Layer

Optional edge nodes deployed along tourism routes.

Capabilities:

- environmental monitoring
- safety event detection
- local vision pipelines
- local reasoning for alerts
- offline data synchronization with tourist devices

Edge nodes operate autonomously and synchronize when connectivity becomes available.

---

### Regional Infrastructure

Regional infrastructure may integrate multiple edge nodes and tourism services.

Functions:

- route management
- safety coordination
- tourism analytics
- optional cloud synchronization
