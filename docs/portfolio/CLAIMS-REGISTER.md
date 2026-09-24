# Claims Register

Last reviewed 2026-09-24.

This file is authoritative for public factual claims in the portfolio. If a claim is not listed here or cannot be mapped to a source, omit it or qualify it.

## Identity and education

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| Emmett Sewell is a Systems Engineering student at Simon Fraser University. | Supplied LinkedIn export | High | Yes | Degree listed as BASc Systems Engineering, 2022-2027. |
| Emmett's portfolio spans systems engineering, software architecture, autonomous systems, infrastructure and production software. | Synthesis from verified projects and LinkedIn | High | Yes | Narrative claim supported by multiple sources; avoid implying equal depth in every area. |

## MAKE Projects internal platform

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| Emmett is/was the sole developer on an internal project-management platform at MAKE Projects. | Supplied LinkedIn export, experience section | High | Yes | Public profile language supports sole-developer statement. |
| The platform began as a no-code/Base44 prototype and was migrated to React/Vite with Supabase/Postgres on Vercel. | Supplied LinkedIn export | High | Yes | Do not expose private migration details beyond this public-safe level. |
| Emmett designed the relational data model and role-based permission architecture. | Supplied LinkedIn export | High | Yes | Public-safe at responsibility level. |
| Permissions are enforced using Postgres row-level security. | Supplied LinkedIn export | High | Yes | Avoid publishing policy logic or schema detail. |
| Emmett owned deployment and release process end to end. | Supplied LinkedIn export | High | Yes | Public-safe. |
| Emmett ran security hardening across authentication, authorization and RLS policy coverage. | Supplied LinkedIn export | High | Yes | Do not imply certification or external audit. |
| Emmett translated project-management staff requirements into product architecture and shipped features. | Supplied LinkedIn export | High | Yes | Public-safe. |
| Emmett led internal testing workshops and folded feedback into the roadmap. | Supplied LinkedIn export | High | Yes | Public-safe. |
| Emmett used spec-driven CLI coding agents, separate architecture/debugging context and persistent decision logging in development. | Supplied LinkedIn export | High | Yes | Present as workflow/process, not as product feature. |
| Nothing ships until a five-stage validation pass covering intent, edge cases, integration, UX and documentation. | Supplied LinkedIn summary | High | Yes | Phrase as Emmett's stated workflow, not a formally certified process. |
| Database permissions are independently audited through a read-only connection. | Supplied LinkedIn summary | High | Yes | Public-safe at high level. |
| The product name is NAVIS. | User-provided project context, not public source | Medium | Conditional | Use only if employer/product-name approval is confirmed. Default public wording: "Internal Project-Management Platform". |
| The platform has specific user counts, savings, productivity gains or business-impact metrics. | No approved source | Low | No | Do not publish unless employer-approved evidence is later supplied. |

## Broadway infrastructure and fleet systems

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| Emmett has served as IT Technician at Broadway Moving and Storage since 2023. | Supplied LinkedIn export | High | Yes | Public-safe. |
| Emmett is the sole technical resource for infrastructure he specified, built and maintained. | Supplied LinkedIn export | High | Yes | Public-safe. |
| Emmett procured and deployed self-hosted server infrastructure. | Supplied LinkedIn export | High | Yes | Do not publish topology, addresses, credentials or vendor-sensitive detail. |
| Emmett built and deployed internal custom systems used day to day. | Supplied LinkedIn export | High | Yes | Keep at responsibility level unless a specific system is separately approved. |
| Emmett integrated the NVR and physical-security stack into the internal infrastructure. | Supplied LinkedIn export | High | Yes | Avoid operational/security specifics. |
| Emmett implemented GPS-driven automated fleet management across the truck fleet. | Supplied LinkedIn export | High | Yes | No live-map screenshots or vehicle/location details without explicit approval. |
| Emmett owns ongoing server uptime, maintenance, upgrades, hardware repair, security-system upkeep and staff support. | Supplied LinkedIn export | High | Yes | Public-safe in concise form. |
| Specific server brands, network topology, NVR vendor, GPS provider or automation architecture. | No approved public source | Low | No | Do not invent or expose. |

