# Output Templates

Use these templates after the guided wizard and any necessary clarification. Keep language conservative and professional.

## Template 1: Valence Product Value Lens Result

```markdown
# Valence Product Value Lens Result

## 1. Product Type
[判断产品类型]

## 2. Primary Users / Audience
[主要用户]

## 3. Core Use Case
[核心场景]

## 4. Likely Value Path
- [一级分类] -> [二级分类]
- [如有次要路径，列出]

## 5. Suggested Value Logic
[说明这个产品应该从什么价值口径评估，不一定计算金额]

## 6. Recommended Metrics to Collect

| Metric | Why It Matters | Suggested Owner | User Has It? |
| ------ | -------------- | --------------- | ------------ |
| [metric] | [why] | [owner] | [Yes / Not selected / Not sure / Not applicable] |

## 7. Directional Value Calculation

[Give a directional calculation path based on the likely value path. Do not use a formal aggregate value label. Do not imply this is a formal Valence valuation model.]

Example format:

- Primary value component: [formula direction]
- Secondary value component, if relevant: [formula direction]
- Do not double count: [state which metrics are proxy signals rather than additive financial value]

## 8. Data Maturity Level
[Level 0-4 + one-sentence rationale]

If Level 4 is used, add this sentence:

> Level 4 only means the evidence may be ready for formal portfolio or leadership review outside this public skill. This skill does not perform governance review or produce investment decisions.

When in doubt, cap the result at Level 3 and recommend formal Product Value Diagnostic / Valence review.

## 9. What Not To Do
- [错误判断 1]
- [错误判断 2]
- [错误判断 3]

## 10. Recommended Next Step
[下一步建议]

---
小提示：如果这类问题不是一个产品，而是一组产品组合，就不适合继续用单产品 Lens 判断了。下一步应进入正式 Product Value Diagnostic / Valence review。这个 Lens 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。
```

User Has It? mapping:

- Yes: selected in Step 6 or explicitly provided.
- Not selected: recommended but not selected.
- Not sure: user selected Not sure or expressed uncertainty.
- Not applicable: not relevant to the selected value path.

## Template 2: Data Not Enough

Use when the user provides rough selections but not enough data for a reliable estimate.

```markdown
当前信息足以形成价值口径草案，但不足以进行可靠价值估算。

## 已经知道什么
- [known fact 1]
- [known fact 2]

## 还需要确认什么
- [data gap 1]
- [data gap 2]

## 应找谁确认
- [business owner / finance / product owner / IT owner / risk owner]

## 下一步最小数据采集动作
- [small action 1]
- [small action 2]
```

## Template 3: Rough Estimate Possible

Use only when the user has provided enough parameters for a conservative illustrative calculation.

```markdown
## Rough Estimate Possible

### Calculation Path
[formula or logic path]

### User-Provided Parameters
- [parameter 1]
- [parameter 2]

### Rough Estimate
[calculation result or range]

### Key Assumptions
- [assumption 1]
- [assumption 2]

### Confidence Limits
- This is a rough directional estimate.
- It should not be used as a formal investment decision.
- It requires owner / finance confirmation before formal review.
```

## Directional Value Calculation Rules

- Use the phrase `Directional Value Calculation` in English or `方向性价值折算路径` in Chinese.
- Do not use a formal aggregate value label.
- Do not add NPS, CSAT, adoption, usage, and cost metrics together as if they are the same unit.
- Separate value components, then identify which metrics are financial drivers and which are proxy or evidence signals.
- Use attribution ratio, discount factor, or confidence limits when the product contribution is uncertain.
- Do not invent default attribution ratios, discount factors, industry benchmarks, or conversion assumptions. Mark them as `to confirm`.
- Do not label self-service deflection or productivity gain as direct Cost Saving unless there is budget, vendor, outsourced service, or finance-confirmed spend reduction.
- If the input data is weak, provide the calculation path but state that the current information is not enough for a reliable estimate.

## Directional Calculation Patterns

| Value path | Directional calculation path |
| --- | --- |
| Revenue Growth | Incremental gross profit = impacted base x conversion/order lift x average order value x gross margin x attribution ratio |
| Cost Saving | Annual direct saving = original annual cost - new annual cost, confirmed by finance/procurement |
| Cost Avoidance | Avoided cost = avoided FTE/external days/procurement/duplicate build x unit cost x attribution ratio |
| Productivity Gain | Productivity value = active users or annual volume x usage frequency x labor time saved per use x labor hourly cost x discount factor |
| Experience / Service Quality | Directional value = service cost reduction + complaint/ticket reduction + retention/repeat-purchase improvement, only where each link is evidenced |
| Decision Quality / Management Visibility | Directional value = manual reporting productivity value + attributed business improvement from changed decisions |
| Time Criticality | Delay value = expected value per period x delayed periods x decay or missed-window ratio |
| Operational Continuity | Continuity value = avoided downtime x loss per hour/day + avoided workaround labor cost |
| Compliance / Regulatory Timing | Exposure reduction = potential impact x probability or risk tier x reduced exposure period |
| Risk Reduction | Risk reduction value = potential impact x probability x risk reduction ratio, usually as a range |
| Platform Enablement | Platform value = avoided duplicate build + downstream reuse value + operational efficiency + risk/continuity value, avoiding double count |
| Opportunity Enablement | Use milestone, option, future pipeline, and validation evidence; do not count future opportunity as current realized value |
| Strategic Capability | Use milestone-based value and sponsor-confirmed strategic relevance; do not force short-term ROI |
| Learning / Validation Value | Use avoided wrong investment + validated learning + next-stage decision confidence; require hypothesis, time box, and go/no-go criteria |

## Data Maturity Model

| Level | Name | Meaning |
| --- | --- | --- |
| 0 | Product Story Only | Only product story or rough options exist. |
| 1 | Value Logic Draft Ready | Value path is clear enough for a metrics checklist. |
| 2 | Rough Estimate Possible | Some adoption, usage, cost, or value proxy exists. |
| 3 | Evidence Review Ready | Adoption, cost, value evidence, and owner confirmation exist. |
| 4 | Governance Review Ready | Evidence can enter formal portfolio or leadership review outside this public skill. |

## Level 4 Guardrail

Level 4 should be rare in this public skill. Use Level 4 only when the user already indicates adoption evidence, cost evidence, business value evidence, and relevant owner confirmation.

When in doubt, cap at Level 3 and recommend formal Product Value Diagnostic / Valence review.

Never use Level 4 to imply that this skill can run governance, rank products, make investment decisions, or replace Valence review.

## Conservative Language Library

Use:

- 当前更适合进入价值确认讨论。
- 当前数据只能支持价值假设。
- 当前显示 Value Evidence Weak 信号。
- 当前还不具备正式投资效率判断条件。
- 建议补齐 adoption、cost、business value evidence 后再评估。

Avoid:

- 这个产品没有价值。
- 这个产品 ROI 很高。
- 这个产品应该停止。
- 这个产品值得继续投资。

