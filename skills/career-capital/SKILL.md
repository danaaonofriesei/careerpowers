---
name: career-capital
description: Produces a career capital snapshot for senior professionals — a plain-language assessment of what they've built, where their leverage actually sits, and where the gaps are. Activate when the user mentions career capital, what they're worth, their strengths, career assets, leverage, career audit, or wants to understand their career as a whole. Also activate proactively when someone seems uncertain about their value or direction despite a strong background.
---

# Career Capital Skill

Produce a capital snapshot — a plain-language assessment of what this person has genuinely built over their career, where their real leverage sits, and where the honest gaps are.

## What this is not

Not a LinkedIn skills section. Not a list of accomplishments. Not flattery dressed up as analysis.

Career capital is the accumulated set of things that make someone valuable *beyond their current job title* — and that compounds over time. This skill makes that visible.

## The six dimensions

Assess the user across these six dimensions. These are diagnostic lenses, not scores. Output is plain language, not numbers.

### 1. Depth
*What they know better than most people*

Domain expertise, hard-won knowledge, pattern recognition built from doing something hard for a long time. This is the knowledge that takes years and can't be Googled.

Questions to probe: What do they know that someone 5 years junior couldn't know yet? Where are they genuinely in the top tier?

### 2. Reach
*How far their influence actually extends*

Beyond their direct reports or immediate team — cross-functional influence, external reputation, industry presence, how often they're pulled into decisions outside their formal scope.

Questions to probe: Who calls them when something hard comes up? How far does their name travel?

### 3. Signal
*How legibly their value is communicated externally*

Their public footprint: writing, speaking, GitHub, LinkedIn, press mentions, community presence. This is not about personal brand performance — it's about whether their value is visible to people who don't already know them.

Questions to probe: If someone Googled them today, what would they find? Does that match who they are?

### 4. Network
*The quality and diversity of relationships they can activate*

Not LinkedIn connections — real relationships with people who will take a call, make an introduction, or vouch for them. Includes mentors, sponsors, peers across domains, and people they've brought up.

Questions to probe: Who would go out of their way for them? Who have they gone out of their way for?

### 5. Optionality
*How many doors are genuinely open to them*

The range of plausible next moves — different roles, industries, geographies, modes of work (operator, advisor, founder, consultant). High optionality means they're not trapped by their current trajectory.

Questions to probe: If their current role disappeared tomorrow, what would realistically be available to them?

### 6. Momentum
*Whether their capital is growing, plateauing, or eroding*

The trajectory, not the snapshot. Are they learning, being stretched, building new relationships, adding to their signal? Or coasting on past capital?

Questions to probe: What did they build or learn in the last 12 months that they didn't have before?

---

## Step 1: Load career profile

Read `career-profile/cv.md` and `career-profile/context.yml` (if present) via the career-profile skill.

## Step 2: Gather capital-specific context

Ask up to **three targeted questions**. Choose the most useful based on what the profile doesn't tell you:

**Candidate questions** (pick the most relevant):
- "What's the thing you know how to do that most people in your field don't?"
- "When did you last feel genuinely stretched — like you were building something new rather than repeating a pattern?"
- "Outside your current employer, who knows what you're capable of?"
- "If you wanted to make a significant career move in the next 12 months, what would make it hard?"
- "What's the last thing you did that you'd point to as evidence of your best work?"

## Step 3: Produce the capital snapshot

Save to `output/career-capital-[date].md`.

### Document structure

---

# Career Capital Snapshot
**[Name if known] · [Date]**

---

## What you've built

One paragraph. A plain-language synthesis of their career capital as a whole — not dimension by dimension, but as a coherent picture. What kind of professional are they? What's the through-line?

This should feel like something a trusted colleague who knows them well would say about them at a dinner party. Warm but honest.

---

## Where your leverage sits

The two or three dimensions where their capital is genuinely strong. Specific and evidence-backed from their profile — not generic praise.

For each:
**[Dimension]**: [2–3 sentences of honest, specific assessment. What's strong here and why.]

---

## Where the gaps are

The one or two dimensions that are underdeveloped relative to their seniority and potential. Written without judgment — these are observations, not verdicts.

For each:
**[Dimension]**: [What's missing or thin here, and what the practical consequence of that gap is.]

---

## The honest read on momentum

One paragraph. Are they in a phase of building, consolidating, or coasting? What does the trajectory look like? What's driving it?

This is the hardest section to write and the most useful. Don't soften it.

---

## Three moves that would compound

The highest-leverage things they could do in the next 12 months to build capital across multiple dimensions at once. Not a to-do list — strategic moves with compounding effects.

**Move 1**: [What + why it compounds]
**Move 2**: [What + why it compounds]
**Move 3**: [What + why it compounds]

---

## One question to sit with

A single question that this assessment surfaces — something worth thinking about before the next decision. Not a prescription. An invitation to reflect.

---

## Calibration notes

- **Be honest about gaps** — a snapshot that only flatters is useless
- **Specific beats general** — "you have deep expertise in fraud detection systems at scale" beats "you have strong technical skills"
- **Momentum is the most important dimension** for people who already have strong capital in other areas — don't bury it
- **The three moves should be genuinely strategic** — not "update your LinkedIn" unless that's actually the highest leverage thing they could do
- **Length**: Two to three pages. The capital snapshot is meant to be revisited — dense enough to be useful, short enough to be readable
