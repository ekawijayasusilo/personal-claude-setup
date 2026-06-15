---
name: linkedin-profile-optimizer
description: Audit and rewrite a software-engineer job-seeker's LinkedIn profile end-to-end for 2026 — headline, About 7-step, Featured, banner, photo, Experience (impact + scope + tech context), Skills with role-relevant pinning, optional verification, custom URL, recommendations. Built around a target-JD keyword workflow, SWE role-family guidance (Backend / Frontend / Full-stack / Platform / AI-ML / Security / Staff IC / EM), and search-mode adjustments (open / discreet / pivot / career break / employed-exploring). Triggers on "review my profile", "rewrite my headline", "fix my About", "profile audit", "LinkedIn bio", "open to work", "applying to jobs", "land more interviews", "improve recruiter visibility", "convert resume to LinkedIn", "engineer LinkedIn", "developer profile".
---

# LinkedIn Profile Optimizer (Software-Engineer Job Seekers)

Audit 10 LinkedIn profile components (photo, banner, headline, About, Featured, Experience, Skills, custom URL, recommendations, verification) against 2026 job-seeker heuristics; rewrite weak sections. Default: **software-engineer job seekers**: backend, frontend, full-stack, platform/DevOps/SRE, AI/ML, security, staff/principal IC, EM. Also fits adjacent technical job seekers (TPMs, technical PMs).

Not for: HR sourcing playbooks, content creators / influencers, service-selling business owners, company-page executive branding.

## When to use

- User wants profile audit before job search
- User is open / discreetly looking and wants recruiter outreach
- User targets specific roles (senior backend, staff IC, EM, ML engineer) and recruiter-search rank
- User pivots role family (Backend → ML, IC → EM, EM → Staff IC)
- User wants headline, About, Experience, or Featured rewrite
- User has target JDs and wants profile language mirrored
- Trigger phrases: "review my profile", "fix my headline", "land more interviews", "recruiter visibility", "applying to jobs", "engineer LinkedIn"

## Input

- Profile URL or section screenshots
- **Target role(s)** — exact titles (e.g., "Senior Backend Engineer", "Staff ML Platform Engineer", "Engineering Manager")
- **Target industry / stack** — e.g., "B2B SaaS · Go + Postgres + Kafka", "FinTech payments · Java", "AI infra · Python + PyTorch"
- **Seniority** — junior / mid-level / senior / staff / principal / engineering manager
- **Search mode** — open / discreet / career pivot / career break or post-layoff / employed-but-exploring (see `references/search-modes.md`)
- **3–5 target job descriptions** — recommended for keyword extraction (see `references/jd-keyword-workflow.md`); else fall back to role-family defaults
- Optional: SWE role family if target role unclear (see `references/swe-role-families.md`)

## Output

1. **Scorecard** (10 sections, pass / fail / needs-work)
2. **Priority fixes** ranked by recruiter-search rank + interview-rate impact
3. **Before → After rewrites** for failing sections, with truthful JD-aligned keywords
4. **Expected outcomes**: keyword match, recruiter-search visibility, trust signal, role-family fit

## Steps

1. **Intake.** Capture profile state, target role, industry / stack, seniority, search mode. Flag missing sections.
2. **Run JD-keyword extraction.** Collect 3–5 target JDs; extract must-include + strong-to-include terms via `references/jd-keyword-workflow.md`. Feed every rewrite. **If no JDs**, continue with `references/swe-role-families.md`; flag keyword targeting as approximate.
3. **Score** 10 sections against checklist.
4. **Rewrite headline** — use 220 chars tightly; front-load must-include terms into first ~100 chars (mobile preview); match search-mode tone (`search-modes.md`).
5. **Rebuild About** — 7-step structure; first ~265 chars must carry target-role pitch; weave 5–7 must-include + 3–5 strong-to-include terms in Specialties.
6. **Curate Featured** — engineer triplet: GitHub / portfolio (Slot 1) + technical writeup or signature project (Slot 2) + optional talk / second project / strong post (Slot 3). De-prioritize LinkedIn posts.
7. **Rewrite Experience bullets** — show **impact + scope + technical context + evidence**. Use metrics when real; don't fake metrics for scope/adoption work. Mirror JD terms only where work happened.
8. **Update Skills** — list truthful JD must-include + strong-to-include terms up to 50 cap. Pin top 3 most **role-relevant** skills, not strongest.
9. **Claim custom URL** + **verification badge (optional)** — verification = soft signal; skip if methods don't apply.
10. **Draft recommendation requests** + deliver before/after diff with expected qualitative outcomes.

