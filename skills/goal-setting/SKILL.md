---
name: goals-setting
description: Produces a structured goals document for senior professionals — annual, quarterly, and monthly SMART goals that serve both their current role and their career trajectory. Activate when the user mentions goal setting, OKRs, goals for the year, quarterly goals, monthly goals, performance goals, career goals, or runs /careerpowers goals. Also activate proactively if context.yml mentions an upcoming review cycle or the user seems uncertain about what to focus on.
---

# Goals Setting Skill

Produce a structured goals document that gives a senior professional clear, actionable goals across three time horizons — annual, quarterly, and monthly — that serve both their current role and their longer-term career trajectory.

## What makes this different from a standard goals exercise

Most goals documents are written for the employer. They optimize for what the company needs from the person right now. careerpowers goals are written for the person — they're designed to make them excellent at their current job *and* build career capital simultaneously. Every goal should serve both masters.

A good goals document from this skill answers: "If I hit all of these, what have I become by the end of the year?" The answer should be: better at my job, and more valuable beyond it.

---

## Step 1: Load career profile

Read `career-profile/cv.md` and `career-profile/context.yml` (if present) via the career-profile skill.

---

## Step 2: Gather goals-specific context

This skill needs more input than the others because goals without context are just wishes. Ask up to **four targeted questions** — this is the one skill where the extra question is worth it.

**Always ask:**
- "What are your company or team's main priorities for this period? Share OKRs, a strategy doc, your manager's last all-hands takeaway — anything that tells me what the organization is optimizing for right now."

**Then pick the two most relevant from:**
- "What does success look like for you in this role 12 months from now — in your manager's eyes, and in yours?"
- "What's the one thing you keep not making time for that you know would matter most?"
- "Is there a skill, relationship, or type of work you want to deliberately build this year — even if it's not in your job description?"
- "What time horizon matters most right now — are you thinking about this quarter, this year, or longer?"
- "Do you have an existing goals framework your company uses (OKRs, MBOs, SMART, etc.)? Should I align to that format?"

If `context.yml` exists and covers some of this, use it. Don't ask what you already know.

---

## Step 3: Analyze before writing

Before producing the document, reason through:

1. **What the company needs**: From their description of org priorities — what does the organization need from someone in this role right now?
2. **What their career needs**: From their profile and context — what would genuinely advance their trajectory, not just their performance rating?
3. **The overlap**: Where do these two align? These are the highest-leverage goals — they satisfy the employer and build the person simultaneously.
4. **The tension**: Where do they diverge? Flag this honestly. Sometimes a goal that's great for the company is neutral or even negative for career capital (pure execution work with no learning, visibility, or compounding value). The person deserves to know.

Hold this analysis internally — it informs the goals but isn't presented as a framework breakdown.

---

## Step 4: Produce the goals document

Save to `output/goals-[period]-[date].md`.

### Document structure

---

# Goals — [Period: e.g., 2026 / Q2 2026]
**[Name if known] · [Role] · [Date]**

---

## The through-line

One paragraph. The connective tissue across all the goals below — what kind of professional they're becoming this period, not just what they're delivering. Written in second person.

This is the "so what" of the whole document. If they read nothing else, this paragraph should tell them what they're building toward.

---

## Annual goals

2–3 goals maximum. These are the big bets — significant enough that hitting them would meaningfully change something about their capabilities, reputation, or trajectory.

Each goal follows this structure:

**[Goal title — specific, not generic]**
- **What**: The specific outcome, defined precisely enough that both they and their manager would agree whether it was achieved
- **Why it matters for the role**: Connection to company/team priorities
- **Why it matters for your career**: What capital it builds — depth, reach, signal, network, optionality, or momentum
- **How you'll know**: 1–2 measurable indicators of success
- **The risk**: What's most likely to get in the way

Do not write more than 3 annual goals. More than 3 means none of them are real priorities.

---

## Quarterly goals

3–5 goals for the current or upcoming quarter. These are milestones that move the annual goals forward, plus any time-sensitive priorities that matter now but aren't year-long commitments.

Each goal:

**[Goal title]**
- **What by when**: Specific outcome + deadline within the quarter
- **Connects to**: Which annual goal this serves (or why it stands alone)
- **Done looks like**: One concrete definition of completion

---

## Monthly focus

The single most important thing to make progress on this month. Not a goal — a focus. One paragraph, written directly.

This changes each month. The document should be revisited monthly and this section updated. Everything else can stay stable for the quarter.

---

## One goal that's purely yours

A goal that serves their career trajectory regardless of what their employer needs. Could be writing something, building a relationship, learning something, shipping a side project, speaking somewhere.

Written separately from the work goals because it deserves its own space. Not optional — this is the compounding investment in themselves.

Format:
**[What]** — [Why this, why now. 2 sentences.]

---

## What to protect

The conditions, boundaries, or commitments they need to maintain to actually hit these goals. Not a wishlist — the 2–3 things that, if they erode, the whole goals document becomes fiction.

Examples: protected deep work time, a weekly 1:1 with their manager, not taking on a fourth direct report before Q3.

---

## Review cadence

A simple reminder:

- **Monthly**: Update the monthly focus section. Check quarterly progress.
- **Quarterly**: Review quarterly goals, set next quarter's. Adjust annual goals if context has changed significantly.
- **Annually**: Full reset. Run `/careerpowers goals` again with the new year's context.

---

## Calibration notes

- **SMART but not sterile**: Goals should be specific and measurable, but written in human language. "Become the person my team calls when X goes wrong" is a better goal than "improve incident response by 20%."
- **Fewer is better**: Push back if they want more than 3 annual goals. That's not ambition, that's avoidance of prioritization.
- **The career goal is non-negotiable**: Don't let it get cut. It's often the first thing people remove under pressure, and it's the one that compounds.
- **Be honest about tension**: If a goal is good for the company but builds no career capital, say so. Let them decide with full information.
- **Length**: 2 pages maximum. If it doesn't fit in 2 pages, the goals are too many or too verbose. A document people actually read monthly has to be short enough to read in 3 minutes.
