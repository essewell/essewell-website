# Design System

Last reviewed 2026-09-24.

## Direction

**Aerospace Engineering Laboratory × Modern Developer Tooling × Technical Editorial Publication**

The site should feel designed for an engineer who works across hardware and software.

It must not resemble:
- cyberpunk
- gaming UI
- crypto
- generic AI startup
- generic developer portfolio
- SaaS dashboard

## Typography

### Families
- **Primary:** IBM Plex Sans
- **Technical labels / metadata:** IBM Plex Mono
- **Editorial serif:** none by default. Introduce only if a specific composition genuinely benefits.

### Type scale

Use fluid sizing with restrained contrast.

Suggested tokens:
- `--type-display: clamp(3rem, 7vw, 6.5rem)`
- `--type-h1: clamp(2.4rem, 5vw, 4.5rem)`
- `--type-h2: clamp(1.9rem, 3.5vw, 3rem)`
- `--type-h3: clamp(1.35rem, 2vw, 1.8rem)`
- `--type-body-lg: clamp(1.05rem, 1.25vw, 1.25rem)`
- `--type-body: 1rem`
- `--type-small: 0.875rem`
- `--type-micro: 0.75rem`

### Line height
- display: 0.96-1.02
- headings: 1.05-1.15
- body: 1.55-1.7
- mono labels: 1.35-1.5

### Tracking
- large display: slightly tight, around -0.03em
- headings: -0.015em to -0.025em
- body: normal
- mono labels: +0.05em to +0.09em, often uppercase

### Measures
- long-form case-study prose: 62-72ch
- hero supporting copy: 38-52ch
- technical metadata: allow wider rows but avoid dense full-width paragraphs

## Color

Restrained, instrumentation-like palette.

Suggested tokens:

```css
:root {
  --bg-0: #0b0f12;
  --bg-1: #11171b;
  --bg-2: #182026;
  --surface-subtle: #1d262c;
  --text-0: #edf1f2;
  --text-1: #c7d0d3;
  --text-2: #8f9ca2;
  --line: #2a353b;
  --line-strong: #3a4950;
  --accent: #6f9fa8;
  --accent-muted: #41636a;
  --success-muted: #75917b;
  --warning-muted: #a58c63;
}
```

The accent should read as sensor/instrumentation cyan-grey, never neon.

No purple gradient system.

## Grid

### Desktop
- max content width: 1440px
- primary reading width: 1180-1280px
- 12-column grid
- outer margins: clamp(24px, 4vw, 72px)
- gutters: 20-28px

### Tablet
- 8-column conceptual grid
- 24-32px outer margin

### Mobile
- 4-column conceptual grid
- 18-22px outer margin
- prioritize readable hierarchy over preserving desktop geometry

### Vertical spacing
Suggested scale:
`4, 8, 12, 16, 24, 32, 48, 64, 96, 128, 160`

Large sections should normally use 96-160px desktop vertical spacing and 64-96px mobile.

## Component language

### Navigation
- thin, quiet, editorial
- no pill-heavy nav
- name/mark left; Projects/About/Contact right
- optional mono coordinate/index label
- sticky only if it remains visually quiet

### Hero
- asymmetric grid
- large identity/discipline typography
- concise support copy
- one meaningful UAV/system schematic
- no giant rounded "hero card"
- no fake terminal window

### Project index
Use editorial rows, split layouts and image/diagram-led compositions rather than repeating identical cards.

### Featured project
Each flagship should feel like a case-study teaser:
- category/label
- title
- one-line system description
- technologies/constraints
- meaningful image or architecture diagram
- direct case-study CTA

### Case-study header
- project category
- project title
- concise technical summary
- context/year/team metadata
- hero image or system diagram
- optional source link where public

### Technical metadata
IBM Plex Mono, compact, subtle separators, no badge-wall aesthetic.

### Architecture diagrams
- thin strokes
- rectangular blocks with minimal radius
- directional connectors
- labels that correspond to real system interfaces
- no gauges or numbers unless they are factual and useful
- highlight pathways with the muted accent
- on mobile, collapse into vertically stacked signal flow rather than shrinking unreadably

