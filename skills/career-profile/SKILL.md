---
name: career-profile
description: Shared context loader for careerpowers. Collects the user's career context either by reading career-profile/profile.md if it exists, or by asking questions conversationally. This runs before any careerpowers skill executes.
---

# Career Profile Loader

Before any careerpowers skill runs, get the user's career context. There are two paths:

## Path A: profile.md exists

If `career-profile/profile.md` exists and has content, read it silently and proceed directly to the skill. Do not tell the user you're reading it. Just use it.

## Path B: no profile yet (default for most users)

Do not ask the user to find a file or set anything up. Just start a natural conversation to collect what you need.

Open with:

> "Before we dive in, I need to learn a bit about your career. I'll ask you a few quick questions — answer however feels natural, no specific format needed."

Then ask these questions **one at a time**, waiting for each answer before asking the next:

1. "What's your current or most recent role, and how long have you been in it?"
2. "Give me a quick tour of your career — where have you worked, what kind of work have you done, roughly how many years?"
3. "What do you want more of in the next phase of your career?"
4. "What do you want to leave behind — work you'd delegate or stop doing if you could?"
5. "Is there anything coming up I should know about — a performance review, a potential move, an offer, a conversation you're preparing for?"

If a user skips a question or says "not sure", accept it and move on. You don't need perfect answers to run a skill.

## After collecting answers

Summarize what you've learned back to the user in one short paragraph so they can correct anything, then proceed to the skill they asked for.

Offer to save their profile:
> "Want me to save this so you don't have to answer these questions next time? Just say yes and I'll create your profile file."

If they say yes, write their answers to `career-profile/profile.md` using this format:

```
## My CV
[their career history from answers]

## What I want more of
[their answer]

## What I want less of
[their answer]

## My situation right now
[inferred from their answers]

## Anything coming up
[their answer]
```

## What to extract and hold in context

From the conversation, summarize:

- **Total years of experience** and career arc
- **Domains and industries** they've worked in
- **Seniority level** (inferred from titles, scope, org size)
- **Apparent strengths** — what keeps appearing across roles
- **Current role** — title, company type, tenure
- **Direction** — what they want more and less of

## Tone calibration

- **IC / specialist** (engineer, designer, analyst, researcher): lead with craft and depth
- **Manager / leader** (EM, VP, Director, Head of): lead with organizational impact
- **Generalist / operator** (COO, Chief of Staff, PM, Ops): lead with systems thinking
- **Unclear**: treat as a thoughtful senior professional who values directness over flattery