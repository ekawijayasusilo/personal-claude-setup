# Profile Headline Formulas (Software-Engineer Job Seekers)

**Character limit:** 220. **Use the space efficiently — not maximally.** A tight 140-char headline that says exactly what role you want and why a recruiter should care beats 220 chars of padded keywords.

## The formula

```text
[Target Role / Specialty] | [Industry / Domain or Stack] | [Signal Keyword or Concrete Result]
```

Three parts separated by `|`. Each part does one job:

- **Target Role / Specialty** — the job title you're applying for (not necessarily your current title)
- **Industry / Domain or Stack** — where you want to work next, or the technical stack that defines your work
- **Signal Keyword or Concrete Result** — a technology, methodology, or proof point recruiters actually search for

## Rules

1. **Lead with the target role, not the current title.** If you're a Senior Engineer applying for Staff roles, lead with "Staff Software Engineer". If you're pivoting (e.g., Backend → ML), lead with the destination.
2. **Be specific.** "B2B SaaS" beats "tech". "Python / Django" beats "web". "FinTech payments" beats "finance".
3. **Pack keywords recruiters actually search for.** Mirror the language of 3–5 target job descriptions (see `jd-keyword-workflow.md`).
4. **No filler adjectives.** Cut "passionate", "driven", "results-oriented" (see SKILL.md §Hard rules).
5. **Capitalize technologies and product names** — "Python", "PostgreSQL", "Kubernetes", "Figma", "AWS".
6. **Front-load the must-include terms.** Mobile preview shows only the first ~100 chars; the top 3 JD-must-include terms should land in that window.

## Before → After (SWE-focused examples)

### Mid-level backend engineer applying for senior backend roles

- ❌ "Software Engineer at Company X"
- ✅ "Senior Backend Engineer | B2B SaaS, Distributed Systems | Go, PostgreSQL, Kafka — cut p99 latency 68% on multi-tenant pipeline"

### Senior frontend engineer applying for staff product-engineering roles

- ❌ "Senior Frontend Engineer"
- ✅ "Staff Product Engineer | B2C Web | React, TypeScript, Design Systems — shipped 0→1 onboarding, +23% activation"

### Full-stack engineer pivoting to AI / ML platform roles

- ❌ "Full-Stack Engineer at StartupCo"
- ✅ "ML Platform Engineer (ex-Full-Stack) | LLM Eval, RAG, Inference | Python, PyTorch, Ray — shipped agent eval framework used by 6 teams"

### Platform / SRE engineer applying for senior platform roles

- ❌ "DevOps Engineer"
- ✅ "Senior Platform Engineer | Reliability, Observability | Kubernetes, Terraform, Datadog — cut p95 deploy time 4h → 12 min"

### Staff engineer applying for principal IC roles

- ❌ "Staff Software Engineer | Tech Leader"
- ✅ "Principal Software Engineer | Platform / Distributed Systems | Go, Postgres, Kafka — led 3-team migration, 99.99% SLO"

### Engineering manager applying for senior EM / director roles

- ❌ "Engineering Manager"
- ✅ "Senior Engineering Manager | Platform / Backend | Scaled team 5→14, 18-month retention >90%, shipped 3 zero-to-one platforms"

### Non-SWE example (formula generalizes)

The formula works for adjacent technical roles where the job-seeker context applies:

- ❌ "Product Manager"
- ✅ "Senior Technical PM | Developer Tools, API Platforms | Shipped public API used by 3K+ teams"

## Section-specific anti-patterns

For general voice / AI-slop anti-patterns, see SKILL.md §Hard rules. Headline-specific anti-patterns:

- "Open to Work" in the headline text — use the dedicated badge (or recruiters-only mode for discreet searches; see `search-modes.md`)
- Emoji chains (🚀🔥💡) — read as low-effort
- All-caps headlines or sections in ALL CAPS
- "10+ years of experience in..." — nobody searches this; convert to a concrete proof point instead
- Chaining every past title with pipes — three identities is the cap
- Padding to 220 chars with weak keywords just to "fill space" — tight beats padded

## Search-keyword placement

For the full keyword-extraction workflow, see `jd-keyword-workflow.md`. The minimum:

- Include the **target role noun** ("Staff Engineer", "ML Platform Engineer", "Senior Backend Engineer")
- Include the **target industry or stack** ("B2B SaaS", "FinTech", "Go + Postgres + Kafka")
- Include 1–2 **specialty keywords** drawn from real JDs ("Distributed Systems", "RAG", "Design Systems", "Observability")
