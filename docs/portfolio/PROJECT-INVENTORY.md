# Project Inventory

Research basis: LinkedIn export supplied to the portfolio project; connected GitHub repositories; repository contents and representative source files; existing asset inventory. Last reviewed 2026-09-24.

## Placement scale

- **Featured** — deserves prominent homepage treatment and/or a dedicated case study.
- **Supporting** — useful evidence of breadth but should not compete with flagship work.
- **Lab/Archive** — technically interesting smaller work, grouped compactly.
- **Omit** — weak, redundant, forked, derivative, insufficiently evidenced, or distracting.

Scores are internal portfolio-strength scores only. They are not to be displayed publicly.

## 1. Autonomous UAV

- **Repository/source:** https://github.com/essewell/Autonomous-UAV-project
- **Public/private:** Public
- **Category:** Autonomous systems / embedded Linux / perception / sensing / flight control
- **Context:** SFU ENSC 351 final project
- **Year:** 2025
- **Individual/team/unknown:** Team project. Exact per-file authorship is not fully established; preserve team attribution.
- **Actual technologies verified:** Python, pymavlink/MAVLink, OpenCV, ONNX Runtime, YOLOv8n ONNX model, SPI, BeagleY-AI-class embedded Linux target, ESP32/Arduino code, VL53L0X LiDAR integration, C/C++ build artifacts.
- **What it does:** Integrates camera-based person detection, LiDAR obstacle sensing, and MAVLink velocity/yaw commands into an autonomous-control pipeline.
- **Notable engineering work:** Real-time camera-frame transport over SPI; ONNX inference and bounding-box extraction; multi-sensor control logic; obstacle-priority fusion; MAVLink command generation; embedded-device integration across camera/sensor/flight-controller boundaries.
- **Interesting constraints:** Embedded compute; multiple buses/protocols; sensor noise/filtering; real-time-ish control loop; physical integration; team attribution; report/privacy constraints.
- **Visual assets:** Drone assembly photo, system flowchart, detection sample, detected-frame sequence, report figures. See ASSET-INVENTORY.md.
- **Portfolio strength:** 10/10
- **Recommended placement:** Featured; flagship personal/academic engineering case study.
- **Factual confidence:** High for architecture visible in source; medium for outcome details not independently demonstrated by a flight video.
- **Unresolved questions:** Exact contribution split across the five-person team; which photos can be published; whether a consent-safe perception frame/video is available; which final integrated tests were completed.

## 2. Internal Project-Management Platform at MAKE Projects

- **Repository/source:** Private professional repository; public-safe facts from LinkedIn export and supplied project context only.
- **Public/private:** Private
- **Category:** Production software / architecture / infrastructure / AI-enabled engineering workflow
- **Context:** Professional work at MAKE Projects LTD
- **Year:** 2026-present
- **Individual/team/unknown:** Emmett is described in the supplied LinkedIn export as the sole developer / sole technical person on the product.
- **Actual technologies verified for public use:** React, Vite, Supabase, PostgreSQL, Postgres row-level security, Vercel. Public profile also supports role-based permissions, deployment/release ownership, QA/testing, documentation, and agentic CLI development workflow.
- **What it does:** Internal project-management software for MAKE Projects. Public treatment must remain high-level.
- **Notable engineering work:** Migration from a no-code prototype to a purpose-built stack; relational data model; role-based permission architecture enforced with RLS; deployment and release workflow; security hardening; requirements translation from project-management staff; internal testing; documentation.
- **Interesting constraints:** Private company IP; non-software stakeholders; production responsibility; security/privacy; solo technical ownership; need to explain work without exposing implementation.
- **Visual assets:** No approved product screenshots. A sanitized public-safe architecture diagram can be created from already-public stack facts.
- **Portfolio strength:** 10/10
- **Recommended placement:** Featured; flagship professional software case study.
- **Factual confidence:** High for claims present in the supplied LinkedIn export; otherwise do not publish.
- **Unresolved questions:** Whether MAKE approves use of the product name NAVIS, logo, or sanitized screenshots; any approved business-impact metrics.

## 3. Broadway Moving and Storage — Internal Infrastructure & Fleet Systems

