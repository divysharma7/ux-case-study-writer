# Wizard Protocol

The conversational layer that collects structured inputs from users before drafting. This protocol sits on top of the per-phase input checklists — it doesn't replace them.

## Universal Flow

Every wizard invocation follows 4 stages regardless of phase:

```
TRIAGE → EXTRACT → FILL GAPS → CONFIRM & DRAFT
```

---

## Stage 1: Triage

Three messages, max. Don't over-explain.

### Message 1 — Identify the phase

Ask: "Which phase are you working on — 1 (Discovery), 2 (Empathy), 3 (Convergence), or 4 (Solution)?"

If user says "not sure" or describes their project without naming a phase:
- Has no prior research → Phase 1
- Has an HMW but no fieldwork → Phase 2
- Has fieldwork + personas but hasn't picked a problem → Phase 3
- Has a chosen problem + need statement but no solution → Phase 3 (late) or Phase 4
- Has a designed solution → Phase 4

### Message 2 — Continuity (Phases 2-4 only)

Ask: "Paste your Project State from the previous phase. If you don't have one, paste your previous brief or tell me your HMW and target user."

Parse the paste for continuity fields:
- HMW question
- Target user
- Geography
- Team / solo
- Framework + focus dimensions
- Key artifacts from prior phases (personas, chosen problem, need statement)

Show what was found, confirm with user. If fields are missing, ask directly — these are non-negotiable for Phases 2-4.

### Message 3 — The big paste

Ask: "Now paste everything you have for this phase — raw notes, interview transcripts, statistics, spreadsheet data, whatever format. I'll extract what I can and show you what's missing."

If the user has nothing to paste, skip to Stage 3 (Fill Gaps).

---

## Stage 2: Extract

Parse the user's paste against these patterns:

| Pattern | Maps to |
|---------|---------|
| Text in quotation marks with `—` or `-` attribution | Interview quote |
| Percentages or fractions + a source/study/report name | Statistics |
| "How might we..." or "HMW" sentences | HMW question |
| "Team X: Name, Name, Name" or similar | Team credit |
| Life-phase language ("in early stages of," "recently," "first-time," "transitioning") | Target user |
| Country/city/region names + cultural references | Geography |
| Numbered or bulleted problem lists | Problem-space inventory |
| Pros/cons format with a service name | Existing service audit |
| Sequential stages with arrows or numbers | Journey stages or filtration funnel |
| Scored matrices, ranked lists, or comparison tables | Scoring data |
| Feature descriptions with mechanism language | Key features (Phase 4) |
| "Q:" / "A:" or FAQ-formatted blocks | FAQs (Phase 4) |

### Extraction rules

- **Extract generously, confirm explicitly.** Over-extract and let the user correct.
- **Never silently resolve ambiguity.** If a paste contains two possible HMW questions, show both: "I found two HMW candidates — (a) '...' (b) '...'. Which is current?"
- **Tag confidence.** Mark extractions as high-confidence (clear pattern match) or needs-confirmation (inferred from context).

### Extraction output format

Show the user what mapped to each cluster:

```
Here's what I found:

Cluster A — Project Identity
  ✓ Topic: [extracted value]
  ✓ Target user: [extracted value]
  ✗ Geography: not found
  ✓ Team: [extracted value]

Cluster B — Research Evidence
  ✓ Quote: "[extracted]" — [attribution]
  ✓ Stats: 3 found ([brief list])
  ✗ Methodology summary: not found

Cluster C — Synthesis
  ✓ HMW: [extracted]
  ~ Journey stages: possibly found, needs confirmation
  ✗ Opportunity areas: not found

Is this correct? For the missing items — do you have them,
or should we proceed without?
```

Use ✓ (found), ✗ (missing), ~ (needs confirmation).

---

## Stage 3: Fill Gaps

For each missing input, decide whether to ask or skip based on this priority:

### Priority 1 — Ask immediately (missing mandatory, high impact)

Ask one focused question per input. Include one good example and one common mistake.

Format:
```
[Input name]: [What I need in one sentence]

Example: "[concrete example from this phase's checklist]"
Common mistake: "[what to avoid]"
```

Don't ask more than 3 mandatory questions in a row without checking if the user wants to continue or proceed with gaps.

### Priority 2 — Ask if willing (missing optional, high impact)

After mandatory gaps are addressed, ask about the top 3 highest-impact optional inputs for this phase:

```
These optional inputs would significantly improve your brief:
1. [Input] — improves [which section]
2. [Input] — improves [which section]
3. [Input] — improves [which section]

Want to provide any of these, or proceed without?
```

### Priority 3 — Skip silently (missing optional, low impact)

Don't ask. Note in the input summary as "not provided" and proceed.

### Quality validation during gap-filling

When the user provides an input, run a light quality check. One nudge max per input, never a rejection:

