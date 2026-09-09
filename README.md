XYZ format resume bullets — a Claude Agent Skill that rewrites weak, task-oriented resume statements into high-impact, Google-style XYZ achievement bullets.

# claude-skill-xyz-resume-bullets

[![Claude Skill](https://img.shields.io/badge/Claude-Agent%20Skill-9E7BFF)](https://claude.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Turn raw, duty-focused resume lines into polished **XYZ-format achievement bullets** — *"Accomplished [X], as measured by [Y], by doing [Z]"* — the format popularized by Google and used by hiring managers at top tech companies. Built as a [Claude Agent Skill](https://claude.ai) so you can rewrite bullets directly inside Claude.

## Why use this

- **XYZ format resume bullets, done right.** Converts task language ("Responsible for...", "Worked on...") into outcome language with real, measurable impact.
- **Never fabricates numbers.** Metrics are only used if you supplied them, or if they're mathematically derivable from what you supplied (e.g. "4 hours to 30 minutes" → 87.5% reduction).
- **Smart placeholders.** If an accomplishment deserves a metric but you didn't give one, the skill inserts a clear placeholder like `[X]%` or `[X] hours per week` — never asks a clarifying question first, never guesses a number.
- **Preserves ownership accuracy.** "Assisted with" never gets inflated to "Led." Honesty over hype.
- **Copy-paste ready output.** No explanations, no breakdowns, no commentary — just the finished bullet(s).

## Example

**Input:**
> Worked on improving API performance using caching

**Output:**
> **Reduced API response time by [X]% by implementing Redis caching and optimizing database queries.**

## Installation

1. Clone or download this repository.
2. Add the `xyz-resume-bullets` skill folder to your Claude Skills directory.
3. Reference it in Claude by sharing a resume bullet, work-experience line, or accomplishment statement.

```bash
git clone https://github.com/<your-username>/claude-skill-xyz-resume-bullets.git
```

## How it works

Internally, every bullet is built on Google's XYZ framework:

> **Accomplished [X], as measured by [Y], by doing [Z].**

- **X — Accomplishment:** the real outcome (increased, reduced, automated, launched...), not the task.
- **Y — Measurement:** the strongest truthful evidence — business impact, technical impact, quantified performance, or scope — used verbatim, derived, or placeholdered.
- **Z — Action:** what you actually did, including relevant tools and technologies.

These are merged into one natural, recruiter-ready sentence — never shown as a labeled formula.

## What it won't do

- Won't invent metrics, percentages, or business outcomes.
- Won't exaggerate your role or ownership level.
- Won't return more than one bullet per input, or merge separate accomplishments.
- Won't show its internal reasoning, even if asked.

## Repository topics

`claude` `claude-skills` `anthropic` `resume` `resume-builder` `xyz-format` `career-tools` `llm-tools` `tools`

## Contributing

Issues and pull requests are welcome — especially additional worked examples and edge cases for the placeholder catalog.

## License

MIT
