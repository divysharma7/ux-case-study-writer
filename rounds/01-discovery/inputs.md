# Input Checklist for the Discovery-Brief Case Study Skill

This document specifies what the user needs to provide for the skill to produce a portfolio-grade case study brief. The skill is only as good as its inputs. **Generic inputs produce generic output. Specific, researched inputs produce a brief that could not have been written by anyone else.**

There are two tiers of inputs:

- **Mandatory inputs** — without these, the skill will either ask you for them before drafting, or produce a draft with obvious placeholder gaps. Do not skip these.
- **High-value optional inputs** — each one significantly improves a specific section of the brief. The more of these you provide, the closer your output gets to portfolio-grade. Skipping all of them is allowed, but the brief will read more like a template than your team's research.

A fillable template is at the bottom of this document. The recommended workflow is to fill out the template, paste it into your conversation with Claude, and then invoke the skill.

---

## Why this matters (read once, then never again)

The original Team Dua brief works because every page is loaded with **specifics only that team could provide** — the psychologist's name and dual identity, the exact 5 stages of their emotional arc, the specific Indian sources, the precise scope of "early stages of motherhood." Those specifics are what separate a portfolio piece from a generic chatbot summary.

When you skip the inputs, Claude has two options: refuse to draft (which slows you down), or fill the gaps with plausible-sounding generic content (which produces a brief that fails the scoring benchmark, especially on Evidence Rigor and Synthesis Sharpness). Neither outcome is what you want.

Treat this checklist as a 30-minute investment that saves you 3 hours of revision later.

---

## Mandatory inputs

### 1. Topic / problem domain

**What:** The broad field you are investigating, in one sentence.

**Example:** "Wellbeing of working women in India, with an early lean toward work-life balance for new mothers."

**Why it matters:** This sets the funnel's top level. Without it, the Introduction can't write itself, and the Global Scenario doesn't know which world-scale problem to anchor on.

**Common mistake:** Stating a solution instead of a problem ("an app for childcare scheduling"). State the *problem*, not the *answer*.

---

### 2. Target user (sharply defined, ideally a life phase)

**What:** Who specifically is affected. The sharpest version is a **role + life phase**, not just a role.

**Example:**
- ❌ "Working women" (too broad — what life phase?)
- ❌ "Working women in Mumbai aged 28–34 with infants" (too narrow — reads like a market segment, not a research subject)
- ✅ "Working women in the early stages of motherhood" (role + life phase — broad enough to generalize, sharp enough to scope)

**Why it matters:** The HMW question on Page 4 will be built from this. The sharpness of the HMW depends entirely on the sharpness of this input. The emotional arc on Page 3 will plot *this person's* journey.

**Common mistake:** Picking a demographic (age, income, geography) instead of a life-phase. Life-phase is what generates an emotional arc.

---

### 3. Geography / regional context

**What:** Where this plays out. Usually a country, sometimes a region or city, occasionally a non-geographic context (e.g., "the gig economy," "the remote-first workforce").

**Example:** "India, with particular attention to urban nuclear families."

**Why it matters:** Page 2's "[National / Regional] Perspective" section is built around this. The comparative framing ("While developed countries… India is still struggling") needs a specific geography.

**Common mistake:** Picking a geography you can't research credibly. If you don't have access to sources from that geography, the brief's Evidence Rigor will fail.

---

### 4. Team name + member names for the credit line

**What:** The name of your team and the full names of all members.

**Example:** "Team Dua: Arya Bhushan, Avni Agarwal, Devanshi Kataria, Urvi Suhane"

**Why it matters:** Appears at the bottom of Page 4 in italics. Without it, you get a `[YOUR TEAM]` placeholder, which you'll forget to fill in before sharing.

---

### 5. Research methodology summary

**What:** A 2–4 sentence summary of the research you actually conducted. Specifically:
- What desk research did you do? (Reports, studies, articles)
- Who did you interview, and how many? (Roles, not necessarily names)
- Did you do any exploratory brainstorming or workshops?

**Example:** "We did desk research across FSG, McKinsey, and government reports. We interviewed 6 working mothers (3 currently working, 3 who left jobs), 2 children of working mothers (ages 8 and 14), and one practicing psychologist who is also a mother."

