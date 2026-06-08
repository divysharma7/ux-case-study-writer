# UX Case Study Writer

Most design students spend 40+ hours writing one case study. It still reads like a ChatGPT summary.

This is a Claude Agent Skill that produces portfolio-grade UX case study briefs. 4 phases. Double diamond. Any domain. Any geography. Solo or team.

You paste your research. It writes the brief. You take it to Figma.

Not a template. Not a fill-in-the-blank worksheet. A 2,300+ line writing system that knows exactly what a Discovery Brief's third paragraph should do, what stat pair type goes on Page 2, and why your emotional arc can't be monotonic.

---

## What actually comes out

4 standalone briefs, one per phase:

```
Phase 1: Discovery Brief       4 pages.  Global context → sharp HMW question.
Phase 2: Empathy Deepening     5 pages.  Ecosystem maps, personas, experience maps.
Phase 3: Problem Convergence   4 pages.  Problem scoring, business case, need statement.
Phase 4: Solution Design       4 pages.  Named solution, features, validation, impact.
```

Each brief includes:
- Actual prose (not bullet points)
- Sourced statistics (real sources, not fabricated)
- Visual element callouts telling you exactly what to design in Figma
- Self-audit scores so you know where it's strong and where it's thin

The output is a content + layout spec. Claude writes the words and describes every chart, icon, and diagram. You handle the pixels.

---

## How it works — the wizard

People think you need a perfectly organized input doc to get a good case study.

Reality: you paste a mess of notes and the wizard figures it out.

### The 4-stage flow

```
TRIAGE → EXTRACT → FILL GAPS → CONFIRM & DRAFT
```

**Stage 1: Triage.** Three messages, max. Identifies your phase. If you don't know which phase you're in, it figures it out:
- No prior research? Phase 1.
- Have an HMW but no fieldwork? Phase 2.
- Have personas but haven't picked a problem? Phase 3.
- Have a designed solution? Phase 4.

For Phases 2-4, it asks for your Project State block from the previous phase. Or your previous brief. Or just your HMW and target user. Whatever you have.

**Stage 2: Extract.** You paste everything — raw interview notes, spreadsheet data, transcripts, statistics, prior briefs. The wizard parses it against 12 pattern types:

| What it finds | What it maps to |
|---------------|----------------|
| Text in quotes with attribution | Interview quote |
| Percentages + source names | Statistics |
| "How might we..." sentences | HMW question |
| Life-phase language ("early stages of," "first-time") | Target user |
| Country/city names | Geography |
| Sequential stages with arrows | Journey stages |
| Scored matrices or ranked lists | Scoring data |
| Feature descriptions | Key features (Phase 4) |
| Q:/A: blocks | FAQs (Phase 4) |

Then it shows you what it found:

```
Cluster A — Project Identity
  ✓ Topic: wellbeing of working women in India
  ✓ Target user: working women in early stages of motherhood
  ✗ Geography: not found
  ✓ Team: Team Dua

Cluster B — Research Evidence
  ✓ Quote: "She is a human before she's a mother" — Shikha Handa
  ✓ Stats: 3 found
  ✗ Methodology summary: not found

Is this correct? For the missing items — do you have them,
or should we proceed without?
```

Over-extracts and lets you correct. Never guesses silently.

**Stage 3: Fill Gaps.** Missing mandatory inputs get one focused question each. With an example. And a common mistake to avoid.

It won't ask more than 3 questions in a row without offering to just proceed.

For optional inputs, it picks the top 3 that would most improve the output:

```
These optional inputs would significantly improve your brief:
1. Three interview insights — improves Page 2 insight blocks
2. Five journey stages — improves Page 3 emotional arc
3. Draft HMW question — improves Page 4 problem statement

Want to provide any of these, or proceed without?
```

Quality nudges happen, but they're light. One nudge max per input. Never a rejection.

"Women aged 25-40" → nudge: "That's a demographic. Can you add a life phase? E.g., 'in early stages of motherhood.'"

"Build a childcare app" → nudge: "That's a solution. Frame it as a direction: 'improving childcare access.'"

**Stage 4: Confirm & Draft.** Shows an input summary. Then drafts. No extra confirmation step. The summary IS the confirmation.

At the end, you get a Project State block. Paste it back when you start the next phase. Zero infrastructure. Just copy-paste continuity.

### The skip path

Don't want the wizard? Say "just write my Phase 2."

The skill checks your message for extractable inputs:
- **>70% mandatory inputs found** — drafts with gaps flagged
- **40-70% found** — "I can draft, but Pages X-Y will be generic. Want to spend 10 minutes on the top 3 missing items?"
- **<40% found** — "I need more. Here are the 5 things that would make the biggest difference."

It never fully blocks. If you insist, it drafts with `[ASSUMPTION-BASED]` markers and reflects the gaps in self-audit scores.

### What the wizard won't do

