---
name: document-structure
description: Organize whole documents using established structural patterns — BLUF, inverted pyramid, PREP, SCQA, and classical lead/body/close. Use when starting a new document, restructuring an existing one, or when sentence-level edits aren't enough because the document's organization itself is the problem. Operates at the document level, not the sentence level.
---

# Document Structure

Sentence polish cannot fix bad organization. Use this skill for document-level order: what comes first, argument shape, reader path.

## When to use this skill

- Starting a document and unsure how to organize it.
- Draft is clean but unfocused: likely structure, not wording.
- Reader may stop midway but still needs key info.
- Material is right but order is wrong.

For sentence-level rules, use `writing-clearly-and-concisely`. For matching structure to audience, use `audience-awareness`.

## The patterns

### BLUF — Bottom Line Up Front

Put conclusion, recommendation, or key takeaway in first 1-2 sentences. Then support it.

Use for: memos, decision docs, status updates, executive-facing writing, busy readers.

Why: many readers stop early; BLUF gets most important info through.

Example structure:

```
Recommendation: migrate the user service to Postgres by Q3.

The current MySQL setup is hitting connection-pool limits during peak traffic
and our schema has outgrown what MySQL handles well. Postgres gives us proper
JSON support, better concurrent-write performance, and aligns with what the
platform team is already running.

[supporting detail follows]
```

Common mistake: burying recommendation in final "Conclusion."

### Inverted pyramid

Order facts most important -> least important. Reader can stop anywhere and keep key info.

Use for: news, announcements, incident reports, change announcements, release notes.

Shape:

1. Lead: what happened, when, who affected.
2. Key details: numbers, scope, impact.
3. Background: how this came about.
4. Context: related events/history.
5. Future: what happens next.

Common mistake: chronology first. Save chronology for postmortem body; lead with outcome.

### PREP — Point, Reason, Example, Point

Paragraph-level persuasive pattern.

1. **Point**: claim.
2. **Reason**: why true.
3. **Example**: concrete evidence.
4. **Point**: restated, now grounded.

Use for: persuasive paragraphs, proposal sections, argumentative blog posts.

Example:

> Code review is more valuable as a teaching moment than as a defect filter. Most defects that matter slip past reviewers anyway — the ones that get caught are usually style or naming nits a linter would also catch. Where review pays off is when a senior engineer explains *why* a pattern is preferred, and that knowledge propagates to the rest of the team. Treat code review as a teaching channel, and the catch-defects function becomes a side benefit rather than the goal.

Common mistake: Point + Reason only. Without Example, argument is opinion; without closing Point, reader must infer.

### SCQA — Situation, Complication, Question, Answer

Analytical framing. Establish why answer matters.

1. **Situation**: accepted context.
2. **Complication**: what changed/went wrong.
3. **Question**: what doc answers.
4. **Answer**: answer.

Use for: analysis docs, strategy memos, consulting-style writeups.

Example shape:

> **Situation**: our authentication service has handled login flow for all our products for five years.
>
> **Complication**: three new acquired products use their own identity providers, and the synchronization between them and our service now causes more incidents than it prevents.
>
> **Question**: should we consolidate onto a single identity provider, federate, or accept the operational cost?
>
> **Answer**: federate via OIDC. Consolidation is too disruptive given the current cycle; the operational cost will grow as we acquire more products; federation has a clear migration path and matches industry norms.

Common mistake: skipping Complication. Then Answer floats as opinion.

### Lead, body, close

Classical essay/article shape.

- **Lead**: invites reader: anecdote, striking fact, question, scene. Not BLUF.
- **Body**: develops topic; each paragraph makes a distinct point.
- **Close**: lands piece by returning to lead, drawing conclusion, or leaving a thought.

Use for: essays, blog posts, opinion pieces, narrative non-fiction. Usually wrong for technical/business writing.

Common mistake: making lead an abstract or BLUF.

## Technical documentation modes (Diataxis)

Technical docs need information architecture. [Diataxis](https://diataxis.fr/) separates four reader needs. Bad docs mix modes: API reference becomes tutorial; tutorial acts like reference. Pick mode first.

### The four modes

- **Tutorial** — teaches beginner through a complete path. Optimize for progress/confidence: prerequisites, realistic path, finished outcome, next step.
- **How-to guide** — helps reader complete a specific task. Optimize for direct steps: task title, prerequisites, numbered steps, verification.
- **Reference** — lookup exact facts. Optimize for completeness/scanning: consistent entries, required/optional params, defaults, returns, errors. Link conceptual material.
- **Explanation** — build mental model. Start with question, define terms, use examples/comparisons, explain tradeoffs/reasons.

README can mix modes; each section should know its job.

### Picking the mode by reader question

| Reader's question | Mode |
|---|---|
| "How do I learn this from scratch?" | Tutorial |
| "How do I do this specific thing?" | How-to |
| "What are the exact details / parameters / fields?" | Reference |
| "Why does it work this way?" | Explanation |

When unsure, ask what reader will do: read once -> tutorial/explanation; return to look up -> reference; follow steps now -> how-to.

### README shape

Flexible default:

1. What this is.
2. Who it is for, if not obvious.
3. Quick start.
4. Common usage.
5. Configuration / integration notes.
6. Troubleshooting.
7. Links to deeper docs.

Tiny libraries can omit sections; large platforms can link each section out.

## Cross-cutting structural choices

### When to use headings vs paragraphs

Use headings when:

- Document is long enough to navigate.
- Sections cover distinct topics.
- Reader will return and re-locate info.

Avoid headings that chop a short flowing argument into bureaucratic two-paragraph chunks.

### When a list beats prose

Use a list when:

- Items are parallel.
- Order is irrelevant, or numbering means order matters.
- Reader will scan.

Use prose when ideas have natural connectives: first, then, because, therefore. Lists flatten relationships.

### Section breaks within a section

Section break (blank line, horizontal rule, `***`) means topic/perspective shift without new heading. Useful in essays, long-form articles, reports. Usually unnecessary in technical/business docs.

## Picking the right pattern

- Memo, status update, decision doc -> **BLUF**
- Announcement, news, release notes, incident report -> **Inverted pyramid**
- Persuasive paragraph/argument -> **PREP**
- Analysis/strategy doc needing setup -> **SCQA**
- Essay, blog post, narrative non-fiction -> **Lead / body / close**
- Technical documentation -> choose **Diataxis mode** first; README uses compact mix

For audience-driven choices, see `audience-awareness`.

## Related skills

- `audience-awareness` - which structure fits which reader/document type.
- `writing-clearly-and-concisely` - sentence polish within sections.
- `de-slop` - remove AI patterns after structure is right.
- `tech-doc-templates` - RFC/ADR templates with structure built in.
