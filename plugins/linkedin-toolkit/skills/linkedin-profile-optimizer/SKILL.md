---
name: linkedin-profile-optimizer
description: Audit and rewrite a software-engineer job-seeker's LinkedIn profile end-to-end for 2026 — headline, About 7-step, Featured, banner, photo, Experience (impact + scope + tech context), Skills with role-relevant pinning, optional verification, custom URL, recommendations. Built around a target-JD keyword workflow, SWE role-family guidance (Backend / Frontend / Full-stack / Platform / AI-ML / Security / Staff IC / EM), and search-mode adjustments (open / discreet / pivot / career break / employed-exploring). Triggers on "review my profile", "rewrite my headline", "fix my About", "profile audit", "LinkedIn bio", "open to work", "applying to jobs", "land more interviews", "improve recruiter visibility", "convert resume to LinkedIn", "engineer LinkedIn", "developer profile".
---

# LinkedIn Profile Optimizer (Software-Engineer Job Seekers)

Audit the ten components of a LinkedIn profile (photo, banner, headline, About, Featured, Experience, Skills, custom URL, recommendations, verification) against 2026 best practices, then rewrite each section that needs work. Defaults to **software-engineer job seekers** — backend, frontend, full-stack, platform/DevOps/SRE, AI/ML, security, staff/principal IC, and engineering manager. The same scaffolding generalizes to adjacent technical job-seekers (TPMs, technical PMs).

Not for: HR sourcing playbooks, content creators / influencers, business owners pitching services, or company-page executive branding.

## When to use

- User pastes their LinkedIn profile URL and asks for an audit before a job search
- User is "open to work" or "discreetly looking" and wants to attract recruiter outreach
- User is targeting specific roles (senior backend, staff IC, EM, ML engineer, etc.) and needs to rank in recruiter search
- User is pivoting role families (Backend → ML, IC → EM, EM → Staff IC) and needs the profile to reflect the destination
- User wants to rewrite their headline, About, Experience bullets, or Featured section
- User has a stack of target job descriptions and wants the profile language to mirror them
- Any of: "review my profile", "fix my headline", "land more interviews", "recruiter visibility", "applying to jobs", "engineer LinkedIn"

## Input

- Profile URL (or screenshots of sections)
- **Target role(s)** — exact job titles being applied for (e.g., "Senior Backend Engineer", "Staff ML Platform Engineer", "Engineering Manager")
- **Target industry / stack** — e.g., "B2B SaaS · Go + Postgres + Kafka", "FinTech payments · Java", "AI infra · Python + PyTorch"
- **Seniority** — junior / mid-level / senior / staff / principal / engineering manager
- **Search mode** — open / discreet / career pivot / career break or post-layoff / employed-but-exploring (see `references/search-modes.md`)
- **3–5 target job descriptions** — recommended for the keyword-extraction workflow (see `references/jd-keyword-workflow.md`); if unavailable, the skill falls back to role-family defaults
- Optional: SWE role family if not obvious from target role (see `references/swe-role-families.md`)

## Output

A structured audit + rewrite in this shape:

1. **Scorecard** (10 sections, pass / fail / needs-work)
2. **Priority fixes** (ranked by impact on recruiter search rank and interview rate)
3. **Before → After rewrites** for each failing section, with JD-aligned keywords woven in
4. **Expected outcomes** (qualitative: improved keyword match, recruiter-search visibility, trust signaling, role-family fit)

## Steps

1. **Intake.** Profile state + target role + industry / stack + seniority + search mode. Flag missing sections.
2. **Run JD-keyword extraction.** Collect 3–5 target JDs; extract must-include + strong-to-include terms via the workflow in `references/jd-keyword-workflow.md`. The output of this step feeds every rewrite below. **If the user can't supply JDs**, don't block — fall back to the role-family defaults in `references/swe-role-families.md`, proceed with the rewrites, and flag that keyword targeting is approximate until real JDs are provided.
3. **Score** each of 10 sections against the checklist (see references/).
4. **Rewrite headline** — use the 220-char space efficiently (tight beats padded); front-load must-include terms so they land in the first ~100 chars (mobile preview). Match the search-mode tone (see `search-modes.md`).
5. **Rebuild About** — 7-step structure; verify the first ~265 chars hook lands the target-role pitch; weave 5–7 must-include terms across the body and 3–5 strong-to-include terms in the Specialties line.
6. **Curate Featured** — engineer-first triplet: GitHub / portfolio (Slot 1) + technical writeup or signature project (Slot 2) + optional talk / second project / strong post (Slot 3). LinkedIn posts are de-prioritized.
7. **Rewrite Experience bullets** — convey **impact + scope + technical context + evidence**; include metrics where they exist, but don't fake them when the work's value is scope or adoption rather than numbers. Mirror JD terms truthfully — only in roles where the work actually happened.
8. **Update Skills** — list every truthful JD must-include + strong-to-include term (up to the 50 cap). Pin the top 3 most **role-relevant** skills, not your strongest.
9. **Claim custom URL** + **verification badge (optional)** — verification is a soft signal; skip if the available methods don't apply.
10. **Draft recommendation requests** with specifics + **deliver before/after diff** with expected qualitative outcomes (keyword match, recruiter-search visibility, trust signaling, role-family fit).

