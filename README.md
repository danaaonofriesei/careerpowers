# careerpowers


careerpowers gives professionals a set of AI-powered skills that produce concrete, honest career documents — a performance review, a positioning brief, a capital snapshot, a goals plan.

> **Not in active job search mode?** Good. That's the point. careerpowers is built for the ongoing work of understanding your career — not only for the panic moment of a job hunt.

---

## What you get

Four skills that each produce a document you can actually use:

| Command | Output |
|---|---|
| `/careerpowers capital` | A capital snapshot — what you've built, where your leverage sits, where the gaps are, and three moves that would compound |
| `/careerpowers position` | A positioning brief — what you're known for, what you want to be known for, the gap, and three narrative angles to close it |
| `/careerpowers goals` | A goals document — annual, quarterly, and monthly SMART goals aligned to your role and your career trajectory |
| `/careerpowers review` | A structured performance self-review — achievements framed with impact, gaps owned, narrative arc for the conversation |

---

## Install

**Using Claude.ai or the Claude interface - no installation needed**

Open any skill on GitHub — start with skills/career-capital/SKILL.md
Click Raw → select all → copy
Paste into a new Claude chat
Add your career details below it and ask Claude to run it

**Using Claude Code**

```bash
git clone https://github.com/danaaonofriesei/careerpowers.git
claude --plugin-dir ./careerpowers
```

---

## Get started

**1. Add your career details** *(optional but recommended)*

Open `career-profile/profile.md` in any text editor — TextEdit on Mac, Notepad on Windows — and fill in your career history and context. Paste from LinkedIn, copy from your CV, or just write it in your own words. No specific format needed.

If you skip this step, careerpowers will ask you a few questions when you run your first skill and build your profile from your answers automatically.

**2. Let careerpowers help you**

```
/careerpowers capital     → Start here. Understand what you've built.
/careerpowers position    → Clarify how you're seen and how you want to be seen.
/careerpowers goals       → Set goals that serve you, not just your employer.
/careerpowers review      → Prep for your next performance review.
```

Or just describe what you're trying to figure out — careerpowers will take it from there.

---

## Your profile file

Everything careerpowers needs lives in one file — `career-profile/profile.md`. Open it and fill in each section:

```
## My CV
[paste your CV or LinkedIn Experience here]

## What I want more of
[the work you want to be doing]

## What I want less of
[what you want to stop or delegate]

## My situation right now
[how you'd describe where you are]

## Anything coming up
[review cycle, offer, conversation, potential move]
```

No special format required. It stays on your machine — it never goes anywhere unless you choose to share it.

---

## Who this is for

Professionals across functions — engineers, PMs, designers, ops leaders, finance, HR, legal, researchers — who have built more than they can see clearly anymore. People who want honest pattern recognition, not flattery.

---

## Agents (coming soon)

The skills produce documents. The agents take action.

| Agent | What it does |
|---|---|
| `opportunity-matcher` | Surfaces roles, conversations, and projects aligned to your capital and direction |

Gemini CLI support also coming — same skills, both agents.

---

## Philosophy

Mid to senior professionals don't lack ambition or capability. They lack clarity — about what they've built, how they're perceived, and what move makes sense next. careerpowers is built for that gap. Not the panic moment of an active job search. The ongoing work of understanding your career as an asset.

---

## Contributing

Skills are markdown files. If you have domain expertise and want to add a skill — interview prep, salary negotiation, advisory positioning, board readiness — contributions are welcome.

---

## Built on

Inspired by [designpowers](https://github.com/Owl-Listener/designpowers) and [career-ops](https://github.com/santifer/career-ops).

---

## License

MIT

---

Built by [Dana Aonofriesei](https://danaaonofriesei.substack.com/) · [Tend](https://tendcareer.com) — career intelligence for professionals
