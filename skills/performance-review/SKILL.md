---
name: performance-review
description: Produces a structured performance self-review document for senior professionals. Activate when the user mentions performance review, self-review, annual review, mid-year review, peer feedback prep, or wants help articulating their impact for a review cycle. Also activate proactively if their context.yml mentions an upcoming review.
---

# Performance Review Skill

Produce a structured self-review document that helps a senior professional walk into their review cycle with clarity, confidence, and language that lands.

## What this is not

Not a generic "here are your achievements" list. The output should read like it was written by someone who deeply understands this person's work — specific, honest about gaps, and framed in the language their organization actually uses to evaluate senior talent.

## Step 1: Load career profile

Read `career-profile/cv.md` and `career-profile/context.yml` (if present) via the career-profile skill.

## Step 2: Gather review-specific context

Ask the user up to **three targeted questions** — no more. Choose the most important ones based on what's missing from their profile:

**Candidate questions** (pick the most relevant):
- "What's the most important thing you shipped or changed in the last 12 months? Walk me through it."
- "Where did you fall short of what you intended? What got in the way?"
- "What do you think your manager sees as your biggest contribution — and does that match what you think?"
- "Is there a gap between how you're currently perceived and what you actually want to be known for?"
- "What do you want from this review cycle — a promotion, a scope change, just alignment?"

If `context.yml` exists and answers some of these, don't ask again. Use what's there.

## Step 3: Produce the self-review document

Write a complete self-review document and save it to `output/performance-review-[date].md`.

### Document structure

---

# Performance Self-Review
**[Name if known] · [Role] · [Review period]**

---

## Summary

Two to three sentences. The "elevator pitch" version of this review cycle — what they did, what it meant, and where they're headed. Written in first person, in their voice. This is what a reader skimming for 20 seconds should take away.

---

## Impact this cycle

For each major contribution (aim for 3–5):

**[What they did — specific, named]**
- Context: Why this mattered / what the situation was
- Action: What they specifically did (not the team — them)
- Result: Quantified where possible, honest where not
- So what: Why this matters at their level of seniority

Do not pad. If they only have 3 real contributions, write 3. A strong 3 beats a weak 5.

---

## Where I fell short

One to two honest gaps. Written without defensiveness. Senior professionals who can name their own gaps build more trust than those who can't.

Format:
- **[Gap]**: What happened, what contributed to it, what they'd do differently.

This section makes the whole document more credible. Don't skip it.

---

## What I'm building toward

Based on their stated goals or inferred trajectory: what they're working on developing, what scope they're ready for, what they want to be known for in the next cycle.

This is forward-facing and should connect naturally to any promotion or scope discussion.

---

## What I need to do my best work

One short paragraph. What conditions, resources, or clarity would help them operate at their best. Written as a direct professional request, not a complaint.

---

## Closing

One sentence. Confident, not boastful.

---

## Step 4: Optional — Talking points

After the document, add a short section (not saved to the main doc):

**Key moments to bring up in the conversation:**
- [3 specific stories or data points to have ready if asked]

**What to listen for:**
- [1–2 things they should pay attention to in their manager's response]

## Calibration notes

- **For ICs**: Lead sections with craft, technical judgment, and concrete deliverables
- **For managers**: Lead with organizational outcomes — team health, hiring, unlocking others
- **For senior leaders**: Lead with strategic bets, cross-functional influence, and what they decided *not* to do
- **Tone**: Direct, first-person, professional. Not corporate. Not self-aggrandizing.
- **Length**: 2–3 pages is right. Anything longer loses the reader.