- Ask for inputs you already provided in your paste
- Ask more than 3 questions without offering to proceed
- Reject an input (it nudges, never gates)
- Load all 4 phase specs to figure out which phase you need
- Re-ask fields that exist in your Project State block
- Force itself on you. The wizard is the recommended path, not the only path.

---

## The 5 rules

Everything else in this skill is guidance. These 5 are enforced.

| # | Rule | Why it matters |
|---|------|---------------|
| 1 | **Diamond shape.** P1 narrows, P2 expands, P3 narrows, P4 delivers. | Break this and the case study's argument doesn't work. |
| 2 | **No fabrication.** Every stat sourced. Every quote verbatim. | One fake number and your portfolio is a liability. |
| 3 | **No solution leakage.** No products or apps mentioned before Phase 4. | Naming a solution in the research phase kills design freedom. |
| 4 | **Continuity checkpoint.** Restate HMW, user, geography at each phase start. | Prevents your case study from silently drifting between rounds. |
| 5 | **Never silently resolve conflicts.** Surface contradictions, let the user choose. | Your research, your call. |

That's it. 5 constraints. Not 50.

---

## What's inside each phase

### Phase 1: Discovery Brief

The funnel phase. Every section is more specific than the last.

```
Global context → National perspective → Sub-group impact → Individual voices
→ Emotional journey → Framework → Opportunities → HMW question
```

6 mandatory inputs. 10 optional ones that make it better. ~15 minutes of conversation.

The playbook specifies everything down to paragraph length, stat pair types (disparity+severity, belief+behavior), the exact structure of insight blocks (operational + relational + emotional), and why your emotional arc needs a scope disclaimer.

12 documented failure modes. Things like: "The funnel didn't narrow." "Statistics aren't paired." "No resilience paragraph after the interview insights." "Opportunities are solutions." The skill checks against all 12 before delivering.

### Phase 2: Empathy Deepening

Takes your Phase 1 HMW and blows it open. Adds fieldwork, bodystorming, second-wave interviews.

23 inputs across 4 clusters. 5 auto-fill from your Project State. The rest come from your actual research.

Produces: filtration funnel, stakeholder map (3 rings, 15+ entities), contrasting personas, problem-space mind-map (30+ sub-issues), experience map, invalidated assumptions.

15 failure modes. The big ones: personas aren't meaningfully contrasting, stakeholder map is too thin, assumptions aren't actually invalidated with evidence.

### Phase 3: Problem Convergence

Scores candidate problems. Picks one. Maps its ecosystem. Builds the business case. Refines the HMW into sub-HMWs and a formal need statement.

31 inputs across 4 clusters. 9 carry forward automatically.

The scoring accepts any format. Spreadsheet paste, summary narratives, ranked lists. The insight matters more than the matrix.

Produces: scoring radar chart, ecosystem map, 15+ pain points, regional scenario, business viability with market data, sub-HMWs, formal need statement.

### Phase 4: Solution Design

The payoff. Names the solution. Shows the features. Presents validation data. Maps the service flow. Closes with impact.

36 inputs across 5 clusters. 9 carry forward.

This is where the stat from Phase 1 gets "reactivated" — brought back with new context to show the full arc of the research. The framework from Page 4 of Phase 1 returns to show which dimensions the solution actually addresses.

Produces: cause-effect tree, how-to questions, solution reveal, key features, service flow, FAQs, validation stats, wellbeing framework return, scalability axes.

20 failure modes. Including: "FAQs restate features instead of explaining mechanisms." "Validation data has no methodology details." "Scalability axes are just 'go to more cities.'"

---

## The playbooks are the product

People think "just give Claude the right prompt and it'll write a good case study."

Reality: Claude writes a good case study when it has a 472-line playbook telling it that Page 2's Interview Insights section needs exactly 3 insight blocks covering operational + relational + emotional flavors, each with a unique icon description and a bolded 2-4 word noun phrase, followed by a pull quote with dual-standing attribution, followed by two closing nuance paragraphs — one about a related stakeholder's perspective, one about the affected group's resilience.

Without that specificity, you get generic prose that passes a casual read but fails any reviewer who's done research themselves.

The playbooks total ~2,300 lines across 4 phases. They encode:
- Section-by-section structure with exact lengths and templates
- Voice rules (first-person plural, past for research, present for findings)
- Visual design language (coral palette, line-art icons, stat callout sizing)
- Stat pair types per section
- Failure modes with specific fixes
- Scoring benchmarks with 4 dimensions
- Worked examples showing the pattern on a different topic

These aren't getting condensed. They're the reason the output matches a specific portfolio style instead of reading like every other AI-generated case study.

---

## Scoring

Every brief self-audits on 4 dimensions before delivery:

| Dimension | Target | What it catches |
|-----------|--------|----------------|
| **AI-Likeness** | 1-3 (lower is better) | "Delve," "navigate the complexities," missing nuance moves, bolded full sentences |
| **Funnel Discipline** | 8-10 | Same-scope sections, standalone methodology section, no visible narrowing |
| **Evidence Rigor** | 8-10 | Unsourced stats, unpaired stats, fabricated numbers, vague attributions |
| **Synthesis Sharpness** | 8-10 | Broad HMW, solution-as-opportunity, flat impact list, missing scope disclaimer |