## Ten-component scorecard

| # | Section | Pass criteria (2026) |
|---|---------|----------------------|
| 1 | **Photo** | ≥400x400, face fills 60% of frame, <3 years old, natural light, slight smile |
| 2 | **Banner** | 1584x396, text in right 2/3, high contrast, signals target role; banner content matches search mode (see `search-modes.md`) |
| 3 | **Headline** | 220-char space used efficiently; format `[Target Role] | [Industry / Stack] | [Signal Keyword]`; top 3 JD must-include terms in first ~100 chars |
| 4 | **About** | 200-300 words, first-person, 7-step structure, hook in first ~265 chars, 5+ JD must-include terms woven through |
| 5 | **Featured** | Engineer-first triplet (GitHub/portfolio + technical writeup + optional third), custom 1200x627 thumbnails |
| 6 | **Experience** | Bullets convey impact + scope + technical context + evidence; metrics where they exist; 5+ skills per role; media attached |
| 7 | **Skills** | Up to 50 listed, top 3 pinned and role-relevant, mirrors target JDs, endorsements improve ranking |
| 8 | **Custom URL** | `linkedin.com/in/firstnamelastname` (not the default hash) |
| 9 | **Recommendations** | At least 3 recent, specific (not generic), from diverse contexts |
| 10 | **Verification** (optional) | Soft trust signal; claim via Government ID (CLEAR) / Workplace / work email when available — skip if methods don't apply |

## Hard rules

Voice rules (apply to every rewritten section):

- **First person by default** ("I shipped...", "I led...") — third person only acceptable for senior exec / board-facing profiles
- **No AI-slop vocabulary** — never "passionate thought leader", "driven professional", "results-oriented", "innovative", "synergy", "disruptor", "seasoned"
- **No wall of text** — use line breaks, especially in the About section
- **Specifics over adjectives** — "Cut p95 latency 68% on a 3M-doc pipeline" beats "significantly improved performance"
- **Action verb + impact in Experience bullets** — open with strong verbs (Led, Built, Designed, Shipped, Cut, Owned, Migrated); include metrics where they exist; never "responsible for" / "worked on" / "helped with"
- **Truthfulness over keyword stuffing** — only mirror JD terms in roles where the work actually happened (see `jd-keyword-workflow.md` §Truthfulness check)

Other:

- Don't pitch services in a job-seeker profile (no "Book a call" CTAs, no "DM me" hooks) — those mis-signal to recruiters that the user wants clients, not jobs
- If the user's current role doesn't match the target role, the headline and About must reflect the **target**; the Experience must reflect the **history**
- For **discreet search**: disable activity broadcasts before editing, and batch all profile changes in one session (exact settings path in `search-modes.md` Mode 2)

## Reference files

- `references/jd-keyword-workflow.md` — collect → extract → frequency → map → truthfulness check for target-JD keywords (run this first)
- `references/swe-role-families.md` — per-family quick reference: headline keywords, Experience emphasis, proof artifacts
- `references/search-modes.md` — open / discreet / pivot / career break / employed-exploring (how each affects sections)
- `references/profile-headline-formulas.md` — formula + SWE before/after examples
- `references/about-section-templates.md` — 7-step structure + job-seeker worked example
- `references/featured-section-playbook.md` — engineer-first Featured triplet, thumbnails, rotation
- `references/banner-photo-specs.md` — dimensions, composition, mobile test, search-mode CTAs
- `references/experience-skills-rules.md` — Experience bullet framing, Skills pinning, optional verification, custom URL, recommendations
