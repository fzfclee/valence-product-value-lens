---
name: valence-product-value-lens
description: Lightweight Valence v0.2 public lens for a single digital product. Use an adaptive option-based wizard to identify the primary audience, main problem, expected change, evidence KPI, directional monetization through Grow / Save / Protect, product-form question, and data readiness. Do not perform formal ROI, portfolio governance, investment, prioritization, or lifecycle decisions.
---

# Valence Product Value Lens v0.2

## Purpose

Help a user turn a rough product description into a simple value-realization hypothesis:

```text
Who → Problem → Change → Evidence → Money → Why this form
```

The output must remain practical and short enough for a normal product manager or Tech BP to use.

## Use This Skill For

- single-product value framing;
- primary audience clarification;
- early monetization direction;
- evidence and measurement readiness;
- product-form challenge;
- preparation for a formal Valence review.

## Do Not Use This Skill For

- formal ROI or finance approval;
- portfolio scoring, ranking, or shutdown decisions;
- full Valence methodology disclosure;
- leadership review packs or governance cadence;
- confidential company, customer, contract, or system data.

## Input Rules

- Ask exactly one question at a time unless the user requests batch intake.
- Prefer 4-7 options plus Other and Not sure.
- Narrow each next question using the prior answer.
- Accept anonymous descriptions, approximate numbers, ranges, and Not sure.
- Do not require all data before producing a result.
- Do not invent benchmarks, attribution ratios, discount factors, or financial assumptions.
- Keep one Primary Audience and one Primary Economic Outcome by default.

## Wizard

Follow [conversation_flow.md](conversation_flow.md).

Collect enough signal to answer:

1. Primary Audience;
2. Main Problem;
3. Expected Change;
4. Evidence KPI;
5. Directional Monetization;
6. Why This Product Form;
7. Data Readiness and Next Action.

## Economic Outcome Rule

Use exactly one primary economic outcome:

- Grow;
- Save;
- Protect.

Use [value_taxonomy.md](value_taxonomy.md) for mechanisms and tie-breakers.

Productivity, experience, decision quality, branding, time criticality, risk, platform reuse, learning, and strategic capability are mechanisms or evidence paths, not final value categories.

If a mechanism cannot yet connect to Grow, Save, or Protect, label it **Unvalidated Value Hypothesis**.

## Monetization Rule

A final answer should show a direction, not a formal valuation.

Examples:

```text
Grow = impacted audience × incremental conversion × unit contribution margin × attribution to confirm
```

```text
Save = annual volume × verified net labor time saved × labor cost × realization factor to confirm
```

```text
Protect = potential economic impact × baseline probability × expected reduction to confirm
```

Do not add leading indicators such as adoption, visits, NPS, messages, or completion rate directly into a monetary total.

## Product Form Rule

Always include one practical question:

> Why does this need to be the current product form?

Possible alternatives may include website, H5, existing system extension, shared platform, API, process change, or no-build option.

Do not conclude that a mini-program, app, dashboard, or platform is justified merely because the underlying capability or brand presence is needed.

## Data Maturity

- Level 0 - Product Story Only;
- Level 1 - Value Realization Draft Ready;
- Level 2 - Directional Estimate Possible;
- Level 3 - Evidence Review Ready;
- Level 4 - Formal Governance Review Candidate outside this public skill.

When in doubt, cap at Level 3.

## Output Rules

Use [output_templates.md](output_templates.md).

The standard output contains:

1. Primary Audience;
2. Main Problem;
3. Expected Change;
4. Value Realization Chain;
5. Primary Economic Outcome;
6. Evidence KPI;
7. Directional Monetization;
8. Product Form Question;
9. Data Readiness;
10. Next Action.

Keep the final answer concise. Do not generate a large consulting report unless the user explicitly asks for detail.

## Guardrails

- Launch, usage, login, and page views are not economic value by themselves.
- Productivity is not direct saving unless actual spend or budget is reduced.
- Revenue growth requires incremental impact and attribution evidence.
- Risk value should normally use a range or risk tier.
- Platform value must avoid double counting downstream results.
- Branding must connect to traffic, conversion, revenue protection, or avoided cost.
- Learning must lead to a decision and cannot justify endless pilots.
- The Lens never says a product should be funded, stopped, merged, or decommissioned.

## References

- [conversation_flow.md](conversation_flow.md)
- [value_taxonomy.md](value_taxonomy.md)
- [data_checklists.md](data_checklists.md)
- [output_templates.md](output_templates.md)
- [examples.md](examples.md)
- [runtime_compatibility.md](runtime_compatibility.md)
- [NOTICE.md](NOTICE.md)
