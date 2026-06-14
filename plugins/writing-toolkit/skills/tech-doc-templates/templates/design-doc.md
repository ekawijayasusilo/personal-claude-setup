<!-- WHEN TO USE THIS TEMPLATE
     Design doc = plan substantial engineering work before build: new system,
     significant feature, hard/novel problem, or cross-team coordination. It
     answers "HOW will we build this?" Direction is broadly agreed.

     Skip for trivial/well-understood work. If deciding whether/which direction
     and alternatives are live, write RFC. If recording one converged decision,
     write ADR.

     Value: early feedback while changes are cheap; writing forces design
     clarity; cross-cutting concerns become hard to forget.

     Lifecycle: useful during design. Not living source of truth after build;
     code owns truth, doc becomes history.

     Length: enough, no more. One page can be fine; large system maybe 10-20.
     Past ~20 pages, split problem. Delete non-applicable sections.

     Strip this comment block before publishing. -->

# Design Doc: [System or feature name]

<!-- guidance: Name thing concretely. Bad: "Design Doc: Backend improvements."
     Good: "Design Doc: Real-time presence service." -->

| Field | Value |
|---|---|
| Author(s) | [names] |
| Reviewers | [names or teams] |
| Status | Draft / In review / Approved / Implemented / Obsolete |
| Created | YYYY-MM-DD |
| Last updated | YYYY-MM-DD |

## Context and scope

<!-- guidance: Objective background: landscape, where system fits, roughly what
     is being built. Facts only, not goals/solution. Keep short. -->

## Goals and non-goals

<!-- guidance: Two short lists. Goals = checkable outcomes. Non-goals = nearby
     assumptions deliberately out of scope; they bound review and stop creep. -->

### Goals

-
-

### Non-goals

-
-

## The design

<!-- guidance: Main/longest section. Start high-level, then detail. Explain
     tradeoffs and why. Use/delete subsections below; add diagrams/state
     machines where they clarify. -->

### System-context diagram

<!-- guidance: One box in larger landscape: users, collaborators, dependencies,
     downstream systems. Helps reviewers place design. -->

### APIs

<!-- guidance: Key interfaces/contracts. Show representative signatures and
     review-relevant parts. Do not paste full IDL/schema/generated output. -->

### Data storage

<!-- guidance: Storage engine, data shape, lifecycle (retention/migration) when
     relevant. Convey model, not every column. -->

### Code and pseudo-code

<!-- guidance: Use sparingly for novel/hard-to-explain ideas: tricky algorithm
     or API feel. Design docs sit above production-code detail. Delete if not
     needed. -->

## Degree of rigor

<!-- guidance: Optional. Validation/confidence level: estimate, prototype,
     load-tested POC, benchmark, formal argument. State done + planned work.
     Fold into The design or delete if no value. -->

## Cross-cutting concerns

<!-- guidance: Easy-to-forget whole-design concerns. Keep each short: sentence
     or two, or explicit "N/A, because...". Do not skip Security, Privacy, or
     Observability. -->

### Security

<!-- guidance: Attack surface, authn/authz, untrusted input, secrets, trust boundaries. -->

### Privacy and compliance

<!-- guidance: PII/sensitive data, retention/deletion, regulatory implications
     (GDPR, HIPAA, SOC2, ...). -->

### Observability

<!-- guidance: How to know healthy and debug unhealthy: logs, metrics, traces,
     alerts. -->

### Scalability and performance

<!-- guidance: Optional. Expected load, latency targets, capacity, first bottleneck. Delete if irrelevant. -->

### Reliability and failure modes

<!-- guidance: Optional. Dependency down/slow behavior: degradation, retries,
     fallbacks, DR. Delete if irrelevant. -->

### Cost

<!-- guidance: Optional. Infrastructure/operational cost if material. Delete if irrelevant. -->

## Alternatives considered

<!-- guidance: Other plausible designs and why chosen design won. Include "do
     nothing" or "use existing system X" when valid. These are alternatives to
     chosen design, not open RFC options. -->

## Dependencies and cross-team impact

<!-- guidance: Optional. Internal/external systems relied on; teams blocked or
     blocking. Name owner/work when dependency is external to team. Delete if
     none. -->

## Rollout and migration

<!-- guidance: Optional. Safe ship plan: feature flags, phased rollout,
     data migration/backfill, rollback. Delete if trivial. -->

## Open questions

<!-- guidance: Optional unresolved details for reviewers. If direction itself is
     open, use RFC instead. -->

## References

<!-- guidance: Originating RFC, related design docs/ADRs, prior art, supporting docs. -->
