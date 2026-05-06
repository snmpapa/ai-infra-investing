# AI Infra Investing

Layered investing skill for AI-driven portfolios.

This skill is built for investors who want to organize AI stock analysis through:

- AI infrastructure stack layers
- portfolio buckets
- add/reduce triggers
- separation of core holdings and high-beta tactical trades

It is designed as a reusable Skill folder that can be used locally in Codex and later moved into a shared repo for reuse across other AI systems.

## What This Skill Does

This skill helps answer questions like:

- Which part of the AI stack does this company belong to?
- Is this a core holding, satellite, theme, defensive, or watchlist name?
- Which AI names are missing from my portfolio?
- Am I duplicating the same layer risk?
- What should I buy first?
- What should I trim first?
- When is a name a real AI infrastructure asset versus just a levered AI trade?

## What Makes It Different

This is not a generic stock-picking template.

It is built around a specific idea:

**AI investing should be managed as a layered system, not as a loose list of hot stocks.**

The framework distinguishes between:

- AI core exposure
- leveraged AI exposure
- business quality
- position size
- long-term holdings
- tactical high-beta trades

## Relationship To `wave-investing`

This skill does **not** replace `wave-investing`.

Use `wave-investing` when the main question is:

- what kind of stock is this?
- is it stable or psychologically hard to hold?
- what wave pattern defines it?
- who is this stock suitable for?

Use `ai-infra-investing` when the main question is:

- where does this name sit in the AI stack?
- what bucket should it go in?
- how should it fit into a portfolio?
- what are the add/reduce triggers?

In practice:

- `wave-investing` = stock personality and holding experience
- `ai-infra-investing` = stack classification and portfolio management

## Core Framework

The workflow is:

1. Classify the name into an AI stack layer
2. Classify the name into a portfolio bucket
3. Decide whether the stock belongs in the portfolio at all
4. Separate thesis quality from position size
5. Write explicit add and reduce triggers
6. Apply special caution to high-beta operators and theme amplifiers

## AI Stack Layers

This skill uses the following AI stack layers:

- Platform demand
- GPU / accelerator
- CPU / system control
- Memory
- Foundry / packaging
- Optical / network interconnect
- AI infrastructure operators
- AI payments / settlement
- Market activity / distribution

Detailed notes live in:

- [references/ai-stack-layers.md](references/ai-stack-layers.md)

## Portfolio Buckets

This skill uses the following bucket system:

- Core holding
- Satellite holding
- Theme position
- Defensive holding
- Watchlist name
- Trading-only high beta

Detailed notes live in:

- [references/portfolio-buckets.md](references/portfolio-buckets.md)

## Files

- [SKILL.md](SKILL.md): primary skill instructions
- [SKILL.zh-CN.md](SKILL.zh-CN.md): Chinese version of the main skill instructions
- [examples.md](examples.md): prompt and output examples
- [agents/openai.yaml](agents/openai.yaml): UI-facing skill metadata
- [references/ai-stack-layers.md](references/ai-stack-layers.md): AI stack classification
- [references/portfolio-buckets.md](references/portfolio-buckets.md): bucket definitions
- [references/triggers.md](references/triggers.md): add/reduce trigger rules
- [references/high-beta-rules.md](references/high-beta-rules.md): rules for operator and tactical high-beta names

## Recommended Use Cases

This skill works especially well for:

- AI portfolio construction
- comparing AI infrastructure stocks
- deciding whether a stock is core or tactical
- controlling overlap across GPU / CPU / memory / operator names
- separating high-conviction holdings from momentum trades

## Current Design Intent

This skill was shaped around an AI investing workflow centered on names such as:

- `GOOG`, `META`
- `NVDA`, `TSM`, `AMD`
- `MU`, `DRAM`
- `CRCL`, `HOOD`
- `CRWV`, `IREN`, `NBIS`
- `GLD` as a defensive buffer

The broader idea is portable even when the exact names change.

## Notes

- This framework is for structured judgment, not automatic prediction.
- It is intentionally compatible with multi-agent research workflows, but it is not tied to any one trading agent implementation.
- It is suitable for local use first, then migration to `~/.codex/skills`, and later publishing to GitHub.
