# Execution Rules

Use this file when the user already has a target portfolio but does not want to rebalance mechanically at current prices.

This file is about execution discipline, not stock ranking.

## Core Idea

Do not confuse:

- `what should be owned`
- `what should be bought right now`

A stock can belong in the target portfolio while still being a poor immediate buy because:

- price is extended
- the user prefers pullback entries
- the user prefers selling puts to get filled
- an existing oversized position can later fund the switch

## Execution-Mode Framework

When the user already knows the target portfolio, classify each holding into one of these states:

### 1. Hold And Leave Alone

Use for:
- holdings that already fit the target structure
- names that are not obviously overextended
- positions the user does not need to touch immediately

### 2. Overweight But Not Forced To Sell Now

Use for:
- positions that are too large versus target
- but the user does not want to sell at a poor price
- or the user intends to use future strength to fund better long-term holdings

Examples:
- a theme stock that is oversized but not attractive to sell immediately

Interpretation:
- this is a `future funding source`, not an emergency mistake

### 3. Target Holding, Wait For Better Entry

Use for:
- names that belong in the portfolio
- but are too expensive to chase right now

Preferred execution:
- buy on pullback
- sell put to get assigned

### 4. Tactical Reduction Candidate

Use for:
- names the user would like to trim first when price improves
- especially theme names or oversized non-core names

### 5. Optional / Low Priority

Use for:
- names that can wait
- names that are not required to complete the portfolio structure

## Preferred Language

When discussing execution, use practical labels like:

- `do not chase`
- `wait for pullback`
- `sell put candidate`
- `future switch source`
- `not urgent`
- `trim on strength`

This is better than pretending every gap to target must be closed immediately.

## Sell Put Logic

When the user explicitly prefers selling puts:

- treat the stock as a valid target holding
- but shift the entry plan from `buy now` to `collect premium while waiting`
- do not describe this as hesitation; describe it as price-disciplined entry

Typical candidates:
- high-quality target holdings that the user wants to own but not chase

Examples:
- `GOOG`
- `TSM`
- sometimes `AMD`, `MU`, or `DRAM` depending on valuation and volatility

## Switching Logic

Use switching logic when:

- the user already owns an oversized non-core or theme position
- the user intends to rotate into a stronger long-term layer later

Examples:
- an oversized `HOOD` position can be treated as a future switch source into `GOOG` or `TSM`

Important:
- do not force the switch at a bad price just to make the model look clean
- focus on execution quality, not cosmetic portfolio symmetry

## What To Output

When the user is in execution mode, prefer this structure:

1. `Target structure`
2. `Already acceptable, do not force action`
3. `Overweight but can wait`
4. `Wait for pullback / sell put entry`
5. `Trim on strength`
6. `Not urgent`

## Key Principle

Target portfolios should be strategically clean.
Execution should still be tactically patient.