### Code excerpts
Use sparingly. Prefer 8-20 lines with annotation. Do not use code as decoration.

### Timeline
Editorial vertical or stepped line; emphasize responsibility and technical progression rather than résumé density.

### Buttons and links
Prefer text links with arrows or understated bordered controls.
Border radius: 0-6px, not pill-shaped by default.

### Image captions
Mono/micro text, factual, with project context and source/attribution where needed.

### Footer
Minimal; GitHub, LinkedIn, email; no phone number.

## Engineering-label grammar

Use concise mono labels such as:
- `AUTONOMOUS SYSTEMS / 2025`
- `PRIVATE / PRODUCTION SYSTEM`
- `SENSING -> PERCEPTION -> CONTROL`
- `EMBEDDED LINUX`
- `CASE STUDY 01`

Labels should orient the reader, not imitate military HUD graphics.

## Technical graphics grammar

### Blocks
Represent actual subsystems:
- Camera
- ESP32
- SPI
- Embedded Linux Compute
- YOLO/ONNX
- LiDAR
- Sensor Fusion / Control Logic
- MAVLink
- Flight Controller
- ESC/Motors

Only include a block if supported by verified project evidence.

### Connectors
- solid line: primary data/control path
- dashed line: optional/secondary relationship only if real
- arrowheads: direction of data/control
- tiny mono labels can name protocol/interface: `SPI`, `UART/MAVLink`

### Annotation
Annotations may identify:
- protocol
- responsibility boundary
- processing stage
- privacy-safe constraint

No fake latency, signal strength, battery percentage or coordinate telemetry.

## Autonomous UAV treatment

Use the UAV as the visual anchor of the site.

Recommended case-study system diagram:

```text
Camera
  ↓ SPI
ESP32 / Camera Transport
  ↓ SPI
Embedded Linux Compute
  ├─ YOLO / ONNX Person Detection
  ├─ LiDAR Input + Filtering
  └─ Sensor Fusion / Control Logic
             ↓ MAVLink
       Flight Controller
             ↓
         ESC / Motors
```

This is a conceptual simplification of verified source and should be reconciled against the exact final architecture before implementation.

Visual material priority:
1. real assembled-UAV photo
2. clean vector architecture diagram
3. consent-safe perception frame
4. compact code excerpt only where useful

## Motion

Allowed:
- subtle section reveal
- line/path highlight on architecture diagram
- project-row hover
- very restrained page transition

Rules:
- motion must communicate hierarchy or flow
- never block reading
- respect `prefers-reduced-motion`
- keep durations generally 120-300ms

Disallowed:
- scroll hijacking
- parallax spectacle
- particle fields
- animated background noise
- cursor followers
- looping ornamental motion
- typing hero text

## Responsive behavior

### 360 / 390
- single-column content
- nav must remain simple
- hero graphic stacks below copy
- diagrams become vertical signal paths
- metadata wraps intentionally
- no horizontal scroll
- minimum touch targets about 44px

### 768
- selective two-column layouts
- case-study diagrams can use simplified horizontal grouping if legible

### 1024
- restore stronger grid relationships
- flagship project split layouts

### 1440
- full 12-column composition
- ample whitespace
- asymmetric editorial layouts

### 1920
- do not stretch prose
- hold max widths
- use negative space intentionally rather than scaling everything up

## Visual anti-pattern checklist

Reject implementation that contains:
- glowing gradient blobs
- purple/blue AI gradients
- repeated glass cards
- fake terminal windows
- excessive corner radius
- technology-logo walls
- skill bars
- animated typing
- fake telemetry
- meaningless charts
- decorative 3D orbits
- generic stock coding imagery
- repetitive three-card grids for every section

## Accessibility design requirements

- body contrast must meet WCAG AA
- focus state clearly visible
- diagrams require text equivalents/captions
- color must not be sole carrier of meaning
- reduced-motion mode must remove nonessential animation
- headings must preserve logical hierarchy

## Art-direction test

A successful page should look plausible as:
- an aerospace lab project page
- a premium developer-tooling product page
- an engineering editorial spread

without becoming any one of those literally.