- **Repository/source:** No public repository supplied; LinkedIn export.
- **Public/private:** Private operational system
- **Category:** Infrastructure / operations / fleet systems / physical-digital integration
- **Context:** Professional/operational work
- **Year:** 2023-present
- **Individual/team/unknown:** Supplied LinkedIn material describes Emmett as sole technical resource for this work.
- **Actual technologies verified:** Self-hosted server infrastructure; internal systems; NVR/physical-security integration; GPS-driven automated fleet management. Specific vendors/protocols are not established in source material and must not be invented.
- **What it does:** Supports day-to-day business operations through self-hosted systems, physical-security integration, and fleet automation.
- **Notable engineering work:** Procurement/deployment, ongoing server administration, internal systems, NVR integration, fleet automation, hardware repair, support.
- **Interesting constraints:** Live business dependency; operational continuity; security-sensitive infrastructure; physical systems and field operations.
- **Visual assets:** None approved. Prefer a sanitized architecture/data-flow diagram over live screenshots.
- **Portfolio strength:** 8.5/10
- **Recommended placement:** Supporting homepage feature with concise case-study section; dedicated route only if safe visual evidence becomes available.
- **Factual confidence:** High for LinkedIn-backed claims; low for technical specifics not named there.
- **Unresolved questions:** Public-safe technical stack; whether company-approved infrastructure photos can be used.

## 4. DragonsDash

- **Repository/source:** https://github.com/essewell/DragonsDash
- **Public/private:** Public
- **Category:** Full-stack/product software prototype
- **Context:** Personal project; exact origin/history beyond the repository is not fully documented.
- **Year:** 2026
- **Individual/team/unknown:** Repository is not a GitHub fork. Authorship history should be checked before making stronger originality claims.
- **Actual technologies verified:** Next.js, React, TypeScript, Tailwind CSS, Zustand, Vitest, SimpleWebAuthn packages, libsodium-wrappers, CSV import/parsing, local application state and calculation utilities.
- **What it does:** Personal-finance-style application surface with dashboard, accounts, spending, bills, markets, settings, CSV import and calculation logic.
- **Notable engineering work:** Componentized UI shell, data calculations, CSV parser/tests, application state, auth/encryption-related modules, responsive navigation.
- **Interesting constraints:** Financial-data UX; import validation; calculations; privacy expectations; repository documentation and implementation need to be reconciled before making security claims.
- **Visual assets:** No screenshots currently inventoried. Capture synthetic-data screenshots only after current build is verified.
- **Portfolio strength:** 7/10
- **Recommended placement:** Supporting project, not a flagship.
- **Factual confidence:** Medium-high for code-level stack and surfaces; medium for product completeness.
- **Unresolved questions:** Origin story; actual deployment status; whether auth/encryption modules are fully wired; intended persistence model.

## 5. ENSC 351 Embedded Linux Labs

- **Repository/source:** https://github.com/essewell/ENSC351
- **Public/private:** Public
- **Category:** Embedded Linux / hardware abstraction / C / SPI
- **Context:** SFU coursework
- **Year:** 2025
- **Individual/team/unknown:** Coursework repository; individual authorship of specific lab files is not fully established from current evidence.
- **Actual technologies verified:** C/C++, CMake/Make, Linux userspace hardware access, HAL-style source organization, SPI/spidev code in assignment material.
- **What it does:** Course/lab work around embedded Linux and hardware interfacing.
- **Notable engineering work:** Useful evidence of low-level hardware/software boundaries and Linux device interaction.
- **Interesting constraints:** Hardware I/O, embedded target, course context, incomplete README.
- **Visual assets:** No lab photos found.
- **Portfolio strength:** 6.5/10
- **Recommended placement:** Supporting collection: "Embedded & Systems Labs".
- **Factual confidence:** Medium.
- **Unresolved questions:** Exact assignment ownership and best representative files; board/peripheral photos.

## 6. ENSC 100 Raspberry Pi Pico project

- **Repository/source:** https://github.com/essewell/ensc100RPiPico
- **Public/private:** Public
- **Category:** Introductory embedded / MicroPython
- **Context:** SFU ENSC 100 project
- **Year:** 2023
- **Individual/team/unknown:** Unknown from repository alone.
- **Actual technologies verified:** Python/MicroPython-style code; repository currently contains a small timer.py file.
- **What it does:** Insufficient repository evidence to describe the full physical project safely.
- **Notable engineering work:** Early embedded exposure.
- **Interesting constraints:** Very small public repository and insufficient documentation.
- **Visual assets:** None found.
- **Portfolio strength:** 3.5/10
- **Recommended placement:** Lab/Archive only if paired with better project evidence; otherwise omit.
- **Factual confidence:** Low-medium.
- **Unresolved questions:** Full project scope, hardware, ownership, outcome.

## 7. C-Misc

- **Repository/source:** https://github.com/essewell/C-Misc
- **Public/private:** Public
- **Category:** C programming / coursework exercises
- **Context:** Academic/practice collection
- **Year:** Multiple/unknown
- **Individual/team/unknown:** Unknown by item.
- **Actual technologies verified:** C-oriented exercise/project folders including BNF, recursion, assignments, Fibonacci and a Snake-like project.
- **What it does:** Mixed practice/coursework rather than one coherent engineered system.
- **Notable engineering work:** Demonstrates language exposure, not portfolio-defining systems work.
- **Interesting constraints:** Mixed provenance and inconsistent documentation.
- **Visual assets:** None inventoried.
- **Portfolio strength:** 3/10
- **Recommended placement:** Lab/Archive at most.
- **Factual confidence:** Medium for repository contents; low for context.
- **Unresolved questions:** Which items are original, course-provided, or team work.

