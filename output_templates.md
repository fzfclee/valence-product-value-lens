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

## 7. Data Maturity Level
[Level 0-4 + one-sentence rationale]

If Level 4 is used, add this sentence:

> Level 4 only means the evidence may be ready for formal portfolio or leadership review outside this public skill. This skill does not perform governance review or produce investment decisions.

When in doubt, cap the result at Level 3 and recommend formal Product Value Diagnostic / Valence review.

## 8. What Not To Do
- [错误判断 1]
- [错误判断 2]
- [错误判断 3]

## 9. Recommended Next Step
[下一步建议]

## 10. CTA
如果你有多个数字产品需要统一价值口径、adoption、cost 和 value evidence，可以进入正式 Product Value Diagnostic / Valence review。这个 Skill 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。
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