| Input | Check for | Nudge |
|-------|-----------|-------|
| Target user | Life-phase language present | "'Women aged 25-40' is a demographic. Can you add a life phase? E.g., 'in early stages of motherhood'" |
| HMW question | Soft verb + scoped user + aspirational outcome | "Strong HMWs use 'help' not 'fix', and name a life phase, not just a role" |
| Interview quote | Verbatim with attribution | "Is this a direct quote? Add the speaker's name and role if possible" |
| Opportunity areas | Directions, not solutions | "This sounds like a specific product. Can you frame it as a direction? E.g., 'improving X' instead of 'building an app for X'" |
| Statistics | Named source present | "What's the source for this number?" |
| Journey stages | Life phases, not emotions | "'Stressed' is a feeling. What life event caused it? That's your stage name" |
| Personas | Meaningful contrast axis | "Both personas look similar. What's the key difference — class, family type, geography?" |
| Need statement | Qualities, not product form | "This names a solution ('an app that...'). Rephrase as qualities: 'a reliable service that prioritises...'" |
| FAQ answers | Mechanism, not policy | "How specifically does this work? Name the feature or process, not just 'we ensure safety'" |

---

## Stage 4: Confirm & Draft

### Input summary

Output a compact confirmation block before drafting:

```markdown
## Input Summary — Phase N Ready

### Cluster A: [Name] ✓
- [field]: [value]
- [field]: [value]

### Cluster B: [Name] ✓
- [field]: [value]
- [field]: [value]

### Cluster C: [Name] ⚠ (N optional items missing)
- [field]: [value]
- Missing: [list]

---
Proceeding to draft Phase N...
```

### Then draft

Load the active phase's spec (`rounds/0N-*/playbook.md`) and draft directly. Don't ask for additional confirmation — the input summary IS the confirmation.

### After drafting — output Project State

At the end of every phase output, append a Project State block:

```markdown
---
## Project State — Phase N Complete

**HMW:** "[current question]"
**Target user:** [current definition]
**Geography:** [current context]
**Team:** [names, or "solo"]
**Framework:** [type] — focus: [dimensions]

### Key Artifacts This Phase
- [List the major artifacts produced: emotional arc, personas, chosen problem, etc.]

### Continuity Notes
- [Any pivots, scope changes, or assumption updates from this phase]

---
Paste this block when starting Phase N+1.
```

---

## Phase-Specific Cluster Definitions

### Phase 1: Discovery Brief (16 inputs → 3 clusters)

**Cluster A — Project Identity** (4 inputs, all mandatory)
1. Topic / problem domain
2. Target user (role + life phase)
3. Geography / regional context
4. Team name + members (or "solo")

**Cluster B — Research Evidence** (4 inputs: 2 mandatory, 2 optional)
5. Research methodology summary [mandatory]
6. Strong interview quote with attribution [mandatory]
7. Story of why the team chose this problem [optional, high-value]
8. Pre-found statistics with citations [optional, high-value]

**Cluster C — Synthesis Artifacts** (8 inputs: all optional but high-value)
9. Three interview insights (operational + relational + emotional)
10. Five journey stages with key touchpoints
11. Trajectory shape preference
12. Framework + focus dimensions
13. Draft HMW question
14. "Why now" structural shift
15. Three opportunity area sketches
16. Visual style preferences

**Phase 1 honest framing:** "This phase needs about 15 minutes of conversation. I need 6 things from you — the rest makes the output better but isn't required."

---

### Phase 2: Empathy Deepening (23 inputs → 4 clusters)

**Cluster A — Continuity** (5 inputs, auto-filled from Project State)
1. Round 1 HMW question
2. Target user
3. Geography
4. Team
5. Visual style

**Cluster B — Structural Research** (7 inputs, all mandatory)
6. Filtration funnel stages (6-8 stages)
7. Intersectional widening (harsher sub-population)
8. Cultural scripts (2-3 norms)
9. Cultural-scenario pull quote with attribution
10. Existing service audit (1 named service, pros/cons)
11. Other named policies and services (3-6)
12. Field visit notes [optional but high-value]

**Cluster C — Stakeholder Ecosystem** (4 inputs, all mandatory)
13. Stakeholder map (15+ across CORE/INVOLVED/INFORMED)
14. Stakeholder quotes (5 from 4+ distinct roles)
15. Problem-space inventory (5-8 categories, 3-8 sub-issues each)
16. Discoveries — 2-3 new statistics [optional]

**Cluster D — Empathy Artifacts** (7 inputs, all mandatory except noted)
17. Day-in-the-life observations (6 stages x 4 layers)
18. Bodystorming session record (or "NOT CONDUCTED")
19. Persona A (full profile + goals + motivations + painpoints)
20. Persona B (contrasting, full profile)
21. Three invalidated assumptions with evidence
22. Closing scope re-affirmation
23. Visual style continuity notes [optional]

**Phase 2 honest framing:** "This phase requires real fieldwork. I'll walk through 4 topic areas with about 15 mandatory items. Some you'll paste, some we'll discuss. Takes 20-30 minutes."

