---
name: empathy-deepening-brief-case-study
description: Write a research-deepening case study brief (Round 2 / "Empathize 2.0" phase) in the Team Dua style — a 5-page service-design brief that takes a sharply scoped HMW problem statement from Round 1 and expands it back into a full ecosystem map, problem space, day-level empathy artifact, and multiple personas. Use whenever the user wants to produce the second-round / deeper-research deliverable of a service design or UX case study, an ecosystem map, a stakeholder map, a problem space mind-map, an experience map (day-in-the-life), user personas with deliberate contrast, an existing-solutions landscape audit, or an "assumptions invalidated" section. Trigger this even when the user just says "write my Round 2", "build the empathy deep dive", "do the persona pages", "expand my problem space", "stakeholder mapping for my case study" — this skill is the Round 2 companion to the discovery-brief-case-study skill and should be consulted whenever such a brief is being authored, even if the user does not name a specific design-thinking phase. Requires that a Round 1 HMW question already exists.
---

# Empathy-Deepening Brief Case Study (Team Dua style, Round 2)

This skill produces a 5-page deeper-research brief in the visual and narrative style of the "Team Dua" working-mothers case study, Round 2. It is the **Empathize 2.0** / **Research Synthesis** phase of a service-design project — the deliverable that takes the reader from "here is the problem we defined" to "here is the entire ecosystem, stakeholder network, problem space, daily reality, and persona variation that this problem lives inside."

It is the companion skill to `discovery-brief-case-study` (Round 1). Round 1 narrowed from global context to a sharp HMW question; Round 2 takes that HMW and **opens it back up** into a comprehensive problem space.

The output is a **content + layout specification**. Claude writes the prose, stakeholder quotes, problem-space inventory, experience map content, persona cards, and assumptions-invalidated content, and specifies the visual elements needed (concentric circles, radial mind-map, multi-layer swim lanes, persona templates). The user takes that spec into Figma, Canva, InDesign, or similar to produce the final designed PDF.

---

## When to use this skill

Use this skill when the user asks for:

- A Round 2 / Phase 2 / Empathize-deepening case study deliverable
- A continuation of an existing Round 1 discovery brief
- An ecosystem or stakeholder map for a service-design project
- A day-in-the-life experience map with bodystorming evidence
- Contrasting user personas
- A problem-space mind-map
- An existing-solutions / landscape audit
- An "assumptions invalidated" section

**Do not use this skill if there is no Round 1 HMW.** The expansion logic of Round 2 only works if there's a sharp problem statement to expand from. If the user hasn't completed a Round 1, suggest they use the `discovery-brief-case-study` skill first.

---

## The core mental model: the Expansion (not the Funnel)

Round 1's pattern was the **Funnel** — global context narrowing to one sharp HMW question. Round 2's pattern is the **Expansion** — taking that HMW and opening it back up along multiple axes to demonstrate that the team has thoroughly mapped the problem space before attempting solutions.

The expansion happens along six axes:

