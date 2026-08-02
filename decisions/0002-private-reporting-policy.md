# ADR-0002: Private Reporting Policy

- Status: Accepted
- Date: 2026-08-02
- Decision owner: Webnist
- Related issue: #5

## Context

Humaicraft needs a private path for security vulnerabilities, Code of Conduct concerns, and privacy or personal-data incidents. Public Issues and Pull Requests are not appropriate for credentials, personal information, private evidence, or sensitive vulnerability details.

Humaicraft is currently maintained by one person, so the first version must be honest about its operational limits and must not claim protections that do not yet exist.

## Decision

Humaicraft will use the following initial private reporting model.

### Contact

- Primary private contact: `report@humaicraft.com`
- The same intake initially receives security, conduct, and privacy reports.
- Reporters may optionally prefix the subject with `[Security]`, `[Conduct]`, or `[Privacy]`.
- Classification is the maintainer's responsibility; reporters are not required to choose correctly.

### Responsibility

- Primary maintainer: Webnist
- Fallback maintainer: not yet assigned
- Until a fallback maintainer exists, Humaicraft cannot provide an independent conflict-of-interest route for reports concerning the primary maintainer.
- This limitation must remain visible and must not be represented as resolved.

### Response targets

- Acknowledgement target: within 3 business days
- Initial assessment target: within 7 business days
- These are targets, not guaranteed service-level commitments.
- High-risk reports should be prioritized when reasonably possible.

### Retention

- Active reports are retained until resolution.
- Resolved reports are retained for 12 months by default.
- Information that is not necessary for investigation or follow-up should be deleted earlier.
- Retention may be extended only when legal, audit, or unresolved operational needs justify it.
- Access must be limited to designated maintainers.

### Conflict of interest

The intended model is a separate fallback recipient for reports concerning the primary maintainer. Because Humaicraft currently has one maintainer, this route is not yet operational.

A fallback contact must be approved and tested before public documentation claims independent handling.

### GitHub Private Vulnerability Reporting

GitHub Private Vulnerability Reporting should be enabled for security vulnerabilities where supported. It supplements `report@humaicraft.com`; it does not replace conduct or privacy reporting.

## Operational prerequisites

The public reporting process is considered operational only after all of the following are verified:

1. `report@humaicraft.com` exists and can receive external mail;
2. access is protected with multi-factor authentication where supported;
3. credentials are not shared through source control, Issues, Pull Requests, or logs;
4. a test report is received and acknowledged without real sensitive data;
5. retention and deletion can be performed;
6. public documentation points to the same current process.

The fallback route remains a known limitation until a second trusted maintainer is appointed and tested.

## Security and privacy

- Collect only information necessary to understand and respond to the report.
- Do not copy sensitive report content into public Issues, Pull Requests, release notes, or unrestricted logs.
- Do not promise confidentiality beyond the actual technical and organizational controls.
- Do not use real vulnerability or personal data in process tests.
- Remove unnecessary attachments, credentials, tokens, and personal data as soon as practical.

## Accessibility

- Reporting instructions must be available as text and must not depend on diagrams or color.
- Reporters must not be required to use a specific inaccessible document format.
- Expected next steps and response targets should be stated clearly.
- Alternative accessible arrangements should be considered when requested and operationally possible.

## Consequences

### Positive

- Humaicraft has one consistent intake for three sensitive report types.
- The model is simple enough for the current project size.
- Response and retention expectations are explicit.
- Known limitations are documented rather than hidden.

### Trade-offs and limitations

- One-person operation creates continuity and conflict-of-interest risk.
- The shared intake provides less separation between report types.
- Response targets may be affected by maintainer availability.
- Independent conduct review is not available until a fallback maintainer is appointed.

## Migration and rollback

Public repository instructions must not point to `report@humaicraft.com` until delivery and access are tested.

If the mailbox becomes unavailable or unmonitored, public guidance must be reverted to a temporary warning that prevents public disclosure and clearly states that the dedicated private channel is unavailable.

A later ADR may supersede this policy when Humaicraft adds maintainers, separates reporting channels, changes retention, or adopts a dedicated case-management system.

## Review

Review this policy after three months of operation, after the first material report, or whenever maintainership or mailbox ownership changes—whichever comes first.