If a dimension misses its target, the skill revises before delivering. But scores are diagnostic, not a gate. The brief always ships. The scores just tell you where to push harder.

Cross-check patterns catch things individual scores miss:

- **Pretty prose + weak research** (low AI-Likeness, low Evidence) — needs more desk research, not better writing
- **Great narrative + vague landing** (high Funnel, low Synthesis) — tighten the HMW
- **Solid data + generic voice** (high Evidence, high AI-Likeness) — rewrite for voice, don't touch the data

---

## Design decisions

These came out of a 21-question council process. Four voices — Architect, Skeptic, Pragmatist, Critic — argued every constraint.

| Decision | Verdict | Why |
|----------|---------|-----|
| Solo vs. team | Solo is default | 90%+ of portfolio builders work alone |
| Geography | Agnostic | Structural patterns transfer. Cultural specifics come from user input. |
| Impact framework | Domain-dependent | Wellbeing radar works for health. Not for fintech. Let users pick. |
| No interviews? | Proceed with gaps noted | Meet users where they are. Label assumption-based sections. |
| Template vs. draft | Draft-first | Users need momentum, not another blank form. |
| State persistence | Copy-paste Project State block | Zero infrastructure. Works across sessions. |
| HMW pivots | Always allowed | A pivot means the research worked. |
| Wizard | Recommended, not required | Some users just want to paste and go. |

---

## Repo structure

```
ux-case-study-writer/
├── SKILL.md                              # Master orchestrator. 5 rules, guidance, operating procedure.
├── references/
│   ├── wizard-protocol.md                # The 4-stage input collection flow
│   ├── phase-1-discovery.md              # 472-line Phase 1 writing playbook
│   ├── phase-2-empathy.md                # 546-line Phase 2 writing playbook
│   ├── phase-3-convergence.md            # 617-line Phase 3 writing playbook
│   ├── phase-4-solution.md               # 706-line Phase 4 writing playbook
│   ├── input-checklist-phase-1.md        # 16 inputs across 3 clusters
│   ├── input-checklist-phase-2.md        # 23 inputs across 4 clusters
│   ├── input-checklist-phase-3.md        # 31 inputs across 4 clusters
│   ├── input-checklist-phase-4.md        # 36 inputs across 5 clusters
│   └── peer-review-guide.md             # Evaluation checklist for humans or AI
└── examples/
    ├── gold-standard-phase-1.md          # Full 4-page Phase 1 brief with actual prose
    ├── working-mothers-overview.md       # All 4 phases summarized (Team Dua project)
    └── adaptation-guide.md               # 3 domain adaptation sketches
```

The SKILL.md is ~190 lines. It points to everything else. Claude loads one phase spec at a time — never all 2,300 lines at once.

---

## The input math

Phase 1: 6 mandatory, 10 optional. 15 minutes.
Phase 2: 18 mandatory, 5 auto-fill from Phase 1. 20-30 minutes.
Phase 3: 22 mandatory, 9 auto-fill from prior phases. 30-40 minutes.
Phase 4: 27 mandatory, 9 auto-fill from prior phases. 30-45 minutes.

Total across all 4 phases: ~106 inputs. Sounds heavy. But 32 auto-carry from previous phases. And the wizard handles the collection so you're never staring at a blank checklist.

The honest version: more inputs = better output. All mandatory inputs only gets you a competent draft. All inputs filled gets you portfolio-grade on the first pass.

---

## Quick start

```
You: "write my case study"
Claude: "Which phase — 1, 2, 3, or 4?"
You: "1"
Claude: "Paste your Project State from a prior phase, or tell me your topic and target user."
You: [paste notes]
Claude: [extracts, shows what's found, asks about gaps]
You: [fill a few gaps]
Claude: [drafts 4-page brief with stats, visual specs, self-audit]
```

Or skip the wizard entirely:

```
You: "Phase 1. Topic: financial literacy for young professionals in India.
     Target user: first-time earners navigating independent finances.
     Geography: urban India. Solo project.
     I interviewed 4 people and here are my notes: [paste]"
Claude: [extracts inputs, drafts directly]
```

---

## Origin

Started as 4 separate case study phase skills reverse-engineered from a real design school project (Team Dua's working-mothers wellbeing case study, India).

Got consolidated into one skill. Then stress-tested through a 21-question grill and a 4-voice council debate. The council killed most of the constraints. What survived: 5 rules and a lot of detailed playbooks.

The playbooks encode a specific visual and narrative style — soft pastels, coral palette, paired statistics, progressive funnel narrowing, nuance moves after every interview section, zigzag emotional arcs with scope disclaimers. It's opinionated. That's the point.

Generic case study generators exist. This one produces output that looks like a specific team wrote it after months of research.

---

## License

MIT
