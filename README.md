# Judgemental Thinker — a Claude Skill

A response format for judgment-call questions. Instead of a single hedged
answer, it gives you three things: an honest opinion, the strongest real
disagreement with it, and what would actually tip the decision one way or
the other.

## Why

Ask most AI assistants "should I take this job" or "is X better than Y"
and you often get a wishy-washy "it depends on your priorities!" that
commits to nothing. This skill forces a real opinion *and* a real
counter-argument, so you get to see the actual shape of the disagreement
instead of a flattened non-answer.

## What you get

When you ask a judgment-call question, Claude responds in three labeled
sections:

- **My take** — an honest, direct opinion, including doubts or caveats.
  No hedging just to seem balanced.
- **Strongest counter-view** — the most credible opposing position a
  smart, informed person could actually hold. Never a strawman built to
  be easily dismissed.
- **What it depends on** — 1–3 concrete factors that would tip a
  reasonable person toward one view or the other.

It does **not** apply this format to factual lookups, definitions, math,
coding help, or small talk — those still get short, normal answers.

## Install

1. Download `judgemental-thinker.skill` from this repo.
2. In Claude, open the file — if your account/org has skill installation
   enabled, you'll see a **Save skill** button.
3. Once installed, just ask a decision/opinion/debate-style question —
   the skill triggers automatically.

Note: skill installation is currently gated by account/org settings on
Anthropic's side. If you don't see a "Save skill" option, that's a
platform limitation, not a problem with the file — you can still copy
the instructions directly into a chat as a one-off prompt (see
`SKILL.md` in this repo for the exact text).

## Example

**Q: Should I quit my stable job to start my own business?**

> **My take** — If you don't have savings to cover at least 6–12 months
> of expenses, or a specific plan for your first customers, quitting now
> is premature...
>
> **Strongest counter-view** — Some businesses genuinely can't be built
> part-time...
>
> **What it depends on** — Whether the business model requires full-time
> hustle to work at all, your actual financial runway, and how
> time-sensitive the opportunity is.

## Feedback

This is an early version — one test prompt in, not hardened against real
usage yet. If you try it and it breaks on something (forces the format
where it shouldn't, or produces a weak counter-view), open an issue or
just say so — it'll get better with real use.

## License

Free to use, copy, modify, and share.
