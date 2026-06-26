# Designer Evaluation Playbook

**The operating manual for analyzing designer portfolios & resumes and producing hire/pass decisions.**

This is the companion to [`hiring-world-class-designers.md`](./hiring-world-class-designers.md). That file is the *knowledge base* — what makes a great designer. This file is the *procedure* — how to digest a batch of real candidates and return a structured verdict for each.

---

## How to use this file (instructions for the AI assistant)

When given a list of candidates (portfolio URLs, resumes, LinkedIn links, or any combination), apply this playbook to each one and return, **per candidate**:

1. **A category-by-category summary** (craft, product thinking, process, outcomes, ownership, authenticity).
2. **A verdict** — `STRONG YES` / `YES` / `LEAN NO` / `NO` — using the criteria in [§5](#5-verdict-criteria).
3. **The reasons** behind the verdict, tied to specific evidence (not vibes).
4. **If advancing:** a tailored list of [vetting questions](#7-legitimacy-vetting-question-bank) to confirm the strongest/most suspicious claims are real.
5. **If passing:** [constructive rejection feedback](#8-rejection-feedback--growth-guidance) with 1–2 specific, actionable growth areas.

Then return a **ranked shortlist** across all candidates. Use the [output template in §6](#6-per-candidate-output-template) for consistency. Always separate **observed evidence** from **concerns** from **recommendation** — and flag confidence level when evidence is thin or a site/resume couldn't be fully accessed.

> **Prime directive:** A portfolio/resume is evidence of *judgment*, not a gallery of artifacts. Score what changed because of the person's work and whether you can trust that they did it. The two failure modes to catch are (a) **renderers** — pretty work, no thinking; and (b) **padders** — claims that won't survive two minutes of specific questioning.

---

## 1. The triage mindset

Reviewers don't *read* portfolios — they **triage** them in escalating tiers, spending cheap signals first and expensive verification only on survivors. First pass is often **under 60 seconds**; a candidate can be cut in the first 5–30 seconds if the reviewer can't place them.

Every review silently answers three questions:
- **Role fit** — what kind of designer is this? (product / UX / UI-visual / interaction / research / systems / design-eng)
- **Seniority signal** — what scope, judgment, and ownership do they operate at?
- **Relevance** — useful for *this* role, *now*?

Run analysis as tiers; stop and mark "pass" if a tier fails hard:

| Tier | Time | What you're doing |
|---|---|---|
| 1. **5-second test** | ~5s | First impression of the hero/landing. Can you tell what they do, their level, and their best work? |
| 2. **Hero scan** | ~30s | Positioning line + project tiles. Is the strongest, most relevant work surfaced? Curated (~3–7 projects) or everything-dump? |
| 3. **One case study, deep** | 3–5 min | Open the project *they* lead with. Evaluate problem framing → role clarity → decisions/tradeoffs → outcome. **Make-or-break.** |
| 4. **Breadth check** | ~2 min | Skim 2–3 others for range and consistency. Was the first a one-off? |
| 5. **Who they are** | — | Only if still alive: About, resume, LinkedIn, links. Cross-check (see [§4](#4-authenticity--fraud-detection)). |

**Read vs. skim:** *Read* problem framing, role/contribution statements, and decision rationale. *Skim* polished final screens, intros, and the generic "Empathize → Define → Ideate" diagram every bootcamp portfolio shares (near-zero signal).

---

## 2. Portfolio analysis protocol

### 2a. Craft heuristics (judged in seconds)

The first fold is a live demo of the candidate's information architecture and visual craft. Fast checks: **spacing & alignment** (consistent rhythm/grid?), **typography** (intentional, limited type scale?), **visual hierarchy** (does the eye flow to the right thing?), **polish/consistency** (sloppiness makes reviewers doubt they can handle a real design system), **restraint** (over-animation and gradient soup signal style over substance).

> Calibrate to specialty: weak craft is near-disqualifying for UI/visual; for UX research or content design, weight clarity and reasoning over pixels.

### 2b. Reading a case study — the CARDIO lens

A strong case study runs **context → process → outcome**, and the signal lives in the *micro-decisions* inside it. Score each axis:

- **C**ontext — the situation and why it mattered.
- **A**ssumptions — what they believed going in.
- **R**esearch — how well they understood the problem.
- **D**iscoveries — what they learned (especially the surprises).
- **I**terations — did the design change in response to evidence?
- **O**utcome — did insight convert to a shipped, measured result?

Reading in order, look for: **problem framing** (did they solve the *right* problem, or jump to screens?), **explicit constraints** (their absence = fantasy-project tell), **process shown not claimed**, **decisions & rejected alternatives** (where judgment becomes visible — rejected options are gold), **iteration**, and **contextualized outcomes** (narrative + numbers).

### 2c. Classify the work realism

Tag every project: **Shipped** / **Client-real** / **Concept-redesign** / **Coursework**. Hiring managers prefer a small thing that *actually shipped* over a beautiful pet project — shipping proves execution under real constraints. A *well-framed* concept (real problem-solving, validation, tradeoffs) still carries weight; an unframed "I made [famous app] prettier" carries almost none.

- **Real-work tells:** named product/company, real constraints (legacy code, deadlines, stakeholder conflict), before/after of live states, engineering-reality awareness, post-launch data.
- **Fantasy tells:** unsolicited redesigns of famous apps, no users/constraints, flawless happy-path-only flows, zero mention of what got cut.

### 2d. Site-level signals (the portfolio is itself a work sample)

Broken links/images, dead case-study links, stale content (>18 months), slow performance, accessibility failures (contrast, focus indicators) — all signal poor operational discipline. A designer's *own* a11y failures are especially telling. Template sites (Framer/Squarespace) are fine and common — but a candidate who claims "I code" on a default template is a mismatch; a hand-built, polished site is a strong positive for design-engineer hybrids.

---

## 3. Resume analysis protocol

Run per resume, in order:

1. **Baseline calibration.** Note target role, claimed level/title, total years, field. Establish what scope/metrics are *plausible* at this level.
2. **Internal consistency.** Do titles, dates, progression cohere? Year-only dates (mask short stints)? Overlaps? Unexplained gaps >3 months? Implausible title jumps?
3. **Ownership scan.** Tag each bullet: **Ownership** (Led/Built/Designed/Shipped + specific artifact) vs. **Duty** ("Responsible for"/"Helped with") vs. **Ambiguous "we."** Compute an ownership ratio.
4. **Metric audit.** For each number, run the [four questions](#4b-reading-metrics-critically). Tag: Credible / Thin / Suspicious.
5. **Scope & level calibration.** Does claimed team size/budget/authority match the title and company stage? Flag authority claimed where only *influence* is evidenced.
6. **Skills sanity check.** Are listed skills demonstrated in experience bullets, or just a 30-item wall? Flag keyword stuffing.
7. **Language-tell scan.** Buzzword density without evidence ("results-driven," "spearhead," "synergy," "leverage"); uniform tone; "responsible for" repetition.
8. **Cross-reference** resume ↔ LinkedIn ↔ portfolio (see [§4c](#4c-cross-checking-sources)).
9. **Cluster the flags.** Decide credibility on whether flags *stack*, not any single one. Separate verifiable-facts-at-risk (degree, title, dates) from embellishment (vague metrics, "we") from acceptable puffery.

### Strong vs. weak resume bullets

| Weak | Strong |
|---|---|
| "Responsible for managing design projects." | "Led a 6-person redesign of enterprise onboarding; cut time-to-value 38%." |
| "Conducted user research." | "Ran 40+ interviews and analyzed 800+ tickets; reframed onboarding, lifting activation 18%." |
| "Increased conversions by 40%." | "Raised checkout conversion from 2.1% to 2.9% over Q2–Q3 via a redesigned cart flow." |

**Verb tells:** Strong = Led, Built, Designed, Shipped, Established, Drove, Spearheaded. Weak (hide the role) = Responsible for, Helped with, Assisted in, Participated in, Worked on, Contributed to.

---

## 4. Authenticity & fraud detection

Credibility ≠ quality. A polished resume can be fabricated; a plain one can be true. Judge whether claims can be *trusted and verified*, separately from whether the work is good. **No single signal is conclusive — look for clusters.** Priors worth knowing: ~64% of people admit to lying on a resume at least once; the highest-fabrication zones are **skills, scope/responsibilities, titles, and dates** — direct scrutiny there.

### 4a. Padding & fabrication tells

| Tactic | Tell | 🚩 Suspicious → ✅ Credible |
|---|---|---|
| **Title inflation** | Title-to-evidence mismatch; "VP" with IC bullets; invented titles ("Growth Ninja") | "VP of Design" (no span of control) → "Senior Designer (led 3 ICs, owned design system)" |
| **Team credit / "we"** | Collective outcome claimed solo, or hides behind "we" so no personal contribution is provable | "Grew revenue $5M" (junior IC) → "Owned the payments module within a 6-engineer rebuild" |
| **Vague/fabricated metrics** | No baseline, timeframe, or attribution; implausible magnitude; round unanchored figures | "Increased conversions 40%" → "From 2.1% to 2.9% over Q2–Q3" |
| **Padded skills** | 30–40 item tool walls; skills never referenced in any bullet | A 40-skill block → "Python — built the ETL pipeline that cut reporting 6d→3d" |
| **Embellished dates** | Year-only dates masking <12-month stints; overlaps; omitted short jobs | "2021–2023" everywhere → honest month/year |
| **Overstated scope** | Scale claims with no scope; *ownership* claimed where only *input* existed | "Led company-wide ops" → "Owned a $3.2M budget across 12 people; approved spend to $50K" |
| **"Responsible for"** | Duty-language describing the job, not what they drove | "Responsible for a team" → "Led a team of 6 to a 20% productivity gain in 6 months" |

### 4b. Reading metrics critically — four questions per number

1. **Baseline given?** "From X to Y" beats "by Z%." A bare percentage is uninterpretable.
2. **Mechanism present?** Does the bullet say *what they did* to cause it? A number with no lever is an assertion.
3. **Attribution honest?** Their impact, or a borrowed team/company outcome?
4. **Plausible?** Does the magnitude fit the title, company size, and tenure?

> Round numbers flag **in clusters**, not individually — real measurement is messy. The fabrication signature is numbers that are round, identically formatted, on *every* bullet, and slightly mismatched to the role. A single round number is not fraud; a pattern is. (AI-generated resumes overproduce these — "AI loves numbers.")

### 4c. Cross-checking sources

- **Resume ↔ LinkedIn** (catches *factual* inconsistency): title mismatches, date/tenure discrepancies, companies in one but not the other, conflicting metrics, education conflicts.
- **Resume ↔ Portfolio** (catches *contribution* inflation): Does the claimed work appear as a real case study? Does the claimed role match what the case study shows? Is team context clear or hidden in "we"? Is there a decision trail, or just pretty mockups?

### 4d. Originality & AI-generation tells (portfolio)

- **Dribbble-bait** — beautiful final screens, no problem/constraints/"why." The biggest single red flag.
- **AI-generated case-study text** — repetitive phrasing, clichés, no personal failures or messiness, suspiciously smooth/generic; can't fake the small operational details of a real project.
- **AI-generated imagery** — malformed UI, nonsensical microcopy, garbled text in screenshots.
- **Plagiarism** — same work on multiple unrelated portfolios; reverse-image-search hits; mirrors a known template's structure. When in doubt, reverse-image-search hero shots and search distinctive sentences; check Archive.org / live URLs.

### The line: healthy self-promotion vs. dishonest padding

Subjective opinion you can't be fact-checked on is fine ("results-driven"); specific factual claims must be true and defensible. Two litmus tests: the **laugh test** ("would your old boss laugh if they saw this?") and the **defensibility test** ("can you prove it if asked?"). Framing your role in a team win with "co-led"/"helped" + a defined slice is honest; claiming sole credit for work you didn't drive is not.

---

## 5. Verdict criteria

Map evidence to a verdict. Score behaviors *at the target level*, not raw talent — a brilliant designer who can't yet operate in ambiguity is a strong Senior, not a Staff.

| Verdict | Meaning | Pattern |
|---|---|---|
| **STRONG YES** | Advance, prioritize | Clear problem framing + visible decisions/tradeoffs + shipped, credibly-measured outcomes + unambiguous ownership + craft at level. Few or no authenticity flags. |
| **YES** | Advance | Solid evidence of thinking and outcomes; minor gaps (e.g., one thin metric, slightly narrow scope) that interviews can resolve. |
| **LEAN NO** | Likely pass; advance only if pipeline is thin | Real strengths but material gaps: outcomes mostly absent, ownership ambiguous, or a cluster of authenticity flags needing verification. Decide via the open questions in [§7](#7-legitimacy-vetting-question-bank). |
| **NO** | Pass | Renderer (craft, no thinking), or padder (claims won't survive questioning), or wrong-level/wrong-fit, or stacked authenticity red flags. |

**Decisive disqualifiers** (push toward NO regardless of polish): can't be placed at all after a full review; only fantasy redesigns with no real constraints (for non-junior roles); pervasive "we" with zero "I"; metrics fabricated (worse than absent); plagiarism/originality concerns; portfolio claims contradicted by resume/LinkedIn.

**Level-calibration quick guide:** Junior → judge craft + learnability, don't penalize limited scope/concept work; look for *potential* and self-awareness. Mid → expect end-to-end execution and a sharpening specialty. Senior/Staff → expect strategy, real constraints, cross-team influence, measurable impact; the frame shifts from "what I designed" to "what I made possible." Weak metrics or pure-visual work is disqualifying at senior+.

---

## 6. Per-candidate output template

Use this structure for each candidate so reviews are comparable and defensible.

```
### [Candidate name] — [target role/level]
Links: [portfolio] · [resume] · [LinkedIn]   | Confidence: [High/Med/Low + why]

VERDICT: [STRONG YES / YES / LEAN NO / NO]
One-line rationale: […]

SUMMARY BY CATEGORY
- Role fit & specialty:   [product / UX / UI / research / systems / design-eng]
- Inferred level:         [junior/mid/senior/staff] + evidence
- Craft (1–5):            [score] — [hierarchy, type, spacing, polish]
- Product thinking (1–5): [score] — [problem framing, business connection]
- Process (1–5):          [score] — [decisions, tradeoffs, iteration shown?]
- Outcomes (1–5):         [score] — [shipped? measured? credible?]
- Ownership:              [Clear "I" / Mixed / "we"-ambiguous]
- Work realism:           [Shipped / Client-real / Concept / Coursework per project]

AUTHENTICITY
- Metrics:        [Credible / Vague / Suspect — with examples]
- Flags:          [dribbble-bait / AI-text / template / plagiarism / cross-source mismatch / none]
- Cross-check:    [resume↔portfolio↔LinkedIn: Aligned / Minor gaps / Material discrepancy]

EVIDENCE (observed)      → [bullets]
CONCERNS / RISKS         → [bullets, each tied to a verification question]

IF ADVANCING → Vetting questions: [3–5 tailored to this candidate's boldest/most-suspect claims]
IF PASSING   → Feedback: [1–2 specific, actionable growth areas + suggested next step]
```

End the batch with a **ranked shortlist** (Strong Yes → Yes → Lean No), each with its one-line rationale.

---

## 7. Legitimacy vetting question bank

For candidates who advance. **Depth is the lie detector:** a real owner answers "why" and "how" three or four levels down — they know the baseline, the instrumentation, the dissenting stakeholder's name. A padder gets *vaguer* and more "we"-heavy exactly when you push for specifics.

**Two universal techniques:**
1. **The "why" ladder** — ask why a decision was made, then why that, then why that.
2. **The questioning funnel** — broad → narrow → verification ("So the baseline was 4.2% and it went to 6.1% over six weeks — is that right?"). Re-approach the same fact later; inconsistency surfaces.

### By claim type

**A claimed metric ("increased conversion 23%")**
- "How exactly did you measure that? What was the metric defined as?"
- "What was the **baseline** before your change?"
- "How was it **instrumented** — what tool, what event, what dashboard?"
- "Who ran the analysis? Did you see the raw query?"
- "Over what time window? Statistically significant, or a small-sample read?"
- "How do you know *your design* caused it and not seasonality / a pricing change / a parallel launch?"
- *Strong:* knows definition, baseline, tool, owner, confidence; flags confounders; comfortable saying "I can't attribute it to my work alone." *Weak:* round numbers, no baseline, "the PM told me," number drifts when re-asked.

**A claimed research study**
- "How did you **recruit and screen** participants? What was the screener?"
- "How many, and how did you decide that was enough?"
- "Moderated or unmoderated? What tool? Who wrote the discussion guide?"
- "What finding **surprised you** or contradicted your hypothesis?"
- "Which finding did the team disagree with or ignore, and why?"
- *Strong:* names recruiting source, sample rationale, a disconfirming finding, the messy fielding reality. *Weak:* "we talked to some users," every finding conveniently confirmed the design.

**A claimed design system**
- "What did it look like before you? What did *you* specifically add?"
- "How many components, and how did you decide what belonged?"
- "What was your **adoption / coverage rate**, and how did you measure it?"
- "What was the **governance model** — contribution, approval, versioning, breaking changes?"
- "How did you get engineers to actually adopt it? What about the team that refused?"
- *Strong:* distinguishes their contribution, knows adoption numbers, owns the adoption struggle. *Weak:* "I made the components," no metric, no governance answer, claims to have "built" something that predated them.

**A claimed "led / owned" project**
- "What does 'led' mean here — how many people, which decisions were **yours** vs. needed sign-off?"
- "Tell me about the **invisible work** — research, tech debt, org politics you navigated."
- "Who else was critical to shipping this, and what did they do?"
- "What would have failed if you'd been out sick for a month?"
- *Strong:* precise about authority, credits collaborators while owning their decisions. *Weak:* "I led the whole thing" but can't describe one hard call; never names anyone (or blames everyone).

**A claimed cross-functional win**
- "Who was your PM and eng lead? What did each push back on?"
- "What did engineering say was impossible, and what did you do?"
- "What did you cut for scope, and who made that call?"
- *Strong:* real names of friction and resolution, genuine give-and-take. *Weak:* frictionless fairy tale, no disagreement, takes credit for the PM's strategy.

### Universal forcing functions
- **"Switch from 'we' to 'I'."** "What did *you personally* decide and do?" (highest-yield single intervention)
- **Demand the tradeoff.** "What did you give up to get that?"
- **Ask for the failure.** "What would you do differently?" (Inability to name any failure while bragging is itself a flag.)
- **Go one level past where they stop.** Genuine experience keeps producing detail; embellishment produces filler.
- **Off-script screen.** In a portfolio walkthrough, pick a secondary screen they're *not* prepared to present and ask them to walk through it cold.
- **Live app critique.** "Critique this product — what works, what doesn't, and *why*? What metric is this team optimizing for, and how can you tell from the UI?" Tests current thinking, not a rehearsed story.

### Conversational legit vs. bluffing

| Legit | Bluffing |
|---|---|
| Goes **deeper** the more you push | Gets **vaguer/more abstract** under pressure |
| Volunteers specifics: names, dates, tools, numbers | Generalities, buzzwords, "leveraged a user-centered approach" |
| Admits failures and tradeoffs | Can't name a single failure; brags throughout |
| Cleanly separates "I" from "we"; credits collaborators by name | Hides in "we," or claims literally everything |
| Consistent when a fact is re-approached | Story shifts; numbers drift |
| Explains *why* a decision worked | Describes *what* happened but not the causal logic |

*(Treat nonverbal "tells" like face-touching as unreliable — lean on content consistency and depth.)*

### Reference / backchannel verification
Go in with **targeted** questions confirming specific claims: "[Candidate] said they led the [X] redesign and it lifted conversion ~23% — does that match, and what was their role?" · "Who else was on that project, how would you split the credit?" · "Was [candidate] a driver/leader or an IC on that work?" *Red flag:* reference downgrades the role ("they supported that; [other person] led it") or can't confirm the headline metric.

---

## 8. Rejection feedback & growth guidance

For candidates you pass on. The best rejection feedback is **fast, specific, evidence-based, framed as "missing evidence of X" (not personal deficiency), tied to job-related criteria, and paired with 1–2 concrete next steps.** That combination is simultaneously the kindest, the most useful, and the most legally defensible.

**Principles:** Close the loop in 3–5 business days (24–48h + a call for final-round candidates). Structure: thank sincerely → state the decision → 1–2 genuine specific strengths → 1–2 specific job-related growth areas → make each actionable → encouraging close. Keep to ~2 growth areas (a wall of criticism reads as justification). Ground everything in what they actually said or did.

### Reframe: "missing evidence," not personal criticism

| Instead of (personal/risky) | Say (evidence-based) |
|---|---|
| "You're not strategic." | "I didn't see enough evidence of how you connect design decisions to business outcomes — a key signal for this role." |
| "Your portfolio was weak." | "Strong final screens, but I couldn't see the decisions and tradeoffs behind them, so I couldn't assess your process." |
| "You're too junior." | "We needed someone who's independently owned ambiguous 0→1 problems; your examples were strong but scoped within a defined brief." |
| "You didn't seem confident." | "On the checkout project the answer stayed at the 'what' rather than the 'why' — I was looking for the reasoning behind the call." |

### Legal/ethical guardrails
Only job-related, behavioral factors. **Never** reference or imply a protected characteristic (race, sex, age, religion, national origin, disability, family/marital status, pregnancy, health). Avoid coded language — "not a culture fit," "didn't seem energetic," "overqualified," "wanted someone younger" all carry bias/discrimination risk; replace with a specific job-related behavior. Apply the same rubric to everyone. **Practical rule: if you wouldn't write it in the debrief scorecard, don't say it to the candidate.**

### Reusable templates by reason

**Strong craft, process not visible**
> "Thank you for sharing your work — your visual craft really stood out, especially on [project]. For this role we wanted more visibility into the *thinking* behind the screens: the tradeoffs you weighed and why you chose one direction. As a next step, I'd pick one case study and walk through 2–3 key decision points and the reasoning. That would make a strong portfolio even stronger."

**No measurable impact**
> "We appreciated the time you put into [project] — clean designs, clear problem framing. The main gap for us was evidence of impact: what changed for users or the business after launch. Adding outcomes (a metric, a usability result, or adoption) would make the strength of your work much more visible."

**Spec/fantasy projects only**
> "Your concept work shows real creativity and craft. For this role we needed more evidence of designing within real constraints — users, stakeholders, technical limits, deadlines. A great next step would be one project with real-world constraints (freelance, volunteer, or a small shipped feature), which would show the judgment side alongside the craft that's clearly there."

**Breadth without depth (esp. senior)**
> "You've clearly worked across a lot of surfaces. For this role we were looking for deeper evidence of owning an ambiguous problem end-to-end and driving it to a measurable outcome. Picking one domain to go truly deep on would strengthen your senior story. We'd genuinely welcome a future application as that depth becomes visible."

**Strong portfolio, weaker walkthrough**
> "The portfolio itself is strong. In the conversation we were looking for more of the *story* — the problem, your specific role, the tradeoffs, what you'd do differently. Practicing a tight narrative (context → problem → your decisions → outcome → reflection) for your top two projects would make the work land even harder."

**Close call, role-fit gap (not a skill gap)**
> "This was a genuinely difficult decision. Your skills and portfolio were strong. We moved forward with a candidate whose experience is a closer match for [specific role need, e.g. shipping in a regulated/0→1/design-system context] — this was about fit to this role's immediate needs, not a reflection of your ability. We'd be glad to see you apply again."

### What to advise designers to do next (by level)
- **Junior:** build 2–3 mentor-reviewed case studies; show *thinking over polish* (why a layout, how it was validated, what was learned); lock down Figma fluency; label hypothetical work but add realistic constraints.
- **Mid:** push toward autonomy (own a full project, make ownership explicit); add metrics and business framing; develop depth in one domain.
- **Senior+:** lead with business impact and measurable outcomes (not screens); demonstrate strategy, influence, and storytelling; show real numbers, real failures, real tradeoffs.

### Weakness → the one next step that fixes it

| Weakness | Next step |
|---|---|
| No process shown | Annotate 2–3 decision forks with the "why" in one case study |
| No outcomes | Add a metric or qualitative result + how you'd measure it |
| Weak structure | Reorder to context → problem → role → decisions → outcome → reflection; front-load strongest signal |
| Weak craft | Audit spacing/type/alignment/component reuse for consistency |
| Fantasy projects | Add one real-constraint project; label hypotheticals |
| Breadth, no depth | Triple-deep your best case study; pick a domain |
| Vague resume bullets | Strong verb + action + measurable outcome |
| Missing ownership | State your specific role: observed / assisted / executed / led |
| Weak interview storytelling | Rehearse a tight narrative for top 2 projects |

---

## 9. The batch workflow (end to end)

1. **Intake** — collect each candidate's portfolio URL, resume, LinkedIn; note the target role/level.
2. **Triage** ([§1](#1-the-triage-mindset)) — run the 5 tiers; drop hard fails early with a one-line reason.
3. **Deep analysis** — for survivors, run the portfolio ([§2](#2-portfolio-analysis-protocol)) and resume ([§3](#3-resume-analysis-protocol)) protocols.
4. **Authenticity pass** ([§4](#4-authenticity--fraud-detection)) — tag metrics, scan for padding/AI/plagiarism, cross-check sources. Cluster the flags.
5. **Verdict** ([§5](#5-verdict-criteria)) — assign STRONG YES / YES / LEAN NO / NO with evidence-based reasons.
6. **Output** ([§6](#6-per-candidate-output-template)) — fill the per-candidate template; generate vetting questions (advancing) or feedback (passing).
7. **Shortlist** — rank all candidates; surface the open questions that would change a LEAN NO into a YES.
8. **Always state confidence** — if a site was inaccessible, a resume was thin, or claims couldn't be cross-checked, say so rather than guessing.

> **Remember:** advancing a candidate isn't a conclusion — it's a hypothesis to verify in the interview. The vetting questions exist to confirm the boldest claims are real before an offer. And every "pass" is a chance to leave a designer better than you found them.

---

*Companion to [`hiring-world-class-designers.md`](./hiring-world-class-designers.md). Compiled from a multi-agent research synthesis across portfolio-analysis methodology, resume authenticity/fraud detection, legitimacy vetting techniques, and rejection-feedback best practices (NN/g, Indeed Design, Dribbble, Holloway, HubSpot, Sourcegraph, Aquent, CCL/SBI, Radical Candor, EEOC/SHRM, CareerBuilder, HireRight, and others). Several primary sources block automated fetching; findings were corroborated across multiple independent sources. Resume-lie statistics converge across CareerBuilder, HireRight, StandOut CV, and ResumeBuilder; design-portfolio "fraud rate" figures are individual practitioner claims, not survey data.*
