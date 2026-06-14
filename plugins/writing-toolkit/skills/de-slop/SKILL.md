---
name: de-slop
description: Remove AI-writing patterns (slop) from prose so it reads as natural, human-written text. Use when editing or reviewing prose — especially anything drafted with AI help — to strip puffery, vague attributions, em-dash overuse, banned-word habits, rule-of-three formulas, copula avoidance, chatbot artifacts, and other tells. Pairs with writing-clearly-and-concisely for sentence-level polish.
---

# De-Slop: Remove AI Writing Patterns

Edit prose so it stops reading as AI-generated. Sources: Flutter team's natural-writing rules + Wikipedia's "Signs of AI writing" catalogue.

## Your task

When de-slopping text:

1. Identify catalogue patterns below.
2. Rewrite problem sections in place.
3. Preserve meaning and intended tone.
4. **Do not invent specificity.** See Factual safety rule.
5. Clean slop only; do not inject new voice.
6. Run self-audit checklist.
7. Final adversarial pass: "what still reads as AI-generated?" Revise.
8. Return final rewrite, optionally with brief change summary.

## Factual safety rule

Most important rule. Removing puffery creates gaps; do not fill gaps with dates, names, numbers, tools, places, causes, or superlatives unless present in source text, user context, cited sources, or inspected files.

Clear unsupported detail is worse than vague truth.

If source does not support a concrete claim:

1. **Remove** unsupported claim.
2. **Narrow** claim to supported facts.
3. **Mark** gap with `[citation needed]` or `[verify: ...]`.

Examples in `references/examples.md` assume writer has facts. Without source material, prefer remove/narrow. Do not invent.

Post-rewrite check: scan for new date, number, named organisation, named tool, location, cause, or superlative. If not sourced, remove, narrow, or mark `[verify: ...]`.

Goal: clarity + reader trust. Not evading AI detectors. Never reduce accuracy, attribution, or transparency just to sound less generated.

## When to use this skill

Use when prose may carry AI tells:

- Editing AI-generated drafts before publication
- Reviewing your own writing after it starts sounding generated
- Cleaning chat-assistant text pasted into a longer document

For grammar/concision, pair with `writing-clearly-and-concisely`. For audience-specific application, see `audience-awareness`.

## Voice calibration (optional)

If user gives prior writing sample:

1. Read it. Note sentence length, word level, paragraph openings, punctuation, recurring phrases, transitions.
2. Match those patterns. Do not only remove AI markers.
3. If no sample, use neutral varied prose matching genre.

Sample forms:

- Inline: "De-slop this text. Here's a sample of my writing for voice matching: [sample]"
- File: "De-slop this text. Use my writing style from [file path] as a reference."

## Pattern catalogue

Scan for 28 patterns. Families: content, language/grammar, style/formatting, communication artifacts.

Worked before/after rewrites for every pattern, plus stacked examples, live in `references/examples.md`. Load `references/examples.md` for a concrete pattern rewrite or multi-pattern paragraph.

### Content

**1. Undue emphasis on significance, legacy, and broader trends** — inflates importance. Facts should show importance.
*Watch: stands/serves as, testament/reminder, vital/significant/crucial/pivotal/key role/moment, underscores/highlights its importance, reflects broader, symbolising ongoing/enduring/lasting, contributing to, setting/marking/shaping, represents/marks a shift, evolving landscape, focal point, indelible mark, deeply rooted.*

**2. Superficial analyses with -ing endings** — dangling present-participle clauses add fake depth. Delete if vague/redundant.
*Watch: highlighting, underscoring, emphasising, ensuring, reflecting, symbolising, contributing to, cultivating, fostering, encompassing, showcasing.*

**3. Promotional, advertisement-like language** — neutral prose drifts into cultural-heritage/sales copy. Keep factual.
*Watch: boasts a, vibrant, rich (figurative), profound, enhancing its, showcasing, exemplifies, commitment to, natural beauty, nestled, in the heart of, groundbreaking (figurative), renowned, breathtaking, must-visit, stunning.*

**4. Vague attributions and weasel words** — name sources or remove attribution.
*Watch: industry reports, observers have cited, experts argue, some critics argue, several sources/publications when few are cited.*

**5. Outline-like "Challenges and Future Prospects" sections** — formulaic endings with no content. Cut; end on last concrete fact.
*Watch: Despite its... faces several challenges..., Despite these challenges, Challenges and Legacy, Future Outlook.*

**6. Generic positive conclusions** — vague uplift adds nothing. End on concrete fact, next action, or last substantive point.

**7. Persuasive authority tropes** — ceremony before ordinary claims.
*Watch: the real question is, at its core, in reality, what really matters, fundamentally, the deeper issue, the heart of the matter.*

