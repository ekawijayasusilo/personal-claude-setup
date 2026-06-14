<!-- WHEN TO USE THIS TEMPLATE
     RFC = proposal for substantive change needing team input before commitment.
     Alternatives are live; decision not made. Purpose: drive discussion.

     If decision already converged, use ADR. Common pattern: RFC -> debate ->
     ADR records chosen outcome.

     Delete sections that do not apply, especially Operations, Timeline, Future
     work. Focused RFC beats complete-looking empty one.

     Strip this comment block before publishing. -->

# RFC: [Title]

<!-- guidance: Concrete title naming proposal. Bad: "Proposal for caching layer
     evaluation." Good: "Add a Redis caching layer for product-detail reads." -->

| Field | Value |
|---|---|
| Author | [Name] |
| Status | Draft / Open for review / Accepted / Rejected / Superseded |
| Created | YYYY-MM-DD |
| Last updated | YYYY-MM-DD |
| Discussion | [link to PR, doc comments, or thread] |

## Summary

<!-- guidance: One paragraph: what proposed and why. Reader should understand
     proposal + motivation from this alone. Aim 3-5 sentences. No buildup. -->

## Goals and non-goals

<!-- guidance: Two short lists. Goals = what proposal accomplishes. Non-goals =
     adjacent assumptions explicitly out of scope; they prevent scope creep.
     If non-goals are hard to list, proposal may be too broad. -->

### Goals

-
-

### Non-goals

-
-

## Background and motivation

<!-- guidance: Current state, why change, cost of not doing it. Use numbers,
     examples, incidents, pain points. Define key terms/internal names. Avoid
     abstract "improve developer experience" unless backed by concrete measure. -->

## Detailed design

<!-- guidance: Main section. What will be built/changed/decided:
       - Solution shape (architecture, schema, API surface)
       - User-facing behavior change
       - Internal mechanics relevant to review
       - Data model changes
       - Migration path for existing behavior
       - Non-trivial rollout plan
     Use subheadings. Diagrams welcome when useful. -->

## Alternatives considered

<!-- guidance: Serious alternatives: what each is and why proposal wins. 2-3 is
     normal; more suggests indecision, fewer suggests weak exploration. Include
     "Do nothing" and prior art when relevant. -->

### Alternative 1: [Name]

<!-- guidance: One paragraph each. -->

### Alternative 2: [Name]

### Alternative 3: Do nothing

## Dependencies

<!-- guidance: Internal/external systems, APIs/vendors, teams, infrastructure.
     If blocked on someone else's work, name owner + work. -->

## Operations

<!-- guidance: Who runs this and what human/process load it adds:
       - Ownership after launch
       - On-call alerts/runbooks
       - Deployment/rollback
       - Recurring maintenance (cert rotation, capacity reviews, ...)
     If no operational surface, write "N/A." -->

## Security, privacy, and compliance

<!-- guidance: Consider attack surface, user-controlled inputs, PII/sensitive
     data, auth/authz, retention/deletion, GDPR/HIPAA/SOC2. If unsure, flag for
     review. "No concerns identified, pending security review" is valid. -->

## Drawbacks and tradeoffs

<!-- guidance: Costs knowingly accepted, distinct from risks. Examples:
     operational burden, downstream migration, vendor/pattern lock-in,
     performance regression, learning curve. If none, proposal may be too small. -->

## Risks and mitigations

<!-- guidance: What could go wrong and response plan. For each: risk,
     likelihood/impact, mitigation. Scan complexity, compatibility, latency,
     dependency maturity, expertise, adoption. No mitigation = worry, not analysis. -->

## Success metrics

<!-- guidance: Concrete evaluation after ship. Examples:
       - "p99 checkout latency drops below 200ms within 30 days of launch"
       - "Cache hit rate on product-detail reads exceeds 80%"
       - "Build pipeline completes in under 4 minutes for 95% of runs"
     If metric impossible, state qualitative condition that would convince you. -->

## Timeline and milestones

<!-- guidance: Optional rough delivery phases. Delete if small or tracked
     elsewhere.

     Example:
       - Week 1-2: schema migration + dual-writes
       - Week 3: backfill
       - Week 4: cut reads over, monitor
       - Week 5: clean up dual-write path -->

## Open questions

<!-- guidance: Unknowns needing input. Number/bullet them. Open questions are
     why RFCs exist. -->

1.
2.
3.

## Future work

<!-- guidance: Optional related out-of-scope work likely to come up. Delete if empty. -->

## References

<!-- guidance: Related RFCs, prior art, articles, docs, discussion threads. -->
