---
name: ai-infra-investing
description: Use this skill when analyzing AI-related stocks, ETFs, or portfolios through AI infrastructure layers, portfolio buckets, and trigger-based position management. Best for requests about AI platform leaders, chips, memory, foundry, cloud GPU operators, AI payments rails, build/add/reduce decisions, portfolio structure, or separating core holdings from high-beta trading positions.
---

# AI Infra Investing

This skill is a portfolio construction and decision framework for AI investing.

It is designed for:
- AI-first stock selection
- layered portfolio construction
- separating core holdings from high-beta theme trades
- add/reduce decisions tied to narrative and operating triggers

It is not designed for:
- day trading calls
- exact price targets
- options structures
- full valuation models

## Use This Skill For

Use this skill when the user asks questions like:
- "How should I structure an AI portfolio?"
- "Is this a core holding, satellite, theme, or watchlist name?"
- "Compare NVDA, TSM, MU, AMD, GOOG, META, CRWV, IREN."
- "What part of the AI stack does this company belong to?"
- "What should I buy first?"
- "When should I add or reduce?"
- "How much theme exposure is too much?"
- "Is this stock a long-term holding or a trading position?"

If the request is mainly about stock personality, holding experience, or wave-like historical behavior, also use `wave-investing` as a supporting lens.

## Workflow

Follow this order:

1. Classify the name into an AI stack layer.
Load [references/ai-stack-layers.md](references/ai-stack-layers.md).

2. Classify the name into a portfolio bucket.
Load [references/portfolio-buckets.md](references/portfolio-buckets.md).

3. Decide whether the stock belongs in the portfolio at all.
Some names are useful only as trading or observation names.

4. Separate thesis quality from position size.
A good business can still deserve a small weight.

5. Write explicit add and reduce triggers.
Load [references/triggers.md](references/triggers.md).

6. If the name is a high-beta operator or theme vehicle, apply special caution.
Load [references/high-beta-rules.md](references/high-beta-rules.md).

7. If the user mixes long-term holdings, tactical high-beta trades, and symbolic narrative exposure, separate them into distinct sleeves.
Load [references/portfolio-structure.md](references/portfolio-structure.md).

8. If the user has target holdings but does not want to chase price, switch from static rebalancing to execution-mode planning.
Load [references/execution-rules.md](references/execution-rules.md).

9. If the user explicitly prioritizes downside protection over speed of deployment, apply margin-of-safety-first execution.
Load [references/margin-of-safety-first.md](references/margin-of-safety-first.md).

## Core Principles

- Distinguish `AI core exposure` from `leveraged AI exposure`.
- Distinguish `great business` from `great stock to hold right now`.
- Distinguish `theme relevance` from `portfolio necessity`.
- Do not let high-beta names become disguised core positions.
- Treat position sizing as a separate decision from stock ranking.
- Prefer clear layers over cluttered narratives.

## Preferred Output

Use this structure unless the user asks for something shorter:

1. `One-line role`
What role does this name play in the AI stack and in the portfolio?

2. `AI stack layer`
Which layer does it belong to?

3. `Portfolio bucket`
Core / satellite / theme / defensive / watchlist / avoid-for-now

4. `Why it matters`
Why this layer matters in the current AI narrative.

5. `Key risk`
One dominant risk that could break the thesis.

6. `Add triggers`
What would make it more attractive?

7. `Reduce triggers`
What would make it less attractive?

8. `Weight guidance`
If included, what rough size range makes sense?

## Standard Bucket Vocabulary

Use these labels consistently:
- `core holding`
- `satellite holding`
- `theme position`
- `defensive holding`
- `watchlist name`
- `trading-only high beta`

## Guardrails

- Do not recommend overweighting multiple names that express the same exact layer risk without saying so explicitly.
- Treat GPU cloud operators, AI infrastructure renters, miners pivoting into AI, and similar names as high-beta operators by default.
- Treat AI payments rails and stablecoin infrastructure as adjacent AI infrastructure only if the user's thesis explicitly includes agent payments.
- If the user already holds a stock and describes it as a trade, respect that framing unless the facts strongly argue otherwise.
- If comparing multiple names, rank both:
  - `business quality / durability`
  - `portfolio priority`

## References

- AI stack layers: [references/ai-stack-layers.md](references/ai-stack-layers.md)
- Portfolio buckets: [references/portfolio-buckets.md](references/portfolio-buckets.md)
- Trigger rules: [references/triggers.md](references/triggers.md)
- High-beta rules: [references/high-beta-rules.md](references/high-beta-rules.md)
- Portfolio structure: [references/portfolio-structure.md](references/portfolio-structure.md)
- Execution rules: [references/execution-rules.md](references/execution-rules.md)
- Margin of safety first: [references/margin-of-safety-first.md](references/margin-of-safety-first.md)