**8. Signposting and announcements** — announces instead of saying. Cut opener.
*Watch: let's dive in, let's explore, let's break this down, here's what you need to know, now let's look at, without further ado.*

### Language and grammar

**9. Overused AI vocabulary** — not banned; clusters signal generated prose. Simplify.
*Watch: actually, additionally, align with, crucial, delve, emphasising, enduring, enhance, fostering, garner, highlight (verb), interplay, intricate/intricacies, key (adjective), landscape (abstract), pivotal, showcase, tapestry (abstract), testament, underscore (verb), valuable, vibrant.*

**10. Copula avoidance** — elaborate verb for simple is/are/has. Use simple form unless verb adds meaning.
*Watch: serves as / stands as / marks / represents [a], boasts / features / offers [a].*

**11. Negative parallelisms and tailing negations** — overused "not only... but..." / "not just X; Y" / clipped "no guessing." Rewrite plainly.

**12. Rule of three** — forced triplets sound comprehensive. Keep third item only if real.

**13. Elegant variation (synonym cycling)** — repeat the name or use pronoun; do not cycle synonyms to avoid repetition.

**14. False ranges** — avoid "from X to Y" unless X/Y are real endpoints on a meaningful scale.

**15. Passive voice and subjectless fragments — with judgment** — make active when actor matters. Keep technical imperatives/fragments ("Run the script." "Returns null if not found.") when useful.

**16. Excessive hedging** — cut stacked uncertainty. Academic/scientific prose may need careful hedging to avoid overclaiming.

**17. Filler phrases** — tighten: "in order to" -> "to"; "due to the fact that" -> "because"; "at this point in time" -> "now"; "has the ability to" -> "can". Full list: `references/examples.md`.

**18. Banned temporal words in code and comments** — relative terms age badly in code, identifiers, comments; prose can still say "currently" when it truly means "as of writing."
*Banned: now, currently, existing behavior, previous behavior, old, new, modern.*

### Style and formatting

**19. Em dash overuse** — replace most with commas, periods, or parentheses.

**20. Overuse of boldface** — bold real emphasis only; cut mechanical keyword bolding.

**21. Inline-header vertical lists** — bold header + colon on every bullet often reads generated. Use prose or simple bullets.

**22. Title case in headings** — prefer sentence case: first word + proper nouns.

**23. Emojis — scoped** — no decorative emoji in formal/long-form prose. Carve-outs: PR descriptions, commit messages, matching README/changelog style, Slack updates, LinkedIn/blog voice. Target filler emoji, not meaningful status markers.

**24. Curly vs straight quotes — scoped** — in code, Markdown, plaintext, and most technical contexts use straight quotes (`"`, `'`). In typeset long-form, curly quotes are correct.

**25. Fragmented headers** — heading followed by one-line restatement before real content. Cut restatement.

### Communication artifacts (chat text pasted into documents)

**26. Collaborative communication artifacts** — pasted chatbot correspondence. Strip it.
*Watch: I hope this helps, Of course!, Certainly!, You're absolutely right!, Would you like..., let me know, here is a...*

**27. Knowledge-cutoff disclaimers** — replace with sourced fact or remove.
*Watch: as of [date], up to my last training update, while specific details are limited/scarce..., based on available information...*

**28. Sycophantic tone** — chatty people-pleasing belongs in replies, not documents.

## Plain-language self-audit checklist

Before done, check:

- **Sentence length** — general prose target ~15-20 words/sentence; technical/academic can run longer, marketing shorter.
- **Length variance** — mix short, medium, occasional long. Uniform rhythm reads robotic.
- **Passive voice** — above ~25% in general prose suggests overuse; scientific/legal can run higher.
- **Adverb density** — many -ly adverbs flag weak verbs.
- **Repeated openers** — avoid every paragraph starting "Additionally / Furthermore / In addition."
- **Paragraph length** — vary by function; uniform blocks feel generated.
- **Factual safety** — new date, number, organisation, tool, location, or causal claim must come from source. Else remove, narrow, or mark.

This skill cannot compute Flesch-Kincaid, Gunning Fog, or lexical diversity without a real tool. Use separate analyzer for deeper readability.

## Related skills

For complementary guidance:

- `writing-clearly-and-concisely` - sentence-level grammar, concision, mechanics. Use together when editing prose.
- `audience-awareness` - adjusts rule strength by audience.

## Attribution

This skill consolidates:

- Flutter Authors' "Rules for Natural Writing" (2026, BSD-style licence - see `LICENSE-UPSTREAM`).
- Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), maintained by WikiProject AI Cleanup.
