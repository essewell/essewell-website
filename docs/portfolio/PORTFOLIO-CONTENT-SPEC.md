# Portfolio Content Specification

Last reviewed 2026-09-24.

This specification defines the public information architecture and content hierarchy for the portfolio. It is subordinate to `CLAIMS-REGISTER.md` for factual correctness and to `DESIGN-SYSTEM.md` for visual treatment.

# 1. Site map

Use the smallest useful route structure:

```text
/
├── /projects
├── /projects/autonomous-uav
├── /projects/internal-project-management-platform
└── /about
```

Optional later route, only if enough public-safe evidence exists:

```text
/projects/infrastructure-fleet-systems
```

Do not create a route for every repository.

The `/projects` index should contain:
- two flagship case studies
- one strong supporting professional/operational system
- a small curated supporting-work section
- a restrained Lab/Archive group

# 2. Home page

## Section 1 — Hero

### Purpose
Establish Emmett's identity and engineering range immediately.

### Information shown
- Emmett Sewell
- Systems Engineering
- Software Architecture / Full-Stack Systems
- Autonomous & Embedded Systems
- concise one-sentence summary
- links: Projects, About, GitHub, LinkedIn

### Recommended hero copy
**Emmett Sewell**  
**Systems engineering across physical systems, software architecture, and production infrastructure.**

Supporting line:
> I build systems that cross hardware, embedded computing, sensing, software, data, and operations.

This supporting line is a narrative synthesis and should remain broad rather than imply equal depth across every layer.

### Visual treatment
Asymmetric first viewport with a meaningful simplified UAV system diagram using verified blocks and interfaces.

### Density
Low to medium.

### CTA
`View selected work →`

## Section 2 — Flagship work

### Purpose
Prove the hero claim immediately.

### Order
1. Autonomous UAV
2. Internal Project-Management Platform

Use different compositions, not identical cards.

### Autonomous UAV teaser
**Category:** Autonomous Systems / Embedded Linux / Perception  
**Title:** Autonomous UAV  
**One-sentence description:** A team-built UAV system integrating camera-based human detection, LiDAR sensing, embedded compute, and MAVLink flight-control commands.

**Technical summary:** Camera frames are transported into an embedded perception pipeline using SPI; YOLO/ONNX performs person detection; LiDAR measurements are filtered; control logic prioritizes obstacle avoidance and emits MAVLink velocity/yaw commands.

**Capabilities demonstrated:**
- embedded Linux
- computer vision
- sensor integration
- control logic
- communication protocols
- physical-system integration

**Technologies:** Python, pymavlink/MAVLink, OpenCV, ONNX Runtime, YOLOv8n, SPI, ESP32/Arduino, LiDAR.

**Recommended visuals:** assembled UAV photo + clean architecture diagram.

**CTA:** `View UAV case study →`

### Internal platform teaser
**Category:** Private / Production Software  
**Title:** Internal Project-Management Platform  
**One-sentence description:** A production internal platform migrated from a no-code prototype to a React/Vite + Supabase/Postgres system deployed on Vercel.

**Technical summary:** Public-safe treatment should emphasize ownership of architecture, relational data modelling, role-based permissions with Postgres RLS, deployment/release process, security hardening, QA, documentation, and requirements translation.

**Capabilities demonstrated:**
- software architecture
- full-stack development
- relational data modelling
- authorization/security
- deployment
- QA/documentation
- product requirements translation

**Technologies:** React, Vite, Supabase, PostgreSQL, row-level security, Vercel.

**Recommended visuals:** public-safe high-level architecture graphic. No private screenshots unless separately approved.

**CTA:** `View software case study →`

## Section 3 — Operational systems

### Purpose
Demonstrate that engineering responsibility extends beyond coursework and app code.

### Project
Broadway Moving and Storage — Infrastructure & Fleet Systems

### Treatment
A wide editorial row or two-column section, not necessarily a full route.