## Autonomous UAV

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| The Autonomous UAV was an SFU ENSC 351 team project. | Repository path/report context | High | Yes | Preserve team attribution. |
| The system includes camera-based person detection. | Public repository source: image_recog_master.py | High | Yes | YOLO/ONNX implementation visible in source. |
| The perception stack uses ONNX Runtime and a YOLOv8n ONNX model. | image_recog_master.py, Autonomous_Drone.py | High | Yes | Public code supports this. |
| Camera frames are received over SPI for on-device perception. | image_recog_master.py and related SPI code | High | Yes | Public-safe. |
| LiDAR data is read and filtered before use in control logic. | import_lidar.py, Autonomous_Drone.py | High | Yes | Public-safe. |
| MAVLink/pymavlink is used to communicate velocity/yaw commands to the flight controller. | Autonomous_Drone.py | High | Yes | Public-safe. |
| The control logic prioritizes obstacle avoidance before person-following behavior. | Autonomous_Drone.py fusion_algorithm | High | Yes | Public-safe. |
| The project integrates camera perception, LiDAR sensing and flight-control commands into one software pipeline. | Multiple public source files | High | Yes | Strong case-study claim. |
| The project used BeagleY-AI-class embedded Linux hardware. | Source comments/report/asset inventory | Medium-high | Yes | Use exact board name only where confirmed by source/report. |
| ESP32 code was part of the camera/SPI subsystem. | ESP32SPI.ino | High | Yes | Public-safe. |
| The UAV successfully completed fully autonomous flight under all intended conditions. | No verified flight evidence in current portfolio sources | Low | No | Do not claim. |
| Emmett personally authored every UAV subsystem. | Team project; authorship split not established | Low | No | Do not claim sole authorship. |
| Any exact latency, accuracy, range or performance metric. | Not approved/independently verified for portfolio use | Low | No | Do not publish unless specifically sourced. |

## DragonsDash

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| DragonsDash is a public TypeScript/Next.js project. | GitHub repository metadata and package.json | High | Yes | Public-safe. |
| It uses Next.js, React, TypeScript, Tailwind CSS, Zustand and Vitest. | package.json and repository contents | High | Yes | Public-safe. |
| It contains finance-oriented surfaces including dashboard, accounts, spending, bills/markets/settings and CSV import. | Repository routes/components | High | Yes | Public-safe. |
| It has test coverage for calculations and CSV parsing. | src/lib/__tests__, src/lib/import/__tests__ | High | Yes | Public-safe. |
| It is a production financial product with audited security. | No evidence | Low | No | Do not claim. |
| All auth/encryption modules are fully wired in production. | Not fully verified | Medium-low | No | Omit unless implementation pass confirms. |

## Embedded & systems labs

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| ENSC351 repository contains embedded-Linux/C lab work. | Public repository structure and files | High | Yes | Keep grouped as coursework/lab work. |
| The work includes Linux hardware-interface/HAL-style code and SPI/spidev interaction. | Public assignment source referenced in asset inventory | Medium-high | Yes | Attribute as coursework; avoid sole-authorship claim unless checked. |
| The ENSC100 Pico repository demonstrates early embedded programming exposure. | Public repository metadata + timer.py | Medium | Yes | Keep minor; do not inflate. |

## Repositories to exclude from ownership claims

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| OpenJarvis is Emmett's original AI framework. | GitHub metadata says repository is a fork | High | No | Explicitly false/unsupported; omit project unless specific upstream contribution is verified. |
| Third-party/forked media in OpenJarvis is Emmett-created work. | Upstream README/metadata | High | No | Do not use. |
| Evan Friesen portrait/social media assets are Emmett-owned portfolio assets. | Repository content | High | No | Do not reuse without permission. |

## Contact

| Claim | Source | Confidence | Public-safe? | Notes |
|---|---|---:|---|---|
| Public contact links may include GitHub, LinkedIn and email. | Canonical workflow + LinkedIn | High | Yes | Use email, GitHub, LinkedIn. |
| Publish mobile phone number. | LinkedIn PDF contains it, but workflow explicitly prohibits it | High | No | Never publish. |

## Claim-writing rules

1. Prefer responsibility + architecture over unverified impact.
2. Preserve team attribution for academic team projects.
3. Do not convert private-repo access into permission to publish private implementation.
4. Do not infer metrics.
5. Do not label a prototype as production unless source evidence establishes production use.
6. If a claim is absent here, either add it with evidence or omit it from the site.