---

### Phase 3: Problem Convergence (31 inputs → 4 clusters)

**Cluster A — Continuity** (9 inputs, auto-filled from Project State)
1. Round 1 HMW (verbatim)
2. Round 2 problem categories
3. Target user
4. Geography
5. Team
6. Round 2 stakeholder map
7. Round 2 existing-services audit
8. Round 2 personas
9. Visual style

**Cluster B — Problem Selection** (6 inputs, all mandatory)
10. 6-8 candidate problems for scoring
11. Scoring criteria (default 7 provided)
12. Scoring data (any format — spreadsheet, summary, rankings)
13. Chosen problem + reasoning
14. 2 rejected problems + reasoning each
15. Pull quote for chosen problem

**Cluster C — Ecosystem Deep-Dive** (8 inputs, all mandatory)
16. Ecosystem map themes (5-7)
17. Ecosystem map data per theme (needs, touchpoints, stakeholders)
18. Inter-theme linkages (4+ with mechanisms)
19. Pain points list (15+ specific to existing service)
20. 2 pull quotes specific to existing service
21. Regional scenario for chosen problem
22. Setbacks of existing service with quantified failure data
23. Field visit notes [optional]

**Cluster D — Synthesis & Framing** (8 inputs, all mandatory)
24. 5 impact statements (individual → society ripple)
25. Business viability — 3 market arguments
26. 2 hard market data points with source
27. 3 refined sub-HMW questions
28. Formal need statement (User + Need + Insight)
29. Team credit line
30. Pre/post-discussion scoring data [optional]
31. Source links for market data [optional]

**Phase 3 honest framing:** "This is the heaviest input phase. You'll need scoring data, market research, and ecosystem mapping — about 18 mandatory items. But 9 carry forward from prior phases automatically. Takes 30-40 minutes."

---

### Phase 4: Solution Design (36 inputs → 5 clusters)

**Cluster A — Continuity** (9 inputs, auto-filled from Project State)
1. Round 1 framework + focus dimensions
2. Round 2 hero stat
3. Round 3 need statement (verbatim)
4. Round 3 chosen problem area
5. Round 3 sub-HMWs
6. Round 3 market data
7. Target user
8. Geography
9. Team

**Cluster B — Research Synthesis** (5 inputs, all mandatory)
10. Project journey recap paragraph
11. 5 macro causes for cause-and-effect tree
12. Sub-causes off the focused cause (5-8)
13. Hero stat to reactivate from prior rounds
14. Round 3 need statement (verbatim confirmation)

**Cluster C — Ideation & Validation** (7 inputs, all mandatory)
15. 12+ how-to questions across multiple angles
16. Current scenario → challenges → vision triple
17. Co-creation methodology details
18. A/B testing methodology details
19. 3 hero validation statistics
20. Challenges conquered (3-5 research-execution challenges)
21. Co-creation session notes [optional]

**Cluster D — Solution Design** (6 inputs, all mandatory)
22. Solution name with built-in meaning
23. Concept description paragraph (3-5 sentences)
24. Primary stakeholders (3-4)
25. 5 key features (each with mechanic + emotional outcome)
26. Service flow (9-12 steps)
27. 6-8 FAQs with mechanism-explaining answers

**Cluster E — Impact & Close** (9 inputs, all mandatory except noted)
28. 12-15 benefits for word cloud (with weighting)
29. Framework return paragraph
30. 5 impact statements (each tied to a feature)
31. 3 scalability directions (distinct growth axes)
32. Closing emotional statement
33. Team credit line
34. A/B testing results breakdown [optional]
35. Visual style notes for isometric illustration [optional]
36. References to Round 2 personas [optional]

**Phase 4 honest framing:** "This phase presents your actual solution. I need 23 inputs — but 9 carry forward from prior phases. You'll need your ideation work, testing data, and fully designed solution ready. Takes 30-45 minutes."

---

## Skip Path (Implicit Triage)

When the user bypasses the wizard ("just write my Phase 2"):

1. Check if their message contains a Project State block or prior brief → extract continuity
2. Check if their message contains any extractable inputs → parse them
3. Assess coverage:
   - **>70% mandatory inputs found** → draft with gaps flagged
   - **40-70% found** → "I can draft this, but Pages [X-Y] will be generic. Want to spend 10 minutes on [top 3 missing items]?"
   - **<40% found** → "I need more to work with. Here are the [N] things that would make the biggest difference: [list top 5]"
4. Never fully block. If the user insists, draft with `[ASSUMPTION-BASED]` markers on thin sections and reflect input gaps in the self-audit scores.

---

## Anti-Patterns

- Asking for inputs the user already provided in their paste
- Asking more than 3 questions in a row without offering to proceed
- Rejecting an input instead of nudging with an example
- Loading all 4 phase specs to decide which phase the user needs
- Re-asking continuity fields that exist in the Project State block
- Treating the wizard as mandatory — it's the recommended path, not the only path
