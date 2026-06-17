# RiseLab Planning Skills
*Plan it right before you build it. By Ibrahim Denis Fofanah.*

A collection of planning partners — opinionated, interrogating skills that force the hard questions *before* work starts. Each one acts like a seasoned practitioner sitting across the table from you: it pushes back, names the failure modes, and produces a planning document you hand to whoever (or whatever) does the implementation.

These are **planning** skills. None of them write production code. The output is always a brief, because the most expensive mistakes in software and data work are made in the first hour, not the last.

## The skills

| Skill | Plays the role of | Use when |
|---|---|---|
| `saas-planning-partner` | Product partner + eng manager | "I have an idea", "is this worth building", "review my architecture" |
| `riselab-data-analytics-partner` | Seasoned analyst (15 years of scars) | "here's a dataset", "analyze this", "make sense of this", "clean this up" |
| `riselab-data-science-partner` | Staff ML engineer | "let's build a model", "predict X", "is this even an ML problem" |

## Install (Claude Code)

```bash
git clone https://github.com/Denis060/riselab-planning-skills.git ~/riselab-planning-skills
cd ~/riselab-planning-skills && ./setup
```

`./setup` symlinks each skill into `~/.claude/skills/` so Claude Code can find them. Invoke a skill by name, e.g. *"run riselab-data-science-partner on this"*.

To uninstall: `rm ~/.claude/skills/saas-planning-partner ~/.claude/skills/riselab-data-analytics-partner ~/.claude/skills/riselab-data-science-partner`

## Use it without Claude Code (any model)

You don't need anything installed. Open the `SKILL.md` for the skill you want, copy it (or just the relevant stage), paste it into a fresh chat, and start answering the questions. The discomfort is the value.

## Philosophy

Three beliefs run through all of them:

1. **An output that changes no decision is a hobby.** Every skill starts by naming the decision the work serves. If there isn't one, it stops.
2. **The boring failure modes are the expensive ones.** Scope creep, dirty data, target leakage, the wrong metric. These aren't exotic — they're predictable, and they're caught by asking, not by cleverness.
3. **Say less, push harder.** The skills are deliberately anti-sycophantic. They take a position and tell you what would change their mind. Comfort means they haven't pushed hard enough.

## Lineage & credit

The SaaS skill's planning structure was adapted from the methodology in Garry Tan's open-source `gstack` (MIT), stripped of its tooling-specific machinery. The data skills are original to RiseLab, grounded in CRISP-DM / CRISP-ML(Q) and the published literature on data leakage, evaluation, and statistical reasoning traps — built to fill a real gap, since no planning-interrogation skill for data work existed.

## License

MIT. Fork it, rebrand it, teach with it, ship it. Keep the license notice.

---
*Part of RiseLab — Africa-centric data science and AI education. Maintained by Ibrahim Denis Fofanah.*
