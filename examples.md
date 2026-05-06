# AI Infra Investing Examples

This file shows how to use `ai-infra-investing` in practice.

The goal is not to provide exhaustive answers, but to show the expected framing.

## Example 1: Single Stock Classification

Prompt:

```text
Use $ai-infra-investing to analyze AMD.
I want to know which AI layer it belongs to, whether it is core or satellite,
and what add/reduce triggers I should watch.
```

Expected shape:

```text
One-line role: AMD is a CPU/system-control layer stock and fits best as a satellite holding.
AI stack layer: CPU / system control
Portfolio bucket: satellite holding
Why it matters: AI infrastructure is broadening from pure GPU demand into full-system compute.
Key risk: CPU optimism may outrun the pace of actual profit expansion.
Add triggers: strong data-center CPU growth, AI attach-rate expansion, pullback without thesis damage.
Reduce triggers: CPU narrative expands faster than margins or earnings.
Weight guidance: mid-single-digit range if it fills a missing CPU layer.
```

## Example 2: Multi-Name Comparison

Prompt:

```text
Use $ai-infra-investing to compare NVDA, TSM, MU, and CRWV.
Rank them by business quality and by portfolio priority.
Also tell me which ones are core exposure and which are leveraged AI exposure.
```

Expected shape:

```text
Business quality ranking:
1. TSM
2. NVDA
3. MU
4. CRWV

Portfolio priority ranking:
1. NVDA
2. TSM
3. MU
4. CRWV

Core exposure:
- NVDA
- TSM
- MU

Leveraged AI exposure:
- CRWV
```

## Example 3: Portfolio Construction

Prompt:

```text
Use $ai-infra-investing to structure an AI portfolio with GOOG, META, NVDA, TSM, MU, AMD, CRCL, HOOD, GLD.
Separate core, satellite, theme, and defensive buckets.
Give rough weight ranges and tell me what feels missing.
```

Expected shape:

```text
Core:
- GOOG
- META

Satellite:
- NVDA
- TSM
- MU
- AMD

Theme:
- CRCL
- HOOD

Defensive:
- GLD

Missing layer:
- optical/network interconnect if the user wants fuller AI infrastructure coverage
```

## Example 4: High-Beta Operator Name

Prompt:

```text
Use $ai-infra-investing to evaluate IREN.
I already treat it as a trade, not a long-term holding.
Tell me whether it belongs in my portfolio or only as a tactical position.
```

Expected shape:

```text
One-line role: IREN is a high-beta AI infrastructure operator and belongs in a tactical sleeve, not as a base holding.
AI stack layer: AI infrastructure operator
Portfolio bucket: trading-only high beta
Why it matters: it gives levered exposure to AI data-center and GPU-cloud enthusiasm.
Key risk: financing and execution risk can move faster than the underlying AI thesis.
Add triggers: improving contracts, utilization, financing terms.
Reduce triggers: narrative outruns execution, or the position starts behaving like disguised core exposure.
Weight guidance: small and controlled.
```

## Example 5: Adjacent AI Infrastructure Thesis

Prompt:

```text
Use $ai-infra-investing to analyze CRCL.
My thesis is that agent payments and stablecoin settlement will become part of AI infrastructure.
Tell me whether that framing is reasonable and how large a position can be justified.
```

Expected shape:

```text
One-line role: CRCL is not core compute infrastructure, but it can qualify as adjacent AI settlement infrastructure when the thesis explicitly includes agent payments.
AI stack layer: AI payments / settlement
Portfolio bucket: theme position
Why it matters: programmable settlement may become useful if agents transact natively.
Key risk: regulation matters more than AI excitement.
Add triggers: better regulation, wider settlement usage, stronger ecosystem adoption.
Reduce triggers: regulatory deterioration or valuation expansion without usage proof.
Weight guidance: small theme allocation, not a core slot.
```

## Example 6: When To Use `wave-investing` Too

Prompt:

```text
Use $ai-infra-investing and $wave-investing to compare GOOG and NVDA.
I want both the AI stack role and the holding experience difference.
```

Expected shape:

```text
AI infra view:
- GOOG = platform demand core
- NVDA = GPU core

Wave view:
- GOOG = steadier compounder, easier hold
- NVDA = explosive upside, harder hold
```

## Suggested Pattern

When using this skill with another model or platform, keep the prompt simple:

1. name the stock or portfolio
2. state your thesis if you have one
3. ask for stack layer
4. ask for bucket
5. ask for add/reduce triggers
6. ask for weight guidance

Good minimal prompt:

```text
Use $ai-infra-investing to analyze {TICKER}.
Tell me its AI stack layer, portfolio bucket, key risk, add triggers, reduce triggers, and rough weight guidance.
```