**Why it matters:** This sentence becomes the Introduction's "we conducted…" beat and the Interview Insights' opener. Without it, Claude cannot make methodology-as-narrative work, and may either invent a methodology or default to a labeled "Methodology" section (which breaks the style).

**Common mistake:** Saying "we did research" without specifying what kind. The triangulation of sources is what makes the methodology credible.

---

### 6. At least one strong interview quote with attribution

**What:** One direct quote from your interviews, 1–2 sentences, with the speaker's name and their **dual identity** if applicable (e.g., "A Psychologist & A Mother").

**Example:** "People need to understand that she is a human before she's a mother. A woman's needs are always neglected, she's never a human being and always has a role to play. — Shikha Handa, A Psychologist & A Mother"

**Why it matters:** The pull quote on Page 2 is one of the most visually and emotionally weighty elements in the brief. Without a real quote, you'll get a placeholder or — worse — a fabricated quote, which is a research integrity violation and obvious to readers who know the style.

**Common mistake:** Providing a paraphrase instead of a verbatim quote. The quote must be word-for-word from the interview transcript.

---

## High-value optional inputs

Each of these strengthens a specific section. Provide as many as you can.

### 7. The story of why your team chose this problem

**What:** 2–3 sentences on what made your team narrow from a broad field (e.g., "wellbeing") to a specific problem (e.g., "working mothers' work-life balance"). Was it a personal connection? An interview that surprised you? A statistic that wouldn't leave you alone?

**Why it matters:** The Introduction's origin story has more authenticity when the team's actual narrowing path is captured. Without this, the Introduction defaults to a generic "we explored X and found Y."

**Example:** "Two of our team members have working mothers. When we started interviewing women about wellbeing, we kept hearing the same story about the postpartum return-to-work moment — and realized none of us had ever seen this discussed in our design coursework."

---

### 8. Three distinct interview insights covering the three flavors

**What:** Three short observations from your interviews, each in one of three categories:
- **Operational / practical** — a time, logistics, or daily-execution struggle
- **Relational / social** — a struggle that involves another person or social expectation
- **Emotional / internal** — a feeling or psychological state

Each insight should name a 2–4 word **key concept** that can be bolded.

**Example:**
- Operational: They face **time management** challenges balancing job demands and family.
- Relational: Husbands are supportive but believe **childcare is primarily the woman's responsibility**.
- Emotional: They report high levels of **stress and guilt** from meeting both sets of expectations.

**Why it matters:** Page 2's three insight blocks are built from this. If you only give Claude one or two themes, or all three themes are in the same flavor (e.g., all operational), the trio coverage breaks and the section reads one-dimensional.

---

### 9. The five journey stages with key touchpoints

**What:** Five chronological life-phase labels for your target user, plus 1–3 key moments or feelings at each stage.

**Example:**
- Stage 1: Pregnancy → "Gets pregnant," "Difficulties during pregnancy"
- Stage 2: Maternity Leave → "Works till third trimester," "No proper policies"
- Stage 3: Return to the Job → "Has to return after 6 months," "Gives quitting a thought"
- Stage 4: Finding Child Care → "Unavailability of credible options," "Settles for unsatisfactory"
- Stage 5: Career Challenges → "Triggered by child struggling," "Eventually leaves"

**Why it matters:** Page 3 (the emotional arc) is built from this. Without it, Claude will either invent stages (risky) or default to generic phases that don't reflect your interview research.

---

### 10. Trajectory shape preference for the emotional arc

