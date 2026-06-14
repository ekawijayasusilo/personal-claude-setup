---
name: tech-doc-templates
description: Scaffold a new technical document from a sensible-default template. Supports RFC (Request for Comments — proposing a substantive change for team input), ADR (Architecture Decision Record — logging a decision that has converged), Design Doc (specifying how a system will be built), and Postmortem (a blameless retrospective after an incident). Use when starting any of these from scratch, or when an existing draft needs to be re-shaped onto a standard structure.
---

# Tech Doc Templates

Starter templates for common engineering docs. Files live in `templates/`; load on demand.

## When to use this skill

- User asks to write/draft an RFC, ADR, Design Doc, or Postmortem.
- New technical document needs structure.
- Existing draft has material but no clear shape.

Scaffolding only. Use sibling skills for prose polish.

## Available templates

| Template | File | Use when… |
|---|---|---|
| RFC | `templates/rfc.md` | Proposing substantive change; team input needed; decision not made. |
| ADR | `templates/adr.md` | Recording converged architectural decision; captures what/why. |
| Design Doc | `templates/design-doc.md` | Specifying how to build agreed system/feature: APIs, data, concerns. |
| Postmortem | `templates/postmortem.md` | Retrospective after incident: impact, causes, timeline, actions. |

## Picking the right template

Fastest choice: question each doc answers.

| Template | Answers | When |
|---|---|---|
| **RFC** | "*Should* we do this, and which way?" | Decision open; want input |
| **Design Doc** | "*How* will we build it?" | Direction agreed; specify build |
| **ADR** | "*What* did we decide, and why?" | Decision converged; record it |
| **Postmortem** | "*What* broke, and how do we prevent it?" | After incident |

Postmortem is retrospective. RFC/Design Doc/ADR are prospective or decision-recording and commonly confused.

### RFC vs ADR

- **RFC asks a question.** Drives discussion; alternatives are live; decision emerges.
- **ADR answers a question.** Records converged decision; alternatives are brief rationale, not deep analysis.

Common workflow: RFC -> debate -> ADR. ADR lives in repo; RFC may or may not.

Signals:

- RFC: open questions + alternatives considered.
- ADR: no open questions; alternatives brief.

### Design Doc vs RFC

Axis: **decision-seeking vs. implementation-describing**.

RFC decides direction: multiple live alternatives, broad audience, goal is decision. Design Doc details agreed direction for builders: internals, APIs, data model, cross-cutting concerns. If settling *which direction*, use RFC. If specifying *the build*, use Design Doc. Some orgs merge them; choose sections that fit.

### Design Doc vs ADR

Design Doc describes system implementation. ADR records one decision tersely. One Design Doc may create several ADRs because design docs stale after build; ADRs persist.

**Common workflow:** RFC (decide direction) -> Design Doc (detail build) -> ADRs (record key decisions) -> Postmortem (if it breaks). Few projects need all four.

## Loading the template

When user wants a document:

1. Confirm template (RFC, ADR, Design Doc, Postmortem). If unclear, ask.
2. Read matching file from `templates/`.
3. Use template as starting structure; fill sections from user context.
4. Template files contain `<!-- guidance: ... -->` comments. Strip comments before final delivery.

## Related skills

When working on scaffolded docs:

- `document-structure` - organize content inside sections.
- `writing-clearly-and-concisely` - sentence polish.
- `de-slop` - strip AI patterns.
- `audience-awareness` - adapt to readers: team, maintainers, incident reviewers.
