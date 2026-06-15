# Target-JD Keyword Workflow

Recruiter search is mostly Boolean keyword match. Rank by using same language target JDs use, woven truthfully across profile.

Workflow: extraction → frequency → mapping → truthfulness.

## Step 1: Collect 3-5 target JDs

- Pick **3-5 currently-open job postings** matching target role + seniority
- Use companies user would actually apply to; avoid aspirational outliers with different talent bar
- Save each JD as plain text for search/grep

For broad searches, pick variety (infra-heavy, product-heavy, platform-heavy). Intersection = strongest recruiter-search language.

## Step 2: Extract terms

For each JD, extract:

| Category | Examples |
| --- | --- |
| **Title + seniority** | "Senior Software Engineer", "Staff", "Principal", "Lead", "Engineering Manager" |
| **Hard skills** | Python, Go, Rust, TypeScript, React, Kafka, Terraform, Kubernetes |
| **Domain terms** | "B2B SaaS", "fintech payments", "healthcare data", "developer tooling" |
| **Responsibility verbs** | "designed", "shipped", "owned", "led", "scaled", "migrated" |
| **System / scale signals** | "distributed systems", "high-throughput", "multi-tenant", "low-latency", "5M+ users" |
| **Process / methodology** | "on-call rotation", "RFC process", "post-incident review", "design reviews" |

Skip generic filler ("strong communicator", "passionate").

## Step 3: Frequency + weight

Count JD appearances:

| Frequency | Treat as |
| --- | --- |
| 4-5 of 5 (or 3-3 of 3) | **Must-include** in headline + Skills + at least one Experience bullet |
| 2-3 of 5 (or 2 of 3) | **Strong-to-include** — fit into About specialties or Skills |
| 1 of 5 | Skip unless personal differentiator |

Frequency prevents chasing one outlier JD.

## Step 4: Map to profile sections

For each must-include term:

| Profile section | What to include |
| --- | --- |
| **Headline** | 3-5 must-include terms across role + industry + signal keywords (within ~220 chars) |
| **About** | 5-7 must-include terms in 7-step body; 3-5 strong-to-include in Specialties |
| **Skills** | Every truthful must-include + strong-to-include term, up to 50 cap |
| **Experience** | Terms in bullets for roles where work happened — don't backfill |
| **Featured** | Title slots with must-include role language ("Backend platform redesign", not "My work") |

## Step 5: Truthfulness check

- **Don't claim skills user lacks.** Recruiters skim; interviewers probe.
- **Don't place terms in roles where work wasn't done.** If no RAG at Company A, don't put RAG in Company A bullets; use side-project Featured slot.
- **Use exact JD phrasing where natural.** Forced phrases read worse than raw skills.
- **Cap must-include density.** 20 headline keywords trigger skepticism + spam heuristics.

## Step 6: Cross-check before publishing

- Headline: top 3 must-include terms in first 100 chars
- About: hook (first ~265 chars) contains 1-2 must-include terms
- Skills: every truthful must-include listed; top 3 pinned are JD-aligned, not legacy
- Experience: at least one bullet per recent role contains a must-include term in context
- Featured: at least one item title contains a must-include term

If a must-include term fits nowhere truthfully, upskill before applying; don't lie.
