# writing-toolkit

Skills for human-readable writing: sentence clarity, AI-slop removal, audience fit, document structure, and technical-doc templates. Skills layer: load closest match; it points to siblings.

## Skills

- **writing-clearly-and-concisely** - Strunk-style sentence polish: tighten prose, fix grammar/punctuation, cut needless words.
- **de-slop** - remove AI-writing tells: puffery, rule-of-three, em-dash overuse, chatbot artifacts.
- **audience-awareness** - identify reader + document type first; technical docs, launch posts, and essays need different rules.
- **document-structure** - organize whole docs with BLUF, inverted pyramid, PREP, SCQA, Diataxis.
- **tech-doc-templates** - scaffold RFC, ADR, Design Doc, or Postmortem.

## How the skills fit together

Typical flow: choose structure (`document-structure` or `tech-doc-templates`), calibrate audience (`audience-awareness`), draft, then polish (`writing-clearly-and-concisely` + `de-slop`). Each skill links siblings.

## Installation

Load via Claude Code marketplace config, or point Claude Code at `plugins/writing-toolkit/` directly. Manifest: `.claude-plugin/plugin.json`.

## Licensing and attribution

Plugin wrapper + original skill content: MIT. Adapted sources: public-domain *The Elements of Style*, Flutter Authors' "Rules for Natural Writing", Wikipedia's "Signs of AI writing". See [LICENSES.md](LICENSES.md).
