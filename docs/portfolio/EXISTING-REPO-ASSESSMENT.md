# Existing Repository Assessment

Repository: `essewell/essewell-website`
Branch assessed: `portfolio-build`
Last reviewed 2026-09-24.

## 1. Current stack

There is currently **no application framework or runtime stack committed** on `portfolio-build`.

The branch contains:
- `AGENTS.md`
- `README.md`
- `linkedin profile.pdf`

The separate research branch contains `ASSET-INVENTORY.md`, but the build branch did not yet contain the required portfolio documentation when this assessment was performed.

There is currently no:
- `package.json`
- source directory
- routing layer
- component system
- styling framework
- test configuration
- lint/typecheck configuration
- deployment configuration in-repo
- public asset hierarchy for the portfolio

## 2. Current architecture

Effectively greenfield at the application level, despite the repository itself already being the canonical production target.

The useful architecture that already exists is **process architecture**, not code:
- a dedicated `portfolio-build` branch
- `AGENTS.md` defining mission, privacy, source-of-truth rules and validation expectations
- a canonical Work -> Codex -> review workflow external to the branch
- a separate research branch containing an asset inventory

## 3. Existing useful work

### Retain
- `AGENTS.md` — this is valuable and should remain the agent policy file.
- `README.md` — retain the file path, but rewrite content after implementation.
- `portfolio-build` branch — correct place for implementation.
- Research work already completed, especially the asset inventory.

### Process decisions worth retaining
- evidence-backed claims
- privacy-first handling of MAKE/Broadway material
- first-viewport human gate
- explicit visual QA
- five-stage final audit
- no generic AI-portfolio aesthetic
- focus on systems engineering rather than frontend identity

## 4. Existing weak work

There is no substantive application code to preserve or criticize yet.

The main weakness is organizational:
- required research/specification files were not consolidated under `docs/portfolio/`
- the existing asset inventory lived on a separate branch at repository root
- the public repository contains the unredacted LinkedIn PDF, including a mobile telephone number

## 5. Technical debt

### Immediate
1. **Privacy debt:** remove the unredacted LinkedIn PDF from the public working tree before launch.
2. **Documentation drift:** consolidate all portfolio specs under `docs/portfolio/`.
3. **Branch divergence:** research output should be copied/reconciled into `portfolio-build`, not left isolated on a research branch.
4. **No implementation scaffold:** framework, tooling and deployment setup still need to be established.

### Later
5. Add build/lint/typecheck/test scripts.
6. Add image-processing/optimization strategy.
7. Add metadata/SEO.
8. Add route/content data model.
9. Add deployment configuration if Vercel defaults are insufficient.

## 6. What should be retained

- Existing repository itself.
- `portfolio-build`.
- `AGENTS.md`.
- Evidence-first research process.
- Dark technical visual direction.
- IBM Plex Sans / IBM Plex Mono design direction.
- UAV and professional software as dual flagships.
- Human approval gate before full build.

## 7. What should be redesigned

There is not yet a UI to redesign.

The implementation should be designed from the verified content specification, not from the current README or raw LinkedIn document.

## 8. What should be removed

Before production:
- unredacted `linkedin profile.pdf` from public branch/working tree
- any future private source document accidentally copied into `public/`
- any generated placeholder content that cannot map to `CLAIMS-REGISTER.md`

Consider repository-history cleanup for the LinkedIn PDF if permanent removal of the mobile number from git history is required.

## 9. What should be added

Required documentation:
- `docs/portfolio/PROJECT-INVENTORY.md`
- `docs/portfolio/PORTFOLIO-NARRATIVE.md`
- `docs/portfolio/CLAIMS-REGISTER.md`
- `docs/portfolio/ASSET-INVENTORY.md`
- `docs/portfolio/EXISTING-REPO-ASSESSMENT.md`
- `docs/portfolio/PORTFOLIO-CONTENT-SPEC.md`
- `docs/portfolio/DESIGN-SYSTEM.md`

Implementation scaffold, to be selected in Codex B1:
- package/runtime configuration
- app/source structure
- route structure
- design tokens
- project content model
- public project assets
- testing/lint/typecheck
- Vercel-ready build

## 10. Is the current project structure appropriate?

The repository is appropriate; the application structure does not yet exist.

No framework migration is needed because there is nothing to migrate.

A clean implementation can be introduced directly on `portfolio-build`.

## 11. Are dependency/framework changes justified?

No "change" exists yet.

The implementation agent should choose a small, maintainable stack appropriate for a static/mostly-static engineering portfolio. The canonical workflow says Codex should reconcile framework choice with actual repository needs rather than rewrite for novelty.

A sensible implementation target would likely be a modern React-capable static/SSR framework with strong TypeScript support and Vercel compatibility, but **the exact framework decision belongs in `docs/IMPLEMENTATION-PLAN.md` during Codex B1**.

Do not add:
- a CMS unless a concrete editing need appears
- a database
- auth
- heavy animation frameworks without need
- large UI kits that push the site toward a generic SaaS look

## 12. Risks Codex should understand

1. **Factual risk:** private professional work is easy to overstate.
2. **Privacy risk:** public repository currently contains a source PDF with a phone number.
3. **Design risk:** generic AI-generated portfolio patterns would actively undermine the intended identity.
4. **Narrative risk:** too many small school/web projects will dilute the flagship work.
5. **Attribution risk:** UAV is a team project; do not imply sole authorship.
6. **Asset risk:** several useful images require teammate/employer/person consent.
7. **Diagram risk:** technical graphics must correspond to real architecture.
8. **Mobile risk:** complex technical diagrams must remain understandable at narrow widths.

## Recommended next action

Finish and commit all seven `docs/portfolio/` files to `portfolio-build`, then run Codex B1 to create `docs/IMPLEMENTATION-PLAN.md` before implementing the first viewport.
