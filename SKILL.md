---
name: ux-case-study-writer
description: Write portfolio-grade UX/service-design case study briefs across all 4 rounds of the design-thinking double diamond. Trigger on "write my case study", "case study Round N", "discovery brief", "empathy phase", "problem narrowing", "solution brief", "design my portfolio case study", or any request for a structured design-thinking deliverable. Works for any geography, any domain, solo or team.
metadata:
  category: "ux"
  tags: ["case-study", "service-design", "design-thinking", "portfolio", "UX-research", "double-diamond", "HMW", "empathy-map", "persona", "journey-map"]
---

# UX Case Study Writer

A 4-phase skill that produces portfolio-grade service-design case study briefs following the design-thinking double diamond. Each phase builds on the previous. The output is a content + layout specification the user takes into Figma, Canva, or InDesign.

## Hard Constraints

These are the only enforced rules. Everything else is guidance — adapt to the user's needs.

```
1. DIAMOND SHAPE: Phase 1 narrows, Phase 2 expands, Phase 3 narrows, Phase 4 delivers.
   If this shape is broken, the case study's argument doesn't work.

2. NO FABRICATION: Every statistic needs a named, real source. Every quote must be
   verbatim from a real interview. If data doesn't exist, say so — don't invent it.

3. NO SOLUTION LEAKAGE: Phases 1-3 must not name products, apps, or specific solutions.
   Opportunities are directions. Solutions appear only in Phase 4.

4. CONTINUITY CHECKPOINT: At the start of each phase (2-4), restate the current HMW,
   target user, and geography. If any changed from the prior phase, acknowledge the
   change explicitly rather than silently drifting.

5. NEVER SILENTLY RESOLVE CONFLICTS: When user inputs contain contradictions, surface
   both interpretations and let the user choose.
```

## Guidance (not rules — adapt as needed)

- **Voice:** First-person plural ("we," "our") works for both solo and team. Match explanation depth to the user's familiarity.
- **Tense:** Past for research actions, present for findings, future-conditional for impacts.
- **Bolding:** Bold 2-4 word key phrases (noun phrases), not whole sentences.
- **Empathy without melodrama:** Show difficulty + counterweight ("Despite these difficulties...").
- **Avoid AI-prose tells:** "delve," "navigate the complexities," "in today's fast-paced world," "comprehensive," "holistic," "robust" as filler.
- **Adapt your mode:** Coach when the user is stuck, write when they have inputs, track progress when they're managing phases. Don't lock into one role.
- **Solo is the default.** If team members are named, activate team elements (credit line, multi-scorer radar). Never require team inputs.
- **Geography-agnostic by default.** The structural patterns (funnel, personas, scoring, HMW) are universal. Cultural scripts, data sources, and regulatory context adapt to the user's stated geography.
- **Impact framework is domain-dependent.** Default to a generic 5-7 dimension impact model. Offer the wellbeing radar as one option for health/social/caregiving domains. Let users define custom dimensions.
- **Primary research produces the best output.** If interviews aren't available, proceed with secondary research and clearly label assumption-based sections. Note evidence source limitations in the self-audit.

## The 4 Phases

| Phase | Name | Pages | Core Deliverable | Key Artifact |
|-------|------|-------|------------------|--------------|
| **1** | Discovery Brief | 4 | Research + problem definition | HMW question |
| **2** | Empathy Deepening | 5 | Ecosystem + personas + experience map | Contrasting personas |
| **3** | Problem Convergence | 4 | Problem scoring + ecosystem map + need statement | Formal need statement |
| **4** | Solution Design | 4 | Solution presentation + validation + impact | Named solution with features |

### Phase 1: Discovery Brief (Define)

Funnels from global context to a sharp HMW question. The key pattern is **progressive narrowing** — each section's noun phrase is more specific than the last.

**Document anatomy:** Introduction > Global Scenario > National Perspective > Impact on Sub-group > Interview Insights > Emotional Arc > Framework > Opportunities > Problem Statement

**Full spec:** `rounds/01-discovery/playbook.md`
**Input checklist:** `rounds/01-discovery/inputs.md`

### Phase 2: Empathy Deepening (Empathize 2.0)

Takes the Round 1 HMW and **opens it back up** into a comprehensive problem space. Adds fieldwork, bodystorming, and second-wave interviews.

**Document anatomy:** Filtration Funnel > Cultural Scenario > Existing Services Audit > Stakeholder Map > Stakeholder Quotes > Problem Space Mind-Map > Experience Map > Personas > Invalidated Assumptions

**Full spec:** `rounds/02-empathy/playbook.md`
**Input checklist:** `rounds/02-empathy/inputs.md`

### Phase 3: Problem Convergence (Converge)

Scores candidate problems, selects one, maps its ecosystem, builds the business case, and refines the HMW into sub-HMWs + a formal need statement.

**Document anatomy:** HMW Restatement > Problem Scoring > Narrowing Down > Ecosystem Map > Pain Points > Regional Scenario > Setbacks > Impact > Business Viability > Sub-HMWs > Need Statement

**Full spec:** `rounds/03-convergence/playbook.md`
**Input checklist:** `rounds/03-convergence/inputs.md`

### Phase 4: Solution Design (Deliver)

Presents the final solution with cause-effect synthesis, ideation breadth, validation data, named features, service flow, FAQs, and impact case.

