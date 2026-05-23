---
name: linkedin-profile-optimizer
description: Audit and rewrite a job-seeker's LinkedIn profile end-to-end for 2026 — headline, About 7-step, Featured, banner, photo, Experience metrics, Skills with pinning + assessment badges, verification, custom URL, recommendations. Triggers on "review my profile", "rewrite my headline", "fix my About", "profile audit", "LinkedIn bio", "open to work", "applying to jobs", "land more interviews", "improve recruiter visibility", "convert resume to LinkedIn".
---

# LinkedIn Profile Optimizer

Audit the ten components of a LinkedIn profile (photo, banner, headline, About, Featured, Experience, Skills, custom URL, recommendations, trust signals) against 2026 best practices, then rewrite each section that needs work. Focused on **job seekers**: applicants targeting specific roles, career pivoters, and candidates leaving stealth mode to attract recruiter outreach.

## When to use

- User pastes their LinkedIn profile URL and asks for an audit before a job search
- User is "open to work" and wants to attract recruiter outreach
- User is targeting a specific role and needs to rank in recruiter search
- User is pivoting careers and needs the profile to reflect the target role, not the current one
- User wants to rewrite their headline, About, or Featured section
- Any of: "review my profile", "fix my headline", "land more interviews", "recruiter visibility", "applying to jobs"

## Input

- Profile URL (or screenshots of sections)
- **Target role(s)** — the exact job titles the user is applying for
- **Target industry / domain** — e.g., "B2B SaaS", "healthcare IT", "fintech"
- **Geography** — remote / city / region (drives keyword choices and recruiter pool)
- **Seniority** — IC / lead / manager / director / exec
- Optional: a target job description to mirror keywords against

## Output

A structured audit + rewrite in this shape:

1. **Scorecard** (10 sections, pass/fail/needs-work)
2. **Priority fixes** (ranked by impact on recruiter search rank and interview rate)
3. **Before → After rewrites** for each failing section
4. **Expected outcomes** (qualitative: improved keyword match, recruiter-search visibility, trust signaling)

## Steps

1. **Intake.** Collect profile state + target role / industry / seniority. Flag missing sections.
2. **Score each of 10 sections** against the checklist (see references/).
3. **Rewrite headline** using `[Target Role / Specialty] | [Industry / Domain] | [Signal Keyword]` — fit all 220 chars with role-keywords recruiters search for.
4. **Rebuild About** with 7-step structure; verify the first ~265 chars hook before "see more" lands the target-role pitch.
5. **Curate Featured** (3 items, job-seeker recipe):
   - **Portfolio / personal site** — best work samples
   - **Top-performing LinkedIn post or article** — demonstrates voice + thinking
   - **Signature project** — GitHub repo, design case study, published research, or shipped artifact
6. **Rewrite Experience bullets** as `action verb + specific metric`. Add 5+ skills per role. Pin top 3 skills in the Skills section.
7. **Claim trust signals** — LinkedIn verification (work email / government ID / workplace) + earn ≥1 skill-assessment badge relevant to the target role.
8. **Claim custom URL** (`linkedin.com/in/firstnamelastname`, not the `-123abc456` default).
9. **Draft recommendation requests** with specifics ("about [project/skill]") — don't send LinkedIn's generic template.
10. **Deliver before/after diff** + a short list of expected qualitative outcomes (better keyword match, recruiter-search visibility, "is this person real?" trust signaling).

## Ten-component scorecard

| # | Section | Pass criteria (2026) |
|---|---------|----------------------|
| 1 | **Photo** | ≥400x400, face fills 60% of frame, <3 years old, natural light, slight smile |
| 2 | **Banner** | 1584x396, text in right 2/3, high contrast, signals target role / portfolio link, tests well on mobile |
| 3 | **Headline** | Uses all 220 chars; format `[Target Role / Specialty] | [Industry] | [Signal Keyword]` |
| 4 | **About** | 200-300 words, first-person, 7-step structure, hook in first ~265 chars |
| 5 | **Featured** | 3 items (portfolio + top post + signature project), custom 1200x627 thumbnails |
| 6 | **Experience** | Every bullet = `action verb + metric`, 5+ skills per role, media attached |
| 7 | **Skills** | 50 listed, top 3 pinned, mirrors target job descriptions, endorsements improve ranking |
| 8 | **Custom URL** | `linkedin.com/in/firstnamelastname` (not the default hash) |
| 9 | **Recommendations** | At least 3 recent, specific (not generic), from diverse contexts |
| 10 | **Trust signals** | LinkedIn verification badge claimed + ≥1 skill-assessment badge earned for a target-role skill |

## Hard rules

Voice rules (apply to every rewritten section):

- **First person by default** ("I help...", "I led...") — third person only acceptable for senior exec / board-facing profiles
- **No AI-slop vocabulary** — never "passionate thought leader", "driven professional", "results-oriented", "innovative", "synergy", "disruptor", "seasoned"
- **No wall of text** — use line breaks, especially in the About section
- **Specifics over adjectives** — "Cut CAC 62%" beats "significantly improved efficiency"
- **Action verb + metric in Experience bullets** — never "responsible for" / "worked on" / "helped with"

Other:

- Don't pitch services in a job-seeker profile (no "Book a call" CTAs, no "DM me" hooks) — those mis-signal to recruiters that the user wants clients, not jobs
- If the user's current role doesn't match the target role, the headline and About must reflect the **target**, the Experience must reflect the **history**

## Reference files

- `references/profile-headline-formulas.md` — 220-char formula + job-seeker before/after examples
- `references/about-section-templates.md` — 7-step structure with character budgets + job-seeker worked example
- `references/featured-section-playbook.md` — job-seeker Featured triplet, thumbnails, rotation
- `references/banner-photo-specs.md` — dimensions, composition, mobile test, job-seeker CTAs
- `references/experience-skills-rules.md` — Experience bullet rewriting, Skills pinning + assessment badges, verification / trust signals, custom URL, recommendations
