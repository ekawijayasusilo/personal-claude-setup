<!-- WHEN TO USE THIS TEMPLATE
     Postmortem = retrospective after resolved production incident: what
     happened, impact, causes, follow-up prevention.

     Write for significant incidents: SEV1/SEV2, customer-visible outage, data
     loss, SLA/SLO breach, monitoring miss, or requested learning review.

     Only retrospective template here. RFCs, ADRs, design docs concern future
     work or decisions.

     Core principle: BLAMELESS. Assume good faith with info available then.
     Focus systems/processes, not people:
       - Attribute actions to roles, not names ("the on-call engineer").
       - Avoid "should have," "failed to," "careless," "if only."
       - Prefer neutral facts: "deploy proceeded because no staging gate."
       - Treat human error as start of investigation, never conclusion.

     Strip this comment block before publishing. -->

# Postmortem: [Incident name] (incident #NNN)

<!-- guidance: Specific/searchable name: what broke, ideally when. Bad: "The
     big outage." Good: "Checkout API 500s during EU peak (incident #465)." Drop
     incident number if org does not number incidents. -->

| Field | Value |
|---|---|
| Date | YYYY-MM-DD |
| Authors | [names or usernames] |
| Status | Draft / In review / Complete, action items in progress / Complete |
| Severity | SEV1 / SEV2 / SEV3 / SEV4 |
| Affected systems | [services / components] |
| Impact window | [start → end, with timezone; total duration] |

<!-- guidance: Severity = business impact and response urgency. Common scale:
       - SEV1: critical — full outage or data loss, all-hands response
       - SEV2: major — significant degradation or partial outage, urgent
       - SEV3: minor — limited impact, workaround available, normal hours
       - SEV4: cosmetic — negligible impact
     Use org scale if different. -->

## Summary

<!-- guidance: 1-2 plain-language sentences: what broke, who affected, duration,
     headline cause. Executive-readable. No jargon/buildup. -->

## Impact

<!-- guidance: Quantify damage. Numbers, not adjectives. Examples:
       - "~12,000 users (8% of EU traffic) could not check out for 47 minutes."
       - "3.2M requests returned 500s; estimated $40k in lost orders."
       - "Breached the 99.9% monthly availability SLO for the checkout service."
     Separate outage vs degradation. If unknown, state known facts + gap. -->

## Root cause & contributing factors

<!-- guidance: Most incidents have several contributing factors. List them.
     Prefer systemic framing: "why did system allow this?" Use 5 Whys as lens,
     not final answer. Keep going past human-error step to safeguards missing
     (confirmation, canary, rollback). Neutral/blameless language. -->

## Trigger

<!-- guidance: Specific event that started incident: deploy, config change,
     traffic spike, dependency failure, cert expiry. Trigger is distinct from
     root cause; it may be benign alone. -->

## Detection

<!-- guidance: How discovered and after how long: alert, customer report,
     manual observation. Slow/manual/customer detection often becomes action
     item. -->

## Resolution

<!-- guidance: What stopped bleeding and restored service. Distinguish temporary
     mitigation from permanent fix. Note failed mitigations too. -->

## Action items

<!-- guidance: Follow-up work to prevent recurrence, detect faster, reduce blast
     radius, or improve process. Every item: specific, owned, dated, tracked in
     real issue tracker. "Be more careful" is not action item.

     Type:
       - prevent: stop cause recurring
       - detect: notice faster
       - mitigate: reduce impact
       - process: runbooks, training, on-call, comms -->

| Action item | Type | Owner | Due | Ticket |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |

## Lessons learned

<!-- guidance: Blameless, specific reflection. Fill all three buckets. -->

### What went well

<!-- guidance: Helpful tooling, fast rollback, clear runbook, quick diagnosis.
     Credit role/action, not heroics. -->

### What went wrong

<!-- guidance: Monitoring gaps, missing safeguards, confusing dashboards,
     unclear ownership. -->

### Where we got lucky

<!-- guidance: Things that broke in our favor but might not next time. Each may
     become action item. -->

## Timeline

<!-- guidance: Chronological timestamped account from trigger to all-clear. Use
     ISO 8601 timestamps in one stated timezone (UTC default); optional T+ offsets.
     Include trigger -> detection -> escalation -> mitigations (worked/failed) ->
     root cause -> fix -> recovery -> all-clear. Terse facts; link evidence. -->

- **YYYY-MM-DDThh:mm UTC** —
- **YYYY-MM-DDThh:mm UTC** —
- **YYYY-MM-DDThh:mm UTC** —

## Supporting information

<!-- guidance: Optional dashboards, graphs, logs, incident channel/bridge,
     related incidents/postmortems. Delete if empty. -->
