# UX Case Study Writer

A Claude Agent Skill that writes portfolio-grade UX/service-design case study briefs across all 4 rounds of the design-thinking double diamond.

Works for **any geography, any domain, solo or team.**

## What It Does

Given your research inputs (topic, target user, interview data, statistics), this skill produces a multi-page content + layout specification for each phase of a service-design case study. You take the output into Figma, Canva, or InDesign to create the final designed PDF.

```
Phase 1: Discovery Brief       — narrows from global context to a sharp HMW question
Phase 2: Empathy Deepening     — expands into ecosystem maps, personas, experience maps
Phase 3: Problem Convergence   — scores problems, selects one, builds business case
Phase 4: Solution Design       — presents the tested solution with features and impact
```

Each phase produces a standalone 4-5 page brief with prose, statistics, visual element callouts, and self-audit scores.

## Quick Start

1. Tell Claude which phase you're working on (or describe your project and let it figure out)
2. Paste whatever you have — raw notes, interview transcripts, prior briefs, statistics
3. Claude extracts inputs, flags gaps, and drafts the brief
4. At the end of each phase, you get a **Project State** block to paste back when starting the next phase

## Repo Structure

```
ux-case-study-writer/
├── SKILL.md                              # Master skill — constraints, guidance, operating procedure
├── references/
│   ├── phase-1-discovery.md              # Phase 1 writing playbook + scoring benchmark
│   ├── phase-2-empathy.md                # Phase 2 writing playbook + scoring benchmark
│   ├── phase-3-convergence.md            # Phase 3 writing playbook + scoring benchmark
│   ├── phase-4-solution.md               # Phase 4 writing playbook + scoring benchmark
│   ├── input-checklist-phase-1.md        # Phase 1 inputs (mandatory + optional)
│   ├── input-checklist-phase-2.md        # Phase 2 inputs
│   ├── input-checklist-phase-3.md        # Phase 3 inputs
│   └── input-checklist-phase-4.md        # Phase 4 inputs
└── examples/
    ├── working-mothers-overview.md       # Team Dua full walkthrough (all 4 phases)
    └── adaptation-guide.md               # 3 domain adaptation sketches + transfer test
```

## Design Philosophy

This skill was designed through a **21-question council process** where four voices (Architect, Skeptic, Pragmatist, Critic) debated every constraint. The result:

**5 hard constraints, ~10 guidance lines, everything else left to Claude's judgment.**

### Hard Constraints (the only enforced rules)

| # | Constraint | Why |
|---|-----------|-----|
| 1 | **Diamond shape** — P1 narrows, P2 expands, P3 narrows, P4 delivers | The argument structure of the case study |
| 2 | **No fabrication** — every stat sourced, every quote verbatim | Research integrity |
| 3 | **No solution leakage** — no products/apps named before Phase 4 | Preserves design freedom |
| 4 | **Continuity checkpoint** — restate HMW/user/geography at each phase start | Prevents silent drift |
| 5 | **Never silently resolve conflicts** — surface contradictions, let user choose | User agency |

### Key Design Decisions

| Decision | Verdict | Rationale |
|----------|---------|-----------|
| Solo vs. team | Solo is default | 90%+ of portfolio builders work alone |
| Geography | Agnostic by default | Structural patterns are universal |
| Impact framework | Domain-dependent | Wellbeing radar is one option, not the default |
| No interview data? | Proceed with limitations noted | Meet users where they are |
| Scoring benchmarks | Diagnostic, never a gate | Always deliver; never block |
| Wizard modes | No explicit modes | Adapt per-cluster based on what user has |
| Template vs. draft | Draft-first | Users need momentum, not fill-in-the-blank |
| State persistence | Portable Project State block | User pastes back; zero infrastructure |
| HMW pivots | Always allowed | Pivots mean the research is working |
| Context management | Load one phase at a time | Never load all 4,594 lines of specs at once |

## Origin

Consolidated from 4 separately-downloaded case study phase skills (originally in the Team Dua service-design style), then redesigned through a structured grill-me interview (21 questions) and a 4-voice council process to determine the right balance of constraints vs. freedom.

**Source material:**
- Phase 1: Discovery Brief (Round 1 / Define)
- Phase 2: Empathy Deepening (Round 2 / Empathize 2.0)
- Phase 3: Problem Convergence (Round 3 / Converge)
- Phase 4: Solution Design (Round 4 / Deliver)

## Roadmap

- [ ] **Smart Triage Wizard** — conversational input collection that assesses readiness and guides users through gaps
- [ ] **Condensed phase specs** — reduce each phase spec from ~500 lines to ~200 lines of principles + examples
- [ ] **Full worked example** — a complete Phase 1 brief (4 pages of actual prose) as a gold-standard reference
- [ ] **Peer review guide** — external review checklist for humans or AI to evaluate briefs

## License

MIT
