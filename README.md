# Humaicraft Foundation

> Software begins with philosophy.

Humaicraft Foundation is the shared home of the ideas, values, principles, commitments, and vocabulary that guide every Humaicraft project.

The goal is not to define every implementation detail. It is to provide a durable reference for making decisions when technologies, products, teams, and circumstances change.

## Purpose

Build a durable foundation before building products.

Humaicraft exists to support **Building Better Builders**: helping people and AI create software that remains understandable, safe, maintainable, accessible, and valuable for the long term.

Humans retain judgment, responsibility, and final authority. AI contributes as a teammate that helps explore, verify, document, and improve the work.

## Scope

This repository owns Humaicraft's enduring philosophy and organization-level direction:

- vision, mission, values, and principles;
- manifesto and charter;
- shared vocabulary;
- durable governance boundaries;
- ecosystem-level responsibility decisions.

## Non-goals

This repository does not own:

- coding conventions or implementation checklists;
- Git and GitHub procedures;
- framework-specific guidance;
- project-specific architecture or requirements;
- reusable UI components, templates, or packages.

Practical guidance belongs in [`humaicraft-guidelines`](https://github.com/Humaicraft/humaicraft-guidelines). Implementation details remain with the project or shared asset that owns them.

## Foundation documents

- [Vision](foundation/VISION.md) — the future Humaicraft seeks to help create
- [Mission](foundation/MISSION.md) — how Humaicraft works toward that future
- [Values](foundation/VALUES.md) — what Humaicraft chooses to protect and prioritize
- [Principles](foundation/PRINCIPLES.md) — how those values guide decisions
- [Manifesto](foundation/MANIFESTO.md) — a public declaration of Humaicraft's beliefs
- [Charter](foundation/CHARTER.md) — durable commitments, boundaries, and authority
- [Glossary](foundation/GLOSSARY.md) — shared definitions for recurring terms

## How the documents relate

```text
Charter
  ↓
Vision and Mission
  ↓
Values
  ↓
Principles
  ↓
Guidelines and Standards
  ↓
Patterns and Products
```

The Charter defines durable boundaries. Vision and Mission define direction and purpose. Values describe what matters. Principles guide decisions. Guidelines, standards, patterns, and products turn the Foundation into practice.

## Repository responsibility model

| Layer | Primary responsibility | Typical location |
| --- | --- | --- |
| Philosophy | Why Humaicraft exists and what it protects | `humaicraft-foundation` |
| Standards | How Humaicraft works and builds | `humaicraft-guidelines` |
| Shared assets | Reusable design and engineering assets | Design system, templates, shared packages |
| Products | User-facing tools and services | Individual product repositories |
| Community | Public communication and participation | Website, organization profile, Discussions |

Every Humaicraft repository should clearly state its **Purpose**, **Scope**, **Non-goals**, and **Relationships**.

See [ADR-0001: Repository Responsibility Model](decisions/0001-repository-responsibility-model.md) for the decision, trade-offs, and migration rules.

## Core commitments

- people and their safety come before implementation convenience;
- humans remain accountable for consequential decisions;
- AI is a teammate, not a replacement for responsibility;
- correctness, clarity, maintainability, accessibility, and reproducibility matter more than short-term speed;
- important behavior and decisions should be explicit;
- work should be built in small, reviewable steps;
- failures and lessons should be preserved rather than hidden;
- documentation is part of the product;
- releases are milestones in continued growth, not finish lines.

## Repository structure

```text
foundation/  Core philosophy and shared vocabulary
decisions/   Architecture and governance decision records
identity/    Brand and communication materials (future phase)
docs/        Supporting documentation and maintainer guidance (future phase)
```

See [ROADMAP.md](ROADMAP.md) for current progress and planned phases.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing or submitting a change.

Participation in Humaicraft spaces is governed by the [Code of Conduct](CODE_OF_CONDUCT.md). Do not place credentials, personal information, private evidence, or sensitive vulnerability details in public Issues or Pull Requests.

Use the Issue templates to report a problem or propose an improvement. Significant changes should explain the problem, recommendation, trade-offs, risks, affected documents, and completion conditions.

Keep each Pull Request focused on one purpose. Useful ideas outside the current goal should be preserved as follow-up Issues rather than silently expanding scope.

## Status

Humaicraft Foundation is a living project in active development.

**v0.1.0 — The First Seed** established the first reviewable Foundation. The current cleanup work defines repository boundaries and prepares the next stage of the Humaicraft ecosystem.

## License

Unless otherwise noted, the contents of this repository are licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](LICENSE) (`CC-BY-SA-4.0`).

This license permits sharing and adaptation, including commercial use, with attribution, an indication of changes, and distribution of adaptations under the same license. It does not grant rights to third-party trademarks, logos, personal information, or material for which contributors do not hold the necessary rights.
