---
name: ux-case-study-writer
description: Write portfolio-grade UX/service-design case study briefs across all 4 rounds of the design-thinking double diamond. Use whenever the user wants to produce a case study, research brief, empathy deep dive, problem convergence brief, or solution-design presentation in the Team Dua style. Trigger on "write my case study", "case study Round N", "discovery brief", "empathy phase", "problem narrowing", "solution brief", "design my portfolio case study", or any request for a structured design-thinking deliverable that synthesizes research into a narrative document. This skill orchestrates 4 phase-specific sub-skills, each producing a distinct multi-page brief.
metadata:
  category: "ux"
  tags: ["case-study", "service-design", "design-thinking", "portfolio", "UX-research", "double-diamond", "HMW", "empathy-map", "persona", "journey-map"]
---

# UX Case Study Writer (Team Dua Style)

## Overview

A 4-phase skill system that produces portfolio-grade service-design case study briefs following the design-thinking double diamond. Each phase builds on the previous, narrowing from global context to a tested solution. The output is a content + layout specification the user takes into Figma, Canva, or InDesign.

```
IRON LAW: Each phase REQUIRES the previous phase's deliverables as input.
Skipping a phase or fabricating prior-round content produces a brief that
fails portfolio review. If the user hasn't completed prior rounds, help
them finish those first — do not invent continuity.
```

## When to Use

- User asks for a portfolio case study in UX / service-design style
- User asks for any specific round: "write my Round 1/2/3/4"
- User wants a research brief, empathy map, problem scoring, or solution presentation
- User says "make me a case study like this" with a design-school deliverable as reference
- User asks for a How-Might-We problem statement with supporting research

## When NOT to Use

- Academic case study research (Yin methodology) — use `grad-case-study` instead
- Business strategy case studies (HBS style) — use `biz-*` skills instead
- UX audit or heuristic evaluation — different deliverable type
- Wireframes, prototypes, or UI design — this skill produces content specs, not designs

## The 4 Phases

| Phase | Name | Pages | Core Deliverable | Key Artifact |
|-------|------|-------|------------------|--------------|
| **1** | Discovery Brief | 4 | Research + problem definition | HMW question |
| **2** | Empathy Deepening | 5 | Ecosystem + personas + experience map | Contrasting personas |
| **3** | Problem Convergence | 4 | Problem scoring + ecosystem map + need statement | Formal need statement |
| **4** | Solution Design | 4 | Solution presentation + validation + impact | Named solution with features |

### Phase 1: Discovery Brief (Define)

Funnels from global context to a sharp HMW question. The single most important pattern is **progressive narrowing** — each section's noun phrase is more specific than the last.

**Document anatomy:** Introduction > Global Scenario > National Perspective > Impact on Sub-group > Interview Insights > Emotional Arc > Wellbeing Framework > Opportunities > Problem Statement

**Full spec:** `references/phase-1-discovery.md`
**Input checklist:** `references/input-checklist-phase-1.md`

### Phase 2: Empathy Deepening (Empathize 2.0)

Takes the Round 1 HMW and **opens it back up** into a comprehensive problem space. Adds fieldwork, bodystorming, and second-wave interviews.

**Document anatomy:** Filtration Funnel > Cultural Scenario > Existing Services Audit > Stakeholder Map > Stakeholder Quotes > Problem Space Mind-Map > Experience Map > Personas > Invalidated Assumptions

**Full spec:** `references/phase-2-empathy.md`
**Input checklist:** `references/input-checklist-phase-2.md`

### Phase 3: Problem Convergence (Converge)

Team scores candidate problems, selects one, maps its ecosystem, builds the business case, and refines the HMW into sub-HMWs + a formal need statement.

**Document anatomy:** HMW Restatement > Problem Scoring Radar > Narrowing Down > Ecosystem Map > Pain Points > Regional Scenario > Setbacks > Impact > Business Viability > Sub-HMWs > Need Statement

**Full spec:** `references/phase-3-convergence.md`
**Input checklist:** `references/input-checklist-phase-3.md`

### Phase 4: Solution Design (Deliver)

Presents the final solution with cause-effect synthesis, ideation breadth, validation data, named features, service flow, FAQs, and impact case.

**Document anatomy:** Background Recap > Cause & Effect Tree > How-to Questions > Co-creation & A/B Testing > Solution Reveal > Key Features > Service Flow > FAQs > Benefits > Wellbeing Return > Impact > Scalability > Closing Statement

