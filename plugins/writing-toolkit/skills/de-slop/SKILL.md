---
name: de-slop
description: Remove AI-writing patterns (slop) from prose so it reads as natural, human-written text. Use when editing or reviewing prose — especially anything drafted with AI help — to strip puffery, vague attributions, em-dash overuse, banned-word habits, rule-of-three formulas, copula avoidance, chatbot artifacts, and other tells. Pairs with writing-clearly-and-concisely for sentence-level polish.
---

# De-Slop: Remove AI Writing Patterns

This skill helps you edit prose so it does not read as AI-generated. It consolidates two bodies of guidance: rules for natural writing (from the Flutter team) and Wikipedia's "Signs of AI writing" catalogue (maintained by WikiProject AI Cleanup).

## Your task

When given text to de-slop:

1. Identify AI patterns from the catalogue below.
2. Rewrite problematic sections in place.
3. Preserve meaning. Match the intended tone (formal, technical, casual).
4. **Do not invent specificity** to fill the gap left by removed puffery. See the Factual safety rule below.
5. Do not "improve" beyond removing slop — this skill is for cleanup, not voice injection.
6. Run the self-audit checklist at the end before declaring done.
7. Run a final adversarial pass: ask yourself "what about this still reads as AI-generated?" Note remaining tells. Revise.
8. Return the final rewrite, optionally with a brief summary of changes.

## Factual safety rule

This is the most important rule in this skill. Read it before applying any other pattern.

Removing AI puffery often leaves a gap. The temptation is to fill the gap with concrete details — dates, named organisations, specific numbers, causal explanations. **Do not do this unless those details are present in the source text, the user's supplied context, cited sources, or files you have been asked to inspect.** Concrete language is not a license to add new facts.

A clear sentence with unsupported details is worse than a vague sentence. At least the vague sentence does not lie.

When the source does not support a concrete claim, you have three valid options:

1. **Remove** the unsupported claim entirely.
2. **Narrow** the claim to what the source actually supports.
3. **Mark** the gap with `[citation needed]` or `[verify: ...]` so the writer can fill it in.

The worked examples in `references/examples.md` show what good rewrites look like *assuming the writer has the relevant facts*. If you apply this skill without source material, prefer the conservative path (remove or narrow). Do not invent.

A useful self-check after rewriting: scan the rewrite for any new date, number, named organisation, named tool, location detail, causal explanation, or superlative. For each one, ask: was it in the source? If not, remove or mark it.

This skill is for clarity and reader trust. It is not a tool for evading AI detectors. Do not make edits that reduce accuracy, attribution, or transparency just to make text appear less AI-generated.

## When to use this skill

Use this skill whenever prose may carry AI tells:

- Editing AI-generated drafts before publishing them
- Reviewing your own writing if it has started to sound generated
- Cleaning up text pasted from a chat assistant into a longer document

For sentence-level grammar, conciseness, and clarity, pair this skill with `writing-clearly-and-concisely`. For audience-specific application of these rules, see `audience-awareness`.

## Voice calibration (optional)

If the user provides a writing sample (their own prior writing), analyse it before rewriting:

1. Read the sample. Note sentence-length patterns, word-choice level, paragraph openings, punctuation habits, recurring phrases, transition style.
2. Match those patterns in the rewrite. Do not just strip AI markers — replace them with patterns from the sample.
3. When no sample is provided, fall back to neutral, varied prose that fits the document's genre.

How the user provides a sample:

- Inline: "De-slop this text. Here's a sample of my writing for voice matching: [sample]"
- File: "De-slop this text. Use my writing style from [file path] as a reference."

## Pattern catalogue

The 28 patterns below are what to scan for. Each gives the rule and, where useful, the words or phrases that signal it. They group into four families: content, language and grammar, style and formatting, and communication artifacts.

Worked before/after rewrites for every pattern — plus two longer passages showing how several stack in one real paragraph — live in `references/examples.md`. Load it for a concrete rewrite of a specific pattern, or to see how to untangle a paragraph carrying several tells at once.

### Content

