# Experience, Skills, Verification, Custom URL, Recommendations

## Experience bullets

### What a strong bullet shows

A strong Experience bullet conveys, in this rough order:

1. **Impact** — what changed because of the work (user, business, system, team)
2. **Scope** — surface area: team size, user count, service count, data scale
3. **Technical context** — the technology, methodology, or system involved
4. **Evidence** — a metric, dataset size, or named artifact when it exists

Metrics are **strong evidence when they exist** — but engineering work often delivers value that doesn't translate into a clean number (a system you designed, an incident you led, a library other teams adopted). Force a fake metric and the bullet reads worse than the honest version.

### Strong vs weak openings

Lead with concrete verbs:

- **Strong:** Led, Built, Designed, Shipped, Cut, Drove, Launched, Grew, Scaled, Migrated, Rebuilt, Hardened, Owned, Authored
- **Weak (avoid):** Worked on, Handled, Assisted with, Responsible for, Participated in, Helped with, Was part of

### Before → After

| ❌ Before | ✅ After |
| --- | --- |
| Worked on the search service | Redesigned the multi-tenant search service (3.2M docs across 400 tenants); cut p95 latency from 820 ms → 260 ms |
| Responsible for CI/CD pipeline | Owned the CI/CD platform used by 60+ engineers; cut average deploy time 4h → 12 min via parallelized test sharding |
| Led product development | Shipped the agent orchestration layer (Python + Ray); now drives 40% of platform revenue |
| Handled on-call rotation | Led incident response for the payments service; authored the postmortem template now used by 4 backend teams |
| Worked on internal tooling | Designed and shipped the internal RAG search system used by 200+ engineers; no quantitative impact metric, but adopted as the default by 3 internal teams within 4 months |

The last row is the key example: a real, valuable engineering bullet **without** a clean metric. Don't fake a number — the scope (200+ engineers, 3 teams, 4 months) carries the evidence.

### Media attachments

Every role should have at least one attached media item:

- Screenshots of metrics dashboards (anonymized)
- Links to live projects, articles, demos
- Architecture diagrams (sanitized)
- Talk recordings
- Public PRs / RFCs

Media gives recruiters something tangible to click — text-only roles read as unverified.

---

## Skills

### Volume rules

- **Up to 50 skills** listed (LinkedIn cap)
- **Pin top 3** at the top of the section (see Pinning mechanics below)
- **Mirror skills** from 3–5 target job descriptions — use the workflow in `jd-keyword-workflow.md`
- Endorsements significantly improve a skill's ranking in recruiter searches; aim for ≥1 endorsement per claimed skill

### Pinning top 3 (mechanics)

LinkedIn doesn't make pinning obvious. The flow:

1. Go to your profile → **Skills** section → click the pencil (edit) icon
2. Find the skill you want to pin → click the three-dot menu on the skill card
3. Select **"Add as top skill"** (LinkedIn allows up to three top skills)
4. The pinned skills appear above all others on your public profile and in recruiter search previews

Choose the three skills that **most directly match your target role** — not your strongest skills, your most *role-relevant* ones. A staff backend engineer pinning "Excel" because they're great at it loses the search match for backend roles.

### 2026 high-value skills (SWE)

Include if genuinely applicable:

- The languages you actually ship in (Python, Go, TypeScript, Rust, Java)
- Datastores you operate (PostgreSQL, Redis, Kafka, ClickHouse)
- Infra you've built on (Kubernetes, Terraform, AWS, GCP)
- AI/ML stack if relevant (PyTorch, RAG, LangGraph, embeddings)
- System-level competencies (Distributed Systems, Observability, Reliability Engineering, API Design)
- Leadership signals where truthful (Technical Leadership, Mentorship, Engineering Management)

### Skills hygiene

- Remove skills you haven't used in 3+ years (stale signal)
- Don't list generic soft skills without evidence ("Leadership", "Teamwork") — back them with roles that prove it
- If you have conflicting skills across roles (e.g., backend + design), keep them — LinkedIn tolerates breadth and recruiters filter by intersection

---

## Verification (optional)

LinkedIn rolled out profile verification in 2023; it's a soft trust signal that helps but isn't required. A verified profile shows a checkmark next to the name in search results and on the profile page.

When it's worth the 5 minutes:

- You're searching openly and want every edge against fake-profile suspicion
- Your name is common or your profile is sparse on past-employer affiliations
- You're a remote candidate where fake-profile rates are higher

When it's fine to skip:

- You already have strong company affiliations and recommendations
- The verification methods available to you don't apply (no current employer for work email, country not supported for Government ID)

Verification methods (use the strongest available):

- **Government ID** via LinkedIn's CLEAR partnership (free, available in US / UK / Canada / India / Mexico and growing)
- **Workplace** — verified via employer HR system (only at some companies)
- **Work email** — verifies you have an active email at your current employer

How to claim:

1. LinkedIn → **Settings** → **Account preferences** → **Verifications**
2. Choose the strongest method available
3. Complete the flow (Government ID via CLEAR takes ~5 minutes)
4. The checkmark appears within 24 hours

---

## Custom URL

### The rule

`linkedin.com/in/firstnamelastname`

Never: `linkedin.com/in/firstname-lastname-123abc456`

### How to claim it

1. LinkedIn → Profile → Edit public profile & URL (top right)
2. Edit custom URL
3. Change to `firstnamelastname` (no spaces, no dashes if possible)

### Why it matters

- **Memorable** — you can say "linkedin.com/in/sergebulaev" in conversation
- **SEO** — Google ranks canonical URLs higher than hash-tail URLs
- **Signal of intent** — the short URL reads as someone who set up their profile deliberately

---

## Recommendations

### Why they matter

For job seekers, recommendations are the closest thing LinkedIn has to a reference check before the reference check. Recruiters skim them to confirm: did past managers/colleagues actually like working with this person, and what did they say specifically?

### How to request (the right way)

1. **Email or call first** — don't use LinkedIn's generic auto-request
2. **Ask for specifics** — "about [specific project / skill / outcome]"
3. **Offer to draft bullets** — make it 2 minutes of their time
4. **Reciprocate** — write theirs first, then ask

### Template for the ask

```text
Hey [Name],

I'm starting a job search and hoping you'd be up for a short recommendation.

If you're open to it, specifically about:
- [specific thing you worked on together]
- [concrete outcome]
- [skill you demonstrated]

Happy to draft 2-3 bullets you can edit. Takes you 60 seconds, helps me a lot.

Also happy to write yours first if that helps.
```

### Rotation

- Target **3 recommendations per year** from current context
- After a role change, ask for 1–2 from the old role (not 5 — looks desperate)
- Diverse contexts matter: managers, peers, direct reports, cross-functional collaborators
