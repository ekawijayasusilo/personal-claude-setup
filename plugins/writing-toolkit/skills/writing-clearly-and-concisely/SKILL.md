---
name: writing-clearly-and-concisely
description: Apply Strunk's Elements of Style for sentence-level clarity, conciseness, grammar, punctuation, and mechanics. Use when editing prose to tighten sentences, fix grammar/punctuation, remove needless words, or improve sentence-level flow. Not for whole-document organization or AI-pattern cleanup — see related skills.
---

# Writing Clearly and Concisely

## Overview

William Strunk Jr.'s *The Elements of Style* (1918) is a compact guide to sentence-level writing: grammar, punctuation, conciseness, parallelism, and word choice. This skill applies its rules when editing prose for clarity at the sentence and paragraph level.

The full reference is in `elements-of-style.md` (~12k tokens). Load it only when actively editing prose; the rule list below is usually enough to guide an edit.

## When to use this skill

Use this skill when the task is sentence-level prose polish:

- Tightening sentences, cutting needless words
- Fixing grammar, punctuation, or parallelism
- Improving sentence rhythm and flow within a paragraph
- Choosing between active and passive voice for a sentence
- Resolving an ambiguous or awkward construction

Do not use this skill for:

- Removing AI-generated writing patterns → use `de-slop`
- Choosing how to organize a whole document → use `document-structure`
- Adapting tone or register to a specific audience → use `audience-awareness`
- Drafting a structured technical document → use `tech-doc-templates`

## Limited context strategy

When context is tight:

1. Write your draft using judgment and the rule list below.
2. Dispatch a subagent with your draft and `elements-of-style.md`.
3. Have the subagent copyedit and return the revision.

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

Alphabetical reference for usage questions. Load from `elements-of-style.md` when needed.

## Caveats on contested rules

A few of Strunk's rules are defaults rather than absolutes. Apply judgment, not orthodoxy.

### Rule 1 — Possessive 's after a final s

Strunk says "Charles's friend" even after a final s. This is the Oxford / US Government Printing Office convention. AP style and many modern house styles prefer "Charles' friend." Either is correct. Match the surrounding text's convention; if there is none, pick one and stay consistent within the document.

### Rule 10 — Use the active voice

Active voice is the right default, but passive voice is correct (not a flaw) when:

- The agent is unknown, irrelevant, or obvious ("The window was broken." "The bill was passed in 1972.")
- The patient deserves emphasis ("The vaccine was administered to 200 children.")
- Conventional in the genre (scientific writing, formal reports, some legal prose)

Strunk himself has been criticized — notably by Geoffrey Pullum — for mislabeling non-passive constructions as passive in his examples. When applying Rule 10, verify the sentence is actually passive before "fixing" it.

## Related skills

For complementary guidance, also load:

- `de-slop` — remove AI-writing patterns (use together with this skill when editing AI-generated prose)
- `audience-awareness` — adapt rules to the reader and document type
- `document-structure` — organize the document above the paragraph level

## Bottom line

Editing prose for clarity? Use the rule list above. For deeper questions on a specific rule or usage point, load `elements-of-style.md`. For complementary edits, layer in `de-slop` and `audience-awareness`.
