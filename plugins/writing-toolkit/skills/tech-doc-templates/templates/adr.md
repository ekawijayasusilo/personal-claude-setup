<!-- WHEN TO USE THIS TEMPLATE
     ADR = record converged architectural decision for future readers. Discussion
     happened elsewhere; this captures what was decided and why.

     If alternatives are still live and team input is needed, use RFC.

     ADRs are append-only. After acceptance, do not edit. If decision changes,
     write new ADR, link both, mark old one Superseded.

     Strip this comment block before publishing. -->

# ADR-NNNN: [Title]

<!-- guidance: Number sequentially (ADR-0001, ADR-0002, ...). Title = short
     imperative/declarative phrase, ideally <50 chars. Bad: "Database choice."
     Good: "Use Postgres as the primary datastore for the user service." -->

| Field | Value |
|---|---|
| Status | Proposed / Accepted / Deprecated / Superseded by ADR-NNNN |
| Date | YYYY-MM-DD |
| Deciders | [names or team] |

## Context

<!-- guidance: Situation requiring decision. Include only context needed to
     understand why this came up. 2-4 short paragraphs typical. Cover forces:
     technical constraints, org constraints, performance needs, commitments. -->

## Decision drivers

<!-- guidance: Short list of criteria weighed. Examples:
       - Must support 50k writes per second
       - Team already operates Postgres in production
       - Vendor lock-in concerns rule out managed-only solutions
       - Compatibility with existing ORM
     Typical: 2-6. If none, decision may be too small for ADR. -->

-
-
-

## Decision

<!-- guidance: Plain declarative voice: "We will use Postgres for the user
     service." Not "We are considering..." Be specific enough to verify later.
     One concise paragraph usually enough. -->

## Consequences

<!-- guidance: Honest results of decision. Include positive and negative.
     No-negative decision is suspicious or trivial. -->

### Positive

<!-- guidance: What gets better. -->

### Negative

<!-- guidance: What gets harder, costs more, or creates risk. -->

### Neutral

<!-- guidance: Optional side effects worth noting. Delete if empty. -->

## Alternatives considered

<!-- guidance: Brief: 1-2 sentences per alternative, what it was and why not
     chosen. ADR is not deep alternative analysis; decision is made. -->

- **[Alternative 1]**: [one or two sentences on why not chosen]
- **[Alternative 2]**: [one or two sentences on why not chosen]

## Confirmation

<!-- guidance: Optional. How to verify implementation matched decision. Delete
     if obvious. Examples:
       - "All new services emit OpenTelemetry traces; verified via the
          observability dashboard at [link]."
       - "Migration plan tracked in [JIRA-XXXX]; complete when all
          services list as migrated in the registry." -->

## References

<!-- guidance: Related ADRs, source RFC, docs, external prior art. -->