**1. Undue emphasis on significance, legacy, and broader trends** — Puffs up importance by claiming arbitrary aspects represent or contribute to a broader topic. If a subject matters, the facts should show it.
*Watch: stands/serves as, is a testament/reminder, a vital/significant/crucial/pivotal/key role/moment, underscores/highlights its importance, reflects broader, symbolising its ongoing/enduring/lasting, contributing to the, setting the stage for, marking/shaping the, represents/marks a shift, evolving landscape, focal point, indelible mark, deeply rooted.*

**2. Superficial analyses with -ing endings** — AI tacks present-participle phrases onto sentences to add fake depth. Delete the dangling clause if it just restates or adds vague commentary.
*Watch: highlighting, underscoring, emphasising, ensuring, reflecting, symbolising, contributing to, cultivating, fostering, encompassing, showcasing.*

**3. Promotional, advertisement-like language** — LLMs drift toward "cultural heritage" rhetoric even in neutral contexts. Keep tone factual.
*Watch: boasts a, vibrant, rich (figurative), profound, enhancing its, showcasing, exemplifies, commitment to, natural beauty, nestled, in the heart of, groundbreaking (figurative), renowned, breathtaking, must-visit, stunning.*

**4. Vague attributions and weasel words** — Attribute opinions to specific people or sources, or do not attribute them at all.
*Watch: industry reports, observers have cited, experts argue, some critics argue, several sources/publications (when few are cited).*

**5. Outline-like "Challenges and Future Prospects" sections** — Formulaic closing sections that contain no real content. Cut them; end with the last concrete fact.
*Watch: Despite its… faces several challenges…, Despite these challenges, Challenges and Legacy, Future Outlook.*

**6. Generic positive conclusions** — Vague upbeat endings ("the future looks bright," "exciting times lie ahead," "a major step in the right direction") add nothing. End on a concrete fact or the last substantive point.

**7. Persuasive authority tropes** — These pretend to cut through noise to a deeper truth, but the sentence that follows usually just restates an ordinary point with extra ceremony.
*Watch: the real question is, at its core, in reality, what really matters, fundamentally, the deeper issue, the heart of the matter.*

**8. Signposting and announcements** — LLMs announce what they are about to do instead of doing it. Cut the announcement; start with the content.
*Watch: let's dive in, let's explore, let's break this down, here's what you need to know, now let's look at, without further ado.*

### Language and grammar

**9. Overused AI vocabulary** — Statistically overused, not banned. Each has legitimate uses, but several in one paragraph is a flag — simplify.
*Watch: actually, additionally, align with, crucial, delve, emphasising, enduring, enhance, fostering, garner, highlight (verb), interplay, intricate/intricacies, key (adjective), landscape (abstract), pivotal, showcase, tapestry (abstract), testament, underscore (verb), valuable, vibrant.*

**10. Copula avoidance** — LLMs substitute elaborate constructions for simple is/are/has. Use the simple form unless the elaborate verb actually means something different.
*Watch: serves as / stands as / marks / represents [a], boasts / features / offers [a].*

**11. Negative parallelisms and tailing negations** — "Not only… but…", "It's not just X; it's Y", and clipped tail negations ("no guessing," "no wasted motion") are overused. Rewrite plainly.

**12. Rule of three** — LLMs force ideas into groups of three to sound comprehensive. Use a third item only if it is a real third item.

**13. Elegant variation (synonym cycling)** — Repetition-penalty artifacts cause excessive synonym swapping ("the protagonist" → "the main character" → "the central figure"). Repeat the name or use a pronoun.

**14. False ranges** — Avoid "from X to Y" unless X and Y are the endpoints of a meaningful scale (time, size). Two random topics are not a range.

**15. Passive voice and subjectless fragments — with judgment** — Rewrite to active voice when it clarifies. But not every fragment is slop: technical writing legitimately uses short imperatives ("Run the script.") and compressed forms ("Returns null if not found."). Target passives that genuinely obscure the actor in prose, not deliberate technical brevity.

**16. Excessive hedging** — Over-qualifying ("could potentially possibly," "might have some effect") signals uncertainty about everything. Exception: hedging is correct in academic/scientific writing, where overclaiming is the real problem.

**17. Filler phrases** — Cut bloat to tighter forms: "in order to" → "to", "due to the fact that" → "because", "at this point in time" → "now", "has the ability to" → "can". (Full list in `references/examples.md`.)

