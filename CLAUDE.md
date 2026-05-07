# careerpowers

Career intelligence for people with complex careers.

careerpowers gives you a set of skills that produce concrete, honest career documents — a performance review, a positioning brief, a capital snapshot. Not templates. Not generic advice. Documents that reflect *your* career, written in language you can actually use.

---

## How to use careerpowers

**First time**: Add your CV or work history to `career-profile/cv.md`. Any format is fine — paste from LinkedIn, upload a PDF, write it yourself. Just get your career history in there.

**Then run any skill:**

```
/careerpowers review      → Performance review document
/careerpowers position    → Positioning brief
/careerpowers capital     → Career capital snapshot
/careerpowers             → Show all options
```

Or just describe what you're trying to figure out. careerpowers will route to the right skill.

---

## Design principles

**Produce something.** Every skill run ends with a document saved to `output/`. You always leave with something in your hands.

**Clarity over comprehensiveness.** A sharp 2-page positioning brief beats a 10-page audit nobody reads.

**No flattery.** Senior professionals don't need to be told they're impressive. They need honest pattern recognition and language they can actually use.

**Careerpowers goes first.** The system reads your profile and leads with what's most useful — it doesn't wait for you to know the right question.

---

## Skills

| Skill | What it does |
|---|---|
| `career-profile` | Loads your career context. Runs before everything else. |
| `career-ops` | Router. Reads your message and activates the right skill. |
| `performance-review` | Structured self-review document for your next review cycle |
| `positioning-review` | Positioning brief: what you're known for, what you want to be known for, the gap, and three narrative angles to close it |
| `career-capital` | Capital snapshot: what you've built, where your leverage sits, where the gaps are, three moves that would compound |

---

## Agents (coming soon)

| Agent | What it does |
|---|---|
| `opportunity-matcher` | Scans for roles, projects, and conversations aligned to your capital and direction |

---

## Your files

```
careerpowers/
├── career-profile/
│   ├── cv.md           ← Your career history (required)
│   └── context.yml     ← Goals, constraints, what you want more/less of (optional)
└── output/             ← Generated documents land here
```

---

## Philosophy

Mid to senior professionals don't lack ambition or capability. They lack clarity — about what they've built, how they're perceived, and what move makes sense next. careerpowers is built for that gap: not the panic moment of an active job search, but the ongoing work of understanding your career as an asset and making intentional decisions about it.

---

Built by [Dana Andersen](https://tendcareer.com) · MIT License
