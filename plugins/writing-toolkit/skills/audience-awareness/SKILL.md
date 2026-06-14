---
name: audience-awareness
description: Identify the reader and document type before applying writing rules. Writing rules from sibling skills (clarity, anti-slop, structure) shift based on audience — what counts as polished for a technical doc is wrong for a launch hype post, and vice versa. Use this skill when starting a new piece of writing, when unsure which conventions apply, or to sanity-check that the rules being applied actually fit the context.
---

# Audience Awareness

Writing rules shift by audience. First identify reader + document type, then apply sibling skills contextually.

## When to use this skill

- Starting a document and unsure which conventions apply.
- A sibling skill (`writing-clearly-and-concisely`, `de-slop`, `document-structure`) suggests edits that feel wrong for context.
- User omitted audience and the right rule depends on it.

## How to use this skill

1. Pick the audience category below.
2. Read which sibling rules shift.
3. Apply sibling skills with those adjustments.

This skill does not re-explain sibling rules. It only says which rules bend by audience.

## The four audience types

### 1. Technical documentation

Reader: user, contributor, or operator trying to act: install, integrate, configure, debug, contribute.

Examples: README files, API docs, tutorials, contribution guides, troubleshooting guides, runbooks.

How sibling rules shift:

- Imperative voice is default: "Run the script. Check output." The `de-slop` rule against subjectless fragments does not apply to deliberate technical imperatives.
- Code examples can interrupt prose. Prose frames code.
- Repeat definitions when useful. `de-slop` elegant variation still applies: do not synonym-cycle.
- Headings and lists carry weight. Scanning is normal.
- Strunk Rule 13 is strict. Cut every word a hurried reader does not need.

### 2. Internal business / professional

Reader: colleague, manager, or cross-team partner. They need decision support or status fast.

Examples: status reports, internal proposals, project updates, decision memos, planning docs, RFC summaries.

How sibling rules shift:

- BLUF: open with conclusion or recommendation. See `document-structure`.
- No throat-clearing: cut "I wanted to reach out to discuss."
- Prefer active voice.
- Hedging is suspicious. `de-slop` excessive-hedging rule applies firmly. If uncertain, state exact uncertainty.
- Length matters. Two-page memo with one-paragraph BLUF beats five pages with no lead.

### 3. Promotional (engineer-flavored)

Reader: peers, colleagues, or professional network. They follow the work; they do not want formal marketing.

Examples: internal launch posts, LinkedIn dev posts, release notes by the shipping engineer, talk teasers, project recaps.

How sibling rules shift:

- Short sentences and some enthusiasm are fine.
- `de-slop` AI-vocabulary rules still apply fully: vibrant, transformative, seamless, etc. Engineer voice uses concrete detail, not abstract intensifiers.
- First person is fine.
- Numbers, screenshots, and examples carry the message. "Reduced p99 from 800ms to 120ms" beats "dramatically improved performance."
- `de-slop` generic-positive-conclusion rule still applies. End on fact or CTA, not "exciting times ahead."

### 4. Personal / opinion writing

Reader: someone who came for perspective and voice, not neutral reporting.

Examples: essays, blog posts, opinion pieces, personal reflections, perspective-driven retrospectives.

How sibling rules shift:

- First person is welcome.
- Sentence rhythm matters. Vary length deliberately.
- Some looseness is fine: tangents, asides, half-formed thoughts. Same moves read as AI slop in technical docs.
- Strunk "omit needless words" still applies, but extra words can earn their place through rhythm or emphasis.
- `document-structure` patterns like BLUF and inverted pyramid usually fit poorly. Essay structure is argument unfolding.
- `de-slop` rules against significance puffery, vague attributions, and chatbot artifacts still apply.

## Common audience mistakes

- **Treating a README like an essay.** No buildup. Lead with what it is and how to use it.
- **Treating an essay like a memo.** No BLUF. Let argument develop.
- **Treating a launch post like marketing copy.** Cut abstract intensifiers. Use numbers/screenshots.
- **Treating internal docs like external docs.** Less hand-holding, more shared context.
- **Defaulting to "general literary prose."** No real audience defaults there. Pick a category first.

## Accessibility checklist

Run before publishing docs, READMEs, RFCs, release notes, or support pages. Writing-level accessibility only; UI accessibility belongs elsewhere.

- **Link text describes the destination.** Avoid "click here," "read more," and bare URLs. Link text should make sense aloud or in a link list.
- **Headings form a logical outline.** Nest levels correctly. Do not skip levels for visual effect.
- **Acronyms expanded on first use.** Unless audience certainly knows term, write "Single Sign-On (SSO)" first, then "SSO."
- **Instructions do not depend on visual cues.** Name controls: "Click **Save changes**," not "green button on the right."
- **Lists serve parallel items, prose serves relationships.** Use list for parallel values; prose for cause, sequence, contrast.
- **Error messages tell next action.** "Authentication failed. Verify your API key, then retry."
- **Plain language when precision survives.** "Use" beats "utilise"; technical terms stay when needed.

## Related skills

For rules this skill points at:

- `writing-clearly-and-concisely` - sentence-level rules (Strunk).
- `de-slop` - AI-pattern removal.
- `document-structure` - whole-document organization patterns (BLUF, inverted pyramid, PREP, SCQA).
- `tech-doc-templates` - structured templates for RFC and ADR documents.
