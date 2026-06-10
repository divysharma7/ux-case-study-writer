# ux-case-study-writer

> "Most UX case studies read like ChatGPT summaries with a coral palette slapped on top." — every reviewer who's read 200 portfolios

When I heard a hiring manager say this, I wanted to find out how to fix it. How does one design student ship a case study that reads like a senior team wrote it after months of research? Team Dua's working-mothers wellbeing brief — built for a real design school project — scored portfolio-grade on the first pass. The revolution is here. A single student with the right tooling can write briefs that look like a 5-person studio produced them.

I'm **Divy Sharma**, a Product Manager who's been writing case studies and watching other PMs and designers write them for years. I've reviewed dozens of portfolios — the same six failure modes show up every time. Vague HMW questions. Fabricated statistics. Solution leakage in the discovery phase. Personas that aren't meaningfully different. Stat pairs that don't pair. Emotional arcs that are flat as a board. Before this skill, I'd written four case study briefs the hard way — by hand, over 40+ hours each — and I knew exactly which paragraphs were load-bearing and which were filler.

**ux-case-study-writer is my answer.** I've been writing case studies for years, and right now I'm producing more portfolio-grade briefs than I ever have. What sits in this repo: 4 standalone phase playbooks across the full double diamond (~2,300 lines), 1 worked-example gold-standard brief, a smart triage wizard that parses messy notes into 12 input clusters, and a peer-review checklist that scores every brief on 4 dimensions. On logical case-study output — not raw word count, which AI inflates — this skill compresses what used to take 40+ hours of writing into a single afternoon of focused input collection and review. The point isn't who typed it, it's what got delivered to the portfolio.

> The AI-prose critics aren't wrong that generic case study generators inflate word counts. They are wrong that normalized-for-inflation, this skill produces less rigorous work. It produces more rigorous work, by a lot. Full methodology, scoring benchmarks, and worked examples: **[examples/round-1-gold.md](examples/round-1-gold.md)**.

Same designer. Different era. The difference is the tooling.

**ux-case-study-writer is how I do it.** It turns Claude into a virtual design research team — a Researcher who funnels global context into a sharp HMW, an Ethnographer who blows the problem space open with fieldwork and personas, a Strategist who scores candidate problems and writes the formal need statement, a Designer who names the solution and shows the validation data, a Triage Wizard who parses your messy pasted notes into 12 recognizable input clusters, and a Peer Reviewer who scores every brief on 4 dimensions before delivery. Four specialists and a wizard, all in one skill, all Markdown, all free, MIT license.

This is my open-source case-study factory. I use it every time I write a brief. I'm sharing it because these tools should be available to every design student.

Fork it. Improve it. Make it yours. And if you want to hate on free open-source design skills — you're welcome to, but I'd rather you just try it first.

**Who this is for:**
- **Design students** — especially the ones with research notes but no idea how to turn them into a brief
- **First-time Claude Code users** — structured phases instead of a blank prompt
- **Senior designers and design educators** — rigorous playbooks, scoring benchmarks, and failure modes on every brief

## Quick start

1. Install the skill (30 seconds — see below)
2. Run `write my case study` — describe your topic
3. Paste your notes — interview quotes, statistics, anything you have
4. Let the wizard extract what's there and ask for what's missing
5. Get a 4-page Phase 1 brief with stats, visual specs, and self-audit scores
6. Stop there. You'll know if this is for you.

## Install — 30 seconds