### Copy direction
> Self-hosted infrastructure, internal systems, physical-security integration, and GPS-driven fleet automation supporting a live moving-and-storage operation.

### Evidence to surface
- sole technical resource
- infrastructure specification/deployment
- internal systems
- NVR integration
- fleet automation
- ongoing maintenance/support

### Visual
Sanitized architecture/data-flow diagram only unless approved photographs become available.

## Section 4 — Engineering range

### Purpose
Show breadth without diluting flagship projects.

### Groups

**Embedded & Systems Labs**
- ENSC 351 embedded Linux lab work
- SPI/spidev hardware interaction
- HAL-style C organization
- early Pico/MicroPython work only if needed

**Software Systems**
- DragonsDash as a supporting personal software project
- emphasize testing, state/data handling, import parsing and product architecture
- do not overstate production/security status

**Lab / Archive**
- selected C/Java coursework only when it fills a real capability gap
- Tarkov-inspired Android prototype only if visually rebranded and authorship/generation provenance is comfortable to discuss
- omit OpenJarvis fork
- omit low-value creator/web work from the homepage

### Visual treatment
Compact rows/index entries rather than large repeated cards.

## Section 5 — Experience

### Purpose
Show progression toward whole-system ownership.

### Timeline
**MAKE Projects LTD — Project Coordinator / Software Developer → Full Stack Developer / Technical Resource, 2026-present**
- internal production software
- architecture/security/deployment
- requirements translation

**Broadway Moving and Storage — IT Technician, 2023-present**
- self-hosted infrastructure
- internal systems
- fleet automation
- operations/support

**Broadway Moving and Storage — Driver, 2020-present**
- concise note only if useful: operational exposure later informed internal systems work

**Point Grey Projects — Apprentice Carpenter, 2021**
- optional one-line entry to show physical construction/project context
- do not let this dominate technical experience

## Section 6 — Engineering index

### Purpose
Allow scanning across systems layers.

Use a systems-oriented index, not ratings.

Suggested structure:

```text
PHYSICAL / AUTONOMOUS
UAV integration · LiDAR · camera systems · flight-control interface

EMBEDDED / SYSTEMS
Embedded Linux · SPI · hardware abstraction · C/C++ · Python

SOFTWARE ARCHITECTURE
React/Vite · data modelling · application architecture · testing

DATA / SECURITY
PostgreSQL · Supabase · RLS · role-based permissions

INFRASTRUCTURE / OPERATIONS
Self-hosted systems · deployment · release process · operational support

AI-ENABLED ENGINEERING
Agentic coding workflows · spec-driven implementation · validation/evaluation
```

Do not claim proficiency levels.

## Section 7 — Contact

Use:
- GitHub
- LinkedIn
- email

No mobile phone number.

# 3. Hero copy directions

Five valid directions:

### A — Recommended
**Systems engineering across physical systems, software architecture, and production infrastructure.**

### B
**Building across the boundary between hardware, embedded systems, and production software.**

### C
**From sensors and control loops to databases, security, and deployed software.**

### D
**Systems/software engineering for real physical and operational constraints.**

### E
**Engineering systems end to end—from embedded sensing to production applications.**

**Recommendation:** A. It is the clearest and least promotional. Use C as supporting copy or section language.

# 4. Featured project hierarchy

## Flagship 1 — Autonomous UAV
Dedicated case-study route. Strongest proof of physical + embedded + software integration.

## Flagship 2 — Internal Project-Management Platform
Dedicated case-study route. Strongest proof of professional production ownership.

## Supporting — Broadway Infrastructure & Fleet Systems
Homepage treatment; dedicated route only if enough safe visual/evidence material becomes available.

## Supporting — DragonsDash
Projects-index item showing modern TypeScript/Next.js product engineering. Do not compete visually with flagships.

## Collection — Embedded & Systems Labs
Grouped coursework/lab evidence.