**18. Banned temporal words in code and comments** — Relative temporal terms lose meaning as the codebase ages. Applies to code, identifiers, and comments — not prose, which can still say "currently" when it genuinely means "as of writing."
*Banned: now, currently, existing behavior, previous behavior, old, new, modern.*

### Style and formatting

**19. Em dash overuse** — LLMs use em dashes (—) more than humans, mimicking "punchy" sales writing. Most rewrite cleanly with commas, periods, or parentheses.

**20. Overuse of boldface** — Bold should mark genuine emphasis, not "this is a keyword." Cut mechanical bolding.

**21. Inline-header vertical lists** — Lists where every item starts with a bolded header and a colon. Use prose or simple bullets.

**22. Title case in headings** — Use sentence case: capitalise the first word and proper nouns only.

**23. Emojis — scoped** — No emoji decoration on headings or bullets in formal or long-form prose (essays, reports, formal docs, academic writing). Carve-outs where conventional: PR descriptions and commit messages (✅ ❌ 🚧), READMEs/changelogs with an existing house style, internal Slack updates, LinkedIn/blog posts matching the author's voice. Target emojis used as filler, not ones carrying real information in their native context.

**24. Curly vs straight quotes — scoped** — In code, Markdown, plaintext, and most technical contexts, use straight quotes (`"`, `'`). In typeset prose (books, magazines, formatted long-form), curly quotes are correct. Target curly quotes leaking into source-file contexts.

**25. Fragmented headers** — A heading followed by a one-line paragraph that just restates the heading before the real content begins. Cut the restatement.

### Communication artifacts (chat text pasted into documents)

**26. Collaborative communication artifacts** — Chatbot correspondence pasted into a document. Strip it.
*Watch: I hope this helps, Of course!, Certainly!, You're absolutely right!, Would you like…, let me know, here is a…*

**27. Knowledge-cutoff disclaimers** — AI disclaimers about incomplete information left in pasted text. Either cite a real source or just state the fact.
*Watch: as of [date], up to my last training update, while specific details are limited/scarce…, based on available information…*

**28. Sycophantic tone** — Overly positive, people-pleasing language belongs in a chat reply, not a document.

## Plain-language self-audit checklist

Before declaring the rewrite done, check the metrics below — the things a model can verify from text alone. They will not catch everything, but a passage that fails several will read as AI-generated even if no single rule above was violated.

- **Sentence length** — target ~15–20 words/sentence for general prose; longer is fine for academic or technical writing, shorter for marketing.
- **Length variance** — mix short (5–10), medium (12–20), and occasional long (25+) sentences. If everything sits within ±3 words of the average, the rhythm reads robotic.
- **Passive voice** — above ~25% in general prose suggests overuse; scientific and legal writing legitimately runs higher.
- **Adverb density** — many -ly adverbs is a flag; a precise verb often beats verb + adverb ("walked slowly" → "trudged").
- **Repeated openers** — vary the first 2–3 words of sentences; do not open every paragraph with "Additionally / Furthermore / In addition."
- **Paragraph length** — uniform paragraph length signals AI patterning; real writing varies it by what each paragraph does.
- **Factual safety** — scan for any new date, number, named organisation, named tool, location, or causal claim not in the source. Remove it, narrow it, or mark it `[verify: ...]`. A clean-sounding rewrite that invents specificity is worse than a slightly vague one.

This skill cannot compute Flesch-Kincaid, Gunning Fog, or true lexical-diversity scores without a real computation tool; the checks above are the ones a language model applies reliably from text alone. For deeper readability analysis, use a separate analyser (script or MCP server).

## Related skills

For complementary guidance, also load:

- `writing-clearly-and-concisely` — sentence-level grammar, conciseness, and mechanics (Strunk). Use together with this skill when editing prose.
- `audience-awareness` — adjusts which of these rules apply most strongly to which audience.

## Attribution

This skill consolidates two upstream sources:

- The Flutter Authors' "Rules for Natural Writing" (2026, BSD-style licence — see `LICENSE-UPSTREAM`).
- Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), maintained by WikiProject AI Cleanup.