**Requirements:** [Claude Code](https://docs.anthropic.com/en/docs/claude-code), [Git](https://git-scm.com/)

### Step 1: Install on your machine

Open Claude Code and paste this. Claude does the rest.

> Install ux-case-study-writer: run **`git clone --depth 1 https://github.com/divysharma7/ux-case-study-writer.git ~/.claude/skills/ux-case-study-writer`** then add a "ux-case-study-writer" section to CLAUDE.md that says to trigger the skill on phrases like "write my case study", "case study Round N", "discovery brief", "empathy phase", "problem narrowing", or "solution brief". Then ask the user if they want a worked example walkthrough first.

### Step 2: Project mode — keep the skill versioned with your portfolio repo (recommended)

From inside your portfolio repo, paste this. Vendors the skill into the repo so collaborators and graders get the exact same version you used:

```bash
git submodule add https://github.com/divysharma7/ux-case-study-writer.git .claude/skills/ux-case-study-writer && git add .gitmodules .claude/ && git commit -m "add ux-case-study-writer skill"
```

No version drift, no "but it worked on my machine when I submitted it." Every Claude Code session in this repo gets the same playbooks, the same scoring benchmarks, the same wizard flow.

### Other AI Agents

ux-case-study-writer is just Markdown. It works anywhere an agent can read SKILL.md and follow the references. Tested on Claude Code. Should work on any agent that supports skills:

| Agent | Install to |
|-------|-------------------|
| Claude Code | `~/.claude/skills/ux-case-study-writer/` |
| OpenAI Codex CLI | `~/.codex/skills/ux-case-study-writer/` |
| OpenCode | `~/.config/opencode/skills/ux-case-study-writer/` |
| Cursor | `~/.cursor/skills/ux-case-study-writer/` |

**Want to add support for another agent?** Open an issue. It's one path, zero code changes.

## See it work

```
You:    write my case study
Claude: Which phase — 1, 2, 3, or 4? If you don't know, tell me what
        you have and I'll figure out where you are in the diamond.

You:    Topic: financial literacy for first-time earners in urban India.
        I interviewed 4 people. Here are the notes: [paste 800 words]

Claude: [extracts against 12 pattern types — quotes, stats, HMW,
        life-phase language, geography, journey stages, scoring data]

        Cluster A — Project Identity
          ✓ Topic: financial literacy for first-time earners
          ✓ Target user: first-time earners navigating independent finances
          ✓ Geography: urban India
          ✗ Team: not found

        Cluster B — Research Evidence
          ✓ Quotes: 3 found
          ✗ Statistics: not found
          ✗ Methodology summary: not found

        Is this correct? For the missing items — do you have them,
        or should we proceed without?

You:    Solo project. I don't have stats — can you find some?

Claude: [searches for current statistics from named sources, dates them]
        [drafts 4-page Phase 1 Discovery Brief with paired stats,
         emotional arc, framework page, opportunities, HMW question]
        [self-audits on 4 dimensions, flags weakest, delivers]

        Project State block ready. Paste it back when you start Phase 2.

You:    /peer-review
        [reads the brief, scores it, highlights the 3 sections to push
         harder on, names specific paragraphs that read AI-generic]
```

You said "write my case study." The skill said "let me extract what you actually have, then write a 4-page brief with sourced statistics and a self-audit" — because it listened to your research, not your request for a template. End to end, one paste. That is not a generator. That is a team.

## The diamond

ux-case-study-writer is a process, not a template. The phases run in the order the double diamond runs:

**Discover → Empathize → Converge → Deliver**

Each phase feeds into the next. Phase 1 writes the HMW that Phase 2 opens back up. Phase 2 produces the personas that Phase 3 scores into a single problem. Phase 3 writes the formal need statement that Phase 4 turns into a named solution. Nothing falls through the cracks because every phase knows what came before it via a copy-pasted Project State block.

| Phase | Your specialist | What they do |
|-------|----------------|--------------|
| **Phase 1: Discovery Brief** | **The Researcher** | Start here. Funnels global context into a sharp HMW question. Six mandatory inputs, ten optional ones that make it better. 4-page brief with paired statistics, emotional arc, framework, and opportunities. 12 documented failure modes. The skill checks against all 12 before delivering. |
| **Phase 2: Empathy Deepening** | **The Ethnographer** | Takes the Phase 1 HMW and blows it open. Adds fieldwork, bodystorming, second-wave interviews. 23 inputs across 4 clusters; 5 auto-fill from Phase 1. Produces filtration funnel, stakeholder map (3 rings, 15+ entities), contrasting personas, problem-space mind-map (30+ sub-issues), experience map, invalidated assumptions. |
| **Phase 3: Problem Convergence** | **The Strategist** | Scores candidate problems, picks one, maps its ecosystem, builds the business case, refines the HMW into sub-HMWs and a formal need statement. 31 inputs across 4 clusters; 9 carry forward automatically. Accepts any scoring format — spreadsheet paste, ranked lists, summary narratives. The insight matters more than the matrix. |
| **Phase 4: Solution Design** | **The Designer** | The payoff. Names the solution. Shows the features. Presents validation data with methodology. Maps the service flow. Closes with the impact framework return. 36 inputs across 5 clusters; 9 carry forward. This is where the stat from Phase 1 gets reactivated to show the full arc of the research. |
| **The Wizard (triage)** | **Smart Triage** | Parses your pasted mess against 12 pattern types: quotes, stats, HMW sentences, life-phase language, country names, journey stages, scoring matrices, feature descriptions, FAQs, and more. Shows ✓/✗/~ per cluster. Never guesses silently. Three messages, max. |
| **Peer Review** | **The Reviewer** | Scores every brief on 4 dimensions before delivery: AI-Likeness (lower is better), Funnel Discipline, Evidence Rigor, Synthesis Sharpness. Flags the weakest dimension with a specific fix. Diagnostic, not a gate — the brief always ships. |

### Which phase should I use?

| You have... | Phase to run | Why |
|-------------|--------------|-----|
| **No prior research** | Phase 1 | Start at the start of the diamond. |
| **An HMW but no fieldwork** | Phase 2 | You've defined; now empathize. |
| **Personas but haven't picked a problem** | Phase 3 | You've empathized; now converge. |
| **A designed solution** | Phase 4 | You've converged; now deliver. |
| **All of the above** | Run them in sequence, paste the Project State block between phases. |

### The 5 rules

Everything else in this skill is guidance. These 5 are enforced.

| # | Rule | Why it matters |
|---|------|---------------|
| 1 | **Diamond shape.** P1 narrows, P2 expands, P3 narrows, P4 delivers. | Break this and the case study's argument doesn't work. |
| 2 | **No fabrication.** Every stat sourced. Every quote verbatim. | One fake number and your portfolio is a liability. |
| 3 | **No solution leakage.** No products or apps named before Phase 4. | Naming a solution in the research phase kills design freedom. |
| 4 | **Continuity checkpoint.** Restate HMW, user, geography at each phase start. | Prevents your case study from silently drifting between phases. |
| 5 | **Never silently resolve conflicts.** Surface contradictions, let the user choose. | Your research, your call. |

That's it. 5 constraints. Not 50.

### Karpathy's four failure modes? Already covered.

Andrej Karpathy's coding rules nail four failure modes: wrong assumptions, overcomplexity, orthogonal edits, imperative over declarative. ux-case-study-writer enforces the case-study equivalents. The wizard forces hidden assumptions into the open before the brief is drafted (rule 5: surface contradictions). The 4-phase split prevents overcomplexity by loading one playbook at a time. The Project State block prevents orthogonal edits across phases — if the HMW drifts, the continuity checkpoint catches it. And the playbooks are declarative: they specify what each section IS, not how to write each sentence. If you already use Karpathy-style rules for code, ux-case-study-writer is the equivalent enforcement layer for design-thinking writing.

### Power tools

| Component | What it does |
|-----------|-------------|
| `references/wizard.md` | **Smart Triage** — the 4-stage input collection flow. Triage → Extract → Fill Gaps → Confirm & Draft. Parses messy paste against 12 pattern types. Never blocks, never silently guesses. |
| `references/peer-review.md` | **Second Opinion** — independent peer review checklist for humans or AI. Run it after the self-audit to catch what the self-audit missed. |
| `rounds/0N-*/inputs.md` | **Input Manifest** — the full input list per phase, organized by cluster. Auto-fill markers show which inputs carry over from prior phases. |
| `examples/round-1-gold.md` | **Worked Example** — full 4-page Phase 1 brief with actual prose. The pattern you're matching. |
| `examples/working-mothers-overview.md` | **End-to-End Walkthrough** — all 4 phases of Team Dua's working-mothers project, summarized so you can see how Phase 1 feeds Phase 4. |
| `examples/adaptation-guide.md` | **Domain Adaptation** — 3 sketches showing how the structural patterns transfer across geographies and domains (health, fintech, climate). |

## Parallel briefs

ux-case-study-writer works well with one brief. It gets interesting with four phases of the same project running in parallel review.

**Research is at the heart.** The Researcher specialist (Phase 1) builds the foundation. Every downstream phase quotes from it. The HMW it produces is the load-bearing sentence in the entire case study. Get this wrong and everything that follows compounds the error.

**The wizard is how you collect inputs without the blank-form anxiety.** You describe what you have. It parses your paste against 12 pattern types. Then it shows you what it found in a ✓/✗/~ grid, asks one focused question per missing mandatory input (with an example, and a common mistake to avoid), and gives you the top 3 optional inputs that would most improve the output. Quality nudges happen, but they're light. One nudge max per input. Never a rejection. "Women aged 25-40" → nudge: "That's a demographic. Can you add a life phase? E.g., 'in early stages of motherhood.'" "Build a childcare app" → nudge: "That's a solution. Frame it as a direction: 'improving childcare access.'"

**The playbooks are the product.** People think "just give Claude the right prompt and it'll write a good case study." Reality: Claude writes a good case study when it has a 472-line playbook telling it that Page 2's Interview Insights section needs exactly 3 insight blocks covering operational + relational + emotional flavors, each with a unique icon description and a bolded 2-4 word noun phrase, followed by a pull quote with dual-standing attribution, followed by two closing nuance paragraphs — one about a related stakeholder's perspective, one about the affected group's resilience. Without that specificity, you get generic prose that passes a casual read but fails any reviewer who's done research themselves. The playbooks total ~2,300 lines across 4 phases. They're the reason the output matches a specific portfolio style instead of reading like every other AI-generated case study.

**The diamond shape is what makes the case study argue.** Without the shape, four phases is four sources of chaos. With the shape — discover, empathize, converge, deliver — each phase knows exactly what to do and when to stop. You manage them the way a CEO manages a team: check in on the decisions that matter (HMW pivots, persona contrast, scoring rationale, solution naming), let the rest run.

**Self-audit on every brief.** Every phase self-audits on 4 dimensions before delivery: AI-Likeness, Funnel Discipline, Evidence Rigor, Synthesis Sharpness. If a dimension misses its target, the skill revises before delivering. But scores are diagnostic, not a gate. The brief always ships. The scores just tell you where to push harder.

**Cross-check patterns catch things individual scores miss.** Pretty prose + weak research (low AI-Likeness, low Evidence) — needs more desk research, not better writing. Great narrative + vague landing (high Funnel, low Synthesis) — tighten the HMW. Solid data + generic voice (high Evidence, high AI-Likeness) — rewrite for voice, don't touch the data.

**The wizard isn't the only path.** Don't want it? Say "just write my Phase 2." The skill checks your message for extractable inputs and decides: >70% mandatory inputs found → drafts with gaps flagged. 40-70% found → "I can draft, but Pages X-Y will be generic. Want to spend 10 minutes on the top 3 missing items?" <40% found → "I need more. Here are the 5 things that would make the biggest difference." It never fully blocks. If you insist, it drafts with `[ASSUMPTION-BASED]` markers and reflects the gaps in the self-audit scores.

**Solo is the default.** 90%+ of portfolio builders work alone. If team members are named, team elements (credit line, multi-scorer radar) activate. Solo users never get blocked on missing team inputs.

**Geography-agnostic by default.** The structural patterns (funnel, personas, scoring, HMW) are universal. Cultural scripts, data sources, and regulatory context adapt to the user's stated geography. Hardcoded India assumptions are explicitly called out as a gotcha in SKILL.md.

**HMW pivots are always allowed.** A pivot means the research worked. The skill notes what changed and flags which prior-phase artifacts may need updating. It doesn't force a full restart for a scope adjustment.

## What the wizard won't do

- Ask for inputs you already provided in your paste
- Ask more than 3 questions in a row without offering to proceed
- Reject an input (it nudges, never gates)
- Load all 4 phase specs to figure out which phase you need
- Re-ask fields that exist in your Project State block
- Force itself on you. The wizard is the recommended path, not the only path.

## The input math

Phase 1: 6 mandatory, 10 optional. 15 minutes.
Phase 2: 18 mandatory, 5 auto-fill from Phase 1. 20-30 minutes.
Phase 3: 22 mandatory, 9 auto-fill from prior phases. 30-40 minutes.
Phase 4: 27 mandatory, 9 auto-fill from prior phases. 30-45 minutes.

Total across all 4 phases: ~106 inputs. Sounds heavy. But 32 auto-carry from previous phases. And the wizard handles the collection so you're never staring at a blank checklist.

The honest version: more inputs = better output. All mandatory inputs only gets you a competent draft. All inputs filled gets you portfolio-grade on the first pass.

## Uninstall

### Option 1: Remove the skill directory

```bash
rm -rf ~/.claude/skills/ux-case-study-writer
```

### Option 2: Per-project cleanup

If you vendored it into a portfolio repo with `git submodule`:

```bash
git submodule deinit .claude/skills/ux-case-study-writer
git rm .claude/skills/ux-case-study-writer
rm -rf .git/modules/.claude/skills/ux-case-study-writer
git commit -m "remove ux-case-study-writer skill"
```

### Clean up CLAUDE.md

The uninstall does not edit CLAUDE.md. In each project where the skill was added, remove the `## ux-case-study-writer` section.

---

Free, MIT licensed, open source. No premium tier, no waitlist.

I open-sourced how I write case studies. You can fork it and make it your own.

> **Contributions welcome.** PRs that add worked examples in new domains (fintech, climate, healthcare), tighten failure-mode catalogs, or improve the wizard's pattern recognition are especially helpful. Open an issue first if it's a larger change.

## Repo structure

```
ux-case-study-writer/
├── SKILL.md                              # Master orchestrator. 5 rules, guidance, operating procedure.
├── rounds/
│   ├── 01-discovery/
│   │   ├── playbook.md                   # 472-line Phase 1 writing playbook
│   │   └── inputs.md                     # 16 inputs across 3 clusters
│   ├── 02-empathy/
│   │   ├── playbook.md                   # 546-line Phase 2 writing playbook
│   │   └── inputs.md                     # 23 inputs across 4 clusters
│   ├── 03-convergence/
│   │   ├── playbook.md                   # 617-line Phase 3 writing playbook
│   │   └── inputs.md                     # 31 inputs across 4 clusters
│   └── 04-solution/
│       ├── playbook.md                   # 706-line Phase 4 writing playbook
│       └── inputs.md                     # 36 inputs across 5 clusters
├── references/
│   ├── wizard.md                         # The 4-stage input collection flow
│   └── peer-review.md                    # Evaluation checklist for humans or AI
└── examples/
    ├── round-1-gold.md                   # Full 4-page Phase 1 brief with actual prose
    ├── working-mothers-overview.md       # All 4 phases summarized (Team Dua project)
    └── adaptation-guide.md               # 3 domain adaptation sketches
```

The SKILL.md is ~190 lines. It points to everything else. Claude loads one phase spec at a time — never all 2,300 lines at once.

## Docs

| Doc | What it covers |
|-----|---------------|
| [SKILL.md](SKILL.md) | The 5 hard constraints, guidance, operating procedure |
| [Wizard Protocol](references/wizard.md) | The 4-stage input collection flow with the 12 pattern types |
| [Peer Review Guide](references/peer-review.md) | Evaluation checklist for humans or AI |
| [Gold Standard Example](examples/round-1-gold.md) | Full 4-page Phase 1 brief with actual prose |
| [Working Mothers Walkthrough](examples/working-mothers-overview.md) | All 4 phases of Team Dua's project |
| [Adaptation Guide](examples/adaptation-guide.md) | 3 domain adaptation sketches |

## Privacy & Telemetry

ux-case-study-writer is pure Markdown. There is no telemetry, no analytics, no phone-home. The skill runs entirely inside your Claude Code session. Your research notes, interview quotes, and draft briefs never leave your machine — unless you paste them somewhere yourself.

- **Default is off, because there is no default-on.** Nothing is sent anywhere, ever.
- **What's collected:** nothing.
- **What's stored:** nothing.
- **Change anytime:** N/A, because there's nothing to change.

If you want analytics, run Claude Code's built-in usage tools. This skill adds nothing on top.

## Troubleshooting

**Skill not triggering?** Make sure your project's `CLAUDE.md` mentions the skill or that you typed one of the trigger phrases ("write my case study", "case study Round N", "discovery brief", "empathy phase", "problem narrowing", "solution brief").

**Wizard asking too many questions?** Tell it: "just write my Phase 1 with what I gave you." It will draft with `[ASSUMPTION-BASED]` markers and reflect the gaps in self-audit scores.

**Output reads AI-generic?** Run `references/peer-review.md` against it. Look at the AI-Likeness dimension. Common fix: rewrite for voice, don't touch the data. Look for "delve," "navigate the complexities," "in today's fast-paced world," "comprehensive," "holistic," "robust" as filler — those are the tells.

**Stats fabricated or unsourced?** That's a Rule 2 violation. Tell Claude: "remove every stat without a named source and a date." Then provide the missing ones or proceed with fewer.

**Solution leaked in Phase 1 or 2?** That's a Rule 3 violation. Tell Claude: "rewrite opportunities as directions, not products. No app names, no platform names, no specific solutions before Phase 4."

**HMW drifted between phases?** That's a Rule 4 violation. Tell Claude: "restate the HMW from the prior Project State block and acknowledge what changed."

**Claude says it can't see the skill?** Make sure your project's `CLAUDE.md` has a section like this:

```
## ux-case-study-writer
Trigger on: "write my case study", "case study Round N", "discovery brief",
"empathy phase", "problem narrowing", "solution brief", "design my portfolio
case study", or any request for a structured design-thinking deliverable.
Skill location: ~/.claude/skills/ux-case-study-writer/SKILL.md
```

## License

MIT. Free forever. Go write something portfolio-grade.
