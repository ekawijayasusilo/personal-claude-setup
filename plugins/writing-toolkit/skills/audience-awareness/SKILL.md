---
name: audience-awareness
description: Identify the reader and document type before applying writing rules. Writing rules from sibling skills (clarity, anti-slop, structure) shift based on audience — what counts as polished for a technical doc is wrong for a launch hype post, and vice versa. Use this skill when starting a new piece of writing, when unsure which conventions apply, or to sanity-check that the rules being applied actually fit the context.
---

# Audience Awareness

Writing rules are not universal. The same sentence can be sharp in one context and inappropriate in another. Before applying rules from sibling skills, identify the audience and document type — then apply the rules contextually.

## When to use this skill

- Starting a new document and unsure which conventions apply.
- A sibling skill (`writing-clearly-and-concisely`, `de-slop`, `document-structure`) is suggesting edits that feel wrong for the context — this skill helps explain why.
- The user has not stated the audience explicitly and the rules being applied depend on it.

## How to use this skill

1. Identify which audience category below matches the writing task.
2. Read the corresponding section to see which sibling-skill rules shift.
3. Apply the sibling skills with those adjustments in mind.

This skill does not re-explain the sibling rules. It says which rules apply differently and points to the skills that own them.

## The four audience types

### 1. Technical documentation

Who's reading: a user, contributor, or operator who wants to do something — install, integrate, configure, debug, contribute. They are reading to act, not to be persuaded.

Examples: README files, API docs, tutorials, contribution guides, troubleshooting guides, runbooks.

How sibling rules shift:

- Imperative voice is the default ("Run the script. Check the output. If you see error X, do Y."). The `de-slop` rule against subjectless fragments does not apply to deliberate imperative fragments in this context.
- Code examples interrupt prose freely — the prose exists to frame the code, not the other way around.
- Definitions are repeated where useful. The `de-slop` rule against elegant variation still applies (do not synonym-cycle), but unlike literary prose, you do not need to vary phrasing to keep the reader engaged — clarity beats variety.
- Headings and lists carry more weight than paragraphs. Scanning is normal.
- Strunk Rule 13 (omit needless words) is especially strict here. Cut every word a hurried reader does not need.

### 2. Internal business / professional

Who's reading: a colleague, manager, or cross-team partner who is busy and wants the point. They are reading to make a decision or stay informed.

Examples: status reports, internal proposals, project updates, decision memos, planning docs, RFC summaries.

How sibling rules shift:

- BLUF (bottom line up front) — open with the conclusion or recommendation, not the buildup. See `document-structure` for the pattern.
- No throat-clearing. Cut "I wanted to reach out to discuss" and similar warm-up phrases.
- Active voice strongly preferred (Strunk Rule 10 applies cleanly here).
- Hedging is suspicious — the `de-slop` rule against excessive hedging applies firmly. If you are uncertain, say what you are uncertain about specifically.
- Length matters. A two-page memo with a one-paragraph BLUF will be read; a five-page memo with no lead will not.

### 3. Promotional (engineer-flavored)

Who's reading: peers, colleagues, or your professional network — people interested in what you shipped or built. They are reading because they follow you or your work, not because they were told to.

Examples: product-launch hype posts on internal Slack, LinkedIn dev posts, release announcements written by the engineer who shipped the thing, conference-talk teasers, project recap posts.

This is specifically NOT formal marketing copy. The audience expects an engineer voice, not a marketer voice.

How sibling rules shift:

- Shorter sentences are normal. Some enthusiasm is appropriate.
- The `de-slop` rules against AI-vocabulary (vibrant, transformative, seamless, etc.) still apply fully. These words do not get a pass here — they are the marketer voice you are explicitly avoiding. The engineer voice expresses enthusiasm through concrete detail, not abstract intensifiers.
- First person is fine ("I built this because…").
- Specific numbers, screenshots, and concrete examples carry the message. "Reduced p99 latency from 800ms to 120ms" beats "dramatically improved performance."
- The `de-slop` "generic positive conclusion" rule still applies. End on a concrete fact or call-to-action, not "exciting times ahead."

### 4. Personal / opinion writing

Who's reading: someone who came for your perspective. They want voice, not neutral reporting.

Examples: essays, blog posts, opinion pieces, personal reflections, retrospectives where the perspective is the point.

How sibling rules shift:

- First person is welcome.
- Sentence rhythm matters more than in other contexts. Vary length deliberately.
- Some structural looseness is fine — tangents, asides, half-formed thoughts read as human in essay form (they read as AI slop in technical docs).
- Strunk's "omit needless words" still applies, but a few well-chosen extra words for rhythm or emphasis are not waste here.
- Document-structure patterns (BLUF, inverted pyramid) are usually wrong for essay form — the structure of an essay is the argument unfolding, not the conclusion stated first.
- The `de-slop` rules against significance puffery, vague attributions, and chatbot artifacts still apply. Personal voice is not a license for vagueness.

## Common audience mistakes

These are mismatches the model tends to make. Watch for them.

- **Treating a README like an essay.** No buildup. No "introduction" paragraph. Lead with what the thing is and how to use it.
- **Treating an essay like a memo.** No BLUF. Let the argument develop.
- **Treating a launch post like marketing copy.** Strip the abstract intensifiers. Use specific numbers and screenshots.
- **Treating internal docs like external docs.** Less hand-holding, more shared context. You can assume your colleagues know what the team's services are called.
- **Defaulting to "general literary prose."** No real audience defaults to that. Always pick a category before applying rules.

## Related skills

For the rules this skill points at:

- `writing-clearly-and-concisely` — sentence-level rules (Strunk).
- `de-slop` — AI-pattern removal.
- `document-structure` — whole-document organization patterns (BLUF, inverted pyramid, PREP, SCQA).
- `tech-doc-templates` — structured templates for RFC and ADR documents.
