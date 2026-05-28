# Fiduciary

A system prompt that turns a frontier LLM into a **retirement-planning
fiduciary**, a focused, evidence-grounded thinking partner for reviewing
your household's retirement readiness. Not to be used as the soul planning tool. 
I am personally using it to compare against other tools like Fidelity's built in planner.

It's grounded in the [Bogleheads](https://www.bogleheads.org/) investment
philosophy (low-cost, broadly-diversified, behaviorally-disciplined
investing) and is designed to behave like a fiduciary: acting in *your*
interest, citing its sources, surfacing uncertainty, and refusing to
freelance numbers.

## When to use it

- You want a structured second or third opinion on your plan.
- You want to think out loud with an AI that won't try to sell you anything,
  won't hand-wave numbers, and will tell you when it's outside its lane.
- You're helping a family member do the same.

## What it is *not*

- Not financial, tax, or legal advice. Use it to prepare better questions
  for a fee-only, fiduciary-bound CFP, EA/CPA, or estate attorney — not to
  replace them.
- Not a calculator. It will pull numbers from authoritative sources (SSA,
  IRS, your plan documents) and walk you through scenarios, but the math is
  only as good as the inputs you give it.

## How to use it

1. **Open a fresh chat** with a frontier LLM (Claude, GPT, Gemini, etc.)
   that has web browsing or tool use enabled if possible.
2. **Paste the entire contents of [`Fiduciary.md`](Fiduciary.md)** as your
   first message (or as a system prompt if your tool supports that).
3. **Follow its lead.** It will start by asking what to gather and how you
   want to work together.

## What to gather before you start

The prompt itself walks you through this, but in short: tax returns, recent
pay stubs, Social Security statements, all retirement-account statements
(401(k)/403(b)/IRA/HSA/brokerage), pension summaries, mortgage statement,
and a rough monthly-expenses estimate. Exports/CSVs are great; screenshots
or PDFs work too.

## Offline grounding (optional)

The prompt prefers live web fetches of Bogleheads wiki articles for
grounding. For users without browsing tools, an offline mirror of the wiki
is available as a separate repo — see the "Appendix: Offline grounding"
section at the bottom of `Fiduciary.md`.

## A note on "fiduciary"

Real-world fiduciaries (RIAs, CFPs operating under fiduciary rules, ERISA
plan administrators) are bound by **law** to act in your interest. An LLM
is not, cannot be, and shouldn't pretend to be one. The prompt asks the
model to *behave* like a fiduciary, to adopt the posture, citation
discipline, and uncertainty-flagging norms, as a north star for how it
should think and respond.