# 5. Autonomous UAV case study

Route: `/projects/autonomous-uav`

## Header
- `AUTONOMOUS SYSTEMS / TEAM PROJECT / 2025`
- Autonomous UAV
- one-sentence description
- technologies
- public GitHub source link
- team-project attribution

## Context
SFU ENSC 351 final project. Preserve team attribution.

## Problem
Explain the integration problem, not a fabricated competition/business problem:
combine camera perception, LiDAR sensing and flight-control communication into an embedded autonomous-control system.

## System
Show the physical/software stack:
- camera subsystem
- ESP32/SPI transport where applicable
- embedded Linux compute
- YOLO/ONNX perception
- LiDAR input/filtering
- fusion/control logic
- MAVLink
- flight controller
- propulsion path

## Architecture
Use a responsive vector diagram based on verified implementation.

### Primary diagram
```text
Camera
  ↓ SPI
Camera Transport / ESP32
  ↓ SPI
Embedded Linux Compute
  ├── YOLO / ONNX Person Detection
  ├── LiDAR Input + Filtering
  └── Fusion / Control Logic
                ↓ MAVLink
          Flight Controller
                ↓
            ESC / Motors
```

Reconcile exact hardware path with source before final labels.

## Perception
Explain:
- OpenCV preprocessing
- ONNX Runtime
- YOLOv8n model
- person-class filtering
- bounding-box centre/area used by control logic

Do not publish inferred accuracy metrics.

## Sensors
Explain LiDAR input and filtering at a high level.
Do not invent sensor range/performance metrics.

## Control
Explain verified priority:
1. obstacle avoidance
2. person-following/alignment logic
3. MAVLink velocity/yaw commands

## Integration
Focus on interfaces:
- SPI
- sensor data
- embedded process
- MAVLink/flight controller

## Constraints
- embedded compute
- multi-device communication
- physical integration
- noisy sensor data
- team project attribution
- limited portfolio-ready test evidence

## Contribution
Do **not** imply sole authorship.

Use wording such as:
> I worked on the team-built system across software integration and embedded/autonomy components; the case study reflects the verified shared system architecture. Specific personal contribution claims should only be added where authorship is established.

If the user later provides an exact contribution breakdown, replace this generic wording.

## Outcome
Only state demonstrated facts. Do not claim full autonomous-flight success unless evidence is supplied.

## Technologies
Python · pymavlink / MAVLink · OpenCV · ONNX Runtime · YOLOv8n · SPI · ESP32 / Arduino · LiDAR · embedded Linux

## Source
Public GitHub repository.

## Visuals
1. assembled UAV photograph
2. clean vector architecture diagram
3. consent-safe person-detection frame if available
4. small source excerpt only if it explains an interface/control decision

# 6. Internal Project-Management Platform case study

Route: `/projects/internal-project-management-platform`

## Header
- `PRIVATE / PRODUCTION SYSTEM / 2026–PRESENT`
- Internal Project-Management Platform
- concise architecture summary
- no GitHub link

## Context
Built inside MAKE Projects from a pre-existing no-code prototype.

## Problem framing
Use only public-safe language:
translate project-management workflows and requirements into an internal software platform.

Do not expose client/project names or proprietary workflows.

## Architecture
High-level public diagram only:

```text
React / Vite Frontend
        ↓
Application / Data Access
        ↓
Supabase
        ↓
PostgreSQL + Row-Level Security
        ↓
Vercel Deployment / Release Workflow
```

This is a communication abstraction, not a full implementation diagram.

## Responsibilities to communicate
- migration from prototype
- frontend/backend ownership
- relational data modelling
- role-based permission architecture
- RLS
- deployment/release process
- security hardening
- QA/testing workshops
- technical documentation
- translating non-software stakeholder requirements
- agentic engineering workflow

## Agentic workflow
Treat as process discipline:
- repo-level specs
- CLI coding agents
- separate architecture/debugging context
- persistent decision logging
- five-stage validation
- read-only database-permission auditing

