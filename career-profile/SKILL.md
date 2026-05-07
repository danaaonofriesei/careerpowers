---
name: career-profile
description: Shared context loader for careerpowers. Reads the user's career profile (profile.md) and makes it available to all skills. This runs before any careerpowers skill executes.
---

# Career Profile Loader

Before any careerpowers skill runs, load the user's career context.

## What to load

Read `career-profile/profile.md` — a single text file containing the user's career history and context.

## If career-profile/profile.md is missing or empty

Do not block. Instead, ask the questions conversationally — one at a time, in a natural tone. You only need enough to run the skill the user asked for. You don't need to collect everything upfront.

Start with:

> "Before we dive in, I need a bit of your career history. Paste your CV below, or just describe your background in your own words — roles, what you've done, how long you've been at it. No specific format needed."

Then ask only what's missing for the skill being run:

- For **performance-review**: also ask what they shipped this cycle and where they fell short
- For **positioning-review**: also ask how people currently describe what they do and whether that feels right
- For **career-capital**: also ask what they know how to do that most people in their field don't
- For **goal-setting**: also ask what their company is focused on right now and what they personally want more of

After the skill runs, write everything the user shared into `career-profile/profile.md` so it's available next time. Tell them:

> "I've saved your profile to career-profile/profile.md — next time you run a skill it'll pick up from there automatically."

## What to extract and hold in context

From the **My CV** section, extract and summarize:

- **Total years of experience** and career arc (IC → management, specialist → generalist, etc.)
- **Domains and industries** they've worked in
- **Seniority level** (inferred from titles, scope, org size)
- **Notable achievements** mentioned explicitly
- **Apparent strengths** — what keeps appearing across roles
- **Gaps or transitions** — career changes, breaks, pivots
- **Current or most recent role** — title, company type, rough tenure

From the context sections, note:

- What they want to be doing more of
- What they want to stop doing
- Their current situation and how they describe it
- Any constraints (location, industry, comp floor)
- Anything upcoming (review cycle, potential move, offer on the table)

If a section is left blank, note it and work with what's there. Do not ask the user to fill in missing sections before running — the skills will ask targeted questions if needed.

## Tone calibration

Once you've read the profile, calibrate your output tone:

- If they're **IC / specialist** (engineer, designer, analyst, researcher): lead with craft and depth, be precise
- If they're **manager / leader** (EM, VP, Director, Head of): lead with organizational impact and people leverage
- If they're **generalist / operator** (COO, Chief of Staff, PM, Ops): lead with systems thinking and cross-functional reach
- If **unclear**: default to treating them as a thoughtful senior professional who values directness over flattery

This calibration applies to all skill outputs in this session.
