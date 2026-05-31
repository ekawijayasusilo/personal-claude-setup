# De-Slop Worked Examples

Concrete before/after rewrites for the patterns catalogued in `SKILL.md`. Load this file when you want a worked rewrite for a specific pattern, or to see how several patterns stack in one passage (the two longer examples at the end).

Each entry maps by number and name to a pattern in the SKILL.md catalogue. The rule and "words to watch" live in SKILL.md; this file is examples only. Patterns whose SKILL.md entry is fully self-contained (e.g. generic positive conclusions, curly vs straight quotes) have no entry here.

Rewrites assume the writer has the relevant facts. Where an "After" depends on source material, that source is noted in parentheses — do not invent such details. See the Factual safety rule in SKILL.md.

## Content patterns

### 1. Undue emphasis on significance, legacy, and broader trends

Before: *The Statistical Institute of Catalonia was officially established in 1989, marking a pivotal moment in the evolution of regional statistics in Spain. This initiative was part of a broader movement across Spain to decentralise administrative functions.*

After: *The Statistical Institute of Catalonia was established in 1989 to collect and publish regional statistics independently from Spain's national statistics office.*

### 2. Superficial analyses with -ing endings

Before: *The temple's colour palette of blue, green, and gold resonates with the region's natural beauty, symbolising Texas bluebonnets, the Gulf of Mexico, and the diverse Texan landscapes, reflecting the community's deep connection to the land.*

After: *The temple uses blue, green, and gold. The architect chose these colours to reference local bluebonnets and the Gulf coast.*

### 3. Promotional and advertisement-like language

Before: *Nestled within the breathtaking region of Gonder in Ethiopia, Alamata Raya Kobo stands as a vibrant town with a rich cultural heritage and stunning natural beauty.*

After (with source material that mentions a market and a church): *Alamata Raya Kobo is a town in the Gonder region of Ethiopia, known for its weekly market and 18th-century church.*

### 4. Vague attributions and weasel words

Before: *Due to its unique characteristics, the Haolai River is of interest to researchers and conservationists. Experts believe it plays a crucial role in the regional ecosystem.*

After (assuming source material like *"2019 Chinese Academy of Sciences survey: 7 endemic fish species"*): *The Haolai River supports several endemic fish species, according to a 2019 survey by the Chinese Academy of Sciences.*

### 5. Outline-like "Challenges and Future Prospects" sections

Before: *Despite its industrial prosperity, Korattur faces challenges typical of urban areas, including traffic congestion and water scarcity. Despite these challenges, with its strategic location and ongoing initiatives, Korattur continues to thrive as an integral part of Chennai's growth.*

After (no additional source material): *Traffic congestion and water scarcity are recurring problems in Korattur.*

After (with source material giving dates and projects): *Traffic congestion increased after 2015 when three new IT parks opened. The municipal corporation began a stormwater drainage project in 2022 to address recurring floods.*

The "challenges" formula needs to be cut either way — but the dates and named projects must come from the source, not from the rewrite.

### 7. Persuasive authority tropes

Before: *The real question is whether teams can adapt. At its core, what really matters is organisational readiness.*

After: *The question is whether teams can adapt. That mostly depends on whether the organisation is ready to change its habits.*

### 8. Signposting and announcements

Before: *Let's dive into how caching works in Next.js. Here's what you need to know.*

After: *Next.js caches data at multiple layers: request memoization, the data cache, and the router cache.*

## Language and grammar patterns

### 9. Overused AI vocabulary

Before: *Additionally, a distinctive feature of Somali cuisine is the incorporation of camel meat. An enduring testament to Italian colonial influence is the widespread adoption of pasta in the local culinary landscape, showcasing how these dishes have integrated into the traditional diet.*

After: *Somali cuisine also includes camel meat, considered a delicacy. Pasta dishes, introduced during Italian colonisation, remain common, especially in the south.*

### 10. Copula avoidance

Before: *Gallery 825 serves as LAAA's exhibition space for contemporary art. The gallery features four separate spaces and boasts over 3,000 square feet.*

After: *Gallery 825 is LAAA's exhibition space for contemporary art. It has four rooms totalling 3,000 square feet.*

### 11. Negative parallelisms and tailing negations

Before: *It's not just about the beat riding under the vocals; it's part of the aggression and atmosphere. It's not merely a song, it's a statement.*

After: *The heavy beat adds to the aggressive tone.*

Before (tailing negation): *The options come from the selected item, no guessing.*

After: *The options come from the selected item without forcing the user to guess.*

### 12. Rule of three

Before: *The event features keynote sessions, panel discussions, and networking opportunities. Attendees can expect innovation, inspiration, and industry insights.*

After: *The event includes talks and panels, with time for informal networking between sessions.*

### 13. Elegant variation (synonym cycling)

Before: *The protagonist faces many challenges. The main character must overcome obstacles. The central figure eventually triumphs. The hero returns home.*

After: *The protagonist faces many challenges, eventually triumphs, and returns home.*

### 14. False ranges

Before: *Our journey through the universe has taken us from the singularity of the Big Bang to the grand cosmic web, from the birth and death of stars to the enigmatic dance of dark matter.*