## Ten-component scorecard

| # | Section | Pass criteria (2026) |
|---|---------|----------------------|
| 1 | **Photo** | ≥400x400, face fills 60%, <3 years old, natural light, slight smile |
| 2 | **Banner** | 1584x396, text in right 2/3, high contrast, target-role signal, search-mode fit (see `search-modes.md`) |
| 3 | **Headline** | 220-char space used tightly; `[Target Role] | [Industry / Stack] | [Signal Keyword]`; top 3 JD must-include terms in first ~100 chars |
| 4 | **About** | 200-300 words, first-person, 7-step structure, hook in first ~265 chars, 5+ JD must-include terms |
| 5 | **Featured** | Engineer-first triplet, custom 1200x627 thumbnails |
| 6 | **Experience** | Impact + scope + technical context + evidence; real metrics; 5+ skills per role; media attached |
| 7 | **Skills** | Up to 50, top 3 pinned and role-relevant, mirrors target JDs, endorsements help rank |
| 8 | **Custom URL** | `linkedin.com/in/firstnamelastname` (not default hash) |
| 9 | **Recommendations** | At least 3 recent, specific, from varied contexts |
| 10 | **Verification** (optional) | Soft trust signal; use Government ID (CLEAR) / Workplace / work email when available; skip if not applicable |

## Hard rules

Voice rules (all rewrites):

- **First person by default** ("I shipped...", "I led..."); third person only for senior exec / board-facing profiles
- **No AI-slop vocabulary** — never "passionate thought leader", "driven professional", "results-oriented", "innovative", "synergy", "disruptor", "seasoned"
- **No wall of text** — use line breaks, especially About
- **Specifics over adjectives** — "Cut p95 latency 68% on a 3M-doc pipeline" beats "significantly improved performance"
- **Action verb + impact in Experience bullets** — start with Led, Built, Designed, Shipped, Cut, Owned, Migrated; include real metrics; never "responsible for" / "worked on" / "helped with"
- **Truthfulness over keyword stuffing** — mirror JD terms only where work happened (see `jd-keyword-workflow.md` §Truthfulness check)

Other:

- Don't pitch services in job-seeker profiles (no "Book a call", no "DM me" hooks); that signals client-seeking, not job-seeking
- If current role != target role: headline + About reflect **target**; Experience reflects **history**
- For **discreet search**: disable activity broadcasts before editing, batch all changes in one session (path in `search-modes.md` Mode 2)

## Reference files

- `references/jd-keyword-workflow.md` — collect → extract → frequency → map → truthfulness check for target-JD keywords (run first)
- `references/swe-role-families.md` — per-family headline keywords, Experience emphasis, proof artifacts
- `references/search-modes.md` — open / discreet / pivot / career break / employed-exploring section effects
- `references/profile-headline-formulas.md` — formula + SWE before/after examples
- `references/about-section-templates.md` — 7-step structure + job-seeker example
- `references/featured-section-playbook.md` — engineer-first Featured triplet, thumbnails, rotation
- `references/banner-photo-specs.md` — dimensions, composition, mobile test, search-mode CTAs
- `references/experience-skills-rules.md` — Experience framing, Skills pinning, optional verification, custom URL, recommendations