## 8. JavaProjects-Misc-main

- **Repository/source:** https://github.com/essewell/JavaProjects-Misc-main
- **Public/private:** Public
- **Category:** Java practice / small games and exercises
- **Context:** Academic/personal mixed collection
- **Year:** Unknown/multiple
- **Individual/team/unknown:** Unknown by item.
- **Actual technologies verified:** Java project structure; image/audio assets.
- **What it does:** Mixed small Java work.
- **Notable engineering work:** Language breadth only.
- **Interesting constraints:** Asset provenance is unknown.
- **Visual assets:** Sprites and WAV files exist but rights/provenance are not established.
- **Portfolio strength:** 2.5/10
- **Recommended placement:** Omit from primary portfolio; optionally mention Java under capability index if otherwise supported.
- **Factual confidence:** Medium.
- **Unresolved questions:** Asset licensing and project provenance.

## 9. blarkov / Tarkov Mobile

- **Repository/source:** https://github.com/essewell/blarkov
- **Public/private:** Public
- **Category:** Android/Kotlin game prototype
- **Context:** Personal/experimental
- **Year:** 2026
- **Individual/team/unknown:** Repository is not a GitHub fork; generation/originality history is not fully established.
- **Actual technologies verified:** Kotlin, Android, Jetpack Compose, DataStore, custom game loop/rendering architecture described in repository docs.
- **What it does:** Top-down extraction-shooter-inspired Android game prototype.
- **Notable engineering work:** Fixed-timestep loop, rendering, AI/pathfinding, ballistics, touch input, persistence architecture, Compose UI.
- **Interesting constraints:** Derivative game concept/branding; documentation states some subsystems remain stubbed.
- **Visual assets:** Runtime-generated visuals; no portfolio-ready media inventoried.
- **Portfolio strength:** 6/10 technically, but lower narrative priority.
- **Recommended placement:** Lab/Archive. Do not feature ahead of systems-engineering work.
- **Factual confidence:** Medium; implementation should be independently sampled before stronger claims.
- **Unresolved questions:** How much was AI-generated vs manually authored; build status; rebranding/IP presentation.

## 10. Evan creator website

- **Repository/source:** https://github.com/essewell/evan-website
- **Public/private:** Public
- **Category:** Web/portfolio frontend
- **Context:** Website for content creator Evan Friesen
- **Year:** 2026
- **Individual/team/unknown:** Repository owner is Emmett; exact design/content collaboration is not established.
- **Actual technologies verified:** HTML, JSX/React-style components, social/embed-oriented portfolio content.
- **What it does:** Creator portfolio/link surface.
- **Notable engineering work:** Web UI work, but weak alignment with target systems-engineering narrative.
- **Interesting constraints:** Third-party likenesses/social embeds and permission concerns.
- **Visual assets:** Evan portrait and external embeds; not suitable as Emmett portfolio evidence without permission.
- **Portfolio strength:** 4/10
- **Recommended placement:** Omit from primary portfolio.
- **Factual confidence:** Medium.
- **Unresolved questions:** Client status, deployment, permissions.

## 11. OpenJarvis fork

- **Repository/source:** https://github.com/essewell/OpenJarvis
- **Public/private:** Public
- **Category:** Forked upstream AI project
- **Context:** Fork of upstream OpenJarvis
- **Year:** 2026
- **Individual/team/unknown:** GitHub metadata explicitly marks this repository as a fork. Upstream README attributes the project to Stanford/Hazy Research contributors.
- **Actual technologies verified:** Upstream project is predominantly Python/local-agent infrastructure, but those are not Emmett-owned claims.
- **What it does:** Upstream local-first personal AI framework.
- **Notable engineering work:** No Emmett-specific contribution established from current evidence.
- **Interesting constraints:** Attribution.
- **Visual assets:** Upstream media only.
- **Portfolio strength:** 1/10 without verified original contributions.
- **Recommended placement:** Omit.
- **Factual confidence:** High.
- **Unresolved questions:** Whether Emmett has commits/PRs beyond a straight fork.

## Expected public hierarchy

1. Autonomous UAV — flagship autonomous/physical systems case study.
2. MAKE internal project-management platform — flagship production software/architecture case study.
3. Broadway infrastructure/fleet systems — supporting real-world systems ownership.
4. DragonsDash and Embedded & Systems Labs — supporting breadth.
5. Curated Lab/Archive — only selected smaller work.
6. Omit forks, weak miscellaneous repositories, and web work that dilutes the systems-engineering story.
