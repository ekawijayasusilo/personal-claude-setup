---
name: writing-clearly-and-concisely
description: Apply Strunk's Elements of Style for sentence-level clarity, conciseness, grammar, punctuation, and mechanics. Use when editing prose to tighten sentences, fix grammar/punctuation, remove needless words, or improve sentence-level flow. Not for whole-document organization or AI-pattern cleanup — see related skills.
---

# Writing Clearly and Concisely

## Overview

William Strunk Jr.'s *The Elements of Style* (1918) covers sentence-level grammar, punctuation, concision, parallelism, and word choice. Apply it when editing prose at sentence/paragraph level.

Compressed reference: `elements-of-style.md`. Load `elements-of-style.md` only when actively copyediting; list below usually suffices. If unsure on a rule, consult `elements-of-style.md`.

## When to use this skill

Use for sentence-level prose polish:

- Tighten sentences; cut needless words
- Fix grammar, punctuation, or parallelism
- Improve rhythm and paragraph flow
- Choose active vs passive voice
- Resolve ambiguous or awkward constructions

Do not use for:

- Removing AI-generated writing patterns -> use `de-slop`
- Whole-document organization -> use `document-structure`
- Tone/register by audience -> use `audience-awareness`
- Structured technical docs -> use `tech-doc-templates`

## Limited context strategy

When context is tight:

1. Draft using judgment + rule list below.
2. Dispatch subagent with draft and `elements-of-style.md`.
3. Ask subagent to copyedit and return revision.

## The rules

### Elementary rules of usage (grammar and punctuation)

1. Form the possessive singular by adding 's
2. Use a comma after each term in a series except the last
3. Enclose parenthetic expressions between commas
4. Place a comma before a conjunction introducing a co-ordinate clause
5. Do not join independent clauses by a comma
6. Do not break sentences in two
7. A participial phrase at the beginning of a sentence must refer to the grammatical subject

### Elementary principles of composition

8. Make the paragraph the unit of composition (one paragraph per topic)
9. Begin each paragraph with a topic sentence
10. **Use the active voice**
11. **Put statements in positive form**
12. **Use definite, specific, concrete language**
13. **Omit needless words**
14. Avoid a succession of loose sentences
15. Express co-ordinate ideas in similar form
16. **Keep related words together**
17. Keep to one tense in summaries
18. **Place the emphatic words of a sentence at the end**

### Section V: Words and expressions commonly misused

Alphabetical usage reference. Load from `elements-of-style.md` when needed.

## Caveats on contested rules

Apply judgment, not orthodoxy. Some Strunk rules are defaults.

### Rule 1 — Possessive 's after a final s

Strunk prefers "Charles's friend." AP and many house styles prefer "Charles' friend." Match surrounding convention; if none, pick one and stay consistent.

### Rule 10 — Use the active voice

Active is default. Passive is correct when:

- Agent unknown, irrelevant, or obvious ("The bill was passed in 1972.")
- Patient deserves emphasis ("The vaccine was administered to 200 children.")
- State matters more than actor, common in technical writing ("The cache is invalidated after 10 minutes.")
- Genre expects it: scientific writing, formal reports, legal prose

Verify sentence is actually passive before fixing. Strunk has been criticized by Geoffrey Pullum for mislabeling non-passives.

### Rule 6 — Do not break sentences in two

Avoid accidental fragments that confuse grammar. Keep deliberate fragments in technical writing ("Returns null if not found."), UI text, dialogue, headings, and essays when they improve scanability/rhythm.

### Rule 9 — Begin paragraphs with topic sentences

Good default for expository, technical, academic, and business writing. Not mandatory for narrative, essays, dialogue, product copy, or short UI text. In technical docs, heading + direct first sentence may already do the job.

### Rule 11 — Put statements in positive form

Positive form is usually clearer. Negative form is correct for contrast, warnings, boundaries, and likely mistakes. "Do not commit secrets to the repo" is better than a softened positive rewrite.

### Rule 18 — Place emphatic words at the end of the sentence

End emphasis helps essays/persuasion. Technical writing often needs key term first for scanning. Prefer scanability in reference docs, procedures, and tables.

## Related skills

For complementary guidance:

- `de-slop` - remove AI-writing patterns (pair with this for AI drafts)
- `audience-awareness` - adapt rules to reader/document type
- `document-structure` - organize above paragraph level