**Full spec:** `references/phase-4-solution.md`
**Input checklist:** `references/input-checklist-phase-4.md`

## Operating Procedure

1. **Identify the phase.** Ask the user which round they need, or infer from context.
2. **Load the phase spec.** Read the corresponding `references/phase-N-*.md` file.
3. **Verify inputs.** Read the corresponding `references/input-checklist-phase-N.md`. Confirm mandatory inputs are present. Flag missing high-value optional inputs.
4. **Check continuity.** For Phases 2-4, verify that prior-round deliverables exist and are consistent.
5. **Do real research.** Search for current statistics. Cite named sources. Never fabricate.
6. **Draft section by section** following the phase spec's playbook. For each section, output prose + statistics + "Visual elements to design" callout.
7. **Audit against failure modes** listed in the phase spec.
8. **Self-score** using the phase's Scoring Benchmark. Revise any dimension that misses its target before delivering.
9. **Deliver** as a single markdown document with page breaks and section headings. Include self-audit scores.
10. **Offer next steps:** iteration on specific sections, visual mockup, or advancing to the next phase.

## Cross-Phase Consistency Rules

These rules apply across ALL phases:

- **Voice:** First-person plural ("we," "our"). Never "I" or "the researchers."
- **Tense:** Past for research actions, present for findings, future-conditional for impacts.
- **Hedging:** Soft-hedge most claims. "Often face," "many of which," "anticipate."
- **Bolding:** Bold only 2-4 word key phrases (noun phrases), never whole sentences.
- **Statistics:** Every numeric claim needs a named, real source. No fabrication.
- **Empathy without melodrama:** Show difficulty + counterweight ("Despite these difficulties...").
- **No AI-prose tells:** Ban "delve," "navigate the complexities," "in today's fast-paced world," "comprehensive," "holistic," "robust" as filler.
- **No solution leakage** in research phases (1-3). Opportunities are directions, not products.
- **Team credit** at the bottom of every brief's final page.

## Visual Design Language (All Phases)

- **Palette:** Soft pastels. Primary warm coral (#E89598). Secondary cream (#FCF4ED). Text dark plum.
- **Typography:** Sans-serif. Display weight for headers. Statistics rendered 3-5x body size.
- **Iconography:** Custom line-art icons. Single weight, rounded corners, figurative subjects.
- **Layout:** 2-column predominant. Generous whitespace. Each page uncrowded.
- **Quote callouts:** Oversized quotation marks. Attribution in italics.

## Gotchas

1. **Fabricating prior-round content for continuity** — if Round 1 doesn't exist, don't fake an HMW to start Round 2. Help the user complete Round 1 first.
2. **Treating all 4 phases as one document** — each phase is a standalone multi-page brief with its own scoring benchmark. Don't merge them.
3. **Skipping the input checklist verification** — the skill is only as good as its inputs. Generic inputs produce generic output. Always verify before drafting.
4. **Using the same statistics across phases** — each phase should introduce new evidence from deeper research, not recycle Round 1 stats (except deliberate stat-reactivation in Round 4).
5. **Losing the funnel discipline** — Phase 1 narrows, Phase 2 expands, Phase 3 narrows again, Phase 4 presents. If Phase 2 is still narrowing or Phase 3 is still expanding, the diamond shape is broken.
6. **Solution leakage before Phase 4** — Phases 1-3 must not name products, apps, or specific solutions. Opportunities are directions. Solutions appear only in Phase 4.

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
```

## References

- `references/phase-1-discovery.md` — Full Phase 1 writing playbook + scoring benchmark
- `references/phase-2-empathy.md` — Full Phase 2 writing playbook + scoring benchmark
- `references/phase-3-convergence.md` — Full Phase 3 writing playbook + scoring benchmark
- `references/phase-4-solution.md` — Full Phase 4 writing playbook + scoring benchmark
- `references/input-checklist-phase-1.md` — Phase 1 mandatory + optional inputs template
- `references/input-checklist-phase-2.md` — Phase 2 mandatory + optional inputs template
- `references/input-checklist-phase-3.md` — Phase 3 mandatory + optional inputs template
- `references/input-checklist-phase-4.md` — Phase 4 mandatory + optional inputs template
