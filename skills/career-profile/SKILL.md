---
name: career-profile
description: Shared context loader for careerpowers. Reads the user's career profile (cv.md and context.yml if present) and makes it available to all skills. This runs before any careerpowers skill executes.
---

# Career Profile Loader

Before any careerpowers skill runs, load the user's career context.

## What to load

1. **Required**: Read `career-profile/cv.md` — the user's CV or work history in any format
2. **Optional**: Read `career-profile/context.yml` if it exists — goals, constraints, what they want more/less of

## If career-profile/cv.md is missing

Tell the user:

> careerpowers needs your career history to get started. Create a file at `career-profile/cv.md` and paste in your CV, LinkedIn About section, or a plain summary of your roles and what you've done. It doesn't need to be formatted — just honest.

Then stop. Do not attempt to run any skill without this file.

## What to extract and hold in context

From the CV, extract and summarize:

- **Total years of experience** and career arc (IC → management, specialist → generalist, etc.)
- **Domains and industries** they've worked in
- **Seniority level** (inferred from titles, scope, org size)
- **Notable achievements** mentioned explicitly
- **Apparent strengths** — what keeps appearing across roles
- **Gaps or transitions** — career changes, breaks, pivots
- **Current or most recent role** — title, company type, rough tenure

From context.yml (if present), note:

- What they want to be doing more of
- What they want to stop doing
- Time horizon (12 months? 3 years?)
- Any constraints (location, industry, comp floor)

## Tone calibration

Once you've read the profile, calibrate your output tone:

- If they're **IC / specialist** (engineer, designer, analyst, researcher): lead with craft and depth, be precise
- If they're **manager / leader** (EM, VP, Director, Head of): lead with organizational impact and people leverage
- If they're **generalist / operator** (COO, Chief of Staff, PM, Ops): lead with systems thinking and cross-functional reach
- If **unclear**: default to treating them as a thoughtful senior professional who values directness over flattery

This calibration applies to all skill outputs in this session.