1. **Contextual expansion** — adding cultural depth and an audit of solutions that already exist
2. **Relational expansion** — mapping every stakeholder, not just the user
3. **Problematic expansion** — exploding the single problem into all its sub-problems
4. **Temporal-micro expansion** — zooming from life-stages (Round 1's arc) into a single day with multi-layer detail
5. **Persona expansion** — revealing that the user has multiple faces along a deliberate contrast axis
6. **Epistemic expansion** — naming and invalidating the team's own initial assumptions

The structural argument the brief makes is: "We have a sharply scoped problem. Now we demonstrate that we've mapped the entire ecosystem this problem lives inside before attempting any solutions."

If your draft doesn't visibly expand along these six axes, the round isn't doing its job. Re-check before finalizing.

---

## Continuity with Round 1

Before drafting, verify the following carry over cleanly from Round 1:

- The HMW question is unchanged (or only sharpened, never pivoted to a different topic)
- The target user is the same (any narrowing is OK; pivoting is not)
- The geography is the same
- The team name and members are the same
- The visual palette and design language are the same

Round 2 should feel like the same team's continued work, not a new project. If the user wants to pivot the user/topic mid-project, that's a Round 1 redo, not a Round 2.

---

## Document anatomy (5 pages)

| Page | Sections | Job to be done |
|------|----------|----------------|
| 1 | National/Regional Scenario (revisited) + Cultural Scenario + Existing Services + Other Policies and Services | Contextual expansion: add cultural depth, audit what already exists, name the gaps |
| 2 | Stakeholder Map + What Stakeholders Said | Relational expansion: reveal the user sits inside an ecosystem of 15–25 stakeholders; collect 5 quotes from 5 distinct roles |
| 3 | Problem Mapping | Problematic expansion: explode the problem into 5–8 primary branches with 3–8 sub-issues each |
| 4 | Experience Map | Temporal-micro expansion: a day-in-the-life with 4 content layers + bodystorming evidence |
| 5 | Two Personas + Discoveries + Assumptions Invalidated | Persona expansion + epistemic expansion: contrasting personas + statistical surprises + invalidated assumptions |

Section names can be adapted to the problem (e.g., "The Indian Scenario" → "The Urban Indian Scenario"), but the **functional role** of each section must remain.

---

## Section-by-section writing playbook

### Page 1, Section 1: The [National/Regional] Scenario (revisited)

**Function:** Re-enter the context from Round 1, but with a NEW lens — usually a filtration/attrition visualization showing the user dropping out of opportunities or roles at multiple stages of life. Then widen to acknowledge an intersectional sub-population.

**Length:** 60–100 words across two paragraphs + 1 filtration funnel visualization.

**Structure:**
- **Paragraph 1:** Name the filtration phenomenon. Use a bolded key phrase like "drop out at multiple stages" or "filtration process." 2–3 sentences.
- **The filtration funnel visualization:** A vertical inverted funnel showing population narrowing through life stages. Each stage labeled. For working women: School Students → University → University Students → Employment → Employed → Continue work after Marriage → Continue work after Children → Pregnancy. For other problems, derive the analogous attrition stages.
- **Paragraph 2:** Widen to acknowledge an **intersectional sub-population** that experiences this filtration more harshly. The original brief names "the informal sector, such as farmers or agricultural laborers." This is a deliberate move that prevents the case study from being only about middle-class users. 2–3 sentences with bolded key phrases (e.g., **underprivileged girls**, **shoulder the burden of care**).
- **Sources cited** below the section (e.g., ASER 2022, Grant Thornton Women in Business 2021).

The intersectional widening is a critical move. Without it, the brief reads as if the team is only studying privileged users.

### Page 1, Section 2: Cultural Scenario

**Function:** Surface the cultural norms and scripts that compound the problem. This depth was not in Round 1's scope.

**Length:** 50–80 words of prose + 1 pull quote with dual-identity attribution.

**Structure:**
- **One paragraph** identifying 2–3 cultural scripts with bolded key phrases. The scripts should name *socialized beliefs*, not biology. Examples of bolded patterns:
  - "**after marriage**" (timing expectation)
  - "**extended family members get involved in childcare**" (joint-family complication)
  - "**uncommon to encounter [exception-case]**" (gender-role rigidity)
- **A pull quote** with dual-identity attribution (a person who is both a domain expert AND a member of the affected group). Format with oversized quotation marks. Different person from the Round 1 pull quote — Round 2 introduces new voices.

The quote should ideally attribute the cultural script to **socialization or conditioning**, not nature. The original's "they have been *seasoned* to believe…" does this work — the word "seasoned" implicates culture, not biology.

### Page 1, Section 3: Existing Services — [Name a Specific Service]

**Function:** Audit a major existing service in the problem space. Show the team did their homework on what already exists, with an honest pros/cons assessment.

**Length:** 1-sentence description + a pros/cons table.

**Structure:**
- **Service name** (heading) — including the local-language name if applicable, e.g., "Anganwadi (आँगनवाडी)"
- **1–2 sentence description** with bolded key terms naming what kind of service it is (e.g., "**government-run childcare facility**", "**preschool-like environment**")
- **A two-column Pros/Cons table:**
  - Pros: 3–5 short labels of what the service actually does well (e.g., "Provide hot meals", "Offer immunizations", "Community engagement", "Play-based education")
  - Cons: 4–6 short labels of where it falls short (e.g., "Underfunded", "Only 10am–1pm", "Poor infrastructure", "Unhygienic conditions", "Poorly trained workers", "Provide minimal services")
- **Source** below (e.g., "Field Visits and Interviews" — signals firsthand investigation, not just desk research)

**This section is the credibility hinge for the rest of the brief.** Without it, any solutions proposed later look ignorant of the existing landscape. With it, the team has earned the right to propose new interventions.

Pick a service the team has *actually investigated* — ideally through a field visit, not just reading about it. The "Source: Field Visits and Interviews" line should be earned, not invented.

### Page 1, Section 4: Other Policies and Services

**Function:** Catalog the broader services landscape, then make the **gap claim** that justifies the need for new intervention.

**Length:** 2 short paragraphs.

**Structure:**
- **Paragraph 1:** Name 3–6 other services or schemes in **bold**, with a 1-sentence purpose-summary of what they collectively aim to do. For the original: "breastfeeding stations, NIPCCD, childcare leaves and centers. Schemes like RGNC, PMSMA, and ICDS offer healthcare, nutrition, and education for working mothers and their children. These aim to promote a work-life balance and improve children's wellbeing." Use real, named schemes only — do not invent acronyms.
- **Paragraph 2:** The gap claim. Use the structural pattern "Despite these initiatives, there are still **gaps in implementation**. Even if the services are implemented properly, they **aren't accessible** to many [USER] because of **geographic and cultural constraints**. This leaves [USER] with limited options to balance their responsibilities." Bolded key phrases: gaps in implementation, aren't accessible, geographic and cultural constraints.

The gap claim is what bridges from "here's what exists" to "here's why we're proposing new work."

### Page 2, Section 1: Who All Are Involved? (Stakeholder Map)

**Function:** A full-page concentric-circle ecosystem diagram revealing that the user sits inside a network of 15–25 stakeholders.

**Length:** A concentric-circle diagram with 3 rings labeled CORE, INVOLVED, INFORMED.

**Structure:**
- **CORE (innermost ring):** 3–5 stakeholders. The direct user + immediate family. For the original: Child, Mother, Spouse, Family (Grandparents, Siblings). For a different problem, identify the analogous "people in the same household / closest relational unit."
- **INVOLVED (middle ring):** 10–15 stakeholders. The active touchpoints — services, professionals, institutions the user interacts with regularly. For the original: Daycare, Anganwadi, Workplace, Healthcare, Caretaker, Nanny, Transport, School, Government, Hospitals, Househelp, Gynecologist, Pediatrician, Psychologist.
- **INFORMED (outermost ring):** 5–7 stakeholders. Peripheral observers — colleagues, neighbors, friends, teachers, extended community.

**Each stakeholder gets a custom line-art icon** (matching Round 1's iconography style — single weight, rounded, figurative).

**The 3-ring distinction matters.** A stakeholder map that just lists everyone in one flat list is not doing structural work. The ring assignment is an argument about who is most affected vs. who is incidental.

### Page 2, Section 2: What Our Stakeholders Said

**Function:** Triangulated voices from 5 distinct stakeholder roles. Where Round 1 had ONE pull quote, Round 2 has 4–6.

**Length:** 4–6 quote blocks.

**Structure of each quote block:**
- **Stakeholder ROLE** (not personal name) — Gynecologist, Pediatrician, Spouse, Child, Caretaker, Employer, etc. The role generalizes the perspective; the personal name would individualize it.
- **An icon** depicting that role (e.g., a doctor figure for Gynecologist, a child figure for Child)
- **A 1–3 sentence quote or paraphrase** in their voice, capturing their specific angle on the problem
- **Oversized quotation marks** for visual treatment

**Triangulation requirement:** The 5+ quotes must come from at least 4 distinct stakeholder *types*. Distribute roughly:
- 1–2 medical/expert voices (Gynecologist, Pediatrician, Psychologist)
- 1–2 family voices from different generations (Spouse, Child, Grandparent)
- 1–2 service-provider voices (Caretaker, Daycare worker, Teacher)
- Optionally: 1 institutional voice (Employer, Government rep)

If all 5 quotes come from the same type of stakeholder, the triangulation is broken and the page fails. Each quote should offer a *different angle* on the problem.

**Important attribution choice:** quotes here are attributed by ROLE, not personal name. This is the opposite of Round 1's pull quote (which had a full name + dual identity). Round 2's quotes are *role-typifying*, Round 1's was *individualized*.

### Page 3: Problem Mapping

**Function:** A full-page radial mind-map that explodes the problem into a comprehensive inventory of sub-issues. Deliberately dense.

**Length:** The full page. One radial diagram.

**Structure:**
- **Center node:** The user (e.g., "Mother" with the local-language label "माँ" if relevant)
- **5–8 primary branches**, each representing a problem category. For the original: Occupational, Financial, Mental Health, Child Personal, Physical Health, Transport.
- **Each primary branch splits into 3–8 sub-problems.** Some sub-problems further split into more specific issues.
- **No prose.** This page is text-as-diagram. Each sub-problem is a short label (1–5 words).

**Density is the argument.** This page should look slightly overwhelming. It's saying "we mapped every aspect of this problem space." A clean, sparse, well-organized version of this page would actually fail — it would suggest the team didn't dig deep enough.

**Drawing from real research:** Every sub-problem should trace back to either desk research, an interview, a field observation, or a bodystorming insight. Do not invent sub-problems to fill space — but also do not over-curate the list. If your interviews surfaced 47 distinct frustrations, list 47 of them across the branches.

**Common primary-branch categories** (adapt to your problem):
- Occupational / Work-related
- Financial / Economic
- Physical Health
- Mental / Emotional Health
- Relational / Social
- Practical / Daily Living
- Infrastructural / Service Gaps
- Cultural / Identity

Pick the 5–8 that fit your problem. The branches don't have to be MECE (mutually exclusive) — some sub-problems may span branches.

### Page 4: Experience Map

**Function:** A day-in-the-life journey map with multiple emotional/cognitive layers + team bodystorming evidence. This is fundamentally different from Round 1's emotional arc.

**Round 1 vs. Round 2 journey artifacts:**
- Round 1's Emotional Arc plots **life stages** (pregnancy → leaves job) over **months/years**
- Round 2's Experience Map plots **time-of-day stages** (wake up → bedtime) over **one day**

**Length:** Full page. One multi-layer swim-lane diagram.

**Structure:**
- **Top caption** (1–2 sentences): "Map of the day in the life of a [USER] to better understand their daily activities, thought process and feelings. Also, conducted a **bodystorming session** to fully empathise with them and know their painpoints." The bodystorming mention is bolded.

- **6 time-of-day stages as columns**, with sun/clock icons indicating time progression:
  - For working mother: Waking Up → Getting Ready → Working → Going Back Home → Household Chores → Going to Sleep
  - For a different user: identify the 6 most distinct phases of *their* day. The stages should match the user's actual rhythm.

- **4 horizontal content layers**:
  1. **Actions** — what they DO at each stage. Concrete, observable verbs. ("preparing dinner, doing dishes, putting the child to sleep")
  2. **Emotions** — an emotion curve plotted across the day with emoji indicators at each stage. The curve should rise and fall — not be monotonic. For the original: it dips during the morning rush, rises slightly during work satisfaction, peaks when reuniting with the child, falls again during evening chores.
  3. **Thoughts** — internal monologue at each stage. Use italicized key words to mark the most charged thoughts (e.g., "*worry* about getting late," "*sense of satisfaction* from working").
  4. **Painpoints** — specific friction points at each stage. Use italicized key words for the sharpest pain (e.g., "*Inadequate* public transport", "*doesn't get time* for herself").

- **A 5th row at the bottom: Empathising (by bodystorming)** — wavy lines for each team member. Each line represents one team member's physical simulation of the user's day. Label each line with the team member's first name in a distinct color. For 4 team members: 4 wavy lines, weaving up and down through the columns to indicate their emotional rhythm during the bodystorming.

**Italicization is the new emphasis tool here.** Round 1 used bold for key phrases. Round 4's experience map uses **italic** for emotionally-charged words inside the Thoughts and Painpoints layers. Use italics sparingly — 1–3 words per cell, the most charged ones.

**The bodystorming row is the credibility move.** Without it, the experience map is theoretical. With it, the team is saying "we physically lived this day."

### Page 5, Section 1: Two Different Worlds (User Persona)

**Function:** Reveal that the user has multiple faces along a deliberate **contrast axis**. Two personas, same template, dramatically different content.

**Length:** Two persona cards side by side.

**Choose a contrast axis** that reveals something meaningful about the problem. Options:
- **Organized vs. unorganized sector** (white-collar vs. blue-collar) — the original's choice. Reveals class-based variation.
- **Urban vs. rural** — reveals infrastructure access variation
- **Nuclear vs. joint family** — reveals support-network variation
- **First-time vs. experienced** — reveals coping-mechanism variation
- **High-resource vs. low-resource** — reveals capability variation
- **Native to context vs. migrant** — reveals cultural-fluency variation

Pick the axis that creates the *sharpest* contrast for your specific problem. If the two personas could be variations of the same person, the contrast axis is too weak.

**Each persona card structure** (identical template, different content):
- **Photo/icon** + **Name** (humanized, e.g., "Chitra Tiwari" — give them a real-sounding name appropriate to the geography)
- **Role description** (italicized, e.g., "*Software Engineer*") — this is the contrast axis made explicit
- **Basic facts block:**
  - Age
  - Kid(s) + age(s)
  - Family Type (Nuclear / Joint / Extended / etc.)
  - Childcare arrangement (Daycare / Parents / Nanny / Self)
  - Working Hours
- **Goals** (3–6 bullets): What they want to achieve. The goals should overlap somewhat (both want child's well-being) but diverge in form (one wants "time for self," the other "to earn a living"). The divergence is the argument — what "work-life balance" means is different across the contrast axis.
- **Motivations** (3–5 bullets): What drives them. Often diverges more sharply than goals.
- **Painpoints and Frustrations** — rendered as a **word cloud** with varied font sizes. The most repeated/severe painpoints rendered larger. Both personas have painpoints, but the relative sizing reveals what matters most to each.

**A test for whether the personas work:** Look at the Goals lists. If Persona A's #1 goal is "self-actualization" and Persona B's #1 goal is "survival," the personas are doing real work. If both lists look interchangeable, redesign.

### Page 5, Section 2: Discoveries

**Function:** 2–3 hero statistics that surfaced during this deeper research phase.

**Length:** 2–3 statistical callouts.

**Structure:**
- Each statistic has a large numeric callout (e.g., **50%**, **86%**)
- A 1-sentence explanation with a bolded key concept (e.g., "**transportation to work**", "**Postpartum Depression**")
- Sourced at the section's bottom (e.g., "Source: Interviews, Field Research, Bodystorming")

These stats should be *new* — different from the ones used in Round 1. They emerged from the deeper research conducted between rounds (bodystorming, additional interviews, field research). If they're the same stats as Round 1, the brief hasn't earned them.

### Page 5, Section 3: Assumptions Invalidated

**Function:** Name 3 assumptions the team held entering this round that the research disproved. The intellectual humility move.

**Length:** 3 assumption-reality pairs.

**Structure of each pair:**
- The assumption stated in **quotes** (italicized or styled to look like a remembered belief): *"Daycares hinder child development."*
- The reality stated as a single sentence with bolded key phrases: Good daycare centres **promote socialisation, independence & maturity.**

**The assumptions should be genuine.** They should be things a reasonable person actually would have believed before doing the research. Examples that work:
- "Women need longer maternity leaves" → research showed shorter is sometimes better
- "Daycares are harmful" → good daycares are beneficial
- "Office work is the hardest part" → the 6–9am rush is harder

Examples that fail (too obviously wrong):
- "Working mothers don't love their children" (strawman — no one believed this)
- "Childcare is easy" (strawman)
- "There are no policies in India for working women" (factually invalidated, not assumption-invalidated)

**This is rare in student work.** Most teams write to confirm their priors. The team that names what they were wrong about earns trust.

### Page 5, Closing: Scope Re-Affirmation

**Function:** One short paragraph (2–4 sentences) acknowledging the validity of what is *outside* scope, then re-stating what is in scope.

**Template:**
> During this phase, we developed an appreciation for the important work performed by [GROUP OUTSIDE SCOPE], including their often-unrecognized [TYPE OF WORK]. While we recognize that [INCLUSIVE STATEMENT], our design process will primarily center on [SCOPED USER].

For the original: "During this phase, we developed an appreciation for the important work performed by mothers at home, including their often-unrecognized unpaid labor. While we recognize that **every mother is a working mother**, our design process will primarily **center on employed mothers**."

This paragraph honors a population the case study does not directly serve, then re-affirms scope. It's the Round 2 equivalent of the Round 1 emotional-arc scope disclaimer.

---

## Voice and tone

Follow all voice and tone rules from the `discovery-brief-case-study` skill. First-person plural ("We"), past tense for research actions, hedged claims, bolded key phrases (not whole sentences), no AI prose tells, empathetic but not saccharine.

**Round 2-specific voice rules:**

- **Honor intersectionality.** When widening to acknowledge sub-populations (e.g., informal sector workers), do so without speaking *for* them. Use language like "underprivileged girls shoulder the burden…" not "they don't know what they're missing." The team's role is to map, not to pity.

- **Use ROLE labels for stakeholder quotes** (Gynecologist, Pediatrician, Spouse, Child) — not personal names. This generalizes the perspective. The exception is the cultural-scenario pull quote on Page 1, which retains the dual-identity full-name attribution from Round 1.

- **Italics for emotional emphasis** inside the Experience Map (Thoughts and Painpoints layers). Bold continues to be used for *concept-naming* (e.g., **bodystorming session**, **gaps in implementation**). The two emphasis tools serve different jobs.

- **Be honest about field research.** If the team did a field visit to an Anganwadi, the source citation should say "Field Visits and Interviews." Do not write "Field Visits" if no team member actually visited the site — that's fabricated methodology.

- **Avoid solution-leakage harder than in Round 1.** Round 2 is closer in the timeline to ideation, and the temptation to start proposing solutions is stronger. Resist. This is still research synthesis. No "we will build…" sentences. No product names.

---

## Visual design language

Follow all visual design rules from the `discovery-brief-case-study` skill. Same palette (warm coral / dusty rose / cream), same custom line-art iconography, same wavy section dividers, same sans-serif typography.

**Round 2-specific visual elements:**

- **Filtration funnel (Page 1):** Vertical inverted funnel showing population narrowing through life stages. Each stage labeled. A small drop icon at the bottom representing the smallest remaining population.

- **Concentric stakeholder map (Page 2):** Three nested circles (CORE / INVOLVED / INFORMED). Stakeholder labels and icons distributed across the three rings. Use dotted or thin lines for ring boundaries — they should feel like soft groupings, not hard categories.

- **Stakeholder quote blocks (Page 2):** Each quote in a soft-rectangle card with rounded corners. Role label as the heading. Icon to the left of the quote. Oversized quotation mark in the top-right.

- **Radial problem mind-map (Page 3):** Center node = user. 5–8 primary branches radiating outward. Sub-branches at the ends. Use varied line weights to distinguish primary branches from sub-branches. Some branches will be denser than others — that's fine. Density variation reflects research depth, not visual imbalance.

- **Multi-layer experience map (Page 4):** A wide swim-lane diagram. Stages as columns at top with time-of-day icons. Layers as horizontal rows. Emotion curve drawn as a smooth line with emoji indicators at each column intersection. Bodystorming row uses wavy lines — one color per team member, with the team member's first name labeled at the left.

- **Persona cards (Page 5):** Two side-by-side cards, identical structure. Persona avatar/icon at top-left. Name + role at top. Basic facts in italic or muted text. Goals + Motivations in two adjacent sub-blocks. Painpoints rendered as a word cloud below — variable font sizes, no bullets.

- **Assumptions invalidated (Page 5):** Each pair rendered as a 2-line block. The assumption in quotes, styled like a remembered belief (italic, slightly muted). The reality below in bold key phrases.

---

## Source and evidence standards

Follow all source standards from the `discovery-brief-case-study` skill. Real, named, retrievable sources. No fabrication.

**Round 2-specific sourcing:**

- **Cite field research when claiming field research.** The Anganwadi pros/cons table can only be sourced to "Field Visits and Interviews" if a team member actually visited an Anganwadi. If they didn't, source the claims to whatever the team actually did (desk research, expert interviews) and remove the field-visit attribution.

- **Bodystorming is a method, not a metaphor.** If the brief mentions a bodystorming session, that session must have actually happened. The wavy lines on the experience map should represent real bodystorming activity — each line for a real team member who actually spent time simulating the user's day.

- **Assumption-invalidation requires evidence.** Each invalidated assumption must be invalidated by something specific: an interview observation, a stat from a study, a field-visit finding. Do not write "We thought X. Actually Y." without being able to say *how* you learned Y.

- **Persona facts should be plausibly sourced.** The two personas don't have to be real individuals (composites are fine), but their facts (working hours, family structure, childcare arrangement) should match real distributions for the contrast axis chosen. If you say "Construction Worker, joint family, parents care for kids," that should reflect actual patterns in that population.

---

## Common failure modes — read before producing the final output

1. **Page 1 just rehashes Round 1.** The Indian Scenario section restates what Round 1 already said, without the filtration funnel or the cultural deep-dive or the existing-services audit. *Fix:* if you wouldn't lose anything by deleting Page 1 of Round 2, you haven't expanded — you've recycled.

2. **No intersectional widening.** Page 1's second paragraph fails to acknowledge a sub-population that experiences the problem differently (often more harshly). *Fix:* name an intersectional group (informal sector workers, rural users, migrant populations, low-income subgroups) and how the filtration affects them differently.

3. **No existing-services audit.** Page 1 skips the Anganwadi-style section. The brief proposes interventions later without acknowledging what already exists. *Fix:* pick one major existing service the team can speak to honestly, with pros/cons. Skip the field-visit attribution if no one actually visited.

4. **Stakeholder map is flat.** Everyone is lumped into one undifferentiated list, or the CORE/INVOLVED/INFORMED rings have arbitrary assignments. *Fix:* re-check ring assignments. CORE = same household / closest relationship. INVOLVED = active touchpoints. INFORMED = peripheral observers.

5. **Stakeholder quotes lack triangulation.** All 5 quotes are from the same type of stakeholder (e.g., all family members, or all medical experts). *Fix:* ensure at least 4 distinct role-types are represented across the 5 quotes.

6. **Stakeholder quotes attributed by name instead of role.** *Fix:* in Round 2, the cultural-scenario quote on Page 1 uses a personal name + dual identity (carryover from Round 1). The 5 quotes on Page 2 use ROLE only — Gynecologist, Pediatrician, Spouse, Child, Caretaker. Different jobs, different attribution conventions.

7. **Problem mapping is sparse or just category labels.** Each branch has only 2–3 sub-items, or sub-items are abstract ("issues," "problems"). *Fix:* the problem mapping page should look slightly overwhelming. If it looks clean and minimal, dig deeper.

8. **Experience Map collapses life-stages and day-stages.** The map plots months/years instead of hours, OR the stages aren't actually one day. *Fix:* Round 1's arc was for life-stages. Round 2's experience map is for ONE DAY. If your stages span longer than 24 hours, you've written a Round 1 artifact in Round 2's slot.

9. **Experience Map missing one of the 4 layers.** Often the Painpoints or Thoughts layer is missing or generic. *Fix:* every column needs content in all 4 layers (Actions / Emotions / Thoughts / Painpoints). Empty cells = under-research.

10. **No bodystorming row.** The Experience Map skips the bottom row entirely. *Fix:* include it. If the team didn't actually bodystorm, either run a quick session before finalizing the brief, OR remove the bodystorming framing from the caption.

11. **Personas don't actually contrast.** Both personas are variations of the same person (e.g., two white-collar mothers from different cities). *Fix:* identify a contrast axis (organized vs. unorganized sector, urban vs. rural, etc.) that creates sharp divergence. If you can swap their painpoints lists and barely notice, the contrast is too weak.

12. **No invalidated assumptions section.** The brief writes only what the team learned, never what they were wrong about. *Fix:* find 3 genuine assumptions the team held entering this phase that the research disproved. If you can't find 3, either the team didn't enter with assumptions (unlikely) or didn't notice their assumptions being invalidated (more likely — go back through the research).

13. **Invalidated assumptions are strawmen.** The "assumptions" listed are things no reasonable person actually believed (e.g., "We assumed working mothers don't love their children"). *Fix:* an assumption only counts if at least one team member, or a representative outsider, actually held it.

14. **No scope re-affirmation paragraph.** The brief ends abruptly after Discoveries or Assumptions Invalidated. *Fix:* add the closing paragraph that acknowledges what's outside scope and re-states the focus.

15. **Solution-leakage.** Sentences like "Our app will provide…" or "The platform we're building…" *Fix:* Round 2 is still research synthesis. No solutions yet. Even if the team has started ideating internally, the brief must remain in research-synthesis mode.

---

## Worked mini-example (adapted to a new problem statement)

To show the pattern's adaptability, here is how this skill would apply to a different topic — continuing the elderly-loneliness example from the Round 1 skill's worked example. **This is illustrative only.**

**Round 1 HMW (carryover):** "How might we help elderly individuals living alone in urban India sustain meaningful daily connection?"

**Round 2 Page 1 — The Indian Scenario (revisited):**
Filtration funnel showing elderly dropping out of community life at stages: Healthy aging with spouse → Spouse's illness → Loss of spouse → Adult children move out / abroad → Mobility decline → Isolation.
Second paragraph widens to acknowledge **elderly domestic workers and informal-sector retirees** who have no pension and continue working into ill health — a different intersection of the same problem.

**Cultural Scenario:** Cultural scripts around **filial duty as son's responsibility**, **shame of "burdening" children**, and **uncommon to encounter elderly who live independently by choice**.
Pull quote from a gerontologist who is also a daughter of an elderly parent: dual identity.

**Existing Services — Day Care Centres for the Elderly:** Government scheme + an NGO example (e.g., HelpAge India). Pros: socialization, structured activities, medical check-ins. Cons: limited hours, transport gap, underfunded, urban-bias, cultural resistance.

**Other Policies and Services:** PMVVY, IGNOAPS, Rashtriya Vayoshri Yojana. Gap claim about implementation + accessibility.

**Page 2 — Stakeholder Map:**
- CORE: Elderly Individual, Adult Children, Spouse / Late Spouse, Grandchildren
- INVOLVED: Domestic Help, Doctors / Healthcare, Neighbors, Religious / Spiritual Community, Day Care Centres, Local Government, Pharmacies, Transport
- INFORMED: Former Colleagues, Extended Family Abroad, Community Welfare Org, Insurance Agent

**Stakeholder Quotes:**
- Gerontologist (medical/expert)
- Adult Daughter (family, different generation)
- Domestic Helper (service provider)
- Religious Community Member (community)
- Pharmacy Owner (commercial-touchpoint observer)

**Page 3 — Problem Mapping:**
Branches: Physical Health, Mental Health, Financial, Mobility, Social Connection, Daily Living, Cultural / Identity.

**Page 4 — Experience Map:**
Day stages: Pre-dawn prayer → Breakfast alone → Mid-morning newspaper → Lunch / TV → Afternoon nap → Evening walk → Dinner phone call with children → Bedtime.
4 layers (Actions, Emotions, Thoughts, Painpoints) + bodystorming row with 4 team members.

**Page 5 — Two Personas:**
Contrast axis: financial security + family proximity.
- **Mr. Subbarao** — Retired Bureaucrat, 72, urban Hyderabad, son in US, financially comfortable, recently widowed.
- **Mrs. Lakshmi** — Former Domestic Worker, 68, urban slum, son nearby but estranged, financially precarious.
Goals diverge: Mr. Subbarao wants "meaningful intellectual engagement"; Mrs. Lakshmi wants "to not be a burden."

**Discoveries:**
- 41% of urban elderly Indians live alone (NSSO)
- 23% report chronic loneliness (a meta-analysis figure)

**Assumptions Invalidated:**
- "Elderly want to live with their children." → Many actively prefer independent living when financially possible; they want connection, not co-habitation.
- "Smartphones can solve isolation." → Many elderly have phones, use them daily, and are still lonely. The phone is not the bottleneck.
- "Religious community provides sufficient social connection." → Religious community provides ritual, but not daily emotional anchoring.

**Closing scope re-affirmation:** Acknowledges the validity of multi-generational care models while keeping focus on solo-dwelling elderly.

---

## Scoring Benchmark

Before delivering any Round 2 brief, score it on the four dimensions below. The first is **lower-is-better** (AI texture should be minimal). The other three are **higher-is-better**. Each maps to a specific cluster of Round 2 failure modes.

| Dimension | What It Measures | Target |
|-----------|-----------------|--------|
| **AI-Likeness** | Generic AI prose, filler phrases, melodrama, missing nuance moves, third-person drift, corporate jargon, solution-leakage. Voice should match Round 1's first-person-plural team voice exactly. | 1–3 |
| **Ecosystem Breadth** | Does Page 1 add new lenses (filtration funnel + cultural deep-dive + existing-services audit + gap claim), NOT just rehash Round 1? Is the stakeholder map populated across all three rings? Does the problem mapping look deliberately dense, with 5–8 branches and 3–8 sub-issues each? Is the intersectional widening present (informal sector or equivalent)? | 8–10 |
| **Empathic Granularity** | Are stakeholder quotes triangulated across 4+ distinct roles? Does the Experience Map have content in all 4 layers (Actions/Emotions/Thoughts/Painpoints) at all 6 stages? Is the bodystorming row present and labeled with real team members? Are italicized words used to mark emotional charge inside the experience map? | 8–10 |
| **Persona Contrast & Humility** | Do the two personas reveal genuinely different facets of the problem via a deliberate contrast axis (not just variations)? Are the 3 invalidated assumptions genuine beliefs (not strawmen)? Is each invalidation backed by specific research evidence? Is the closing scope re-affirmation paragraph present? | 8–10 |

### What each dimension looks like at low vs. high scores

**AI-Likeness (lower is better)**
- *1–3 (target):* Reads like the same team that wrote Round 1. First-person plural throughout. Hedges where appropriate. Bolded phrases name specific concepts. Both contextual seriousness (the existing-services audit, the intersectional widening) and intellectual humility (the invalidated assumptions, the scope re-affirmation) are present. No solution-leakage. No "delve," "navigate the complexities," "comprehensive," "holistic," "in today's [noun]" filler.
- *7–10 (fail):* Generic, third-person, corporate. Skips intersectional widening. Sneaks in product names or solution language. The voice doesn't match Round 1 — reads as a different team's work.

**Ecosystem Breadth (higher is better)**
- *8–10 (target):* Page 1 adds three new lenses on top of Round 1's context (filtration, culture, existing services). The stakeholder map has 15+ entities across 3 rings with deliberate ring assignments. The problem mapping has 5+ branches with real sub-issue depth. The intersectional widening explicitly names a sub-population.
- *1–4 (fail):* Page 1 rehashes Round 1 without adding new lenses. The stakeholder map has 7 entities all crammed into the CORE ring. The problem mapping has 3 branches each with 2 sub-items.

**Empathic Granularity (higher is better)**
- *8–10 (target):* 5+ stakeholder quotes spanning 4+ roles. Experience map has all 4 layers populated at all 6 stages with specific, observable content (not "feels tired" but "*demotivated* by the workload"). Bodystorming row present with real team member names. Italicized words mark the emotional charge inside Thoughts and Painpoints layers.
- *1–4 (fail):* 3 stakeholder quotes all from one role-type. Experience map has 2 layers populated, others left empty or filled with generic content. No bodystorming row. No italicization for emphasis.

**Persona Contrast & Humility (higher is better)**
- *8–10 (target):* Two personas on a sharp contrast axis. Their goals and painpoints visibly diverge — the case study could not be reduced to one user. 3 invalidated assumptions, all genuine (not strawmen), each backed by specific research evidence. Scope re-affirmation paragraph honors what's outside scope.
- *1–4 (fail):* Two personas that are variations of each other (Persona A is just Persona B with a different name). 1 invalidated assumption, or 3 strawman assumptions. No re-affirmation paragraph.

### Scoring output format

After scoring, output a justification block in this format alongside the brief:

```
## Self-Audit Scores

| Dimension | Score | Justification |
|-----------|-------|---------------|
| AI-Likeness | X/10 | [one sentence — name specific markers present or absent] |
| Ecosystem Breadth | X/10 | [one sentence — note new lenses, stakeholder ring distribution, problem-map density] |
| Empathic Granularity | X/10 | [one sentence — note quote triangulation, experience-map completeness, bodystorming evidence] |
| Persona Contrast & Humility | X/10 | [one sentence — note contrast axis sharpness, assumption-invalidation quality] |
```

### Important diagnostic cross-checks

- **AI-Likeness low AND Ecosystem Breadth low** → Clean prose around shallow research. Reader sees pretty writing but no new depth from Round 1. Likely needs more field research, more interviews, or more time mapping the stakeholder ecosystem.
- **Ecosystem Breadth high AND Empathic Granularity low** → The team mapped breadth but not depth. The brief is impressive at the system level but hollow at the human level. Add more specific micro-observations to the Experience Map, more direct stakeholder quotes.
- **Empathic Granularity high AND Persona Contrast & Humility low** → The team did good observational work but didn't pattern-match across sub-populations or examine their own assumptions. Strengthen the persona contrast axis and find genuine assumption-invalidations.
- **All dimensions high but feels formulaic** → Check whether the team is *demonstrating* expansion or just *performing* it. Each new artifact (stakeholder map, problem map, experience map, personas) should reveal something the team learned, not just fill a section slot.

If any dimension scores below target after the first draft, revise that dimension before delivering.

---

## Operating procedure

When the user invokes this skill:

1. **Verify Round 1 exists.** Confirm the user has a completed Round 1 HMW question and the surrounding context (target user, geography, team). If they don't, suggest they invoke `discovery-brief-case-study` first and return when Round 1 is complete. Do not draft Round 2 without a Round 1 anchor — the expansion logic only works if there's a sharp problem statement to expand from.

2. **Verify inputs against the input checklist.** Read `references/input-checklist.md` and confirm the user has provided the mandatory Round 2 inputs. If anything mandatory is missing, ask for it before drafting. If high-value optional inputs are missing, note which ones and explain how their absence will limit the output's quality.

3. **Do real research.** Search the web for current statistics relevant to the filtration funnel, cultural context, and existing services. Cite named sources. Do not fabricate. If a statistic can't be sourced, remove the claim.

4. **Plan the expansion.** Before drafting, sketch all six expansion axes and verify each is covered: contextual (cultural + existing services), relational (stakeholder map), problematic (problem mind-map), temporal-micro (experience map), persona (two contrasting), epistemic (assumptions invalidated).

5. **Draft section by section** following the section playbook above. For each section, output:
   - The prose / content
   - Required statistics with citation
   - A "Visual elements to design" callout describing what the user needs to design (chart type, icons needed, layout, visual emphasis)

6. **Audit against the failure modes list.** Walk through all 15 failure modes and confirm none apply.

7. **Self-score using the Scoring Benchmark.** Score the draft on all four dimensions. If any dimension misses its target range, revise and re-score before delivering. Include the final scoring table in the output.

8. **Deliver as a single document** structured as the 5 pages, with clear page breaks and section headings, formatted in markdown unless the user requests a different output format. Include the self-audit scores at the end.

9. **Offer next steps.** Ask whether the user wants:
   - A visual HTML/SVG mockup of any specific section (especially the stakeholder map, problem mind-map, experience map, or persona cards — these are visually distinctive)
   - A second iteration on a specific dimension where the score missed target
   - Help drafting Round 3 (ideation / solution phase, which this skill does NOT cover)

---

## Reference files

- `references/input-checklist.md` — The full list of mandatory and high-value optional inputs the user should provide before invoking the skill, plus a fillable template. Read at the start of every invocation to verify inputs.
