# ADR-0001: Repository Responsibility Model

- Status: Accepted
- Date: 2026-07-29
- Decision owners: Humaicraft maintainers
- Related issue: #6

## Context

Humaicraft is growing from a single foundation repository into an ecosystem of philosophy, practical guidance, shared assets, products, and community spaces.

Without explicit boundaries, enduring principles can become mixed with implementation procedures, project-specific requirements can be copied into organization-wide guidance, and contributors can struggle to determine where a change belongs.

The responsibility model must keep stable ideas separate from practices that change with tools, projects, and experience. It must also allow future repositories to be introduced without redefining the entire ecosystem.

## Decision

Humaicraft will organize repositories and documentation into five responsibility layers.

| Layer | Primary responsibility | Typical location |
| --- | --- | --- |
| Philosophy | Why Humaicraft exists and what it protects | `humaicraft-foundation` |
| Standards | How Humaicraft works and builds | `humaicraft-guidelines` |
| Shared assets | Reusable design and engineering assets | Design system, templates, shared packages |
| Products | User-facing tools and services | Individual product repositories |
| Community | Public communication and participation | Website, organization profile, Discussions |

### Foundation

`humaicraft-foundation` is the durable source for Humaicraft's purpose, vision, mission, values, principles, manifesto, charter, shared vocabulary, and organization-level direction.

It does not own coding conventions, Git procedures, framework-specific guidance, project requirements, or implementation checklists.

### Guidelines

`humaicraft-guidelines` explains how the Foundation is applied in practice. It may contain shared guidance for development, AI collaboration, security, accessibility, testing, architecture, Git and GitHub workflow, releases, and documentation.

It does not redefine Humaicraft's mission or values, own product requirements, or duplicate implementation details maintained by individual projects.

### Shared assets

Shared-asset repositories provide reusable implementation resources such as design tokens, components, templates, and packages. They must state which Foundation principles and Guidelines they implement, while keeping asset-specific documentation close to the asset.

### Products

Product repositories own their domain requirements, architecture, code, tests, operations, and release history. They reference Foundation and Guidelines rather than copying them as independent policy.

### Community

Community-facing repositories and spaces explain Humaicraft publicly, support participation, and provide navigation across the ecosystem. They do not become alternate sources of philosophy or engineering policy.

## Repository contract

Every Humaicraft repository should make the following explicit in its primary documentation:

1. **Purpose** — why the repository exists;
2. **Scope** — what it owns;
3. **Non-goals** — what it intentionally does not own;
4. **Relationships** — how it depends on or supports other repositories.

When content could fit more than one layer, ownership is determined by the most specific durable responsibility. Other repositories link to the owning source instead of duplicating it.

## Consequences

### Positive

- Contributors can identify the correct home for a proposal.
- Foundation remains stable as tools and implementation practices evolve.
- Guidelines can change independently without rewriting organizational philosophy.
- Project-specific decisions remain close to the projects they affect.
- Duplication and contradictory policy are easier to detect during review.

### Trade-offs

- Cross-repository changes may require coordinated Issues or Pull Requests.
- Moving existing content requires traceable migration rather than simple deletion.
- Contributors must follow links across repositories instead of finding every detail in one place.

These trade-offs are accepted because explicit ownership is more maintainable than a single repository with mixed responsibilities.

## Security and accessibility

- Repository boundaries do not permit secrets, personal information, private evidence, or unpublished vulnerability details to be copied into public documentation.
- Diagrams must have equivalent text descriptions.
- Navigation and document structure must remain usable with keyboard and assistive technologies.
- Security rules that apply to one implementation stay with that implementation unless they are genuinely shared guidance.

## Migration and rollback

Existing content will be reviewed before movement. Migrations should preserve Git history where practical and leave links or notes when readers may rely on an old location.

If this model proves insufficient, it can be superseded by a later ADR. Rollback must not silently discard guidance; ownership changes must be documented in the roadmap and changelog.

## Validation

This decision is accepted because:

- a contributor can determine where a proposed document belongs;
- Foundation and Guidelines describe compatible boundaries;
- no existing policy is removed without a traceable destination;
- the README links to this decision and summarizes the responsibility model.