**What:** Which shape does your user's emotional journey take? Options:
- **Descending zigzag** — emotional highs followed by deeper lows, ending below where they started (system fails through accumulated friction; Team Dua's original choice)
- **Ascending zigzag** — obstacles overcome over time, ending above where they started (resilience story)
- **U-shape** — gets worse before getting better (turning-point story)
- **Flat with sharp drop** — a single shock event reshapes everything (acute trauma story)

**Why it matters:** The shape is an argument. A descending zigzag implicitly argues "the system fails the user." An ascending zigzag implicitly argues "the user finds their way despite the system." Choose the one your research actually supports.

---

### 11. Framework + focus dimensions for Page 4

**What:** Which structured framework will you reference, and which 1–2 dimensions will you focus on?

**Default framework:** 6 dimensions of wellbeing (Physical, Emotional, Environmental, Social, Financial, Occupational).

**Alternatives** (use one if it fits your problem better):
- Maslow's hierarchy of needs (5 levels)
- Service ecosystem layers (people, processes, channels, products)
- Capability dimensions (knowing, being, relating, doing)
- A custom 5–7 dimension framework specific to your domain

**Example:** "Wellbeing framework. Focus on Emotional + Occupational. Ripple expected on Social and Physical."

**Why it matters:** Page 4's "Types of Wellbeing Affected" section needs a clear, named framework. If you don't provide one, Claude defaults to the wellbeing radar, which may not fit your problem.

---

### 12. Draft HMW question (or your team's hunch toward one)

**What:** Your current best draft of the How-Might-We question, even if it's rough. Or a sentence describing what you want the brief to point toward.

**Example:** "How might we help working women in early stages of motherhood attain a sustainable work-life balance?"

**Why it matters:** Claude can refine an HMW you provide. If you don't provide one, Claude will generate one — and you may end up with an HMW that doesn't match what your team actually researched.

---

### 13. The "why now" structural shift for Page 4

**What:** A societal, technological, or structural change that makes your problem more urgent today than 10 years ago. One sentence.

**Example:** "Nuclear families are rapidly replacing joint families in urban India, eliminating the support systems that previously absorbed childcare load."

**Why it matters:** The paragraph below the HMW on Page 4 needs to explain *why now*. Without this input, that paragraph reads as filler.

---

### 14. Three opportunity area sketches

**What:** Three rough directions where intervention could happen. **Directions, not products.** Each at a different systemic layer if possible (policy / community / infrastructure).

**Example:**
- "Modifying existing work policies" (policy layer)
- "Providing support within community" (community layer)
- "Improving childcare facilities" (infrastructure layer)

**Why it matters:** Page 4's "Opportunities Identified" branches from these. If you skip this input, Claude will infer opportunities from the rest of your research — usually competently, but you may find they're not the directions your team actually wants to pursue in Round 2.

---

### 15. Pre-found statistics with citations

**What:** Any stats your team has already found, with the source you'd cite. Particularly valuable for region-specific or sub-group-specific numbers that Claude's web search might miss.

**Example:**
- "58% of women employees in India quit due to family responsibilities in last two years. Source: Business Insider"
- "80% of new mothers not working cited child responsibility. Source: FSG GLOW report 'Creating a Gender-Equitable Workforce in India'"

**Why it matters:** Claude will do its own research, but your interview-adjacent stats are often more relevant than what a web search surfaces. Providing them improves Evidence Rigor.

---

### 16. Visual style preferences

**What:** Any specific visual choices you want to lock in. Optional dimensions:
- Color palette (e.g., "warm coral and cream, like the original Team Dua brief")
- Iconography style (e.g., "line-art, single weight, rounded corners")
- Layout density (e.g., "two columns, generous whitespace")
- Specific charts you want or don't want

**Why it matters:** The skill outputs a content + layout spec, not a designed PDF. But the "Visual elements to design" callouts in each section will be more useful if Claude knows your visual direction.

---

## How to gather these inputs (practical tips)

**For the interview quote:** Pull your raw interview transcripts and re-read them. Look for the 3–4 sentences that made you stop and re-read. That's your candidate quote.

**For the three insight themes:** Before invoking the skill, do a quick affinity sort of your interview notes. Cluster observations into three buckets (operational / relational / emotional). The dominant theme in each bucket becomes your insight.

**For the emotional arc stages:** Map the timeline of your target user's life. Identify the 5 most distinct phases. For each, list the 2–3 most emotionally significant moments you heard about in interviews.

**For the framework + focus dimensions:** Ask yourself, "If I had to limit my Round 2 solution space to 2 dimensions of impact, which 2 would they be?" Those become your focus dimensions.

**For pre-found statistics:** Keep a running doc during your research phase where you log every statistic you find with its source. By the time you invoke this skill, you should have 8–15 cited stats to choose from.

---

## Fillable template

Copy this template, fill it out, and paste it into your conversation with Claude before invoking the skill.

```
## Discovery-Brief Inputs

### MANDATORY

**1. Topic / problem domain:**
[1 sentence]

**2. Target user (role + life phase):**
[1 sentence]

**3. Geography / regional context:**
[1 sentence]

**4. Team name + members:**
Team [Name]: [Member 1], [Member 2], [Member 3], [Member 4]

**5. Research methodology summary:**
[2-4 sentences covering desk research + interviews + any other methods]

**6. Strong interview quote with attribution:**
"[Verbatim quote here]"
— [Speaker name], [Dual identity / role]

### HIGH-VALUE OPTIONAL

**7. Why your team chose this problem:**
[2-3 sentences]

**8. Three interview insights (operational + relational + emotional):**
- Operational: [Sentence with bolded **key concept**]
- Relational: [Sentence with bolded **key concept**]
- Emotional: [Sentence with bolded **key concept**]

**9. Five journey stages with touchpoints:**
- Stage 1: [Phase name] → [Key moments]
- Stage 2: [Phase name] → [Key moments]
- Stage 3: [Phase name] → [Key moments]
- Stage 4: [Phase name] → [Key moments]
- Stage 5: [Phase name] → [Key moments]

**10. Trajectory shape:**
[Descending zigzag / Ascending zigzag / U-shape / Flat with sharp drop]

**11. Framework + focus dimensions:**
Framework: [Name]
Focus on: [2 dimensions]
Ripple expected on: [Other dimensions]

**12. Draft HMW question:**
How might we help [SHARPLY SCOPED USER IN A LIFE PHASE] [SOFT VERB] [ASPIRATIONAL OUTCOME WITH ENDURANCE WORD]?

**13. "Why now" structural shift:**
[1 sentence]

**14. Three opportunity area sketches:**
- Policy-layer direction: [4-7 words]
- Community-layer direction: [4-7 words]
- Infrastructure-layer direction: [4-7 words]

**15. Pre-found statistics:**
- [Stat 1] — Source: [Citation]
- [Stat 2] — Source: [Citation]
- [Stat 3] — Source: [Citation]

**16. Visual style preferences:**
[Palette, iconography, layout notes]
```

---

## Common input mistakes (read before submitting)

1. **Target user is a demographic, not a life phase.** "Women aged 25–40 in Tier 1 cities" vs. "Women in the early stages of motherhood." Life phases generate emotional arcs; demographics generate market segments.

2. **No real research underneath.** You're asking the skill to do all the work. The skill can do real web research, but it cannot replace your team's interviews. Without your interview-grounded inputs (quote, themes, journey stages), the brief will pass a casual reading but fail any reviewer who's done research themselves.

3. **The HMW is a solution in disguise.** "How might we build a childcare-coordination app for working mothers?" is a product spec wearing a question mark. Strip out the solution. The HMW names the *gap*, not the *fix*.

4. **Generic theme list.** "They face challenges with time, family, and work" is one theme repeated three times, not three themes. Each theme should be in a different flavor (operational / relational / emotional) and name a distinct concept.

5. **Pre-found statistics without sources.** "73% of women feel guilty" with no citation is unusable. If you can't name the source, the stat doesn't go into the brief.

6. **Trajectory shape doesn't match the research.** You pick a descending zigzag because the original used one, but your interviews actually told a U-shape story. The shape is an argument — pick the one your data supports.

7. **No team credit line.** You forget to provide names. The brief outputs with a `[YOUR TEAM]` placeholder you may forget to fix before sharing.

---

## What happens at each input quality level

To set expectations:

- **Mandatory inputs only:** You get a competent draft with generic-feeling Page 3 (emotional arc) and Page 4 (synthesis). The brief will pass the Scoring Benchmark on AI-Likeness and Funnel Discipline but may fall short on Evidence Rigor (because Claude has to research most stats) and Synthesis Sharpness (because the HMW and opportunities are inferred, not your team's).

- **Mandatory + half the optional inputs:** You get a strong draft that mostly hits the Scoring Benchmark targets. Some sections will feel more "yours" than others.

- **All inputs filled in:** You get a portfolio-grade draft where every page reflects your team's specific research. The Scoring Benchmark targets should all be met on the first pass. Most of your revision time goes into voice tuning and visual design, not content correction.

The 30 minutes you spend on this checklist is the single highest-leverage investment in the brief's final quality.