After: *The book covers the Big Bang, star formation, and current theories about dark matter.*

### 15. Passive voice and subjectless fragments

Before (passive, agent matters): *The decision was made to discontinue the legacy API in Q3.*

After: *The platform team decided to discontinue the legacy API in Q3.*

### 16. Excessive hedging

Before: *It could potentially possibly be argued that the policy might have some effect on outcomes.*

After: *The policy may affect outcomes.*

### 17. Filler phrases

- "In order to achieve this goal" → "To achieve this"
- "Due to the fact that it was raining" → "Because it was raining"
- "At this point in time" → "Now"
- "In the event that you need help" → "If you need help"
- "The system has the ability to process" → "The system can process"
- "It is important to note that the data shows" → "The data shows"

### 18. Banned temporal words in code and comments

Bad: `// This function now uses the config parser instead of hardcoding.`

Good: `// Resolves paths via ConfigParser.loadConfig to support custom config locations.`

## Style and formatting patterns

### 19. Em dash overuse

Before: *The term is primarily promoted by Dutch institutions—not by the people themselves. You don't say "Netherlands, Europe" as an address—yet this mislabeling continues—even in official documents.*

After: *The term is primarily promoted by Dutch institutions, not by the people themselves. You don't say "Netherlands, Europe" as an address, yet this mislabeling continues in official documents.*

### 20. Overuse of boldface

Before: *It blends **OKRs (Objectives and Key Results)**, **KPIs (Key Performance Indicators)**, and visual strategy tools such as the **Business Model Canvas (BMC)** and **Balanced Scorecard (BSC)**.*

After: *It blends OKRs, KPIs, and visual strategy tools like the Business Model Canvas and Balanced Scorecard.*

### 21. Inline-header vertical lists

Before:

```
- **User Experience:** The user experience has been significantly improved with a new interface.
- **Performance:** Performance has been enhanced through optimised algorithms.
- **Security:** Security has been strengthened with end-to-end encryption.
```

After: *The update improves the interface, speeds up load times through optimised algorithms, and adds end-to-end encryption.*

### 22. Title case in headings

Before: `## Strategic Negotiations And Global Partnerships`

After: `## Strategic negotiations and global partnerships`

### 23. Emojis

Before (formal report): *🚀 **Launch Phase:** The product launches in Q3 / 💡 **Key Insight:** Users prefer simplicity / ✅ **Next Steps:** Schedule follow-up meeting*

After: *The product launches in Q3. User research showed a preference for simplicity. Next step: schedule a follow-up meeting.*

### 25. Fragmented headers

Before:

```
## Performance

Speed matters.

When users hit a slow page, they leave.
```

After:

```
## Performance

When users hit a slow page, they leave.
```

## Communication patterns (chat artifacts in pasted text)

### 26. Collaborative communication artifacts

Before: *Here is an overview of the French Revolution. I hope this helps! Let me know if you'd like me to expand on any section.*

After: *The French Revolution began in 1789 when financial crisis and food shortages led to widespread unrest.*

### 27. Knowledge-cutoff disclaimers

Before: *While specific details about the company's founding are not extensively documented in readily available sources, it appears to have been established sometime in the 1990s.*

After: *The company was founded in 1994, according to its registration documents.*

### 28. Sycophantic tone

Before: *Great question! You're absolutely right that this is a complex topic. That's an excellent point about the economic factors.*

After: *The economic factors you mentioned are relevant here.*

## Longer passages — several patterns at once

Single-rule examples show patterns in isolation. Real prose carries several at once. These two show how to untangle a paragraph carrying multiple tells.

### Example A — significance puffery, copula avoidance, -ing dangling, rule of three, em dash

Before:

> The introduction of containerisation marked a pivotal moment in the evolution of software deployment, representing a fundamental shift in how engineering teams ship, scale, and operate their systems. At its core, Docker serves as a packaging mechanism — one that has enduring influence across the industry — fostering a vibrant ecosystem of orchestrators, registries, and runtimes. It is not just a tool; it is a foundation. By standardising the runtime environment, Docker enabled a new wave of practices, transforming how developers think about portability, reproducibility, and operational consistency.

After:

> Docker, released in 2013, packages an application with its dependencies into a runnable image. Teams adopted it because the same image runs on a developer laptop and a production server. That shifted how applications are shipped: a build artifact became a container image, and the gap between development and production environments narrowed. Kubernetes, Nomad, and other orchestrators were built to schedule and manage these images at scale.

### Example B — chatbot artifact, hedging, vague attribution, generic conclusion

Before:

> Great question! Based on available information, it could potentially be argued that adopting feature flags might have several benefits for engineering teams. Industry observers have noted that this practice continues to grow in popularity. Despite some challenges related to operational complexity, the future of feature-flagging looks bright. Let me know if you'd like me to expand on any of these points!

After:

> Feature flags let teams ship code without making it visible to users. The cost is operational: stale flags accumulate and the codebase ends up carrying many half-completed migrations. Teams that use flags well treat each one as having an expected lifetime and audit them on a schedule. LaunchDarkly, Flipper, and Unleash are common managed and self-hosted options.