**Document anatomy:** Background Recap > Cause & Effect Tree > How-to Questions > Co-creation & Testing > Solution Reveal > Key Features > Service Flow > FAQs > Benefits > Framework Return > Impact > Scalability > Closing Statement

**Full spec:** `rounds/04-solution/playbook.md`
**Input checklist:** `rounds/04-solution/inputs.md`

## Operating Procedure

Follow the wizard protocol (`references/wizard.md`) for input collection:

1. **Triage** — identify the phase, collect continuity from prior phases, ask the user to paste everything they have.
2. **Extract** — parse pasted content for recognizable inputs (quotes, stats, HMW, stages, etc.). Show ✓/✗/~ per cluster. Confirm with user.
3. **Fill gaps** — walk missing mandatory inputs with examples. Ask top-3 optional inputs. Validate quality with light nudges, never rejections.
4. **Confirm & draft** — output an input summary, then draft directly. Don't front-load a template review step.
5. **Check continuity (Phases 2-4).** If the HMW, target user, or geography changed from the prior phase, acknowledge it explicitly.
6. **Do real research.** Search for current statistics. Include source dates. Never fabricate.
7. **Draft directly.** After collecting inputs, proceed to drafting. Don't front-load a template review step.
8. **Always deliver.** Include self-audit scores as a diagnostic, not a gate. Highlight the weakest dimension and suggest what would improve it. Never block delivery on an internal score.
9. **Output a Project State block** at the end of each phase — a compact summary (HMW, target user, geography, team, key artifacts) the user pastes back when starting the next phase. Keep it under 30 lines.
10. **Offer next steps:** iteration on specific sections, visual mockup, or advancing to the next phase.

## Input Handling

- **Target user:** Show the demographic-vs-life-phase distinction with one example ("'women aged 25-40' is a demographic; 'women in early stages of motherhood' is a life phase — life phases generate emotional arcs"). Confirm their intent. Don't algorithmically reject valid demographic scoping.
- **Scoring data (Phase 3):** Accept any format — spreadsheet paste, summary narratives, ranked lists. If individual scores aren't available, work with team-level rankings or relative comparisons. The insight matters more than the matrix.
- **Validation data (Phase 4):** Include methodology details (N, method, materials) in the output alongside stats. Make the evidence trail visible so reviewers can assess credibility.
- **Reactivated stats:** Include the source date. If a stat is notably old relative to a fast-changing domain, note this — but don't block or auto-reject.
- **HMW pivots:** Allow them. Pivots mean the research is working. Note what changed and flag which prior-phase artifacts may need updating. Don't force a full restart for a scope adjustment.

## Visual Design Language

These are defaults — adapt to user preferences if stated.

- **Palette:** Soft pastels. Primary warm coral (#E89598). Secondary cream (#FCF4ED). Text dark plum.
- **Typography:** Sans-serif. Display weight for headers. Statistics rendered 3-5x body size.
- **Iconography:** Custom line-art icons. Single weight, rounded corners, figurative subjects.
- **Layout:** 2-column predominant. Generous whitespace.
- **Quote callouts:** Oversized quotation marks. Attribution in italics.

## Output Format

Each phase outputs a markdown document structured as numbered pages:

```markdown
# [Phase Name] Case Study Brief

## Page 1
### [Section Name]
[Prose content]

**Visual elements to design:**
- [Chart/icon/layout specification]

[Statistics with sources]

---
## Page 2
[...]

---
## Self-Audit Scores

| Dimension | Score | Justification |
|-----------|-------|---------------|
| [Dim 1] | X/10 | [one sentence] |
| [Dim 2] | X/10 | [one sentence] |
| [Dim 3] | X/10 | [one sentence] |
| [Dim 4] | X/10 | [one sentence] |

---
## Project State (paste this back for the next phase)

- **Phase completed:** N
- **HMW:** [current question]
- **Target user:** [current definition]
- **Geography:** [current context]
- **Team:** [names, or "solo"]
- **Key artifacts:** [list what this phase produced]
```

## Gotchas

1. **Fabricating prior-round content** — if Round 1 doesn't exist, help the user complete it first. Don't invent continuity.
2. **Merging all 4 phases into one document** — each phase is a standalone brief with its own scoring benchmark.
3. **Recycling the same statistics across phases** — each phase should introduce new evidence from deeper research (except deliberate stat-reactivation in Round 4).
4. **Forcing the wellbeing framework on non-health domains** — use domain-appropriate impact frameworks.
5. **Requiring team inputs from solo users** — solo is the default. Team features activate only when team data is provided.
6. **Hardcoding India-specific assumptions** — structural patterns are universal. Cultural specifics come from the user's stated geography.

## References

- `rounds/01-discovery/playbook.md` — Phase 1 writing playbook + scoring benchmark
- `rounds/02-empathy/playbook.md` — Phase 2 writing playbook + scoring benchmark
- `rounds/03-convergence/playbook.md` — Phase 3 writing playbook + scoring benchmark
- `rounds/04-solution/playbook.md` — Phase 4 writing playbook + scoring benchmark
- `rounds/01-discovery/inputs.md` — Phase 1 inputs template
- `rounds/02-empathy/inputs.md` — Phase 2 inputs template
- `rounds/03-convergence/inputs.md` — Phase 3 inputs template
- `rounds/04-solution/inputs.md` — Phase 4 inputs template
- `references/wizard.md` — Smart triage wizard flow, extraction patterns, cluster definitions, validation rules
- `references/peer-review.md` — Evaluation checklist for humans or AI