Avoid naming model vendors unless useful and current.

## Constraints
- private company IP
- solo technical ownership
- non-software stakeholders
- production responsibility
- security/privacy
- public communication boundaries

## Outcome
Do not invent usage, savings or impact metrics.
Safe outcome language:
> The platform was deployed internally and continued under active development.

## Visuals
- public-safe architecture graphic
- no private screenshot by default
- optional employer-approved sanitized screenshot later

# 7. Broadway infrastructure treatment

Default: homepage supporting feature + projects-index entry.

Do not create a dedicated case-study page until safe visuals or more public technical specifics are approved.

### Title
Infrastructure & Fleet Systems

### Copy
> Self-hosted infrastructure and internal operational systems, including physical-security integration and GPS-driven fleet automation, maintained for a live moving-and-storage business.

### Supporting bullets
- server/infrastructure deployment and maintenance
- internal business systems
- NVR/physical-security integration
- fleet automation
- frontline technical support

### Visual
Sanitized system diagram; never expose topology, addresses, live vehicle data, feeds or credentials.

# 8. Secondary engineering work

## Embedded & Systems Labs
A compact grouped collection.

Possible entries:
- ENSC 351 embedded Linux / SPI
- Raspberry Pi Pico introductory project
- selected C systems/coursework only if individually meaningful

## DragonsDash
Supporting standalone project.

### One-line description
A TypeScript/Next.js personal-finance application prototype with state management, calculations, CSV import/parsing and automated tests.

### Technologies
Next.js · React · TypeScript · Tailwind · Zustand · Vitest

### Visuals
Capture synthetic-data screens after build verification.

## Lab/Archive
Keep sparse.
Do not include OpenJarvis fork as original work.
Do not surface every GitHub repository.

# 9. About

Recommended copy:

> I'm a Systems Engineering student at Simon Fraser University working across software, embedded systems, infrastructure, and autonomous systems. My professional work has centred on owning an internal production software platform end to end; outside that, my strongest engineering work includes embedded perception/control systems and operational infrastructure.
>
> I tend to work at interfaces—between sensors and software, users and data models, or deployment and operations. I use AI coding agents heavily, but as engineering infrastructure: implementation is constrained by specifications, review, testing, and explicit validation rather than treated as an automatic result.

Keep this to roughly 100-150 words on the live site.

# 10. Experience

Use concise entries, not full LinkedIn copy.

### MAKE Projects LTD
**Full Stack Developer / Technical Resource**  
2026-present  
Internal project-management platform: architecture, full-stack development, data/security model, deployment, QA and documentation.

### Broadway Moving and Storage
**IT Technician**  
2023-present  
Self-hosted infrastructure, internal systems, fleet automation, physical-security integration and technical operations.

### Optional context
Driver role and carpenter role may appear as compact secondary entries if they strengthen the real-world/physical-systems narrative.

# 11. Engineering index

Use the index defined in the homepage specification.
No percentages, stars, ratings, or "expert/intermediate" labels.

# 12. Contact

Display:
- GitHub
- LinkedIn
- email

Do not display:
- mobile number
- address
- private social accounts

# 13. Content source map

## Homepage hero
Source: synthesis of PROJECT-INVENTORY + PORTFOLIO-NARRATIVE; wording must not exceed claims register.

## UAV
Source: public Autonomous-UAV-project repository + approved asset inventory.

## Internal platform
Source: supplied LinkedIn export and public-safe claims register only.

## Broadway
Source: supplied LinkedIn export only unless new approved evidence is added.

## DragonsDash
Source: public GitHub repository code/package configuration.

## Embedded labs
Source: public ENSC351 / ensc100RPiPico repositories.

## Experience / About
Source: LinkedIn export + claims register.

Any public statement not mapped above must be checked against `CLAIMS-REGISTER.md` before inclusion.
